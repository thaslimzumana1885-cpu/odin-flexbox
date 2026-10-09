# The Last Kingdom - Landing Page

A beautifully themed, fully semantic landing page based on **The Last Kingdom** TV series. This project transforms a structural mockup into a medieval-inspired fan portal using modern HTML5 layout semantics and custom CSS styles.

---

## 🛠️ Project Structure & Architecture

The application layout is structured cleanly across semantic HTML blocks and matching modular CSS declarations:

| Component / Section | HTML Element / Class | CSS Selector & Purpose |
| :--- | :--- | :--- |
| **Global Shell** | `<body>` | Handles base viewport rendering height (`100vh`). |
| **Top Hero Panel** | `<div class="container">` | Uses `#1f2937` background wrapper containing header navigation and hero split pane. |
| **Navigation Bar** | `<div class="header">` | Handles space tracking via `flexbox` layout with an automatic left-margin alignment menu. |
| **Hero Pane Split** | `<div class="split">` | Coordinates left-aligned introductory typography (`.top`) with right-aligned scene image (`.image`). |
| **Feature Cards Section** | `<div class="middle">` | Wraps a centered section header and an explicit horizontal visual element alignment loop (`.cards`). |
| **Content Cards** | `<div class="card">` | Isolated flexible boundary box (`400px` by `450px`) setting custom inner spacing and image border radius tweaks. |
| **Quote Callout** | `<div class="description">` | Custom italic block styling utilizing a soft background tint layer (`#e5e7eb`) with custom horizontal tracking buffers. |
| **Call To Action Banner**| `<div class="float">` | Explicitly sized container (`800px`) using `#3882f6` coloring, matching text layouts with an action button setup. |
| **Site Footer Bar** | `<div class="footer">` | Dark-tint block managing centered block configurations for social elements and system text loops. |

---

## 🚀 Getting Started & Local Setup

To quickly run and review this webpage structure locally, execute the following actions sequentially:

1. **Clone or Download the Project Sources:** Ensure both the `index.html` file and your `styles.css` file sit inside the exact same root directory folder.
2. **Launch a Local Web Server Instance:**
   * If you are utilizing **VS Code**, install the extension [Live Server by Ritwick Dey](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer "Live Server VS Code Extension"). Open your project folder, look at the bottom-right status bar, and click **Go Live**.
   * Alternatively, if you have Python available locally on your system terminal, start a server directly inside your workspace folder using:
     ```bash
     python -m http.server 8000
     ```
3. **Open and Preview:** Direct any modern web browser safely to your active port string (e.g., `http://localhost:5500` or `http://localhost:8000`).

---

## ✍️ Modifying and Extending Content

Follow these direct structural modification procedures when adding extra content layers to your web app layout:

### How to Append a New Feature Card
To safely insert a new character or feature module block without breaking structural symmetry, apply these sequential updates within the main `.cards` wrapper element:
1. Open your `index.html` script configuration file.
2. Locate the parent wrapper container block designated with class markup `class="cards"`.
3. Directly paste a fresh structural card element right after the last existing card block:
   ```html
   <div class="card">
       <img src="YOUR_IMAGE_LINK_HERE" alt="Descriptive alternative placeholder text">
       <h5>New Character Label</h5>
       <p>Provide a descriptive theme sentence showcasing the character's legacy or battle significance.</p>
   </div>
   ```
4. *Note:* Because the backing styling rules contain `flex-wrap: wrap;` configurations inside `.cards`, inserting a fifth element automatically pushes it down smoothly into an aligned second row line layout.

### Updating or Changing the Main Quotes
To update the core central thematic testimonial or historical quote:
1. Locate the block designated with class container markup `class="description"`.
2. Swap out the string content sitting comfortably inside the structural header level three block `<h3>...</h3>`.
3. Change the corresponding alignment citation parameter tracking tag underneath inside `<p> - Author</p>`.

---

## 🎨 Future Layout Optimization Tips

To make the styling variables even cleaner and resolve structural conflicts present in the foundational CSS setup, consider implementing these layout enhancements later:
* **Normalize Button Scale Rules:** The default globally declared target marker button rule handles font size sets at `font-size: 35px;`. Consider separating these out via strict modular scoping naming patterns (e.g., creating unique classes like `.btn-primary` and `.btn-outline`) to prevent structural sizing overflow inside your narrow float banner.
* **Convert Explicit Container Width Boundaries:** Your current call-to-action layout `.float` is bound tightly to a fixed hardware pixel boundary rule set to `width: 800px;`. To make sure the text panels fluidly break and reshape nicely across small phone interfaces, consider switching that directly to dynamic percent rules like `max-width: 800px; width: 100%;`.
