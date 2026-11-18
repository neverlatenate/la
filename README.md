🏙️ # L.A. Lasts A Lifetime

**Landmark & Address Index · Los Angeles County, A to Z**

L.A. Lasts A Lifetime is an alphabetical index of exactly 4,900 places in Los Angeles County: landmarks, neighborhoods, businesses, and houses both famous and ordinary. Each entry gives the place's name, where it is, and a short account of why it matters. It runs from A to Zuma Beach.

Los Angeles is often called "72 suburbs in search of a city." This index doesn't try to settle that argument. It writes down the addresses.

**View the index:** [neverlatenate.github.io/la](https://neverlatenate.github.io/la/)

> This is a working draft. The full A–Z is being prepared for launch, and the pages here are still in progress.

---

## How the index works

- **4,900 places, A to Z.** The count is fixed, and Zuma Beach is the last entry.
- **Filing.** Names that begin with "The" file under the word that follows. There is no # section; every place files under a letter.
- **Addresses.** Homes of living people are included without a street address. Noteable private homes are listed with their street addresses, if a well-known person once lived there, the house is a landmark, or it is simply a house worth knowing, but with a caveat. The caveat for private homes is do not knock on their doors, trespass on their property, or do anything else that might disturb the residents. 
- **See it then.** Where a vintage photograph exists, the entry links to it on [Martin Turnbull's](https://martinturnbull.com) site of historic Hollywood and Los Angeles images.
- **Sourcing.** Entries are checked claim by claim. When a source contradicts an entry, the entry is corrected. Some details are still unconfirmed and are being checked.

## Corrections

Los Angeles is a lot of city. If you spot a wrong address, a wrong date, or a place that has closed, please [open an issue](https://github.com/neverlatenate/la/issues) with the entry name and, if you have one, a source.

## Under the hood

Plain HTML, CSS, and JavaScript with no build step, hosted on GitHub Pages.

- `neighborhoods_data.js`: places grouped by neighborhood, with name, type, address, coordinates, and a Google Maps link
- `neighborhoods_descriptions.js`: entry text, keyed by neighborhood and place
- `neighborhoods.min.js` and `descriptions.min.js`: compressed copies of the two data files; these are what the pages load, so edits to the readable files need to be re-minified before they show up on the site
- `index2.html`: interactive map of the places (draft)

## Credits

Compiled by **Jeremy Nathan Schulman**, educator and design historian · [nateschulman.com](https://nateschulman.com)

"See it then" photographs: [Martin Turnbull](https://martinturnbull.com)



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
