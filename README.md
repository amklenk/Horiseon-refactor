# Horiseon-refactor

## Description

The goal of this project is to refactor Horiseon's code to make their website more accessible by assistive technologies and for SEOe. They are looking for: 

- Correct HTML semantics
- Correctly-working links
- Cleanly written, working CSS styling blocks


## Table of Contents (Optional)

These sections show each expectation and the changes that were made:

- [Installation](#installation)
- [Links](#links)
- [Usage](#usage)
- [Refactoring] (#refactoring)
- [Credits](#credits)
- [License](#license)

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
- section
- article
- footer  

* The images did not have alt attributes. Alt attributes with descriptions were added to each simple image. Empty alt attributes were added to each SVG. 

### HTML Link Fixes
* The title did not have a homepage link. This was fixed with href="/".

* The link in the nav for "Search Engine Optimization" was not working. An id attribute was added that contained the href of the nav link. 

### CSS Organization and Consolidation

* The font-family was placed in the header class styling block. It was moved to the body element styling block so that it can apply to the whole body section. 

* The a element is only in the header section at the moment, as such an a element selector was used. For possible future additions, the header element selector was added in front of the a element selector to make sure that the styling refers to the header a tags only. 

* The header section and the footer section did not need the specificity of a class (header and footer, respectively) since there can only be one of each section. The class style blocks were changed to element style blocks. 

* The class selector "header div" was changed to "header nav" to match the tag change.

* The p element styling refers to the p elements within the body section tags. The class selectors were added for possible future addiitions. 

* The styling for the left and right sections were mixed on the style sheet. The styling blocks were organized based on their section. 

* The article elements within the left section used different classes for floating within the style sheet. This was

* There were repeated styling blocks for similar elements with different classes. The styling blocks were condensed by using the same classes ("content-description" for the left elements and "benefits-description" for the right elements) so that the elements could be styled from one block (one for each section). 

### Comments

* It would be a good idea to change the SEO in Horiseon to make it darker and have it truly pop.

* It would be helpful to add headings to each section so that the user quickly understands the difference. 

* The footer could use some of the same styling as the header to continue the site's brand. 

## Credits
The following sites were used as references: 
- []()
- []()

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

