---
layout: post
title:  "Add a new post tutorial"
author: hubi
image: assets/images/developer_image.png
featured: true
toc: true  # Table of content
beforetoc: "A dummy guide to add a new post."
---


# Instructions for adding a new blog post

First of all, login on the [diegoenicole](https://github.com/diegoenicole/diegoenicole.github.io) page using your credentials:
```
email: diegoenicole.australia@gmail.com
password: you should know it lol
```

## Add the post file

Open the `diegoenicole.github.io/_posts` folder and add a new file: `Add file -> Create new file`. You should see an editor like the one in the following picture.

{% include image.html url="/assets/images/editor_github.png" width=600 %}

### Name of the file

The name of the file (that you shall insert under `Name your file...`) **MUST** be formatted in the following way:

```
YYYY-MM-DD-your-title.md
```

- `YYYY` is the year (4 digits), `MM` is the month (2 digits, if the month is January with 1 digit only, put `01`), `DD` is the day (2 digits, if the day has less than 2 digits put a zero in front). The date is important because posts are sorted by date (most recent first).

- `-your-title` is a meaningful name for the blogpost (**do not use spaces**, use hyphens `-` instead).

- The extension of the file must be `.md`.

For example, this post's file name is: `2022-01-08-add-post-instructions.md`. The posts you add should be similar too!

### Header

In the editor open, copy this header (including the three hyphens `---` at the beginning and at the end):

```
---
layout: post
title:  "Your title"
author: diegoenicole
image: assets/images/NAME_OF_THE_IMAGE
featured: false
---
```

Here is a short description of the entries:

- `layout: post`: leave it as it is.
- `title: "Your title"`: Instead of `Your title` insert a meaningful title for the page. This is what gets displayed in the homepage in the blog post preview. Remember not to delete the `"` characters!
- `author: diegoenicole`: This is who writes the post. You have four possibilities (although you should use only three lol). Remember that the syntax for the names cannot be changed (copy-paste them so that you don't make mistakes!)
    1. `diego`: Only Diego.
    2. `diegoenicole`: Both Diego and Nicole.
    3. `nicole`: Only Nicole.
    4. `hubi`: The author of this tutorial. Don't use this author ;)
- `image: assets/images/NAME_OF_THE_IMAGE`: This is the image that gets displayed in the blog post preview. You should substitute the `NAME_OF_THE_IMAGE` with the name of the picture that you upload. More instructions in the section [Add pictures](#add-pictures).
- `featured: false`: you can choose either `true` or `false` (with this exact syntax!). If the post is featured, then it appears on top of all other posts in the homepage regardless of its date. See image below: the only featured post is the page `Add a new post tutorial`.

{% include image.html url="/assets/images/featured_vs_nonfeatured_posts.png" width=600 %}

For example, the header for this blog post is:

```
---
layout: post
title:  "Add a new post tutorial"
author: hubi
image: assets/images/developer_image.png
featured: true
---
```

### Synatx

Below the header, you can write what you want. As easy as that! :) 

A small caveat: the page is written using [Markdown](https://www.markdownguide.org/basic-syntax/#bold-best-practices) language. Don't be scared, it is super easy.

Just a few simple instructions (if you get super interested you can learn all keywords at the link above):

- To make a large title, use the hashtag character. For example, in order to make the big title at the beginning of the page you can use `# Instructions for adding a new blog post` (always put a space after the `#`).
- To go to a new line, you have to press enter twice.
- To write a sentence, simply write the sentence as you would do in any Word document!

Although it might look complicated and scary, it really isn't! To have a look at a well-formatted markdown file, please have a look at the file `diegoenicole.github.io/_posts/2021-12-22-diego-and-nicole-leave.md`.


### Save

In order to save, you have to press the green button `Commit changes` leaving all other fields empty! If you want to modify a file after it has been saved, you have to press the small pencil button "edit file"

{% include image.html url="/assets/images/edit_button.png" %}


## Add pictures

Hopefully, your blogposts are going to be super full of beautiful pictures <3 

Inserting an image in your blogpost takes only 2 passages:

1. uploading the picture
2. use the correct markdown syntax

### Upload the picture

In order to upload the picture, you need to move to the folder `diegoenicole.github.io/assets/images/`.

For the records, you can see your current path as in the screenshot below

{% include image.html url="/assets/images/path_screenshot.png" %}

Press the button `Add file -> upload files` and choose your files. Press the green button `Commit changes` and the image is uploaded. Notice: **you cannot upload more than 1GB of pictures**!


### Syntax

After you have uploaded the image to the right folder `/assets/images/...`, you can finally add such image to any of your blog posts. In order to do it, simply move to the directory `diegoenicole.github.io/_posts` and open the blog post that you want to modify (adding an image). Click the edit button (the small pencil)

{% include image.html url="/assets/images/edit_button.png" %}

and you should be displayed with the editor. 

Where your image should be, simply type:


{% raw %}
```markdown
{% include image.html url="/assets/images/yourpicture.png" %}
```
{% endraw %}

The only thing that you have to change is `yourpicture.png`, which needs to be the precise name of the picture you have uploaded. 

See the file `diegoenicole.github.io/_posts/2021-12-22-diego-and-nicole-leave.md` for an example.

Always remember to save the file with the green button `Commit changes`.

If the picture is too large, you can shrink it by using the following syntax:

{% raw %}
```markdown
{% include image.html url="/assets/images/yourpicture.png" width=500 %}
```
{% endraw %}

Usually pictures taken with a phone have a width of 1080 or 1920 (depending if the picture is vertical or horizontal). If the picture is horizontal and you want to cut it in half (1/4 of the total surface) just use as width 1920/2 = 960.


## Wait

To conclude: the page gets rendered in a few seconds/minutes. Hence, every time you press the green button and do some changes, you have to wait a few seconds or minutes before the website [diegoenicole.github.io](https://diegoenicole.github.io) is actually modified.