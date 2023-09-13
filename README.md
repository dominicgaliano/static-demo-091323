A front-end design that I built based on [this figma template](https://www.figma.com/file/nh0V05z3NB87ue9v5PcO3R/writings.dev?type=design&node-id=0%3A1&t=2iQplaIojU3ydAfW-1) as part of the [roadmap.sh](roadmap.sh) full-stack developer path.

[See this project in action here](https://dominicgaliano.github.io/static-demo-091323/)

Skills that I worked on:

- Flexbox
  - This site uses flexbox several times for responsive behavior in the navbar, article filters, card content spacing, and pagination selector.
- Grid

  - The article cards are displayed using a responsive grid. To create this effect, the following two styles were added to the card parent containers:
    ```css
    .articles {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(390px, 1fr));
    }
    ```
    This code creates as many columns as can fit in the parent container with class name `.articles`. No row specifications were made, so the additional cards wrap to create as many rows as needed.

- Figma
  - Figma's new developer mode made replicating the Figma template much easier

Future Plans:

- Implement mobile layout
  - The current layout is only usable down to 600px width.
  - Key mobile features include switching the nav and article filters to a hamburger menu and shrinking pagination selector.
- Selecting better font sizes
- Fix `<hr>` formatting method
  - I am currently using a method to display a full width hr that I believe is suboptimal.
- Implementing actual functionality such as tile-view vs. list-view.
