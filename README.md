# css-challenge

## Summary

The challenge is to implement a specific layout,
according to the requirements below,
in pure CSS that works in all major modern browsers (Safari, Firefox, Chrome, Edge)
without Javascript.

The [demo](https://hsch.github.io/css-challenge/) implements this layout correctly
(tested in Safari, Firefox, Chrome),
but it does use Javascript.

DO create a pull request, if you think you have a solution.
This repository is licensed under the [WTFPL](http://www.wtfpl.net)
and by creating a pull request you agree to submitting your work
under the same license.

DO NOT try to trick the requirements.
I think the intentions should be clear, please play along.
If you have questions, please create an issue.

DO NOT nit-pick on how the demo is built. :-)

## Disclaimer

This is for a pet project of mine and there are 0 commerial gains involved.

## Requirements

- The **layout** consumes the full page (i.e. all of the viewport),
  but doesn't extend beyond it.
- There is no scrollbar.
- The layout always adjusts to a resizing window.
- There is a **header**.
- The header always sticks to the top of the page.
- The height of the header is based on its content, e.g. the font size.
- There is a **footer**.
- The footer always sticks to the bottom of page.
- The height of the footer is based on its content, e.g. the font size.
- Header and footer might have different heights.
- There is a **content block**.
- The content block consists of an image, and a navigation area.
- The **image** shrinks in width and height as necessary to make things fit,
  and always maintains its aspect ratio.
- The image never extends beyond its original size.
- The image can be of any size and format (landscape, portrait, square),
  i.e. don't assume the dimensions in the demo are constants.
- You can assume the page (HTML and inline CSS) to be generated
  with knowledge of the dimensions of the image,
  i.e. using constant expressions is permitted
  as long as they don't require recalculation on window resize.
- The top of the **navigation bar** always sticks to the bottom of the image,
  but there is a fixed sized margin between them.
- The height of the navigation bar is based on its content,
  and it may contain more complex elements than just text
  e.g. buttons or smaller images acting as buttons.
- The width of the navigation bar always aligns with the width of the image.
- The **content area** as a whole (image plus navigation bar) is always centered
  between footer and header, both vertically and horizontally.
- There is a fixed minimum size margin around the content area.
- The height of header, footer, and navigation bar can be assumed to be static,
  e.g. there is no need to account for potential word wrap.

## License

[WTFPL](http://www.wtfpl.net)
