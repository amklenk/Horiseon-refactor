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

The simple images did not have alt attributes. Alt attributes were added to each simple image. 

## Links
The title did not have a homepage link. This was fixed with href="/".

The link in the nav for "Search Engine Optimization" was not working. An id attribute was added that contained the href of the nav link. 

## CSS

The font-family was placed in the header class styling block. It was moved to the body element styling block so that it can apply to the whole body section. 

The a element is only in the header section at the moment, as such an a element selector was used. For possible future additions, the .header class was added in front of the a element to make sure that the styling refers to the header a tags only. 

The p element styling refers to the p elements within the body section tags and the footer tag. The class selectors were added for possible future addiitions. 

FIX FLOAT OF NAV
FIX FLOAT CLASSES
(DO THIS) The footer did not have the same styling as the header, which will help with the site's branding. CSS styling for the footer was added. 
