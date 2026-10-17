# Daud Warsame — Student Portfolio

A single-page student portfolio for the WEEK06 HCI lab. It uses HTML and CSS only: no JavaScript, frameworks, downloaded templates, external fonts, or tracking.

## Purpose and audience

The goal is to introduce Daud Abdulkadir Warsame, show his current learning and project ideas, and organise his skills clearly. The audience is lecturers, classmates, and people interested in student collaboration.

## Planning and design

The page follows this order: header and navigation, introduction, about, projects, skills, contact, and footer. Visitors can move directly to a section using the navigation. Projects have clear status labels so a proposal is not mistaken for a finished website.

Desktop uses side-by-side content. Mobile stacks sections and keeps every navigation link visible, avoiding a JavaScript menu. The project notes use native HTML `details` and `summary` elements.

Colours:
- Paper background: `#f6f5ee`
- Dark green text and buttons: `#1b342e`
- Muted green: `#53665f`
- Orange hover accent: `#aa4526`
- Pale green section: `#e9eddf`

Fonts: Arial for body text and headings; Georgia for italic highlights. Both are system fonts, so no font download is required. The initials illustration is intentional; no fake profile photo is used. All SVG artwork was created for this exercise.

### Design files

`design/desktop-plan.svg` and `design/mobile-plan.svg` are planning artboards made before final packaging. They are editable SVGs, not a Figma or Canva export and not screenshots of the running website. The `.png` versions are image previews of these plans.

The assignment still requires a design created in Figma or Canva, a screenshot, and a share link. Bring these SVGs into your chosen design tool, review and customise the layouts, save the file, then capture the design and copy its share link. Check the final design against the implemented page.

## Files

- `index.html`: page structure and content
- `style.css`: colours, layout, spacing, hover effects, and responsive rules
- `images/`: local illustrations for the hero and projects
- `design/`: desktop and mobile planning artboards
- `SUBMISSION.md`: remaining requirements and email template

## Run locally

1. Extract the ZIP file.
2. Open the `portfolio` folder in VS Code.
3. Open `index.html` in a browser, or use your installed Live Server extension.
4. Keep `index.html`, `style.css`, and `images` together so the relative paths work.

## Understand the code

- `header`, `nav`, `main`, `section`, `article`, and `footer` describe the purpose of the content.
- Links such as `href="#projects"` point to an element with `id="projects"`.
- The CSS `.container` limits the page width while leaving space on both sides.
- Flexbox arranges navigation, hero content, project cards, and other sections.
- `box-sizing: border-box` includes padding and borders in an element's width.
- `max-width: 100%` keeps images within their container.
- Media queries at 900px and 600px adjust spacing and stack content on smaller screens.
- `clamp()` lets heading sizes grow with the screen while keeping a minimum and maximum size. If this is new in class, read the three values as minimum, preferred, and maximum.
- `details` opens and closes project notes without JavaScript.
- `:hover` changes link and button appearance; `:focus-visible` helps keyboard users see the selected control.
- The reduced-motion rule turns off smooth scrolling and transitions for visitors who prefer less motion.

## Personalise before submission

1. The contact email is `daauuddaada77@gmail.com`. Check that it is correct and test its email link.
2. Check the biography and project descriptions. Remove or rewrite anything you cannot explain or do not want to publish.
3. Make your own design or content changes and describe them honestly in this README.
4. Add your actual repository, live website, and Figma/Canva links to `SUBMISSION.md`.
5. Do not publish your Student ID or private phone number in this repository. Put the required Student ID in the submission email.

## Testing

Static source checks were performed for section links, local assets, HTML structure, CSS parsing, and the absence of JavaScript. The SVG files were checked as XML. Browser testing and the hosted W3C checks have NOT been completed in this environment.

Before submission, use your browser's responsive view at 1440px desktop, 768px tablet, and 390px mobile. Also check 320px width and zoom to 200%.

Check that:
- There is no sideways page scrolling or overlapping text.
- Navigation and Back to top move to the correct sections.
- Each project note opens and closes.
- Images load and text stays readable.
- Tab moves through links and summaries, and the focus outline is visible.
- The email link opens an email application using your email application.
- The hover effect changes the main button colour and lifts it slightly.

Record the results you actually observe. Do not claim that a test passed before running it.

## GitHub Pages and validation

Publish this static folder using GitHub Pages. Put `index.html` at the root of the publishing source, with `style.css` and `images` alongside it. Do not upload only the ZIP; extract it and upload the actual files.

When a public URL is available, validate it with:
- HTML: https://validator.w3.org/
- CSS: https://jigsaw.w3.org/css-validator/

Fix any reported errors and check the deployed page again. No deployment or validator result is claimed in this package.

## AI assistance

ChatGPT helped prepare the initial layout, content, illustrations, HTML/CSS, and documentation. This is an AI-assisted starter. The student still needs to understand the code, personalise it, test it in a browser, and complete the design and deployment work. The assignment warns against submitting unchanged AI-generated work or code that the student does not understand.
