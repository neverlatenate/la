🏙️ # L.A. Lasts A Lifetime

**Landmark & Address Index · Los Angeles County, A to Z**

L.A. Lasts A Lifetime is an alphabetical index of exactly 5,555 places in Los Angeles County: landmarks, neighborhoods, businesses, and houses both famous and ordinary. Each entry gives the place's name, where it is, and a short account of why it matters. It runs from A to Zuma Beach.

Los Angeles is often called "72 suburbs in search of a city." This index doesn't try to settle that argument. It writes down the addresses.

**View the index:** [neverlatenate.github.io/la](https://neverlatenate.github.io/la/)

> This is a working draft. The full A–Z is being prepared for launch, and the pages here are still in progress.

**1. Purpose & Core Flows**
L.A. Lasts A Lifetime is a searchable, map-backed digital gazetteer of 5,555 places across Los Angeles County, spanning Acton to Zuma. Its user experience is structured like a two-part reference book with interactive wayfinding:
Cover & Front Matter (header.cover, section.intro, section.howto): Pairs an interstate-sign hero title block (.bigsign) with an interactive county-wide dot map (#iMapCv) over 270 L.A. Times Mapping L.A. boundaries, a cycling place spotlight (#flick), a featured random-entry card (#pick), a clickable wall of ~200 place names (#names), and a visual reading legend.

Part One — The A to Z of Placenames (#viewAreas): An index of L.A. County neighborhoods, cities, unincorporated communities, historic districts, and HPOZs. Users filter by category pills (#atabs), search (#aq), jump via an A–Z letter rail (#arail), expand collapsible neighborhood profiles (details.pf), or download a 11-page PDF companion (la_regional_directory.pdf).

Part Two — The A to Z of Places (#viewPlaces): The primary 5,555-entry gazetteer. A sticky filter bar (div.finder) combines full-text search (#q), a custom ARIA combobox for filtering by area (#areaBox / #areaList), a List/Map segmented switch (#vseg), an A–Z jump rail (#rail), and removable filter chips (#chips). Users browse either a two-column editorial spread (main#book) or an interactive dot map (section#mapView) with status-coded markers and preset topic pills (#mtry).

Persistent Wayfinding & Back Matter: A scroll-triggered fixed utility bar (nav.util) and back-to-top button (#totop) provide quick part switching and filter resets, leading down to the colophon (section.about) and Terms of Service (section.tos).


**2. Technical Architecture**
Stack: Zero-dependency, single-file architecture (index.html) combining semantic HTML, inline CSS, embedded JSON datasets (<script type="application/json" id="areas"> and #data), and vanilla ES6+ JavaScript.

CSS Strategy: Driven by semantic CSS custom properties (--paper, --ink, --muted, --label, status tokens --gone / --shift / --maybe, --sign, and map tokens --m0–--m2). Supports automatic OS dark mode via @media (prefers-color-scheme: dark) plus manual [data-theme="light"|"dark"] overrides, fluid clamp() typography, and env(safe-area-inset-*) notch padding.

Layout & Rendering: Uses CSS Grid for the cover, intro, and map views; Flexbox for toolbars and rails; CSS multi-column layout (columns: 2 at 700px, columns: 3 at 1100px) for print-like book spreads; and custom HTML5 <canvas> rendering for both dot maps.


**3. Existing Visual Voice**
Editorial Book Meets Caltrans Freeway Signage: The visual identity juxtaposes classic reference-book typography with Southern California highway wayfinding.

Typography: Newsreader (an optical-size editorial serif) sets display titles and entry prose; Overpass (modeled on FHWA Highway Gothic) sets neighborhood headers, addresses, tags, and A–Z rails; Overpass Mono sets tabular entry IDs (A-001) and large counters (5,555).

Palette & Rhythm: Crisp white/newsprint ground (#ffffff / #f5f2ed), warm charcoal ink (#24211e), burnt-terracotta index accents (#b5472a), and interstate green (#0f6440) reserved for the cover plaque, intro hero card, and PDF badge. High-density print conventions—dotted tab leaders (.lead), 65ch reading measures, tabular numerals, and hanging punctuation—give the app unmistakable character.## Credits

Compiled by **Jeremy Nathan Schulman**, educator and design historian · [nateschulman.com](https://nateschulman.com)

📌 Project Overview
Los Angeles is often described as "72 suburbs in search of a city." This project seeks to categorize that search. By documenting everything from the high-desert enclaves of the Antelope Valley to the historic HPOZs of South L.A., the Gazetteer provides a standardized, accessible resource for historians, designers, and urban explorers.

Key Features

A-Z Navigation: A sticky navigation rail for rapid access.

Geographic Integrity: Accurate regional categorization, including cultural corridors like Little Ethiopia and Thai Town.

Accordion Interface: A clean, scannable UI that allows users to focus on specific entries without "scrolling fatigue."

🚀 Deployment
This project is hosted via GitHub Pages.

Clone or download the repository.

Open index.html in any modern web browser.


📜 Research Notes & Credits
This gazetteer was compiled with a focus on:

Architectural Preservation: Identifying Historic Preservation Overlay Zones (HPOZs).

Geographic Accuracy: Re-homing communities that are often miscategorized in generic data exports.

Author: Jeremy Nathan Schulman

Educator & Design Historian
