# Irena | Author Website

The official website of Irena, author of **The Gate of Ararich**, a young adult fantasy about parallel worlds and magical adventures.

Live site: https://YOUR-USERNAME.github.io

## About this site

A simple, static three-page website. There is no build step: edit a file, push it, and the live site updates.

- **Home** (`index.html`): about the author and a teaser for the book
- **The Book** (`book.html`): full description and the Amazon link
- **Contact** (`contact.html`): contact form

Built with plain HTML and [Tailwind CSS](https://tailwindcss.com) (loaded from a CDN). Fonts are Fraunces and DM Sans from Google Fonts. The contact form is handled by [Web3Forms](https://web3forms.com).

## Project structure

```
/
├── index.html
├── book.html
├── contact.html
├── images/
│   ├── author.jpg    (author portrait, roughly 4:5, under 500 KB)
│   └── cover.jpg     (book cover, roughly 2:3)
└── README.md
```

## Editing the site

1. Open the folder in a code editor such as VS Code.
2. Edit the text or swap the images. To replace a photo, keep the same file name.
3. Preview locally by opening `index.html` in a browser, or use the Live Server extension in VS Code.
4. Commit and push (GitHub Desktop works well). GitHub Pages updates within a couple of minutes.

The header and footer are repeated in each HTML file, so if you change the navigation or footer links, change them in all three files.

### Common edits

| What | Where |
| --- | --- |
| Bio text | `index.html`, top section |
| Book description | `book.html` |
| Amazon link | `book.html`, the "Buy on Amazon" button |
| Instagram and Goodreads links | Footer of all three pages |
| Colors | The `tailwind.config` block at the top of each file (`ink`, `paper`, `accent`) |

## Still to do

- [ ] Add `images/author.jpg` and `images/cover.jpg`
- [ ] Add the Goodreads link in the footer (currently `href="#"`) on all three pages
- [ ] Optional: connect a custom domain under Settings, then Pages

## Contact form

The form posts to Web3Forms, which emails each message to the inbox it was registered with. The access key in `contact.html` is public by design: it can only send messages to that one inbox. To change where messages go, create a new access key at [web3forms.com](https://web3forms.com) and replace the `access_key` value in `contact.html`.

## Deployment

The site is hosted on GitHub Pages from the `main` branch (root folder). To set it up: **Settings, then Pages, then Branch: `main` and `/ (root)`, then Save**.

## Credits

Website by [YOUR NAME]. Book and content &copy; Irena. All rights reserved.
