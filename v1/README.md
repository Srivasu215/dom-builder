# dom-builder

> **Writing HTML is Tough. We Made It Simple.**

`dom-builder` is an all-HTML presentation and documentation suite articulating the real-world struggles of writing HTML &mdash; and how KeshavSoft's declarative JSON architecture solves them.

---

## 📖 The 4 Core Struggles of Real-World HTML

1. **Writing Correct HTML is Tough**: Nested string concatenation and manual `document.createElement` calls are verbose, repetitive, and error-prone.
2. **Composite Controls are Complex**: Real applications require complex composite trees &mdash; **Tables** (`thead`, `tbody`, `tfoot`, row serials `#`, column alignments, calculated totals) and **Forms** (input groups, labels, autocomplete datalists).
3. **Classes & Theming are Not a Small Thing**: Sprinkling CSS classes across hundreds of cells and tags is exhausting. Switching themes (Dark, Light) requires rewriting classes across every element.
4. **Attributes Require Deep Knowledge & Endless Boilerplate**: Remembering and wiring `colspan`, `type="number"`, `align="right"`, `list="datalist-id"`, `id`, `name`, and `placeholder` without missing details.

---

## 💡 How We Made It Simple

- **You declare pure JSON**: Just your data array, column definitions, and layout configurations.
- **Renderers assemble composite controls automatically**: `Table` and `Form` handle all nested tag hierarchies, serial numbers, and calculated footers.
- **Theming via Catalogs**: CSS classes are decoupled into theme dictionaries (`classes.json`). Switch themes with a single method call: `.setTheme({ inTheme })`.
- **Attributes wired automatically**: Column alignments, datalist bindings, and control IDs are linked without manual boilerplate.
- **Compiled to Native DOM**: The `json-to-dom` engine recursively translates the JSON spec into native DOM nodes with zero Virtual DOM overhead.

---

## 📂 The HTML Suite

| File | Purpose | What It Demonstrates |
| :--- | :--- | :--- |
| [**`index.html`**](index.html) | **The Master Story** | Overview of the 4 HTML struggles vs. the declarative solution, side-by-side comparison, and live interactive demo. |
| [**`story.html`**](story.html) | **5-Slide Interactive Presentation** | Full-screen presentation (use Arrow Left/Right keys) walking through each struggle and the declarative breakthrough. |
| [**`table.html`**](table.html) | **The Composite Table** | Deep-dive into automated serials (`#`), column alignments, multi-tier footer sums, formula evaluations (`GST 18%`), and dynamic theme switching. |
| [**`form.html`**](form.html) | **The Composite Form** | Deep-dive into schema-driven input groups, automatic HTML5 `<datalist>` frequency bindings, and control-tree ID indexing. |

---

## 🚀 How to View

This suite is built with **pure HTML, CSS, and JavaScript**:
- **Zero build steps**
- **Zero node_modules**
- **Zero local dependencies**

Simply open [index.html](index.html) or [story.html](story.html) directly in any web browser!

---

## 📄 License

Licensed under the **ISC License**. Developed by [KeshavSoft](https://github.com/keshavsoft).
