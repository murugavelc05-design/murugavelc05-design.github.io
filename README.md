# TUVI Landing Page

The official landing page website for **TUVI — Money, made clearer.** 
Designed to be hosted entirely on GitHub Pages as a lightweight, static site.

## Features

- **Premium Dark Theme**: Modern UI built with raw CSS and HTML, featuring glassmorphism and subtle glowing accents.
- **Standalone Visuals**: The website utilizes custom CSS visualizations (e.g., CSS Phone Frame, CSS split-bill receipt) and free placeholder avatars (`ui-avatars.com`) to look premium without requiring heavy image assets.
- **Dynamic Legal Pages**: To keep the website and Android app in sync, the `privacy.html` and `terms.html` pages dynamically fetch the raw `.txt` files directly from the `/doc/` folder and format them instantly via JavaScript.

## Directory Structure

```text
/
├── index.html          # Main premium landing page
├── style.css           # Global stylesheet containing the dark theme and layout
├── privacy.html        # Dynamic privacy policy viewer
├── terms.html          # Dynamic terms & conditions viewer
├── /assets/
│   └── tuvi_app_icon.png # The official Tuvi app logo
└── /doc/
    ├── Tuvi_Privacy_Policy.txt       # Raw text file (Update this file to update the site)
    └── Tuvi_Terms_and_Conditions.txt # Raw text file (Update this file to update the site)
```

## How to Update Legal Documents

You do **not** need to edit the HTML files to update your Privacy Policy or Terms & Conditions.

1. Open the `/doc/` folder.
2. Replace or edit the plain text files (`Tuvi_Privacy_Policy.txt` or `Tuvi_Terms_and_Conditions.txt`).
3. Commit and push the changes. The `privacy.html` and `terms.html` files will automatically fetch and format the latest text upon loading.

## Deployment

This website is designed for zero-config deployment via **GitHub Pages**. 
Simply push this directory to the `main` branch of your `your-username.github.io` repository or an equivalent GitHub repository, and enable GitHub Pages in the repository settings.

## Built With
- Pure HTML5
- Pure CSS3 (Flexbox/Grid, Animations)
- Vanilla JavaScript (for text document parsing)
