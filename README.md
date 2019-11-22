# Timeline Content Element for TYPO3 (ce_timeline)

This extension provides a new content element of type "Timeline" (ce_timeline) that contains inline records of different timeline entries. Please note that this is not a plugin and there are no records visible in any list view by default. Feel free to use the code or the extension as a basis for your own stuff.

## Features

- User friendly and very easy to handle
- Includes predefined light, dark and pink stylesheets
- 100% responsive
- 2 different entry types (time and text)
- Entries can be ordered manually
- Optional header and text (rte) above each timeline
- Does not require any JavaScript
- Does not require any other Extension
- Translated in English, German and Spanish

## Installation

Install the extension by downloading it in the extension manager or on https://extensions.typo3.org/extension/ce_timeline/.

## Basic configuration

You don't need to configure much to get this extension running.

- add the static TypoScript (Timeline - Content Element) to your template record
- choose a static TypoScript (e.g. Timeline Styles - Default) to make the timeline look nice
- add a content element of type "Timeline" and add some entries
- have fun!

## Need custom CSS Styling or even SASS?

No problem! Just do NOT include the Static TypoScript as mentioned above and the extension will render just plain HTML. If you want to use the styles that come with the extension, feel free to use the SASS file in "Resources/Private/Scss" and change them to your needs.

## Changing the template files

Since this is NOT a plugin but a regular content element, you need to change the following paths in order to overwrite the HTML/Fluid template paths with your own paths:

### Page Setup

```
lib.contentElement{
    templateRootPaths{
        1277 = EXT:ce_timeline/Resources/Private/Templates/
    }
    partialRootPaths{
        1277 = EXT:ce_timeline/Resources/Private/Partials/
    }
}
```

### Template files

Files you need to copy in order to overwrite them:

Main Template file:
https://github.com/koehlersimon/ce_timeline/blob/master/Resources/Private/Templates/Timeline.html

Partials:
https://github.com/koehlersimon/ce_timeline/tree/master/Resources/Private/Partials

## Support & Service

If you have any problems with the extension, please let me know! Since this is open source, I only guarantee 100% expert support when I get paid, but I also like to support the community. Please don't hesitate to open an issue here on GitHub or send a message: https://simon-koehler.com/en/contact
