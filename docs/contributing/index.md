---
title: Contributing
layout: default
has_children: no
nav_order: 3
---

# Contributing

This section will walk you through uploading an article as a Markdown file to csartisan.org. If you have not yet done so, follow [Getting Started](/docs/getting-started/) to prepare for these steps. It's only necessary to do this once.

{: .important }
This section of the guide has specific instructions based on the interface of [Dillinger](https://dillinger.io).

## Required Reading

This section will briefly touch on important vocabulary important to know before contributing. Some terms will have a link to more info on them, and all terms will be included in the site [Glossary](/docs/glossary/). 

### Front Matter
Front Matter acts like metadata leading every post. This is essential to the post being correctly rendered on the website. It is lead and trailed by three dashes `---`. This is to separate it from the rest of the text and hide it from being rendered. Front Matter contains information that the website uses to fill out things like title, author name, category, and more.

{: .important }
Front Matter is essential to a functional post, so carefully follow the Guidelines to use it.

Unfortunately, Dillinger shows the Front Matter when previewing the Markdown file. Thankfully, you will not be able to see it on the website. Please look past this flaw.

### Images
__EVERY POST NEEDS AN IMAGE__.

This is the biggest rule in this guide. Every post requires a corresponding image.

Most new articles should have an image supplied to you by the editor, and many old articles have an accompanying photo. Great, now how do we use those?



#### Importing an image
- This may seem tedious, but every image must be 800x600px in size. This is to ensure every image slot is of an equal size when it is published to the site. Trust us, it looks great. This can be done with a photo editor, but if you cannot do it, send it to club IT and we would be happy to format it for you.
- Make sure the image is a `.jpg` or `.jpeg` file. This is to save server storage. Your changes will not be accepted if the image isn't a JPG/JPEG. Feel free to convert another image type to a JPG/JPEG, as long as it reaches us as one you're good to go.
- Take the image and move it to `/Documents/GitHub/csartisan.github.io/assets/images/posts`.
- Rename it to the title of the corresponding post. (ex. `art-therapy.jpg`)
You will use this image name in a little bit.

#### What if I don't have an image?
No problem. The website already has 10 filler images for posts with no images.

Every file is numbered from 1-10. So to use them, enter one of the following files in the `image:` tag in your Front Matter: 

`./assets/images/posts/none/1.jpg`  
`./assets/images/posts/none/2.jpg`  
`./assets/images/posts/none/3.jpg`  
...  
`./assets/images/posts/none/10.jpg`  

These images are all colorful gradients that make posts look great even when they dont have photo of their own! Be careful though, too many articles with the same filler image may look bad, so be sure to change the image up when you're contributing lots of articles at a time.

### Categories

EVERY post needs a category, if there isn’t an apparent one, use `[misc]`.

#### All categories
- `[events]`
- `[productions]`
- `[reviews]`
- `[opinions]`
- `[interviews]`
- `[essays]`
- `[updates]`
- `[misc]`

{: .danger }
DO NOT capitalize the `category:` input. This will separate it into a separate, identically named category.

### Tags

Tags will define how the back-end handles posts’ appearances. For example, adding `[ sticky ]` to a post makes the post, regardless of release date, appear as a large card just below the latest posts. 

|Tag     |Function|
|-------:|:-------|
|sticky  |Presents post as a large card below latest posts, regardless of date posted.|
|featured|Presents post as a large card below latest posts and added to “Featured” Sidebar underneath featured posts. Until it is older than the four most recent posts, then it is removed from the large card and kept permanently in the “Featured” section below.|

{: .danger }
When contributing, do not edit the `tags:` front matter space unless instructed by a head editor. This is not for all contributions and is only for special articles.

***

## Starting a new file

It is highly recommended to use the template post (`template.md`) because it contains correctly formatted [Front Matter](index#front-matter).

1. Go to [dillinger.io](https://dillinger.io)
2. Select `Import From ↓` dropdown button in the upper-right corner of Dillinger,
3. Select `Markdown File`, this will open a file select menu,
4. Navigate to `/Documents/GitHub/csartisan.github.io/_posts/template.md`

{: .danger }
DO NOT import from GitHub. Although this seems like the most straightforward path, Dillinger doesn't have the right permissions and can give unwanted results.

### Renaming the new file

For the post to function properly, the file name must first be formatted in a very specific way.

Every post must use the following format:

`YEAR-MONTH-DAY-title.md`

Where `YEAR` is a four-digit number (i.e. 2023), `MONTH` and `DAY` are two-digit numbers. `title` is where the title of your article will go. This isn't the title that will be seen on the website, instead, it is the title that appears in the URL (ex. `csartisan.github.io/art-therapy/`). Try to keep this as close to the actual title as possible.

Ex: `2022-12-16-art-therapy.md`

Make sure to get the date correct, because this is the only spot to do so.

{: .important }
If you are transferring old csartisan.wordpress.com posts, the date of the article will prepend the PDF viewer. It is expected that these old articles are set to the date of the issue release.

### Adding to the Front Matter

|Tag|Use|Example|
|---:|:---|:---|
|`layout:` | Do not touch this section. It should always be `post`. | `post`|
|`title:` | The title of your article, in quotation marks. | `"Art Therapy"`| 
|`author:`| The author of your article as "First Last", in quotation marks. | `"Octavia Roberts"`|  
|`categories:` | The category your post will be in, between [brackets]. If the category is unapparent, use `[ misc ]`. See ["Categories"](index#categories) for all available categories. | `[ misc ]` |
|`image:` |The full path to your article's image. See "[Images](index#images)" for more info.| `./assets/images/posts/none/1.jpg`
|`imagecred:` |Credit to image source, in quotation marks. If none, leave __completely blank__, no quotation marks. | `"Kathryn Mueller"`
|`tags:`  |This should only be edited by a head editor, it defines a post's location on the main page. Leave blank unless instructed otherwise. See ["Tags"](index#tags)| `[ ]`

## Content Guidelines

This is a very important step. Although many things may be up to personal interpretation, these guidelines will instruct choices that you will have to make when formatting new articles. 

### Section 1 - Importants

#### 1.1
Do not edit any original content in the article.

#### 1.2
Keep the general structure of the article.

#### 1.3
Fulfill all required [Front Matter](index#adding-to-the-front-matter).

#### 1.4
Add an image that correctly represents the article.

#### 1.5.1
All file names must use dashes to separate each word.

i.e. `interviewing-the-endelman.md`

#### 1.5.2
Keep all file names relative to the article title.

#### 1.6
Do not indent paragraphs.  

### Section 2 - Markdown Formatting

#### 2.1
Keep all paragraphs in body form. (Unformatted)

#### 2.2
Separate new paragraphs by a full line break. Markdown doesn't make new paragraphs unless they are separated by a full line break. See below.

![](/assets/img/markdownlinebreakartisan.png)

#### 2.3 
Interviews from the WordPress with questions as headers should use `h3` headers.

#### 2.4
Remove every __first__ quotation mark from a quote and replace them with a `>`. See below.

<div class="code-example" markdown="1">

> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged." 

</div>
```markdown
> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged."
```
This will render on the website as a large drop quotation. See below.

![](/assets/img/dropquoteartisan.png)

#### 2.5
Do not add credits to the author at the end of the article. This is done automatically by the website from the Front Matter.

***

## Exporting

Exporting from Dillinger is even easier than importing. 

1. Ensure that your document is finished and follow the rules from [Contributing](dillinger#contributing),
2. Select `Export As ↓` button in the upper-right of Dillinger,
3. Select `Markdown`,
4. Save file to `/Documents/GitHub/csartisan.github.io/_posts/template.md`, being sure not to change to name of it whilst saving.
5. Using your system file explorer, rename this new file from `template.md` to the name of your article, ending in `.md`. (i.e. `interviewing-the-endelman.md`) Refer to sections [1.5.1](index#151), [1.5.2](index#152).

Congratulations! Your post is now in your local copy of the club website. Now onto the final step, getting your post checked and added to the website.

{: .next }
Continue to [Finalizing](/docs/finalizing/).