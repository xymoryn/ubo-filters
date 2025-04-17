# Anti Annoyance

## Bypass Link Confirmation

### Note

If you need to use [$urlskip()](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#urlskip) or [trusted-click-element.js](https://github.com/gorhill/uBlock/wiki/Resources-Library#trusted-click-elementjs-) to bypass redirect links, please refer to the [uBO wiki](https://github.com/gorhill/uBlock/wiki/Advanced-settings#trustedlistprefixes) to add this filter as trusted.

### Subscribe

- https://raw.githubusercontent.com/xymoryn/ubo-filters/main/anti-annoyance/bypass-link-confirmation.txt
- https://cdn.jsdelivr.net/gh/xymoryn/ubo-filters/anti-annoyance/bypass-link-confirmation.txt

### Rule

- [$urlskip](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#urlskip)
  - Can only be used in a trusted-source origin. See <https://github.com/gorhill/uBlock/wiki/Advanced-settings#trustedlistprefixes>
  - Extracts a URL from another URL according to one or more transformation steps, thereby skipping over intermediate network request(s) to remote servers.
- [href-sanitizer.js](https://github.com/gorhill/uBlock/wiki/Resources-Library#href-sanitizerjs-)
  - Set the href attribute to a value found in the DOM at, or below the targeted a element, and optionally with transformation steps.
- [addeventlistener-defuser.js](https://github.com/gorhill/uBlock/wiki/Resources-Library#addeventlistener-defuserjs-)
  - Prevents attaching event listeners.
- [:remove-attr()](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#subjectremove-attrarg-subjectremove-classarg)
  - Remove attributes or event handler attributes.
- [:watch-attr()](https://github.com/gorhill/uBlock/wiki/Procedural-cosmetic-filters#subjectwatch-attrarg)
  - Force re-evaluation when one or more attribute changes on the matching elements.
- [trusted-click-element.js](https://github.com/gorhill/uBlock/wiki/Resources-Library#trusted-click-elementjs-)
  - Click elements on webpages in a sequence.

### Acknowledgements

This filter was inspired by or based on the following projects:

- [Open-the-F-king-URL-Right-Now](https://github.com/OldPanda/Open-the-F-king-URL-Right-Now) by [OldPanda](https://github.com/OldPanda)
- [redirect 外链跳转](https://github.com/sakura-flutter/tampermonkey-scripts/blob/gh-pages/redirect.js) by [sakura-flutter](https://github.com/sakura-flutter)
- [跳转链接修复（移除重定向外链直达）](https://github.com/maomao1996/tampermonkey-scripts/blob/gh-pages/remove-redirect.user.js) by [maomao1996](https://github.com/maomao1996)
- [Intercept Redirect](https://github.com/bjornstar/intercept-redirect) by [bjornstar](https://github.com/bjornstar)