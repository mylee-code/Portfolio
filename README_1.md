# Myles Lee — Personal Portfolio

> A hand-built personal website that introduces who I am, what I'm learning at i.c.stars, and the projects I've worked on.

![Portfolio home page](docs/screenshot.png)

**Live site:** https://mylee-code.github.io/Portfolio/

---

## Overview

This is a one-page portfolio website built with plain HTML, CSS, and a small amount of JavaScript. It has four sections:

| Section | What it shows |
|---|---|
| **About** | My background, my goal of working in data analysis, and my interests outside of tech |
| **Skills & Learning** | Clickable skill "chips" that expand to show what I've learned in tech and business |
| **Projects** | A stop-motion short film, a car restoration, and this portfolio itself |
| **Contact** | Email and GitHub links |

## Why I Built This

I'm an intern at **i.c.stars**, where I'm learning both technology and the business side of how organizations run. I built this site to:

- **Show employers who I am** beyond a resume: my skills, my growth, and the hands-on projects I enjoy.
- **Practice real web development** by writing HTML and CSS by hand instead of using a website builder.
- **Practice a professional Git workflow**, with version control, clear commit messages, and branches and pull requests.

The site is a living project. It grows as I learn new skills.

## Tech Stack

| Technology | Used for |
|---|---|
| HTML5 | Page structure and content |
| CSS3 | Layout (flexbox and grid), colors, animations, responsive design |
| JavaScript | Scroll fade-in effects and expandable skill descriptions |
| Google Fonts | Space Grotesk (headings) and Inter (body text) |
| Git & GitHub | Version control and hosting |
| GitHub Pages | Free deployment of the live site |

There are no frameworks or packages to install.

## Repository Structure

```
Portfolio/
├── index.html        # The entire website: content, layout, and JavaScript
├── style.css         # All styling: colors, fonts, layout, responsive rules
├── images/           # Photos used on the site, plus SVG fallback illustrations
│   ├── profile.jpg   #   Hero photo        (fallback: profile.svg)
│   ├── engines.jpg   #   About section photo
│   ├── film.jpg      #   Stop-motion project (fallback: film.svg)
│   ├── car.jpg       #   Car restoration     (fallback: car.svg)
│   └── portfolio.jpg #   This portfolio      (fallback: code.svg)
├── docs/             # Screenshots used in this README
└── README.md         # Project documentation (this file)
```

## Setup

All you need is a web browser. Everything the site uses is already in the repository, including every image.

### Option 1: View the live site

Go to **https://mylee-code.github.io/Portfolio/**

### Option 2: Run it on your own computer

1. **Clone the repository**
   ```bash
   git clone https://github.com/mylee-code/Portfolio.git
   cd Portfolio
   ```
   *(Or click the green **Code** button on GitHub, then **Download ZIP**, and unzip it.)*

2. **Open the site.** Double-click `index.html`, or drag it into Chrome, Edge, Firefox, or Safari.

3. **(Optional) Run a local server.** If you have VS Code, install the **Live Server** extension, right-click `index.html`, and choose **Open with Live Server**. The page reloads automatically whenever you save a change.

> **Note:** Fonts load from Google Fonts, so the site looks best with an internet connection. Without one, it falls back to your system font and everything still works.

## How to Use

1. **Navigate:** use the top menu (**About · Skills · Projects · Contact**) to jump to any section.
2. **Explore skills:** in **Skills & Learning**, click any skill chip (for example, *Technology* or *Leadership*) to read a description. Click it again to close it.

   ![Skill chip expanded](docs/skills.png)

3. **View projects:** scroll to **Projects** to see each project with a photo, a description, and tags.
4. **Get in touch:** use the **Contact** buttons to send an email or visit my GitHub.

The layout adjusts for phones and tablets, so you can try resizing the browser window.

## Technical Decisions

- **Plain HTML and CSS instead of a framework (React, Bootstrap, etc.):** I wanted to learn the fundamentals first. It also keeps the site fast, with nothing to install or build.
- **A single page with anchor links:** The content is short enough for one page, and visitors can scroll through my whole story without clicking between pages.
- **CSS custom properties (variables):** All colors are defined once at the top of `style.css`, so I can change the color scheme by editing a few lines.
- **Clickable skill chips:** Long skill descriptions would make the page overwhelming. Hiding them behind a click keeps the page clean while still letting visitors read more.
- **SVG fallback images:** If a photo fails to load, a lightweight illustration appears in its place, so the page never shows a broken image.
- **Accessibility:** I used semantic HTML (`header`, `nav`, `main`, `section`, `article`), alt text on every image, `aria-expanded` on the skill buttons, and I turn off animations for users who have "reduce motion" enabled.
- **GitHub Pages for hosting:** It's free, it deploys straight from this repository, and every push to `main` updates the live site.

## Future Improvements

- Add a SQL / data analysis project to the Projects section
- Add a downloadable resume
- Add a LinkedIn link to the Contact section
- Compress the photos so the page loads faster on mobile
- Move the JavaScript into its own file (`js/main.js`)

## Author

**Myles Lee**: aspiring data analyst and intern at i.c.stars
- GitHub: [@mylee-code](https://github.com/mylee-code)
- Email: mylee@icstars.org
