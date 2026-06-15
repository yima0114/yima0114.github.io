# Yi Ma Artist Website

A simple static portfolio made with HTML and CSS for GitHub Pages.

## Project files

- `index.html` - homepage
- `works.html` - image galleries
- `research.html` - research and archive placeholder
- `cv.html` - CV placeholder
- `contact.html` - contact details
- `style.css` - all visual styling
- `images/` - existing artwork images

No build tools or frameworks are required.

## Preview the website

Open `index.html` in a web browser. The navigation links will work locally and on GitHub Pages.

## Replace an image

The pages use relative image paths such as:

```html
<img src="images/02-metalwork/1-1.jpg" alt="Description of the artwork">
```

To replace an image while keeping the existing page code:

1. Find the image inside its current folder.
2. Replace it with the new image using the exact same filename and file extension.
3. Refresh the browser.

To use a new filename, add the image to the appropriate existing folder and update the `src` path in `index.html` or `works.html`. Paths and filenames are case-sensitive on GitHub Pages.

Keep images inside these folders:

- `images/01-oil-painting-scarf`
- `images/02-metalwork`
- `images/03-color-work`

## Edit captions

Open `index.html` or `works.html` in a text editor. Search for:

```html
<figcaption>Title, medium, dimensions, year.</figcaption>
```

Replace only the text between `<figcaption>` and `</figcaption>`. For example:

```html
<figcaption>Your title, your medium, your dimensions, your year.</figcaption>
```

Comments beginning with `EDIT` mark the main places where text and captions can be changed.

## Add another artwork

In `works.html`, copy one complete `<figure>...</figure>` block inside the correct gallery. Change its image path, alternative text, and caption:

```html
<figure>
  <img src="images/03-color-work/your-image.jpg" alt="Short description" loading="lazy">
  <figcaption>Title, medium, dimensions, year.</figcaption>
</figure>
```

## Publish with GitHub Pages

1. Create a GitHub repository.
2. Upload all website files and the complete `images` folder to the repository root.
3. Make sure `index.html` is at the top level of the repository.
4. In the repository, open **Settings**, then **Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and the `/(root)` folder, then save.
7. Wait for GitHub to publish the site, then use the **Visit site** link on the Pages settings screen.

GitHub's current instructions are available in [Configuring a publishing source for your GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

After publishing, push or upload future edits to the same branch. GitHub Pages will publish the updated files automatically.
