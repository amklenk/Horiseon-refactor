# Horiseon Refactor

## Description

The goal of this project is to refactor Horiseon's code to make their website more accessible by assistive technologies and for SEOe. They are looking for: 

- HTML semantics that adequately describe each element
- Correctly-working links
- Cleanly written, condensed, working CSS styling blocks


## Table of Contents (Optional)

These sections show each expectation and the changes that were made:

- [Installation](#installation)
- [Links](#links)
- [Usage](#usage)
- [Refactoring](#refactoring)
- [Credits](#credits)
- [License](#license)
- [Tests](#tests)

## Installation
The original code was cloned from the urban-octo-telegram respository on GitHub. The refactored code is in the Horiseon-refactor repository on GitHub. It includes an index.html file and an assets folder. Within the assets folder, there are CSS and assets folders that contain the style sheet (style.css) and images, respectively. 


## Links 
- [GitHub Refactored Code Repository Site](https://github.com/amklenk/Horiseon-refactor)
- [Refactored Site](https://amklenk.github.io/Horiseon-refactor/)


## Usage
The following screenshot shows the site after refactoring. It is visually the same as the unfactored site. 
![screenshot of Home Page - Horiseon](./assets/images/amklenk.github.io_Horiseon-refactor.png)


## Refactoring
### HTML Semantics Additions/Changes
* The website title did not give enough of a description. It was changed from "website" to "Home Page - Horiseon" to fit the common naming convention.

* Besides the head and body tags, the rest of the page used div tags. The following tags were used as replacements: 
        - header
        - nav
        - main
        - section
        - aside
        - footer  

* The images did not have alt attributes. Alt attributes with descriptions were added to each simple image. Empty alt attributes were added to each icon in the aside.

* The footer had an h2 tag, which does not fit the focus/importance of the heirarchy (the aside section had h3 tags). This was switched to an h4 tag, which is also reflected in the assigned CSS styling block.

### HTML Link Fixes
* The title did not have a homepage link. This was fixed with href="/".

* The link in the nav for "Search Engine Optimization" was not working. An id attribute was added that contained the href of the nav link. 

### CSS Organization and Consolidation

* The font-family was placed in the header class styling block. It was moved to the body element styling block so that it can apply to the whole body. 

* The a element is only in the header at the moment, as such an a element selector was used. For possible future additions, the header element selector was added in front of the a element selector to make sure that the styling refers to the header a tags only. 

* The header and the footer did not need the specificity of a class (.header and .footer, respectively) since there can only be one of each. The class style blocks were changed to element style blocks. 

* The class selector "header div" was changed to "header nav" to match the tag change.

* The p element styling refers to the p elements within the body tags. The class selectors were added for possible future addiitions. 

* The styling for the main and aside were mixed on the style sheet. The styling blocks were organized based on whether or not they belong in the in either the main or the aside. 

* There were repeated styling blocks for similar elements with different classes. The styling blocks were condensed by using "content-description" for the main elements and "benefits-description" for the aside elements. 

### Comments

* It would be a good idea to change the SEO in Horiseon to make it darker and have it truly pop.

* It would be helpful to add headings to each section so that the user quickly understands the difference. 

* The footer could use some of the same styling as the header to continue the site's brand. 

## Credits
The following sites were used as references: 
- [HTML Semantic Elements - W3Schools](https://www.w3schools.com/html/html5_semantic_elements.asp#:~:text=or%20Vice%20Versa%3F-,The%20element%20specifies%20independent%2C%20self%2Dcontained%20content,defines%20section%20in%20a%20document)
- [Multiple Class / ID and Class Selectors](https://css-tricks.com/multiple-class-id-selectors/)

## License

MIT License

Copyright (c) [2022] [Amanda Klenk]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Tests

The site should have the same layout, content, and visible styling as the live site.

