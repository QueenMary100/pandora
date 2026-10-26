# Pandora

An e-commerce demo site (sneakers, headphones, bags and watches) built page by page during the eMobilis HTML, CSS and Bootstrap course. Each page practises one topic from class.

## How to open it

- Easiest: open `index.html` in any browser (double-click it), then use the links.
- Recommended: open this folder in VS Code and click **Go Live** (Live Server extension) while `index.html` is open.

There is nothing to install or build, and the project works offline.

## Pages

| Page | What it shows | Styling | Class |
|---|---|---|---|
| `index.html` | Boilerplate, title, `h1`, paragraphs, text formatting tags (`b`, `i`, `u`, `mark`), New Arrivals with a button, Featured Deals with 10 images, navigation links with `target` examples, footer | External `css/style.css` plus one inline example | 2, 3, 5 |
| `about.html` | Company story, lists, an image, links | `css/style.css` | 2, 3, 5 |
| `contact.html` | Contact details (description list), opening hours (table), a simple contact form | `css/style.css` | 3, 5 |
| `payment.html` | Payment methods table, ordered steps, FAQ (description list) | `css/style.css` | 3, 4 |
| `products.html` | Top four ordered list, `hr`, men's clothing unordered list, plus the assignments: nested list, description list and list marker variations with `list-style-type` | Internal CSS | 4 |
| `services.html` | Customer support `div` (`#customer`, `#paragraph`), "Why choose us" flex section (`#main`, `.one`) | External `css/services.css` | 4 |
| `employee.html` | Employee table (`border-collapse`, centred cells), plus a roster table using `colspan` and `rowspan` | Internal CSS | 3 |
| `register.html` | Full registration form: text, email, password, date, datetime-local, tel, number, file, plus dropdown, radio buttons, checkboxes, textarea and a styled button | External `css/register.css` (form box, legend, attribute selectors) | 5 |
| `inventory.html` | Bootstrap table, buttons, text and background utilities, `container`, `d-flex` with `gap` and `text-center`, `row` and `col` grid | Bootstrap only | 6 |
| `login.html` | Login form with remember-me checkbox | Bootstrap classes only (no custom CSS file) | 6 |

## Folder structure

```
pandora/
  index.html, about.html, contact.html, payment.html
  products.html, services.html, employee.html, register.html
  inventory.html, login.html
  css/        style.css, services.css, register.css
  assets/     10 product images (SVG) and logo.svg
  bootstrap/
    css/      bootstrap.min.css
    js/       bootstrap.bundle.min.js
```

HTML files stay in the project folder. Everything else lives in a sub-folder.

## Bootstrap

Bootstrap 5.3.3 is supplied **locally** (official `bootstrap-5.3.3-dist` release from the Bootstrap project, MIT licence). The two pages that use it link it in the `head`:

```html
<link rel="stylesheet" href="bootstrap/css/bootstrap.min.css">
<script src="bootstrap/js/bootstrap.bundle.min.js" defer></script>
```

In class the instructor linked `bootstrap.min.js`. This project uses `bootstrap.bundle.min.js` instead because it includes Popper, which Bootstrap needs for dropdowns, tooltips and popovers. Both files are loaded the same way. The `.map` files next to them are only used by browser developer tools and can be deleted.

## Images

The product pictures in `assets/` are simple illustrations drawn for this project (SVG), so there are no copyright or hot-linking issues. Keep file names short and lowercase, and keep the original extension. To use real photos, drop them into `assets/` and update the `src` and `alt` in the pages.

## Notes

- `register.html` and `contact.html` forms use `action="#"`: they only display the form. Saving data needs a back end, which comes later in the course.
- The `<marquee>` tag from class 3 is not used: it is obsolete in HTML5 and fails validation.
- Phone number, email, address and employee names are made up for the demo.
