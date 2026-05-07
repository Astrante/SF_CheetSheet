# Refactor sf-cheatsheet.html → Horizontal Tree + Nav Panel

Refactor the file from a radial mind-map into a horizontal tree layout. Keep all existing data (`TOPICS`), flip-cards, dark/light theme, IBM Plex fonts, and accessibility.

---

## 1. Horizontal Tree (main view)

- Root **"Salesforce"** centered; branches go **left and right** symmetrically
- Nodes — rounded rectangles; connecting lines colored per group (`--color-*`)
- Each non-leaf node has a **[+]/[−]** collapse/expand toggle
- Render in **SVG**; 4 hierarchy levels (Platform & Config, Development, UI & Frontend, Automation & Integration, Tools & Process, AI — split left/right)
- On mobile (< 768px) → switch to vertical top-down tree or indented list

## 2. Navigation Panel

- **☰ button** pinned top-right → slide-in panel with a **vertical accordion** mirroring the tree
- Clicking any item navigates to its content view and closes the panel

## 3. Content View

- Clicking a node **replaces** the tree with a content view (hash routing, no reload)
- **Breadcrumb** at top (clickable): `Salesforce › Development › Apex`
- Sub-topics as **compact accordions** in a CSS grid:
  ```css
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  ```
- Inside each accordion — existing **flip-cards** in adaptive grid (~200px)
- Cards support **drag-and-drop reorder** within their group only (use SortableJS)
- **"Back to Tree"** link returns to the main view

## 4. Preserve

| What | How |
|---|---|
| Flip-cards | Unchanged |
| Dark/light theme | Keep toggle + `prefers-color-scheme` |
| Accessibility | `aria-expanded`, keyboard nav (Tab / Enter / Space) |
| IBM Plex fonts | Sans for UI, Mono for code |
| `TOPICS` data | Derive tree from it, don't restructure |

## 5. Output

Single self-contained **`sf-cheatsheet.html`** — all CSS/JS inlined. CDN links for fonts and SortableJS are fine.
