# ACME Supplies – Intelligent Websites test front end

Static HTML and CSS for contract HCP-140. No scripts, no fixed words; every visible word is in a slot.

## Pages
- `home.html` – heading, text, `home.image`
- `category.html` – category title, heading, text and image, then the product grid
- `product.html` – product fields, categories, add-to-basket form
- `basket.html` – empty and full states, lines, total, checkout
- `notfound.html` – heading and text

Every page shares the same header (site name, basket link), category nav and footer (footer and contact text).

## Assets
- `assets/site.css` – the only stylesheet, linked as `/assets/site.css`

## Fonts
- Public Sans 400, 600, 700 (Google Fonts), falling back to the system sans-serif

## Design notes
- Nav indenting comes from `data-iw-depth` (0 to 3 styled, 16 px per level).
- Repeated slots hold two to four samples to show the layout; only the first is the template.
- Image slots have no `src`. Grey boxes show the reserved space, sized in CSS (wide 21:9, product 1:1).
- `<title>` carries `data-iw-text="site.name"`.
- Forms have no `action` or `method`; the product adds these.
- Colours: ink #1d1c1a, background #faf9f7, accent #a3361c (buttons, hover).
