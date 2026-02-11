# periodic-table
Periodic Table Photocards  Visual collection of all 118 chemical elements presented in card format.   Includes photos, key data, short descriptions, interesting facts, and QR links. Single-file HTML + CSS implementation.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Periodic Table Photocards - Elements 1 to 50</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            background-color: #f8f9fa;
            margin: 0;
            padding: 20px;
            color: #333;
        }
        h1 {
            text-align: center;
            color: #2c3e50;
        }
        .intro {
            text-align: center;
            max-width: 800px;
            margin: 0 auto 30px;
        }
        .container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 20px;
            max-width: 1400px;
            margin: 0 auto;
        }
        .card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            overflow: hidden;
            text-align: center;
            padding: 15px;
            transition: transform 0.15s;
        }
        .card:hover {
            transform: translateY(-5px);
        }
        .element-img {
            width: 100%;
            height: 180px;
            object-fit: contain;
            background: #f1f3f5;
            border-radius: 6px;
            margin-bottom: 10px;
        }
        .card h2 {
            margin: 10px 0 5px;
            font-size: 1.4em;
            color: #2980b9;
        }
        .desc, .fact {
            font-size: 0.95em;
            line-height: 1.4;
            margin: 8px 0;
        }
        .desc strong {
            color: #34495e;
        }
        .qr {
            margin-top: 12px;
            width: 100px;
            height: 100px;
        }
    </style>
</head>
<body>

    <h1>Periodic Table Photocards<br>Elements 1–50</h1>
    <p class="intro">Scan the QR code on each card to return to this page. Great for classrooms, study aids, or element collectors!</p>

    <div class="container">

        <!-- 1 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/hydrogen.jpg" alt="Hydrogen">
            <h2>1 – Hydrogen (H)</h2>
            <p class="desc"><strong>Description:</strong> Colorless, odorless, highly flammable diatomic gas; lightest element.</p>
            <p class="fact"><strong>Fact:</strong> Makes up \~75% of the elemental mass of the universe.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 2 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/helium.jpg" alt="Helium">
            <h2>2 – Helium (He)</h2>
            <p class="desc"><strong>Description:</strong> Colorless, inert noble gas; second lightest element.</p>
            <p class="fact"><strong>Fact:</strong> Makes your voice high-pitched when inhaled because it travels faster than air.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 3 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/lithium.jpg" alt="Lithium">
            <h2>3 – Lithium (Li)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery-white alkali metal; highly reactive.</p>
            <p class="fact"><strong>Fact:</strong> Used in rechargeable batteries that power phones and electric cars.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 4 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/beryllium.jpg" alt="Beryllium">
            <h2>4 – Beryllium (Be)</h2>
            <p class="desc"><strong>Description:</strong> Hard, grayish metal; lightweight and strong.</p>
            <p class="fact"><strong>Fact:</strong> Used in aerospace alloys because it's six times stiffer than steel by weight.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 5 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/boron.jpg" alt="Boron">
            <h2>5 – Boron (B)</h2>
            <p class="desc"><strong>Description:</strong> Black-brown metalloid; very hard.</p>
            <p class="fact"><strong>Fact:</strong> Borax (a boron compound) is used in slime and as a cleaning agent.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 6 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/carbon.jpg" alt="Carbon">
            <h2>6 – Carbon (C)</h2>
            <p class="desc"><strong>Description:</strong> Nonmetal; exists as diamond, graphite, graphene, etc.</p>
            <p class="fact"><strong>Fact:</strong> Basis of all known life — found in DNA, proteins, and you!</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 7 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/nitrogen.jpg" alt="Nitrogen">
            <h2>7 – Nitrogen (N)</h2>
            <p class="desc"><strong>Description:</strong> Colorless, odorless diatomic gas; makes up 78% of Earth's atmosphere.</p>
            <p class="fact"><strong>Fact:</strong> Essential for fertilizers, helping grow food for billions.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 8 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/oxygen.jpg" alt="Oxygen">
            <h2>8 – Oxygen (O)</h2>
            <p class="desc"><strong>Description:</strong> Colorless, odorless diatomic gas; highly reactive.</p>
            <p class="fact"><strong>Fact:</strong> Makes up 21% of air and is vital for respiration in most life forms.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 9 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/fluorine.jpg" alt="Fluorine">
            <h2>9 – Fluorine (F)</h2>
            <p class="desc"><strong>Description:</strong> Pale yellow, highly reactive halogen gas.</p>
            <p class="fact"><strong>Fact:</strong> Added to toothpaste to prevent tooth decay.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 10 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/neon.jpg" alt="Neon">
            <h2>10 – Neon (Ne)</h2>
            <p class="desc"><strong>Description:</strong> Colorless noble gas; inert.</p>
            <p class="fact"><strong>Fact:</strong> Glows red-orange in neon signs when electrified.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 11 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/sodium.jpg" alt="Sodium">
            <h2>11 – Sodium (Na)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery alkali metal; highly reactive with water.</p>
            <p class="fact"><strong>Fact:</strong> Combined with chlorine to make table salt (NaCl).</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 12 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/magnesium.jpg" alt="Magnesium">
            <h2>12 – Magnesium (Mg)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-white alkaline earth metal; lightweight.</p>
            <p class="fact"><strong>Fact:</strong> Burns brightly in flares and fireworks.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 13 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/aluminum.jpg" alt="Aluminum">
            <h2>13 – Aluminum (Al)</h2>
            <p class="desc"><strong>Description:</strong> Lightweight, silvery metal; resistant to corrosion.</p>
            <p class="fact"><strong>Fact:</strong> Used in beverage cans and aircraft due to its strength-to-weight ratio.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 14 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/silicon.jpg" alt="Silicon">
            <h2>14 – Silicon (Si)</h2>
            <p class="desc"><strong>Description:</strong> Gray, crystalline metalloid; semiconductor.</p>
            <p class="fact"><strong>Fact:</strong> Key component in computer chips and solar panels.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 15 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/phosphorus.jpg" alt="Phosphorus">
            <h2>15 – Phosphorus (P)</h2>
            <p class="desc"><strong>Description:</strong> Waxy, white nonmetal; highly reactive.</p>
            <p class="fact"><strong>Fact:</strong> Used in matches; glows in the dark (phosphorescence).</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 16 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/sulfur.jpg" alt="Sulfur">
            <h2>16 – Sulfur (S)</h2>
            <p class="desc"><strong>Description:</strong> Bright yellow, brittle nonmetal; smells like rotten eggs when burned.</p>
            <p class="fact"><strong>Fact:</strong> Component in gunpowder and vulcanized rubber.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 17 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/chlorine.jpg" alt="Chlorine">
            <h2>17 – Chlorine (Cl)</h2>
            <p class="desc"><strong>Description:</strong> Greenish-yellow, toxic halogen gas.</p>
            <p class="fact"><strong>Fact:</strong> Used as a disinfectant in swimming pools and drinking water.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 18 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/argon.jpg" alt="Argon">
            <h2>18 – Argon (Ar)</h2>
            <p class="desc"><strong>Description:</strong> Colorless noble gas; inert.</p>
            <p class="fact"><strong>Fact:</strong> Used in welding to provide an inert atmosphere.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 19 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/potassium.jpg" alt="Potassium">
            <h2>19 – Potassium (K)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery alkali metal; reacts violently with water.</p>
            <p class="fact"><strong>Fact:</strong> Abundant in bananas; essential for nerve function.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 20 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/calcium.jpg" alt="Calcium">
            <h2>20 – Calcium (Ca)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-white alkaline earth metal.</p>
            <p class="fact"><strong>Fact:</strong> Builds strong bones and teeth; found in milk.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 21 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/scandium.jpg" alt="Scandium">
            <h2>21 – Scandium (Sc)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-white transition metal; rare earth-like.</p>
            <p class="fact"><strong>Fact:</strong> Used in high-strength aluminum alloys for aerospace.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 22 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/titanium.jpg" alt="Titanium">
            <h2>22 – Titanium (Ti)</h2>
            <p class="desc"><strong>Description:</strong> Strong, lightweight transition metal; corrosion-resistant.</p>
            <p class="fact"><strong>Fact:</strong> Used in medical implants and aircraft frames.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 23 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/vanadium.jpg" alt="Vanadium">
            <h2>23 – Vanadium (V)</h2>
            <p class="desc"><strong>Description:</strong> Hard, silvery-gray transition metal.</p>
            <p class="fact"><strong>Fact:</strong> Added to steel for high-strength tools and axles.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 24 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/chromium.jpg" alt="Chromium">
            <h2>24 – Chromium (Cr)</h2>
            <p class="desc"><strong>Description:</strong> Lustrous, hard transition metal.</p>
            <p class="fact"><strong>Fact:</strong> Used for chrome plating on cars and stainless steel.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 25 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/manganese.jpg" alt="Manganese">
            <h2>25 – Manganese (Mn)</h2>
            <p class="desc"><strong>Description:</strong> Gray-white, brittle transition metal.</p>
            <p class="fact"><strong>Fact:</strong> Essential in steel production and some batteries.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 26 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/iron.jpg" alt="Iron">
            <h2>26 – Iron (Fe)</h2>
            <p class="desc"><strong>Description:</strong> Malleable, ductile transition metal; magnetic.</p>
            <p class="fact"><strong>Fact:</strong> Key in hemoglobin for oxygen transport in blood.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 27 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/cobalt.jpg" alt="Cobalt">
            <h2>27 – Cobalt (Co)</h2>
            <p class="desc"><strong>Description:</strong> Hard, lustrous transition metal.</p>
            <p class="fact"><strong>Fact:</strong> Central atom in vitamin B12, essential for health.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 28 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/nickel.jpg" alt="Nickel">
            <h2>28 – Nickel (Ni)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-white transition metal; tough.</p>
            <p class="fact"><strong>Fact:</strong> Used in coins and stainless steel alloys.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 29 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/copper.jpg" alt="Copper">
            <h2>29 – Copper (Cu)</h2>
            <p class="desc"><strong>Description:</strong> Reddish, malleable transition metal; excellent conductor.</p>
            <p class="fact"><strong>Fact:</strong> Used in electrical wires and plumbing pipes.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 30 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/zinc.jpg" alt="Zinc">
            <h2>30 – Zinc (Zn)</h2>
            <p class="desc"><strong>Description:</strong> Bluish-white metal; brittle at room temperature.</p>
            <p class="fact"><strong>Fact:</strong> Coats iron to prevent rust (galvanizing).</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 31 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/gallium.jpg" alt="Gallium">
            <h2>31 – Gallium (Ga)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery metal; melts at low temperature.</p>
            <p class="fact"><strong>Fact:</strong> Melts in your hand at about 86°F (30°C).</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 32 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/germanium.jpg" alt="Germanium">
            <h2>32 – Germanium (Ge)</h2>
            <p class="desc"><strong>Description:</strong> Grayish-white metalloid; semiconductor.</p>
            <p class="fact"><strong>Fact:</strong> Used in early transistors and fiber optics.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 33 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/arsenic.jpg" alt="Arsenic">
            <h2>33 – Arsenic (As)</h2>
            <p class="desc"><strong>Description:</strong> Gray metalloid; toxic.</p>
            <p class="fact"><strong>Fact:</strong> Historically used as a poison but also in semiconductors.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 34 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/selenium.jpg" alt="Selenium">
            <h2>34 – Selenium (Se)</h2>
            <p class="desc"><strong>Description:</strong> Gray nonmetal; semiconductor.</p>
            <p class="fact"><strong>Fact:</strong> Used in anti-dandruff shampoos and photocopiers.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 35 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/bromine.jpg" alt="Bromine">
            <h2>35 – Bromine (Br)</h2>
            <p class="desc"><strong>Description:</strong> Red-brown liquid halogen; toxic fumes.</p>
            <p class="fact"><strong>Fact:</strong> Used in flame retardants and water purification.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 36 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/krypton.jpg" alt="Krypton">
            <h2>36 – Krypton (Kr)</h2>
            <p class="desc"><strong>Description:</strong> Colorless noble gas; inert.</p>
            <p class="fact"><strong>Fact:</strong> Used in high-performance lighting like flashlights.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 37 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/rubidium.jpg" alt="Rubidium">
            <h2>37 – Rubidium (Rb)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery alkali metal; highly reactive.</p>
            <p class="fact"><strong>Fact:</strong> Used in atomic clocks for precise timekeeping.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 38 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/strontium.jpg" alt="Strontium">
            <h2>38 – Strontium (Sr)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-yellow alkaline earth metal.</p>
            <p class="fact"><strong>Fact:</strong> Gives red color to fireworks and flares.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 39 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/yttrium.jpg" alt="Yttrium">
            <h2>39 – Yttrium (Y)</h2>
            <p class="desc"><strong>Description:</strong> Silvery transition metal; rare earth.</p>
            <p class="fact"><strong>Fact:</strong> Used in LEDs and phosphors for color TVs.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 40 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/zirconium.jpg" alt="Zirconium">
            <h2>40 – Zirconium (Zr)</h2>
            <p class="desc"><strong>Description:</strong> Lustrous, gray-white transition metal.</p>
            <p class="fact"><strong>Fact:</strong> Used in nuclear reactors due to low neutron absorption.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 41 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/niobium.jpg" alt="Niobium">
            <h2>41 – Niobium (Nb)</h2>
            <p class="desc"><strong>Description:</strong> Soft, gray transition metal; superconducting.</p>
            <p class="fact"><strong>Fact:</strong> Used in superalloys for jet engines.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 42 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/molybdenum.jpg" alt="Molybdenum">
            <h2>42 – Molybdenum (Mo)</h2>
            <p class="desc"><strong>Description:</strong> Silvery transition metal; high melting point.</p>
            <p class="fact"><strong>Fact:</strong> Essential trace element in enzymes for life.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 43 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/technetium.jpg" alt="Technetium">
            <h2>43 – Technetium (Tc)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-gray transition metal; radioactive.</p>
            <p class="fact"><strong>Fact:</strong> Used in medical imaging as a tracer.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 44 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/ruthenium.jpg" alt="Ruthenium">
            <h2>44 – Ruthenium (Ru)</h2>
            <p class="desc"><strong>Description:</strong> Hard, white transition metal; platinum group.</p>
            <p class="fact"><strong>Fact:</strong> Used as a catalyst in chemical reactions.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 45 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/rhodium.jpg" alt="Rhodium">
            <h2>45 – Rhodium (Rh)</h2>
            <p class="desc"><strong>Description:</strong> Silvery-white transition metal; very reflective.</p>
            <p class="fact"><strong>Fact:</strong> Used in catalytic converters to reduce car emissions.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 46 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/palladium.jpg" alt="Palladium">
            <h2>46 – Palladium (Pd)</h2>
            <p class="desc"><strong>Description:</strong> Lustrous, silvery transition metal.</p>
            <p class="fact"><strong>Fact:</strong> Used in jewelry and hydrogen storage.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 47 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/silver.jpg" alt="Silver">
            <h2>47 – Silver (Ag)</h2>
            <p class="desc"><strong>Description:</strong> Lustrous, white transition metal; best conductor.</p>
            <p class="fact"><strong>Fact:</strong> Used in photography and antibacterial products.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 48 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/cadmium.jpg" alt="Cadmium">
            <h2>48 – Cadmium (Cd)</h2>
            <p class="desc"><strong>Description:</strong> Soft, bluish-white metal; toxic.</p>
            <p class="fact"><strong>Fact:</strong> Used in Ni-Cd batteries and pigments.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 49 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/indium.jpg" alt="Indium">
            <h2>49 – Indium (In)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery-white post-transition metal; very ductile.</p>
            <p class="fact"><strong>Fact:</strong> Used in touchscreens (indium tin oxide) — it's in most smartphones.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

        <!-- 50 -->
        <div class="card">
            <img class="element-img" src="https://images-of-elements.com/tin.jpg" alt="Tin">
            <h2>50 – Tin (Sn)</h2>
            <p class="desc"><strong>Description:</strong> Soft, silvery-white metal; resistant to corrosion.</p>
            <p class="fact"><strong>Fact:</strong> "Tin cry" — it makes a cracking sound when bent due to crystal structure change.</p>
            <img class="qr" src="https://api.qrserver.com/v1/create-qr-code/?size=100x100&data=https://yourusername.github.io/periodic-table/" alt="QR to site">
        </div>

    </div>

</body>
</html>
