periodic table of elements
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
