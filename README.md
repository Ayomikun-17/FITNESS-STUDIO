# FITNESS-STUDIO
Fitness studio webpage with classes information etc 
 a fitness studio site. Class schedule, trainer bios as cards, and membership tiers as pricing cards

# Pulse Studio

A single-page, responsive website for a fitness studio. It shows the weekly class schedule, trainer profiles as cards, and membership tiers as pricing cards. Built with plain HTML5 and CSS3, with no frameworks.

## Sections

| Section | What it shows | Layout |
| --- | --- | --- |
| Trainers | Five trainer cards with photo, name, specialty, bio and training days | CSS Grid |
| Class Schedule | Weekly timetable: class, day and time, instructor, studio, level | CSS Grid |
| Membership | Three pricing tiers (Starter, Regular, Elite), with Regular highlighted as most popular | Flexbox |

## Tech

- HTML5 with semantic landmarks (`header`, `nav`, `main`, `section`, `article`, `footer`) and one `h1`
- CSS3 with custom properties (variables) for all colours
- `box-sizing: border-box` applied globally
- Responsive design with media queries and no horizontal scroll on phone, tablet or desktop
- No frameworks or libraries

## Project structure

```
pulse-studio/
├── index.html
├── style.css
├── README.md
├── rowing-machines.jpg
├── pure-gym.jpg
├── spin-bikes.jpg
├── coach-assessment.jpg
└── boxing-coaching.jpg
```

Keep the images in the same folder as `index.html`, because the paths in the HTML are relative.

## Run it locally

1. Clone the repo:
   ```
   git clone <repo-url>
   ```
2. Open the folder.
3. Double-click `index.html` to open it in your browser.

No build step or install is needed.

## How the layout works

**Trainers (Grid):** The cards use five equal columns, so they sit in one row on desktop. Photos use `object-fit: cover` so they are cropped to the same height without being stretched. Below 1000px the grid drops to 3 columns, and below 600px to 1 column.

**Schedule (Grid):** Each row is a five-column grid. Below 700px the header row is hidden visually and each class becomes a stacked card.

**Pricing (Flexbox):** The cards sit in a wrapping flex row. Each card can grow or shrink from a base width of 260px, so they stack on small screens without a media query. The feature list takes up the spare space, which keeps all the buttons aligned at the bottom of the cards.

## Colours

All colours are CSS variables defined in `:root` at the top of `style.css`. To change the look of the site, edit those values.

| Variable | Use |
| --- | --- |
| `--color-bg` | Page background |
| `--color-surface` | Card background |
| `--color-surface-alt` | Alternate section background |
| `--color-text` | Main text |
| `--color-muted` | Secondary text |
| `--color-accent` | Buttons, highlights, borders |
| `--color-border` | Card and table borders |

## Accessibility

- Semantic landmarks and a single `h1`
- Every image has descriptive `alt` text
- Each section is labelled with `aria-labelledby`
- Visible focus styles on links and buttons
- Schedule table keeps its header row for screen readers on small screens

## Requirements checklist

- [x] Single page, plain HTML5 and CSS3, no frameworks
- [x] Semantic landmarks and one `h1`
- [x] Working navigation links
- [x] `box-sizing: border-box` globally
- [x] Custom CSS variables for colours
- [x] Real use of Flexbox (pricing cards)
- [x] Real use of Grid (trainer cards and schedule)
- [x] No horizontal scroll on phone, tablet or desktop
- [x] Responsive layout
- [ ] GitHub repo with small, real commits (team to confirm)

## Team

| Name | Part |
| --- | --- |
| _Add name_ | Trainer cards and pricing cards |
| _Add name_ | Class schedule |
| _Add name_ | Header, navigation and footer |

## Notes

- Trainer names, prices and bios are placeholder content.
- Photos are stock images used for this student project.
