---
title: Other
layout: default
nav_order: 5
---

# Other Contributing

## Banner 

The banner is an optional part of the website that appears at the very top of the home page. The color of it is light blue. It has two attributes: `bannercontent` and `bannerlink`. 

These attributes are located in the `_config.yml` on line 13.

```yml
# Promo Banner
bannercontent: 
bannerlink: https://csartisan.org/docs
```
The banner can be used for:
- Club collaborations
- School announcements
- Redirects
- Forms
- Messages

##### Adding the banner
1. Locate and open `_config.yml` in the root directory.
2. Scroll to `# Promo Banner` comment (line 13)
3. Add your desired message after `bannercontent:`
4. (Optional) Add your desired link after `bannerlink:`
5. Check your staging site to confirm you have the desired link and content.
6. [Publish](/docs/finalizing/)

##### Removing the banner
1. Locate and open `_config.yml` in the root directory.
2. Scroll to `# Promo Banner` comment (line 13)
3. Remove all text after `bannercontent:`

You don't need to delete the link if you think you'll use it again, keeping the link will still remove the banner.