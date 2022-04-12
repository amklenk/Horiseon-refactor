# Horiseon-refactor

## Description

The goal of this project is to refactor Horiseon's code to make their website more accessible by screen readers and for SEOe. They are looking for: 

- Correct HTML semantics
- A logical flow of h elements
- Correct and succinct alt attributes, when necessary
- Links that work correctly

## Table of Contents (Optional)

If your README is long, add a table of contents to make it easy for users to find what they need.

- [Semantics](#semantics)
- [Links](#links)
- [CSS](#css)

## Semantics

Besides the head and body tags, the rest of the page uses div tags. This is not the best practice for semantics as a screen reader will not be able to adequately assess the true nature of each element. The following tags were used as replacements: 
- header
- nav
- section
- article
- footer 

The website title did not give enough of a description. It was changed from "website" to "Home Page - Horiseon" to fit the common naming convention. 

The sections in the body of the page did not have headings. The following headings were added to each section: (CHECK ON THIS)
- "What We Offer" (Search Engine Optimization, Online Reputation Management, and Social Media Marketing)
- "How We Can Help" (Lead Generation, Brand Awareness, Cost Management)

## Links
The title did not have a homepage link. This was fixed with href="/".

## CSS
List your collaborators, if any, with links to their GitHub profiles.

If you used any third-party assets that require attribution, list the creators with links to their primary web presence in this section.

If you followed tutorials, include links to those here as well.
