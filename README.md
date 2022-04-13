# Horiseon-refactor

## Description

The goal of this project is to refactor Horiseon's code to make their website more accessible by assistive technologies and for SEOe. They are looking for: 

- Correct HTML semantics
- Correctly-working links
- Cleanly written, working CSS styling blocks

## Table of Contents (Optional)

These sections show each expectation and the changes that were made:

- [Semantics](#semantics)
- [Links](#links)
- [CSS](#css)
- [Comments] (#comments)

## Semantics

The website title did not give enough of a description. It was changed from "website" to "Home Page - Horiseon" to fit the common naming convention.

Besides the head and body tags, the rest of the page used div tags. The following tags were used as replacements: 
- header
- nav
- section
- article
- footer  

The images did not have alt attributes. Alt attributes with descriptions were added to each simple image. Empty alt attributes were added to each SVG. 

## Links
The title did not have a homepage link. This was fixed with href="/".

The link in the nav for "Search Engine Optimization" was not working. An id attribute was added that contained the href of the nav link. 

## CSS

The font-family was placed in the header class styling block. It was moved to the body element styling block so that it can apply to the whole body section. 

The a element is only in the header section at the moment, as such an a element selector was used. For possible future additions, the header element selector was added in front of the a element selector to make sure that the styling refers to the header a tags only. 

The header section did not need the specificity of a class since it is the only (and can be the only) header section. The class style blocks were changed to element style blocks. 

The p element styling refers to the p elements within the body section tags and the footer tag. The class selectors were added for possible future addiitions. 

The styling for the left and right sections were mixed on the style sheet. The styling blocks were organized based on their section. 

The article elements within the left section used different classes for floating within the style sheet. This was

There were repeated styling blocks for similar elements with different classes. The styling blocks were condensed by using the same classes ("content-description" for the left elements and "benefits-description" for the right elements) so that the elements could be styled from one block (one for each section). 

## Comments

It would be a good idea to change the SEO in Horiseon to make it darker and have it truly pop.

It would be helpful to add headings to each section so that the user quickly understands the difference. 

The footer could use some of the same styling as the header to continue the site's brand. 
