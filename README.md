## How to Write/Publish to blog.ksp2mars.org ##

This document is a guide on how to write for and publish to the KSP2Mars [blog](https://blog.ksp2mars.org), which is powered and hosted by [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com) respectively.


----------


When creating a post, you will probably have to write content and then insert images. Markdown is used to write posts for the site; a pretty good WYSIWYG in-browser Markdown editor is [stackedit.io](https://stackedit.io), which also has Google Drive integration so you can save directly to the KSP2Mars Drive share if you wish.

To insert images, please first upload them under *assets/images/image_name.png*<sup>[\*]</sup>. Note that the image will then be available under *https://blog.ksp2mars.org/assets/images/image_name.png*. If you are using StackEdit, to insert your image click the "image" icon in the top panel and paste the URL for your image.

To publish your post, please create a new file with the structure *YYYY-MM-DD-some-title.md*, under the *_posts* directory<sup>[\*]</sup>; inside the file, place the following **before** the body of your post.

    ---
    layout: post
    title: Title Of Your Post
    date:   YYYY-MM-DD 12:00:00
    tags: some_tag
    subclass: 'post tag-some_tag'
    categories: 'casper'
    navigation: True
    logo: 'assets/images/ksp2marsv1.png'
    cover: 'assets/images/cover4.jpg'
    ---
Please update the title, date, tags, subclass and cover items accordingly.

The cover is used for a fullwidth image over the post, and helps build atmosphere. You may specify the image in the same way as mentioned above, but here it is simpler to only use the path to the image (*assets/images/my_image.png*). If you do not wish to use a cover image, then update the line to say:

    cover: false
Which will stop the cover from showing.


----------
<sup>[\*]</sup> When in the respective directories in GitHub's web interface (under [this](https://github.com/KSP2Mars/blog.ksp2mars.org/) repository), click *Upload Files* to upload images and *Create New File* to create a markdown file; you will then need to "save" these by committing the file(s) to the repository.

<sup>[†]</sup>[This](http://commonmark.org/help/) is a relatively good, general Markdown cheat sheet.
