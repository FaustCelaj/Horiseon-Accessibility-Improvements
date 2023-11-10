# Horiseon-Accessibility-Improvements
Refactoring existing HTML and CSS for Horiseon Marketing Agency


## Description

The goal of this project was to refactor the existing HTML and CSS code for Horiseon Marketing Agency.

The HTML code did not follow semantic HMTL rules, everything was labeled as div which hinders the performance of search engines and user devices to help with accessibility (ex screen readers). CSS code needed to be adjusted due to changes in the naming of divs and to increase legibility for other developers.

This project helped me as a developer understand the importance of semantic HTML structure not only for accessibility and search engine performance but also as a user reading the code - it's much easier to follow along and understand what I am editing.

You can view the [live page here].

## Changes

Below are changes that were made to the HTML and CSS files.

### HTML Changes
- The HTML title was changed from "Website" to "Horiseon Marketing Agency".
- Updated `<div>` tags to properly reflect semantic HTML structure across the file.
- classes were removed where not required.
  - ex. Previously written as `<div class="header">` and was changed to `<header>`
  - these changes were applied throughout all of the HTML document
- A tag of `<main>` was added in the body element to house our information and separate it from any other elements such as the footer.
- Added `<section>` element to further separate items.
- Added the `<article>` element  to necessary sections to help the search engine and screenreaders identify what it is.
- Some elements contained an unnecessary `id=""` and it was removed.
  - ex. Previously `<div id="online-reputation-management" class="online-reputation-management">`, the id was removed
- `alt=""` descriptions were added to all images and icons
- Changed the `<div class="benefits">` section to `<aside class="benefits">`
- Changed the `<div class="footer">` section to `<footer>`

### CSS Changes
- CSS Selectors had to be updated accordingly across the document after updating the semantic structure of the HTML.
    - ex. Previously written as `.header div` and was changed to `nav` due to updating the HTML
- Consolidated many styles in the CSS stylesheet to help reduce code and provide an easier reading experience for future developers.
- Selectors were reorganized to follow the same structure as the HTML.

Regarding the point made above, here is an example of what was changed:
 
```
.benefit-lead {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}
```

This was updated to show:

```
.benefit-lead, .benefit-brand, .benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}
```
- Other similar snippets of code were grouped together in the same manner.
- Added Comments above areas of code to help other developers see what areas the CSS was being applied to

## Final Results

Below is a screenshot of the final product which users will view. 

![Screenshot 2023-11-09 at 11 32 20 PM](https://github.com/FaustCelaj/Horiseon-Accessibility-Improvements/assets/149631014/8459efa4-397f-444b-9395-50dfdb7206b9)
