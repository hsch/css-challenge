# css-challenge

## Summary

The challenge is to implement a specific layout,
according to the requirements below,
in pure CSS that works in all major modern browsers (Safari, Firefox, Chrome, Edge)
without any use of Javascript.

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

## Why?

I think this is something that _should_ be doable in CSS, but it doesn't seem to be.
And it's really bothering me that I can't figure it out.

However, even if I can't do it myself, I would still love to see a solution.

The Javascript implementation is good enough from a "business" perspective,
but it is a bit annoying tech-pride-wise:
The repositioning of the navigation bar always lags a bit behind
(I suppose it wouldn't if the browser handled the layout "natively"),
it is fragile and falls apart e.g. when you rotate your (or: some) devices
(I guess you could just tweak the event handling more, but then again, we do you even need to?!),
and it only works when the image has loaded
(so the event handling needs to account for that, too).
It just doesn't feel nice and clean.

Anyway, I claim this is impossible to solve.

Prove me wrong. :-)


## Disclaimer

This is for a pet project of mine and there are 0 commerial gains involved.

## Requirements

Generally speaking, and if in doubt, the layout must behave pretty much like the [demo](https://hsch.github.io/css-challenge/):

- The **layout** consumes the full page (i.e. all of the viewport),
  but never extends beyond it.
- There is no scrollbar.
- The layout adjusts when the window is resized.
- There is a **header**.
- The header always sticks to the top of the page.
- The height of the header is based on its content, e.g. the font size.
- There is a **footer**.
- The footer always sticks to the bottom of page.
- The height of the footer is based on its content, e.g. the font size.
- Header and footer might have different heights.
- There is no need to account for potential word wrap.
- There is a **content block**.
- The content block consists of an image, and a navigation bar.
- The **image** shrinks in width and height as necessary to make things fit,
  and always maintains its aspect ratio.
- The image is always shown as large as possible,
  without violating the other layout constraints.
- The image is never shown larger than its maximum, original dimensions.
- The image file can be of any size and format (landscape, portrait, square),
  i.e. don't assume the specific dimensions in the demo to be part of the specification.
- The top of the **navigation bar** always sticks to the bottom of the image,
  but there is a fixed sized margin between them.
- The width of the navigation bar always aligns with the width of the image.
- The height of the navigation bar may be pixel-perfectly hardcoded, if needed,
  or simply be based on content.
- The **content block as a whole** (image plus navigation bar) is always centered
  between footer and header, both vertically and horizontally.
- There is a minimum fixed size margin around the content block,
  i.e. on the left and right of it
  and between content block and header and footer respectively.
- Neither the image nor the content block ever extend over the header or footer
  or push them out of the viewport.
- Header, footer, and navigation bar are proper block elements (e.g. `<div>`)
  so that they can contain and position child elements.

## Notes

- You don't have to build upon the demo at all.
  Start from scratch as much as you want to.
  Solve the challenge however you like.
- You may assume that the page (HTML and inline CSS) is generated
  with knowledge of the absolute dimensions of the image file,
  i.e. using some constant expressions in inline styles is permitted
  as long as they are based on image dimensions only (e.g. not on the window size)
  and don't require recalculation on window resize.

## License

Copyright © 2018

This work is free. You can redistribute it and/or modify it under the
terms of the Do What The Fuck You Want To Public License, Version 2,
as published by Sam Hocevar.
