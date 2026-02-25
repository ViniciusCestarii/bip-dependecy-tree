# Bitcoin BIP Dependency Tree

A lightweight, client-side web application that visualizes the dependency graph of Bitcoin Improvement Proposals (BIPs). 

The tool fetches `.mediawiki` and `.md` files directly from the official `bitcoin/bips` repository, parses the headers for `Requires:` fields, and renders an interactive hierarchical tree.

## Features

* **Direct Fetching:** Pulls data directly from the GitHub raw content API without requiring a backend server.
* **Interactive Visualization:** Uses `vis-network` for a drag-and-drop, zoomable node graph.
* **Node Details:** Clicking a node displays the BIP number, title, direct dependencies, and a link to the official repository file.
* **Fallback Parsing:** Handles both `.mediawiki` and `.md` file extensions used in the Bitcoin repository.

## Usage

1. Clone this repository or download the `index.html` file.
2. Open the `index.html` file in any modern web browser.
3. Click the **Generate Tree** button in the sidebar.
4. Wait for the fetch process to complete. You can click on individual nodes to view more details in the sidebar.

## Dependencies

* [vis-network](https://github.com/visjs/vis-network) (Loaded via CDN)
* Google Fonts (Inter)

## License

MIT
