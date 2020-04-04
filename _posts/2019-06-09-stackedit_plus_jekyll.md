---
layout: post
title: 'An unusual and practical CMS for Jekyll: StackEdit'
author: Danilo Lessa Bernardineli
tags: 'jekyll, cms, markdown, stackedit, bloggin'
categories: blog
date: '2019-06-09'

---


Today I've found out an very interesting way to manage Jekyll websites on GitHub/GitLab which fits very neatly onto my workflow, which is using StackEdit. There are a lot of advantages of trying that, which includes:

1. StackEdit is platform-agnostic and runs well on PCs and smartphones, as it is an progressive web app. So yeah, you can utilize it as if were an 'normal' app anywhere.
2. StackEdit have workspace synchronization through Google, which means that you can work on different devices without having to do any differently when you go to another device.
3. You can select explicitly what you want to share, and what you want to be private. This makes StackEdit an powerful warehouse of all kinds of writing that you do have.
4. You can reutilize photos easily from Google Photos, which makes the StackEdit enviroment almost perfect for an Google ecossystem user.

![StackEdit works on Android too](https://lh3.googleusercontent.com/cDzuTZjICt-uK53TSYeXpbnTHp6bZj8a9gJ_SB1m5JULLXG7SWnY_HtDT6-X6_gZ835N8B1ZUCsDIQ "StackEdit works on Android too")

Summing it up, StackEdit mitigates a lot of the weaknesses associated with the editorial workflow for Jekyll when you are a lonely blogger without an complete tech team and infrastructure for backing you up. For you that uses websites on public repositories, maybe this is what you've been searching all along!

![This is the StackEdit writing workspace and blogging CMS](https://lh3.googleusercontent.com/acH8KxqJEQlAiqu0NfAcog7rreAfnrR_ya8r9D0gDCUaAizmbe4nTWlN2aqIFZ55bqgaECiYlX9fyg "StackEdit writing workspace")

In fact, this post is actually an working test of using it as an CMS.

For this to work, there are a number of steps:

1. First, you must be able to publish StackEdit documents through GitHub/GitLab, which means that you're going to create an OAuth2 Application URL on your account. 
2. Then, you must configure StackEdit by putting the relevant configuration parameters when trying to publish an document.
3. Now you must prepare StackEdit to be able to publish your posts and pages in a manner that Jekyll recognizes.

The last step depends a lot on your Jekyll configuration. For example, on my gitlab website I use this template for creating posts on my blog or documents sections:
```
---  
layout: page  
{{{files.0.content.yamlProperties}}}  
---    Publish now Update current file publications.
  
  
{{{files.0.content.text}}}
```

The yamlProperties on this template is given by the parameters on File properties for each StackEdit document, which for this post are:
```
title:  'An unusual and practical CMS for Jekyll: StackEdit'  
author: Danilo Lessa Bernardineli  
tags:  'jekyll, cms, markdown, stackedit, bloggin'  
categories: blog  
date:  '2019-06-09'
```
Afterwards, publish it on your Jekyll repository and into the correct filepath, and you're done! StackEdit will automatically publish newer editions when you edit it, and you can visualize your output while you're editing your document. Awesome

![Publishing to GitLab example](https://lh3.googleusercontent.com/wqrzTQzcr6UU9Zf_gCtkvovyivnDzE_u9sbGOlp9cPt0RH5qRa5ZEoIjFqOPqZXduBarE_ASKVA2rQ "Publishing to GitLab")


