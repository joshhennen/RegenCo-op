---
layout: article
title: How to Write a New Article
permalink: /info/How-to-Write-a-New-Article
comments: false
---

This guide will be a step-by-step manual on how to create an article and propose that it be added to the website using GitHub.

## Write the Article:

Before you start writing the article, it is recommended that you read the [article formatting guidelines](#todo) to get familiar with the basics of how our articles are formatted.

***

1. ### Download the template article:
   
   - Right click on the following link and click save link as... to save it to your desktop: [ArticleTemplate.md](https://github.com/RegenCo-op/RegenCo-op/raw/master/docs/_articles/ArticleTemplate.md)

2. ### Open the file from step 1 in your favorite Markdown editor.  
   **Note:** A good online editor is [StackEdit](https://stackedit.io/editor), and from now on we will assume you are using that editor for the purposes of this guide:
   
   - Using Stack Edit, for example, click on the "**#**" in the upper left corner.
   - Then click on "import from disk".
   - Then click "browse" and open the file from step 1.

3. ### Write the article: **Do not worry about pictures for now.**
   
   1. #### Fill out the top section:
      
      - **Ignore the first line that says layout: article**
      - Delete the text that says "Article Title Goes Here" and fill it in with your article's title.
      - Delete the text that says "Unique-Article-Permalink-Goes-Here" and replace it with a phrase that is unique.  
        **No spaces are allowed. Only letters (a-z), numbers (0-9), and hyphens (-) are allowed**.  
        The easiest thing would be your article's title, replacing the spaces with hyphens (-). For example: using the title: `My Article Title`, one would choose a permalink: `My-Article-Title`.  
        The most important thing is that it **doesn't share a permalink with another article**.  
        **_Make a note of what you typed here, as we will use it later, as follows:_** `Your-Permalink-Here`
      - **Most articles should leave the _comments: true_ section alone.**

   2. #### Write the content:  
      Now you can start writing your article after the last line with the three hyphens (---).
      
      - Make a note of where you want to put a picture, if any, but do not worry about how to insert it for now.
      - Keep in mind the [article formatting guidelines](#todo).
      - Also remember to refer to the [Kramdown reference guide](https://kramdown.gettalong.org/quickref.html) if the text isn't formatting the way you want it to.

   3. #### Save the article:
     
      - Using Stack Edit, for example, click on the "**#**" in the upper left corner.
      - Click the "**Export to disk**" button.
      - Click the "As markdown" button.

   4. #### Rename the article:
      Using the same permalink text you used in step 3, rename the article. It will look like this:  
      `Your-Permalink-Here.md`

4. ### Using images:  
   **Skip to the next step if you _do not_ want to use any pictures**.
   
   1. #### Prepare the images:
      
      1. Make sure pictures you want to use are copyright free or are your own original work.
      2. Rename the files so that they **do not contain any spaces**.
      3. Make sure the files are .jpeg, .png, .gif, or .svg format (you can use this [online converter](http://image.online-convert.com/convert-to-jpg) if they are not).
      4. [Compress the files here](https://compressor.io/). Compressed images make the page load faster and improve user experience for people with a slow internet connection.
      5. Put all the images you want to use in a folder on your desktop. Rename the folder the same as your permalink:  
`Your-Permalink-Here`

   2. #### Insert the images into the document:  
      **Note: _Images you use here won't appear in any previews_**
      
      1. Using the markdown format, insert the images into the article wherever you want. The format you use will look like this: `![image description](/images/Your-Permalink-Here/Your-Image-Here.ext)`
      2. Make sure to replace `Your-Permalink-Here` with the same permalink text you used in step 3.
      3. Make sure to replace `Your-Image-Here.ext` with the image filename, and **don't forget to use the right filename extension**.

## Set Up a New Fork

**Note:** You only need to follow these steps one time; In the future you can skip to the [next section](#submit-your-article-to-github).

1. Either [sign into github](https://github.com/login) or [make a new account](https://github.com/join).
2. Go to the [RegenCo-op repository on GitHub](https://github.com/RegenCo-op/RegenCo-op).
3. In the upper right corner, you will see a button called "Fork". Click on it to fork the repository to your account.
4. After a few seconds, you should now have a personal copy of all the files on the website.
5. It would be wise to make a bookmark of your forked repository, as that is what you will use to submit articles. If you do not, you can find it later at:  
   `https://github.com/YOUR-GITHUB-USERNAME-HERE/RegenCo-op`

## Submit Your Article to GitHub

By now you should have your article written and named: `Your-Permalink-Here.md` along with your images folder named: `Your-Permalink-Here`. You should also have [forked the RegenCo-op repository](#set-up-a-new-fork) and be signed into your [Github account](https://github.com/login). You are ready to submit your article to the website to be reviewed and published by members of the co-operative.

1. ### Updating your fork:
   - Go to your forked repository of the website. It can be found at:  
     `https://github.com/YOUR-GITHUB-USERNAME-HERE/RegenCo-op`
   - 

1. Making a topic branch:
   
1. Making and Pushing Changes:
  1. Open the RegenCo-op project folder (it will be wherever you saved it on your desktop during step 3 of setting up a new fork).
  2. Move the article file to the docs/_articles folder.
  3. Move the images folder to the docs/images folder.
  4. Edit the article layout:
    1. Open the docs/_data folder.
    2. Open the article_layout.yml file with a text editor.
    3. Following the directions in that file, type `Your-Permalink-Here` in whichever category you wish. If you want to make a new category, follow the given layout.
    4. Save and close the article_layout.yml file.
  5. Open the Github for Desktop application.
  6. When you’re ready to submit your changes, type up a commit summary in GitHub for Desktop, and click Commit. Right now, you’ve essentially told Git, “Okay, I’ve taken a snapshot of my changes!” You can continue to make more changes, and take more commit snapshots. When you’re ready to push your changes up to GitHub.com, click on the Sync button, which is right above your list of changes.
2. Making a Pull Request:  
At last, you’re ready to propose changes into the main project!
  1. Go to your forked repository. It will be at: `https://github.com/<your_username>/RegenCo-op`
  2. You’ll see a banner indicating that you’ve recently pushed a new branch, and that you can submit this branch “upstream,” to the original repository. Clicking on Compare and Pull Request sends you to a discussion page, where you can enter a title and optional description. It’s important to provide as much useful information and a rationale for why you’re making this Pull Request in the first place.
  3. Click on Create Pull Request to propose your new article.