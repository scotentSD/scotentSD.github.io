# Blog
The Blog page has code to display any posts in the **posts** folder. The default layout is in the **Layout** folder: post.html

![Design in the open](/images/blogpost-code.PNG)


# Creating a Blog post
Create a markup file in the posts folder and name it in the format :

**yyyy-mm-dd-title.md**

This date will be used to create the line at the bottom of your post:

Written on dd mmm, yyyy

At the top of your file, add the following lines:  

```
---
layout: post
title: Welcome to this new blog
author: # (this is optional)
tags:  # to discuss, optional as a list:  ['a11y', 'communication', 'pattern'] for example  
published:  # if you don't want it to be displayed yet, then the value should be false - otherwise put true or ommit the line all together
---
```



This will give the correct layout for your post, and use that title for the blog post itself and for it to be listed with the other blog post on the main blog page.

If an excerpt marker is defined in the `\_config.yml` file then you can mark a section of the post as the excerpt. 
Everything above the  `<!—more—> `code will be the summary we can see on the main blog page. Anything below can only be seen if you click on the blog post link.

```
<!--more--> 
```

Add this line to the `_config.yml` to enable the excerpt marker:

``` 
excerpt_separator: "<!--more-->" 
```
