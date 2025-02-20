# Tree Selection UI

This project is a simple tree selection UI built using HTML, CSS, jQuery, and JavaScript. It allows users to navigate a hierarchical tree structure and select/deselect items while ensuring parent-child relationships are maintained properly.

## Features
- **RTL Support:** The interface is designed for right-to-left (RTL) languages such as Arabic.
- **Hierarchical Selection:** Selecting a parent node selects all its children, and deselecting updates accordingly.
- **Parent Auto-Update:** Parent nodes update their selection state based on their children.
- **Tree Rendering:** The tree structure is dynamically generated from a JavaScript object.
- **Smooth UI Interactions:** Uses jQuery for efficient DOM manipulation and event handling.

## Technologies Used
- **HTML5** for structuring the UI
- **CSS3** for styling
- **jQuery** for handling events and DOM updates
- **JavaScript** for tree data processing and selection logic

## Project Structure
```
├── index.html  # Main file containing UI and script
├── styles.css  # Styles (included in index.html as internal CSS)
├── script.js   # jQuery script for tree selection logic (embedded in index.html)
```

## How It Works
1. **Tree Data Initialization:**
   - The tree structure is defined as a JavaScript object.
   - Each node has a `name`, `selected` state, and optional `children`.

2. **Tree Rendering:**
   - The `renderTree` function recursively generates the tree structure inside a `<ul>` list.
   - Each node has a checkbox to toggle its selection.

3. **Selection Behavior:**
   - When a node is selected/deselected, its children update accordingly.
   - The `updateParents` function ensures parent nodes reflect the correct state based on their children.
   - The `refreshTree` function re-renders the tree to reflect changes.

## How to Run
1. Download or copy the `index.html` file.
2. Open `index.html` in a web browser.
3. Interact with the tree by selecting/deselecting nodes.

## Future Enhancements
- Add expand/collapse functionality for better usability.
- Store selections in local storage or a database.
- Improve styling for a more modern look.

## License
This project is open-source and can be used freely.

