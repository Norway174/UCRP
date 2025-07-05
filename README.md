# Universal Crafting Recipe Planner (UCRP)

A powerful, visual crafting recipe planner that helps you organize complex crafting trees for games, projects, or any hierarchical recipe system. Built as a single-page web application with an intuitive node-based interface and automatic layout system.

### [Click here to access the UCRP Online!](https://norway174.github.io/UCRP/UCRP.html)

![UCRP Interface](https://iili.io/Fckn6va.png)

## ✨ Features

### Visual Tree Builder
- **Interactive Canvas**: Pan and zoom to navigate your recipe trees with smooth camera controls
- **Node-based System**: Each item is represented as a node with quantity and completion tracking
- **Automatic Layout**: Intelligent positioning system that organizes your trees hierarchically
- **Flexible Orientation**: Switch between top-to-bottom and left-to-right tree layouts
- **Ghost Nodes**: Automatic handling of circular dependencies with visual indicators

### Recipe Management
- **Smart Item System**: Reuse items across multiple recipes with automatic synchronization
- **Quantity Calculation**: Automatic calculation of total quantities needed for materials
- **Completion Tracking**: Mark items as complete with cascading status updates
- **Notes Support**: Add both global (item-level) and local (node-specific) notes

### Data Persistence
- **Auto-save**: Automatic saving to browser localStorage
- **Preset System**: Save and load named recipe configurations
- **Export Options**: Share recipes as JSON, ASCII tree view, or materials list
- **Import/Export**: Full recipe data portability

### User Experience
- **Responsive Design**: Works on desktop and mobile devices
- **Dark Theme**: Easy-on-the-eyes interface optimized for long planning sessions
- **Keyboard Navigation**: Full keyboard support for dropdown menus
- **Smart Suggestions**: Autocomplete for existing item names

## 📋 Getting Started

### 🌐 Use Online
**No installation required!** Simply open the link below in any modern web browser:

👉 **[Launch UCRP Online](https://norway174.github.io/UCRP/UCRP.html)**

- Works instantly on desktop and mobile
- Your data is saved locally to your browser (Nothing is ever sent to any servers!)
- No downloads, no setup, no registration needed

### 💾 Download for Offline Use
1. **Right-click** on this link: [UCRP.html](https://norway174.github.io/UCRP/UCRP.html)
2. **Select "Save As"** or "Save Link As"
3. **Open the downloaded file** in any modern web browser
4. **You're ready to go!** - Works completely offline

### Basic Usage

1. **Create your first recipe**:
   - Click "Add Root Node" to create a top-level item
   - Click the item name to set it (e.g., "Sword")
   - Set the quantity you want to craft

2. **Add ingredients**:
   - Click the "+" button below the item to add ingredients
   - Name each ingredient and set quantities
   - Continue adding sub-ingredients as needed

3. **Track progress**:
   - Mark items as complete when you have them
   - View the materials list in the left panel
   - See total quantities calculated automatically

## 🎯 Use Cases

- **Game Crafting**: Plan complex crafting chains in games like Minecraft, Factorio, or Satisfactory
- **Project Planning**: Organize hierarchical task dependencies
- **Recipe Management**: Break down cooking recipes into ingredient lists
- **Manufacturing**: Plan production workflows and bill of materials
- **Education**: Visualize concept dependencies and learning paths

## 🛠️ Advanced Features

### Tree Synchronization
When you reuse an item across multiple recipes, UCRP automatically synchronizes:
- Item names and properties
- Child recipes and dependencies
- Quantities and completion status
- Notes and metadata

### Circular Dependency Handling
UCRP automatically detects and handles circular dependencies by:
- Creating "ghost nodes" that reference the original item
- Preventing infinite loops in calculations
- Maintaining visual clarity with distinct styling

### Export Formats

#### JSON Export
```json
{
  "nodes": [...],
  "items": [...],
  "nextId": 15,
  "nextItemId": 8,
  "treeDirection": true
}
```

#### ASCII Tree View
```
╔══════════════════════════════════════════════════════════════╗
║                      RECIPE TREE VIEW                        ║
╚══════════════════════════════════════════════════════════════╝

└── [✓] Iron Sword
    Qty: 1 | Total: 1
    ├── [ ] Iron Ingot
    │   Qty: 2 | Total: 2
    │   └── [ ] Iron Ore
    │       Qty: 2 | Total: 4
    └── [ ] Wooden Handle
        Qty: 1 | Total: 1
```

#### Materials List
```
╔══════════════════════════════════════════════════════════════╗
║                    REQUIRED MATERIALS                        ║
╠══════════════════════════════════════════════════════════════╣
║ 4x Iron Ore                                                  ║
║ 1x Wooden Handle                                             ║
╚══════════════════════════════════════════════════════════════╝
```

## ⚙️ Technical Details

### Architecture
- **Single-page Application**: All functionality contained in one HTML file
- **Vanilla JavaScript**: No external dependencies
- **CSS Grid/Flexbox**: Responsive layout system
- **localStorage**: Client-side data persistence

### Browser Support
- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge
- Any modern browser with ES6+ support

### Performance
- Optimized for trees with 100+ nodes
- Efficient automatic layout algorithm with caching
- Smooth pan/zoom controls with transform optimization
- Lazy loading of UI elements
- Minimal memory footprint

## 🎨 Customization

### Themes
The application uses CSS custom properties for easy theming:
```css
:root {
   --bg-primary: #1e1e1e;
   --bg-secondary: #2d2d30;
   --bg-tertiary: #252526;
   --accent-color: #007acc;
   --accent-color-hover: #005a9e;
   --text-primary: #cccccc;
   --text-secondary: #999999;
   --text-muted: #6a6a6a;
   --border-color: #3c3c3c;
   --border-color-hover: #4c4c4c;
   --success-color: #4CAF50;
   --success-color-hover: #45a049;
   --warning-color: #ff9800;
   --danger-color: #d73a49;
   --danger-color-hover: #b31d28;
   --info-color: #2aafc7;
   --info-color-light: #1f889b;
}
```

---

### Support

**Made with ❤️ for crafters, planners, and organizers everywhere!**

If you find UCRP helpful and want to support continued development, consider buying me a coffee! ☕

[![Ko-Fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/norway174)

Every contribution helps keep this project free and open-source for everyone to enjoy! 

---

FYI, the whole project. Including this ReadMe is "vibe coded" with AI. lol.  
It works tho! Enjoy!