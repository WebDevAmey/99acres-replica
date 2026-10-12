# 99acres Bengaluru — HTML/CSS build of the Figma high-fidelity screens

Open `index.html` in a browser. Pages are linked in the same flow as the design:

| Page | Figma frame |
|---|---|
| `index.html` | Home and smart search (50:1041) |
| `search.html` | Search results (50:1144) |
| `compare.html` | Compare properties (50:1251) |
| `detail.html` | Property detail and contact owner (50:1390) |
| `contact.html` | Contact confirmation (77:93) |

All styles live in `styles.css`. Icons are inline Lucide SVGs (the same set used in the Figma file). Font: Inter via Google Fonts.

## Adding the photos

Export these layers from Figma (select layer → Export → JPG, 2x) and save them into `assets/` with exactly these names. Until a file is present, its slot shows a soft green placeholder at the correct size.

| File in `assets/` | Figma layer (node id) |
|---|---|
| `hero.jpg` | Home › Hero image (50:1073) |
| `home-cedar-house.jpg` | Home › Property image, card 1 (50:1093) |
| `home-nila-residences.jpg` | Home › Property image, card 2 (50:1109) |
| `home-the-grove.jpg` | Home › Property image, card 3 (50:1125) |
| `search-cedar-house.jpg` | Search › Property image, card 1 (50:1198) |
| `search-nila-residences.jpg` | Search › Property image, card 2 (50:1214) |
| `search-the-grove.jpg` | Search › Property image, card 3 (50:1230) |
| `map.jpg` | Search › Map (50:1245) — hide its two labels before exporting |
| `compare-cedar-house.jpg` | Compare › Image, column 1 (50:1282) |
| `compare-nila-residences.jpg` | Compare › Image, column 2 (50:1289) |
| `compare-the-grove.jpg` | Compare › Image, column 3 (50:1296) |
| `detail-living.jpg` | Detail › Main image (50:1410) — also used on the contact page |
| `detail-bedroom.jpg` | Detail › Bedroom image (50:1412) |
| `detail-balcony.jpg` | Detail › Balcony image (50:1413) |

## Small deviations from the Figma file (bug fixes)

- "99acres verified" badges size to their text instead of clipping at 109px.
- Contact page: "Bengaluru" no longer overlaps the logo, and "Rhea Menom" is corrected to "Rhea Menon".
- The property-detail disclaimer layer sits off-canvas in Figma (not visible), so it is omitted.
