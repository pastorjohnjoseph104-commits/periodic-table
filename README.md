 periodic table of elements
import os
import requests
import json
from PIL import Image, ImageDraw, ImageFont
import qrcode
from textwrap import wrap

# Fetch periodic table data from a reliable JSON source
url = "https://raw.githubusercontent.com/Bowserinator/Periodic-Table-JSON/master/PeriodicTableJSON.json"
response = requests.get(url)
data = json.loads(response.text)
elements = data['elements']

# Create output folder
folder = "Periodic_Table_Photocards"
os.makedirs(folder, exist_ok=True)

# Define color-coding for element categories (RGB tuples)
category_colors = {
    "diatomic nonmetal": (255, 165, 0),   # orange
    "polyatomic nonmetal": (0, 0, 255),   # blue
    "noble gas": (238, 130, 238),         # violet
    "alkali metal": (255, 0, 0),          # red
    "alkaline earth metal": (255, 255, 0),# yellow
    "metalloid": (0, 128, 0),             # green
    "post-transition metal": (128, 128, 128),  # gray
    "transition metal": (255, 192, 203),  # pink
    "lanthanide": (128, 0, 128),          # purple
    "actinide": (165, 42, 42),            # brown
    "unknown": (211, 211, 211)            # light gray
}

# Function to extract 2-3 sentence description
def get_short_description(summary):
    sentences = [s.strip() for s in summary.split('.') if s.strip()]
    if len(sentences) > 3:
        return ' '.join(sentences[:3]) + '.'
    return ' '.join(sentences) + '.'

# Attempt to load fonts (assume system fonts; fallback to default if not found)
try:
    large_font = ImageFont.truetype("arial.ttf", 30)
    font = ImageFont.truetype("arial.ttf", 20)
    small_font = ImageFont.truetype("arial.ttf", 16)
except IOError:
    large_font = ImageFont.load_default()
    font = ImageFont.load_default()
    small_font = ImageFont.load_default()

# Generate cards for elements 1-118
for element in elements:
    if element['number'] > 118 or element['number'] < 1:
        continue

    name = element['name']
    symbol = element['symbol']
    atomic_number = element['number']
    atomic_mass = round(element['atomic_mass'], 4) if isinstance(element['atomic_mass'], float) else element['atomic_mass']
    group = element.get('group', 'N/A')
    period = element['period']
    category = element['category']
    description = get_short_description(element['summary'])
    discovered_by = element.get('discovered_by', 'unknown sources')
    fact = f"Interesting fact: Discovered by {discovered_by}."
    source_url = element['source']

    # Determine background color based on category
    cat_key = category.lower()
    if "nonmetal" in cat_key and "diatomic" in cat_key:
        bg_color = category_colors["diatomic nonmetal"]
    elif "nonmetal" in cat_key and "polyatomic" in cat_key:
        bg_color = category_colors["polyatomic nonmetal"]
    elif "noble gas" in cat_key:
        bg_color = category_colors["noble gas"]
    elif "alkali metal" in cat_key:
        bg_color = category_colors["alkali metal"]
    elif "alkaline earth metal" in cat_key:
        bg_color = category_colors["alkaline earth metal"]
    elif "metalloid" in cat_key:
        bg_color = category_colors["metalloid"]
    elif "post-transition metal" in cat_key:
        bg_color = category_colors["post-transition metal"]
    elif "transition metal" in cat_key:
        bg_color = category_colors["transition metal"]
    elif "lanthanide" in cat_key:
        bg_color = category_colors["lanthanide"]
    elif "actinide" in cat_key:
        bg_color = category_colors["actinide"]
    else:
        bg_color = category_colors["unknown"]

    # Create card image (400x600 pixels)
    width, height = 400, 600
    img = Image.new('RGB', (width, height), color=bg_color)
    draw = ImageDraw.Draw(img)

    # Add a border for collectible look
    draw.rectangle([(10, 10), (width - 10, height - 10)], outline="black", width=5)

    # Add text elements
    draw.text((20, 20), name, fill=(0, 0, 0), font=large_font)
    draw.text((20, 70), f"Symbol: {symbol}", fill=(0, 0, 0), font=font)
    draw.text((20, 100), f"Atomic Number: {atomic_number}", fill=(0, 0, 0), font=font)
    draw.text((20, 130), f"Atomic Mass: {atomic_mass}", fill=(0, 0, 0), font=font)
    draw.text((20, 160), f"Group: {group}, Period: {period}", fill=(0, 0, 0), font=font)
    draw.text((20, 190), f"Category: {category.capitalize()}", fill=(0, 0, 0), font=font)

    # Description (wrapped)
    desc_lines = wrap(description, width=40)
    y = 230
    for line in desc_lines:
        draw.text((20, y), line, fill=(0, 0, 0), font=small_font)
        y += 18

    # Interesting fact (wrapped)
    y += 20
    fact_lines = wrap(fact, width=40)
    for line in fact_lines:
        draw.text((20, y), line, fill=(0, 0, 0), font=small_font)
        y += 18

    # Generate QR code linking to source
    qr = qrcode.QRCode(version=1, box_size=5, border=2)
    qr.add_data(source_url)
    qr.make(fit=True)
    qr_img = qr.make_image(fill_color="black", back_color="white")
    qr_size = 100
    qr_img = qr_img.resize((qr_size, qr_size))
    img.paste(qr_img, (width - qr_size - 20, height - qr_size - 20))

    # Save as PNG
    filename = f"{atomic_number:03d}_{name.replace(' ', '_')}.png"
    img.save(os.path.join(folder, filename))

print("All 118 photocards have been generated and saved in the 'Periodic_Table_Photocards' folder.")
