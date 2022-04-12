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

The simple images did not have alt attributes. Alt attributes were added to each simple image. 

## Links
The title did not have a homepage link. This was fixed with href="/".

The link in the nav for "Search Engine Optimization" was not working. An id attribute was added that contained the href of the nav link. 

## CSS
FIX FLOAT OF NAV
FIX FLOAT CLASSES?
FIX SEO IN HEADER
(DO THIS) The footer did not have the same styling as the header, which will help with the site's branding. CSS styling for the footer was added. 
