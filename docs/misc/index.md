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

## Making changes locally

{: .danger }
This section of the guide is unfinished.

There are many advantages to hosting the site locally when uploading your articles. It allows you to quickly see your changes to the website even before they are published. This could be helpful when making an article with many Markdown elements that you need to test, or when updating the graphics of the site. It works by hosting your local copy of the website (which you should already have) as a website accessible by any web browser. When you make a change to your local copy, it will change immediately on the local website.

However, this can take a little to set up, and every computer is different, so be prepared to solve some of these issues yourself. I recommend only doing this if you believe you have enough computer skill to do so.

{: .important }
This section of the guide is only written for macOS. This is simply because I do not have Windows to test this on. However, if you are a contributor with Windows, please reach out so we can work together to expand this section

##### "What does section set up?"

This section will install and set up:

- [Ruby](https://www.ruby-lang.org/en/downloads/) (& RubyGems)
- [Jekyll](https://jekyllrb.com/)
- [Bundler](https://jekyllrb.com/docs/ruby-101/#bundler)
- GCC & Make

##### Requirements
1. A local copy of csartisan.org. (See [Getting Started](/docs/getting-started))
2. Experience with the command line. (macOS, see [Terminal User Guide](https://support.apple.com/guide/terminal/welcome/mac))
3. macOS 11.0.0 or higher.
4. [Homebrew](https://brew.sh/) is installed.

Jekyll & all of Jekyll's requirements. (See Jekyll's [Installation Requirements](https://jekyllrb.com/docs/installation/#requirements) and [Installation Guide (macOS)](https://jekyllrb.com/docs/installation/macos/))

[Jekyll](https://jekyllrb.com/) is a static site generator. It takes text written in Markdown and uses layouts (templates) to create a static website. You can tweak the site’s look and feel, URLs, the data displayed on the page, and much more. 

To install Jekyll, the following utilities are required:
- [Ruby](https://www.ruby-lang.org/en/downloads/) 2.5.0+
- RubyGems
- GCC and Make

### Ruby

Jekyll is written in Ruby. To run Jekyll, you need to install Ruby.

##### Installing Ruby

1. Navigate to your Home directory.

    ```bash
    cd
    ```

1. Use Homebrew to install `rbenv`, a version manager for Ruby installations. 

    ```bash
    brew install rbenv ruby-build
    ```

1. Install version 3.1.2 of Ruby using `rbenv`

    ```bash
    rbenv install 3.1.2
    ```
    [Troubleshooting this step](https://github.com/rbenv/rbenv)

1. Check that the installation was successful with `ruby -v`

    The result should look something like this:

    ```
    ruby 3.1.2p20 (2022-04-12 revision 4491bb740a) [x86_64-darwin22]
    ```

1. Navigate to your local copy of the website.

    ```bash
    cd /Documents/GitHub/csartisan.github.io/
    ```

1. Set the Ruby version for this project.

    ```bash
    rbenv local 3.1.2
    ```

1. Install [RubyGems](https://rubygems.org/) using this link: https://rubygems.org/pages/download

Congratulations! You've successfully installed and set up Ruby 3.1.2 and RubyGem in your local copy!

##### Installing Jekyll

1. Navigate to your Home directory.

    ```bash
    cd
    ```

1. Install Jekyll & Bundler using `gem`.

    ```bash
    gem install jekyll bundler
    ```

    [Troubleshooting this step](https://jekyllrb.com/docs/troubleshooting/)

Congratulations! You have successfully installed Jekyll and Bundler!

##### Build & Host locally

1. Navigate to your local copy of the website.

    ```bash
    cd /Documents/GitHub/csartisan.github.io/
    ```

1. Build the site and host it on a local server.

    ```bash
    bundle exec jekyll serve
    ```

    [Troubleshooting this step](https://jekyllrb.com/docs/troubleshooting/#configuration-problems)

Congratulations! You have successfully started a live server of [csartisan.org](https://csartisan.org)! 

While running, you can see your site by going to [http://127.0.0.1:4000](http://127.0.0.1:4000). Now, when you change anything in the code of your local copy, this site will update with your changes.

{: .important }
To end your server, simply open your terminal and press `^C` or `control + C` on your keyboard.