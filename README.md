# Admin Dashboard

![Status](https://img.shields.io/badge/Status-Completed-success)
![Focus](https://img.shields.io/badge/Focus-CSS_Grid_Architecture-blue)

## Description

This project is a complete responsive admin dashboard interface.

The primary objective was to leverage **CSS Grid** to construct a complex, rigid layout consisting of a sidebar, header, and dynamic main content area. Unlike my previous projects that relied heavily on Flexbox for linear layouts, this project demonstrates how to control two-dimensional layouts using grid areas and tracks.

## Features

- **Grid-Area Layout:** The entire page structure is defined using semantic grid areas (`"sidebar header"`, `"sidebar main"`), ensuring the sidebar spans the full height while the header and content stack adjacent to it.

- **Responsive Card Grid:** The "Projects" section utilizes `auto-fit` and `minmax` to automatically flow cards onto new rows based on available screen width.

- **Sticky Navigation:** The sidebar navigation remains pinned to the viewport (`position: sticky`) while the main content scrolls.

- **Complex Nesting:** Combines outer Grid layouts with inner Flexbox containers for components like search bars, user profiles, and action buttons.

- **SVG Integration:** Features inline SVG icons for navigation items and interactive buttons, styled directly with CSS.

- **Truncated Text:** Implements `-webkit-line-clamp` to elegantly truncate long announcement text with ellipses after 3 lines.

## Skills Demonstrated

By completing this project, I have demonstrated proficiency in the following areas:

### 1. CSS Grid Mastery

- **Template Areas:** Mapped out the high-level layout using `grid-template-areas`, allowing for intuitive placement of major page regions.
- **Track Sizing:** Mixed static units (`px`, `rem`) with fractional units (`fr`) to create fluid layouts that consume available space efficiently.
- **Auto-Placement:** Utilized `grid-template-columns: repeat(auto-fit, minmax(400px, 1fr))` to create a responsive grid that adapts without media queries.

### 2. Advanced Positioning & Overflow

- **Sticky Positioning:** Applied `position: sticky` to the sidebar navigation (`top: 0`) and project card titles to enhance user experience during scrolling.
- **Overflow Management:** Used `overflow: auto` on internal cards (like Announcements and Trending) to handle excess content without breaking the parent grid structure.

### 3. Component Styling

- **Visual Hierarchy:** Created depth using box shadows (`0px 0px 5px`) and distinct color blocking (`#8bae66`, `#ebd5ab`) to separate UI regions.
- **Flexbox Interoperability:** Used Flexbox within Grid cells (e.g., `.nav-link`, `.user-menu`) to handle one-dimensional alignment of icons and text.
- **CSS Reset:** Implemented a standard `box-sizing: border-box` reset to ensure padding and borders do not affect element width.
