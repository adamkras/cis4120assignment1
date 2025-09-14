# Path@Penn Mobile Prototype

# Author: Adam Krasilovsky

A prototype that simulates a mobile Path@Penn workflow with **three screens**:

- **Search** — keyword input, “don’t overlap” checkbox, and **multi-select** filter pickers that open modals and show selection counts.
- **Course (CIS 1200)** — lecture/recitation choices and a schedule preview grid.
- **Schedule (Dashboard)** — summary tiles and cart cards showing **Seats remaining** and an **Add/Added** state. The CIS 4120 card includes a **Permission Request** row.

---

## Files
/
├─ index.html # Markup + small inline JS for screen switching, modals, and button state
├─ styles.css # Styles for layout, modals, cards, and schedule grid
└─ README.md # This file

## How to Run

You can open the file directly or serve it locally.

## Screen switching
- Register tab -> Search screen
- Schedule tab -> Schedule dashboard
- Search button on the Search screen -> Course (CIS 1200) screen

## Multi-select pickers (Advanced Search)
- Buttons: Subject, School, Level, Schedule Type, Credit, Campus/Online, Class Status, Part of Term, Honors.
- Each button opens a modal with checkboxes.
- The button turns green when at least 1 item is selected.
- The inline label shows “(N selected)”.
- Done applies current selections. Clear unchecks all.
- Clicking the dimmed backdrop closes the modal.

## Course (CIS 1200)
- Lecture/recitation rows show availability (green border for available, yellow-orange for full).
- The schedule grid highlights the selected blocks (along with already registered courses).

## Schedule (Dashboard)
- Each course card shows Seats remaining (bottom-left).
- The action button (bottom-right) toggles between Add (red) and Added (green).
- CIS 4120 shows a Permission Request line with an Approved badge.
