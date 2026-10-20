# dom-builder

> **Writing HTML is Tough. We Made It Simple.**

`dom-builder` is an all-HTML presentation, interactive showcase, and documentation suite articulating the real-world struggles of writing HTML &mdash; and demonstrating how KeshavSoft's modern declarative JSON architecture solves them.

---

## 📖 The 4 Core Struggles of Real-World HTML

1. **Writing Correct HTML is Tough**: Nested string concatenation and manual `document.createElement` calls are verbose, repetitive, and error-prone.
2. **Composite Controls are Complex**: Real applications require complex composite trees &mdash; **Tables** (`thead`, `tbody`, `tfoot`, row serials `#`, column alignments, calculated totals) and **Forms** (input groups, labels, autocomplete datalists).
3. **Classes & Theming are Not a Small Thing**: Sprinkling CSS classes across hundreds of cells and tags is exhausting. Switching themes requires rewriting classes across every element.
4. **Attributes Require Deep Knowledge & Endless Boilerplate**: Remembering and wiring `colspan`, `type="number"`, `align="right"`, `list="datalist-id"`, `id`, `name`, and `placeholder` without missing details.

---

## 💡 The Modern 3-Tier Architecture

KeshavSoft solves this with a clean, decoupled 3-tier pipeline:

```
┌───────────────────────────────────────┐
│        1. Guard Layer                 │
│   (json-renderers-guard)              │
│   • Validates types & compulsory keys │
└──────────────────┬────────────────────┘
                   ▼
┌───────────────────────────────────────┐
│        2. Headless Spec Builder       │
│   (json-renderers-build)              │
│   • Table (simple, withFooter, etc.)  │
│   • Datalist, Select, Form            │
└──────────────────┬────────────────────┘
                   ▼
┌───────────────────────────────────────┐
│        3. Fast Native DOM Mount       │
│   (json-renderers + json-to-tag)      │
│   • Synthesizes native DOM elements   │
│   • Mounts into target container      │
└───────────────────────────────────────┘
```

---

## 📂 The Interactive HTML Suite

| File | Purpose | What It Demonstrates |
| :--- | :--- | :--- |
| [**`index.html`**](index.html) | **The Master Story** | Overview of the 4 HTML struggles vs. the declarative solution, the 3-tier architecture, and live tabbed demos. |
| [**`story.html`**](story.html) | **5-Slide Interactive Presentation** | Full-screen presentation (use Arrow Left/Right keys) walking through each struggle and the declarative breakthrough. |
| [**`table.html`**](table.html) | **Composite Table Suite** | Deep-dive into automated serials (`#`), column alignments, multi-tier footer sums, and modular builders (`simple`, `withFooter`, `headerOnly`, `bodyOnly`, `footerOnly`). |
| [**`datalist.html`**](datalist.html) | **Datalist Autocomplete** | Declarative HTML5 `<datalist>` suggestion popovers generated directly from JSON arrays with live search inputs. |
| [**`select.html`**](select.html) | **Select Dropdowns** | Declarative `<select>` dropdowns and option lists with live interactive selection handlers. |
| [**`form.html`**](form.html) | **Composite Form** | Schema-driven input groups, automatic autocomplete datalist bindings, and control indexing. |
| [**`playground.html`**](playground.html) | **Live Playground / Sandbox** | Interactive real-time sandbox to edit JSON specs and immediately see rendered DOM components. |

---

## 🚀 How to View

This suite is built with **pure HTML, CSS, and modern JavaScript**:
- **Zero build steps**
- **Zero node_modules**
- **Zero local dependencies**

Simply open [index.html](index.html), [table.html](table.html), or [playground.html](playground.html) directly in any web browser!

---

## 📄 License

Licensed under the **ISC License**. Developed by [KeshavSoft](https://github.com/keshavsoft).
