# Vũ Lê Đình Hoàng — Portfolio

A dependency-free, one-page portfolio for Computer Vision, Applied AI, and Embedded AI internship applications. It is designed for GitHub Pages and works without a build step.

## Folder structure

```text
docs/
├── index.html
├── styles.css
├── script.js
├── README.md
├── assets/
│   ├── cv/
│   │   ├── Le_Dinh_Hoang_Vu.pdf
│   │   └── Le_Dinh_Hoang_Vu_Embedded_AI.pdf
│   └── images/projects/
│       └── wsl-dr-grad-cam.png
└── data/
    └── projects.json
```

## Preview locally

Open `docs/index.html` directly in a browser. For the same path behavior as GitHub Pages, run:

```powershell
cd docs
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Update project information

Edit the matching project article in `index.html`, then keep `data/projects.json` in sync. The HTML contains the display content so the portfolio still works when opened directly with a `file://` URL.

## Replace CV files

Replace the PDFs in `assets/cv/` while keeping these filenames:

- `Le_Dinh_Hoang_Vu.pdf`
- `Le_Dinh_Hoang_Vu_Embedded_AI.pdf`

## Add screenshots

1. Copy an optimized PNG, WebP, or JPEG into `assets/images/projects/`.
2. Add an `<img>` or `<figure>` to the relevant project card in `index.html`.
3. Write specific alt text describing what the image shows.

## Deploy with GitHub Pages

1. Push the repository to GitHub.
2. Open the repository **Settings**.
3. Go to **Pages**.
4. Select **Deploy from a branch**.
5. Choose branch **main**.
6. Choose folder **/docs**.
7. Save.
8. Wait for the GitHub Pages URL.

No package install, build command, or backend is required.
