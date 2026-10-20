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

## 📂 Repository Structure

```text
dom-builder/
│
├── index.html                  <-- Master Portal (Clean, simple, live tabs, quickstart)
├── playground.html             <-- Interactive Live Sandbox (edit JSON & mount live)
├── story.html                  <-- 5-Slide Full-screen Presentation
│
├── json-renderers/             <-- Complete documentation & component suites for json-renderers
│   ├── index.html              <-- Documentation hub & runtime guide
│   ├── table.html              <-- Composite Table deep-dive (simple, withFooter, alignments)
│   ├── datalist.html           <-- HTML5 Datalist autocomplete guide
│   ├── select.html             <-- Select dropdown guide
│   ├── form.html               <-- Composite Form guide
│   ├── subDoc/                 <-- Conceptual house-building & advanced mental models
│   │   ├── simpleDoc.html
│   │   ├── advanceDoc.html
│   │   └── index.html
│   └── samples/                <-- Step-by-step CDN and window.ks sample tracks
│       ├── table/
│       ├── datalist/
│       └── select/
│
├── json-to-tag/                <-- Tag generation & engine
│   ├── tags.html               <-- Tag generator workbench
│   └── engine.html             <-- Native DOM synthesis deep-dive
│
├── v1/                         <-- Archived v1
└── v2/                         <-- Archived v2
```

---

## 🚀 How to View

This suite is built with **pure HTML, CSS, and modern JavaScript**:
- **Zero build steps**
- **Zero node_modules**
- **Zero local dependencies**

Simply open [index.html](index.html) or [playground.html](playground.html) directly in any web browser!

---

## 📄 License

Licensed under the **ISC License**. Developed by [KeshavSoft](https://github.com/keshavsoft).
