# Eminence Web Developer Portfolio (Module 02 Final Project)

## Project name and description

**Eminence | Web Developer Portfolio** is a complete multi-page website built with **HTML only**. It presents Eminence as a web developer: who he is, the services he offers, short blog posts, how to get in touch, and a full project application form.

There is no CSS, no JavaScript, no framework, no template, and no inline style attribute. The plain appearance is intentional. This project is about structure, meaning, accessibility, and correctness.

## Folder structure

```
website/
├── index.html
├── about.html
├── services.html
├── blog.html
├── contact.html
├── README.md
├── images/
│   ├── profile.jpg
│   ├── kings-palace-estate.jpg
│   ├── html-structure-diagram.png
│   ├── divider.svg
│   └── favicon.png
├── media/
│   ├── intro.mp4
│   ├── intro.vtt
│   ├── intro.m4a
│   └── intro.mp3
└── pages/
    └── application.html
```

## Pages included

| Page | Purpose |
|---|---|
| `index.html` | Home page with introduction, profile figure, featured project, and links to other pages |
| `about.html` | Story, skills, planning process, web terms, and a video and audio introduction |
| `services.html` | Services offered, a package comparison table, and how a project works |
| `blog.html` | Three short blog posts, each in an `article` element |
| `contact.html` | Email and GitHub links, common questions, and a link to the form |
| `pages/application.html` | Complete project application form, in a child folder |

## HTML features used

- **Document structure:** `<!DOCTYPE html>`, `lang="en"`, UTF-8, title, description, viewport, author, and a favicon on every page.
- **Landmarks:** `header`, `nav`, `main`, `section`, `article`, `footer`, and `address`. A skip link is the first element on every page.
- **Headings:** one `h1` per page, with `h2` and `h3` in logical order.
- **Text meaning:** paragraphs, `strong` for importance, `em` for emphasis, `blockquote`, `code`, `pre`, and `time`.
- **Lists:** unordered lists (skills, services), ordered lists (planning steps, project steps), and description lists (web terms).
- **Links:**
  - relative links in the same folder, for example `about.html`
  - a link into a child folder, `pages/application.html`
  - a link back to the parent folder, `../index.html`
  - fragment links on the same page and across pages, such as `#featured-project` and `services.html#packages`
  - external HTTPS links that open safely with `rel="noopener noreferrer"`
  - email links using `mailto:`
- **Images:** meaningful `alt` text, an empty `alt` on the decorative divider, `width` and `height` on content images, and `figure` with `figcaption`.
- **Media:** native `video` with captions (`track`), native `audio` with two `source` files, and fallback text for both.
- **Table:** a real data table with `caption`, `thead`, `tbody`, and `th` header cells with `scope`.
- **Form:** text, email, telephone, URL, select with `optgroup`, radio buttons, checkboxes, and textarea, each with a `label`. Controls are grouped with `fieldset` and `legend`, and use constraints (`required`, `minlength`, `maxlength`, `pattern`) and a submit button.
- **Native interactive elements:** `details` and `summary` for the FAQ, all usable with the keyboard.

## Validation

Each page was checked with the W3C Nu HTML Checker at https://validator.w3.org/nu/ using the **Text Input** or **File Upload** option.

| Page | Result |
|---|---|
| `index.html` | Add result after validating |
| `about.html` | Add result after validating |
| `services.html` | Add result after validating |
| `blog.html` | Add result after validating |
| `contact.html` | Add result after validating |
| `pages/application.html` | Add result after validating |

Screenshots of each result are submitted as validation evidence.

## Publishing with GitHub Pages

The GitHub Actions workflow in `.github/workflows/pages.yml` publishes the site from the repository root whenever a commit is pushed to `main`. After the first push, GitHub Pages is enabled automatically and the deployed URL is available in the repository's **Settings → Pages** and in the workflow run.

## What I learned

- Choosing elements for their **meaning** makes a page easier for screen readers, keyboards, and search engines to understand.
- Relative paths depend on where the current file is: `../` goes up to the parent folder, and `pages/` steps down into a child folder.
- Every form control needs a visible, connected `label`, and related controls belong in a `fieldset` with a `legend`.
- Good alt text describes the purpose of an image, and decorative images should use an empty `alt`.
- A table needs a `caption` and `th` cells so that data cells can be understood in context.
- Validation catches small mistakes that are easy to miss by eye.

## Challenges encountered

- **Git push problems:** GitHub's automatic README made my first pushes fail, so I learned to create the repository empty and to resolve a README merge conflict.
- **Network errors:** a "Could not resolve host" error stopped a push until my connection and DNS worked again.
- **Relative paths:** getting every link in `pages/application.html` to use `../` correctly took careful checking.
- **Writing useful alt text:** describing images in a short sentence without repeating the caption.
- **Form constraints:** choosing patterns and length limits that help users without blocking valid answers.

## Resources and media licences

| Item | Source and licence |
|---|---|
| `images/profile.jpg` | My own portrait, used with my consent |
| `images/kings-palace-estate.jpg` | Cropped screenshot of my own Kings Palace Estate project (https://kingspalaceestate.netlify.app/) |
| `images/html-structure-diagram.png` | Created by me for this project |
| `images/divider.svg` | Created by me for this project |
| `images/favicon.png` | Created by me for this project |
| `media/intro.mp4`, `media/intro.vtt` | Created for this project. The visuals use my own images, and the voice is computer-generated |
| `media/intro.m4a`, `media/intro.mp3` | Created for this project. The voice is computer-generated |

External pages are linked, not copied: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#alt), my [GitHub profile](https://github.com/emmanueleminence1), and the [Kings Palace Estate website](https://kingspalaceestate.netlify.app/). No third-party images, audio, video, fonts, or code are included.

The contact email `hello@example.com` is a placeholder and should be replaced with a real public address. The form sends nothing to a server. It uses a `mailto:` action, and no passwords or private information are collected.
