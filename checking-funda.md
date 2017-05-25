# Checking Funda's PE Usage

This document is a check of the [Funda website](http://funda.nl) which focusses on the following 8 features (or the lack there of):

1. [Images](#images)
2. [Custom Fonts](#custom-fonts)
3. [JavaScript](#javascript)
4. [Color](#color)
5. [Fast Internet](#fast-internet)
6. [Cookies](#cookies)
7. [localStorage](#localstorage)
8. [Mouse / Trackpad](#mouse-trackpad)

## Images
Looking at images of realestate is a _major_ functionality and use-case of a realestate website. It's no surprise that the experience of looking for houses falls flat when images aren't allowed to be loaded.

|Page        | With images                                   | Without images                                          |
|------------|-----------------------------------------------|---------------------------------------------------------|
|Homepage    | ![Homepage](./checking-funda-images/home.png) | ![Homepage](./checking-funda-images/home-no-images.png) |
|Search      | ![Search](./checking-funda-images/search.png) | ![Search](./checking-funda-images/search-no-images.png) |
|Single item | ![Single](./checking-funda-images/item.png)   | ![Single](./checking-funda-images/item-no-images.png)   |

Note that all icons are images as well. Some options of the website are completely missing without these images. For example the button in the top right on the single item page is rendered useless and the 'share' buttons are missing.

_This was tested by disabling images under Settings > Advanced Settings > Content Settings > Images in Chrome Version 58.0.3029.110_

## Custom Fonts

Funda uses Googles Proxima Nova font for all it's copy. The font is being loaded asynchronously, with the system-default `sans-serif` font as fallback. This prevents a [FOIT](https://css-tricks.com/fout-foit-foft/). The `sans-serif` default on a Mac is actually quite similar in look and feel to Proxima Nova, so I didn't even notice the font missing the first time around.

![Home header with Proxima Nova](./checking-funda-images/home-with-fonts.png)
_Home with custom font_  

![Home header without Proxima Nova](./checking-funda-images/home-withouth-fonts.png);
_Home header without custom font_

_This was tested by removing the `fonts-loaded` class and throttling the network speed_
