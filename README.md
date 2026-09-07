# Academic GitHub Pages homepage

A minimalist personal homepage for a researcher in graph theory.

## 1. Replace personal information

Open `index.html` and replace:

- `YOUR NAME`
- `YOUR POSITION`
- `YOUR INSTITUTION`
- `YOUR DEPARTMENT`
- `YOUR CITY, COUNTRY`
- `YOUR_EMAIL@example.com`
- `YOUR_USERNAME`

## 2. Publications are grouped by year

The publication section is organized in descending year order, for example:

- 2026
- 2025
- 2024

Within each year, published papers and arXiv preprints can appear together.

Each paper is an expandable `<details>` block. Clicking the title area opens a lower panel containing the abstract and links.

### Unpublished paper

Use:

- badge: `Preprint`
- bibliographic line: `arXiv:xxxx.xxxxx, YEAR`
- buttons: `arXiv` and `PDF`

### Published paper

Use:

- badge: `Published`
- bibliographic line: journal name, volume/year/pages as appropriate
- buttons: `Journal`, `DOI`, `PDF` (and optionally `arXiv`)

## 3. Upload paper PDFs

Put PDF files in the `papers/` folder, for example:

`papers/balanced-subdivisions-2026.pdf`

Then use this in `index.html`:

```html
<a class="paper-button" href="papers/balanced-subdivisions-2026.pdf" target="_blank">PDF</a>
```

## 4. Add a new paper

Copy one complete block beginning with:

```html
<details class="paper-entry">
```

and ending with:

```html
</details>
```

Paste it inside the correct year's `<div class="paper-list">`.

Change the title, authors, journal/arXiv information, abstract, and links.

For a new year, copy an entire `<section class="publication-year">...</section>` block and change the year.

## 5. Add your CV

Put your CV in the repository root and name it:

`cv.pdf`

## 6. Add a profile photo

Put an image such as `photo.jpg` in the repository and replace the photo placeholder in `index.html` with:

```html
<img class="portrait-photo" src="photo.jpg" alt="YOUR NAME">
```

Then add to `style.css`:

```css
.portrait-photo {
  width: 100%;
  aspect-ratio: 4 / 5;
  object-fit: cover;
  border-radius: 10px;
  display: block;
}
```

## 7. Publish with GitHub Pages

Create a repository named exactly:

`YOUR_USERNAME.github.io`

Upload all files to the repository root, then go to:

`Settings -> Pages`

Choose:

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/(root)`

## 8. Mathematical notation

MathJax is enabled, so abstracts may contain LaTeX such as:

```html
\(K_{s,t}\), \(\mathrm{ex}(n,H)\), \(d(G)\)
```
