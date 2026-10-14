# Three years with Sudu

A mobile-first anniversary surprise made with plain HTML, CSS, and JavaScript. It has no build step, account, server, or external library. The default page works on its own; add your own photos and personal words before sharing it.

The entrance uses a date picker. Enter **October 15, 2023** to unlock the page. This is a playful front-end gate, not real security: the date check is in the JavaScript, and files on a public GitHub Pages site can still be accessed directly.

## Project files

```text
three-years-with-sudu/
├── index.html
├── style.css
├── script.js
└── photos/
    └── README.txt
```

## Make it yours

1. Open `script.js` and edit the `surpriseContent` object near the top.
   - `letter`: the typewriter letter, shown one word at a time.
   - `memories`: 22 memory cards. Edit each title, caption, and photo description.
   - `hiddenNotes`: the messages revealed by the stars.
   - `finalMessage` and `signature`: the last reveal.
2. The 22 images currently in `photos/` are already mapped to the memory cards. The first image assigned to **The beginning** is unchanged. Keep these filenames as they are, or update the matching `photo` value in `script.js` if you replace a picture.
3. Use JPG or PNG, and resize very large phone photos before adding them so the page loads quickly on mobile data.
4. Preview `index.html` in a browser. If an image path is missing, that card falls back to its placeholder.

Treat a public GitHub Pages URL as public: only use photos and words you are comfortable sharing with its link.

## Publish with GitHub Pages

1. Sign in to GitHub and create a new repository. On GitHub Free, choose **Public** to use Pages; private-repository Pages requires an eligible paid plan.
2. Upload the contents of this folder (`index.html`, `style.css`, `script.js`, and the `photos` folder) to the repository's top level. Do not upload the outer `three-years-with-sudu` folder as an extra nested directory.
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose the `main` branch and the `/(root)` folder, then click **Save**.
6. Wait for GitHub to finish publishing. The Pages address will be shown on that Settings page. It usually looks like `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`.
7. Open the address in Safari on the iPhone. If it shows an older version, refresh after the Pages deployment finishes.

GitHub's [publishing-from-a-branch guide](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) has screenshots of these settings. **The published Pages website is public on the internet, even if the repository is private**, so only add photos and messages Sudu is happy to share through that link.

You can also upload these same files through GitHub's website: open the repository, choose **Add file → Upload files**, drag in the files, and commit the upload.

## iPhone 7 notes

- The site uses system fonts, small CSS animations, and no remote assets or JavaScript libraries.
- It fits narrow screens and includes safe-area padding, touch-friendly controls, a swipeable memory strip, and a reduced-motion setting.
- Use optimized JPG or PNG images around 1200 pixels on the long edge or smaller. The cards lazy-load photos; compress them so all 22 still load quickly on mobile data.
- Test the published link in Safari before sending it. GitHub Pages is the host; this site needs no backend.
