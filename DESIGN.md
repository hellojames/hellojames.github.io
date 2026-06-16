---
version: continuous
name: hellojames

colors:
 primary: "#1A1C1E"
 secondary: "#6C7278"
 link-hover: "#890309"
 link-active: "#0000FF"
 background: "#FFFFFF"
 surface: "#F7F5F2"


typography:
  body:
    fontFamily: Georgia, serif
    fontSize: 24px
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: Anonymous Pro, monospace
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.6
  h1:
    fontFamily: Georgia, serif
    fontSize: 84px
    fontWeight: 400
    lineHeight: 1.025
  h2:
    fontFamily: Georgia, serif
    fontSize: 42px
    fontWeight: 400
    lineHeight: 1.6
  h3:
    fontFamily: Georgia, serif
    fontSize: 30px
    fontWeight: 400
    lineHeight: 1.6

spacing:
  gutter: 24px
  margin: 32px

rounded:
  default: 0px

components:
  link:
    textColor: "{colors.primary}"
    textDecoration: underline
    states:
      hover:
        textColor: "{colors.link-hover}"
        textDecoration: none
      active:
        textColor: "{colors.link-active}"
        textDecoration: none
      visited:
        textColor: "{colors.primary}"
        textDecoration: underline
  nav:
    typography: "{typography.label}"

---

<!-- 
DESIGN.md for hellojames.co.uk
Design intent specification and interface design guidance for AI agents 
https://github.com/google-labs-code/design.md/blob/main/docs/spec.md
Updated     2026.06.16


DESIGN.md is a self-contained, plain-text representation of a design system.
It defines a visual identity, thereby ensuring stylistic choices are followed
across design sessions and between different AI agents and tools.
As a human-readable, open-format document, it serves as a living source of truth
both humans and AI can understand and refine.

A DESIGN.md file contains two parts:
- YAML front matter contains machine-readable design tokens
- Markdown body provides human-readable design rationale and guidance for how to apply tokens
-->


## Overview

Designer's personal site. The presentation is intentionally minimal: restrained colour, no decoration, no animation. Typography and whitespace do all the work. Every stylistic addition has to justify itself.

The brand personality is authoritative yet approachable. It evokes the clean layouts of traditional print editorial work combined with modern web interactivity.

- Style: swiss international typographic style, brutalist, greyscale
- Qualities: clear structure, focused, generous type, honest materials
- Designed to be read, not clever


## Color

Palette is intentionally sparse to honour the written word and maximise accessibility. Black text on off-white background. Occasional colour accents in links and images.

- Primary ({colors.primary}): all body text and headings
- Secondary ({colors.secondary}): metadata, timestamps, labels
- Background ({colors.background}): page background
- Surface ({colors.surface}): call-out sections background

Links use black text with underline, and colour to indicate the interaction state. The design relies on typography and spacing for aesthetic beauty.


## Typography

Georgia for everything you read — body, headings, prose. Matthew Carter designed it in 1996 for screens, not print. Large x-heights, open counters, built for pixels. 24px at 1.6 line height. It's a system font, so it loads instantly.

Anonymous Pro for everything that's a label — code, timestamps, metadata, navigation. 12px at 1.6 line height. Signals "this is supplementary." The size contrast creates hierarchy without needing colour or weight.

At wide layouts:
- H1 headings are 84px / 1.025
- H2 headings are 42px / 1.6
- H3 headings are 30px / 1.6


## Layout

Single column. 680px max-width. No grids, no sidebars. 680px gives roughly 65–75 characters per line — the comfortable range for reading. Sections are separated by whitespace, not dividers. Mobile-first, fluid responsive design. On smaller screens, margins shrink proportionally and elements stack vertically.


## Elevation & Depth

This is a flat design aesthetic. Visual depth is rejected in favour of site rendering performance and avoid aesthetic noise. Hierarchy is established through scale, grouping, and typographic contrast.


## Shapes

Sharp edges and no rounded corners.


## Components

- Links: black and underlined, don't override
- Navigation: Text only, no icons or separators. Uses the label typography token
- Forms: Plain HTML, no custom styling, works without JavaScript


## Do's and Don'ts

- Do use whitespace to create structure
- Do respect the typographic hierarchy
- Do use semantic HTML — structure belongs in the markup, not CSS
- Do write evergreen content — articles should age well

- Don't allow reading text blocks to exceed 75-character line length limit
- Don't add colour outside the defined palette, shadows, or decoration
- Don't add images unless they're essential
- Don't add JavaScript for anything HTML handles natively
- Don't add tracking, analytics, or third-party cookies
- Don't add social share buttons, comment sections, or other widgets
- Don't reduce font size below 12px at any breakpoint

