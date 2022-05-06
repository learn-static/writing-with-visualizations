---
section: Write Your Essay
nav_order: 2
title: Markdown 
topics: Markdown
description: >
    This text is a 'section description'. Directly below this is an example section video embed. This demonstrates the front matter options in action.
youtubeid: moJgWrD6dwg
---


## Step 3. Practice adding text content to your essay page

1. While viewing your website, click on the "Essay In Progress" link in the navigation menu. This should take you to a page titled "My Essay Title." Scroll down this page, taking note of the different heading styles, font styles, bullet point lists, images, pdfs, and citations.
2. To edit the content on this page, go back to the tab/window that contains your GitHub repository.
3. In your GitHub repository, locate and click on the "pages" folder.  
4. Inside the "pages" folder, click on the file titled "essay-01.md." Then select the pencil button in the top right corner of the `essay-01.md` file to open editing mode. 
{:#frontmatter}
5. Once in editing mode, at the very top of the file, you'll see the following:
```
---
title: Essay 1
layout: about
permalink: /essay-01.html
---
```
This little grouping of text is called "frontmatter."
It must be left exactly as it is for your site to work correctly, so ***don't change it!***. 
Just ignore it, and skip to the line of text below it that says `# My Essay Title`.

Remember your "Essay In Progress" page that we just looked at?
It was also titled "My Essay Title"! 
That's because the `essay-01.md` file is the "back end" for the "Essay In Progress" webpage.
In other words, when you write content into the `essay-01.md` file, that content will show up on the "Essay In Progress" page on your website.

You'll notice that the content currently in `essay-01.md` is formatted in a way that's probably different from what you're used to. 
This is because this content is written in a format called "Markdown."
Markdown was developed as a simple way to write content for the web without using HTML (hyptertext markup language), a language commonly used to write content for websites.
We're using Markdown for your essays because it is much simpler than HTML, yet it will still allow you to easily incorporate images, pdfs, and visualizations into your essays.

Markdown is very similar to the way you write and format content in Microsoft Word documents, with a few key differences:

{:#headings}
### Headings

Headings are used to title a section in your essay, and are indicated with one or more pound signs (`#`) in front of them.
One `#` indicates the largest heading: heading one. For example:

`# Heading One` in your `essay-01.md` will look like:

# Heading One

on your "Essay In Progress" webpage.

You can make smaller headings, too:

Two `##` indicates heading two, which is slightly smaller than heading one:

## Heading Two

Three `###` indicates heading three, and so on.

### Now try it yourself

1. In your `essay-01.md` file, replace the words in the first heading `# My Essay Title` with a new title for your essay (note, this doesn't have to be what you officially title your essay, it can be anything you want right now, this is just practice). Make sure you include one `#` in front of your essay title, like this: `# My New Essay Title`.
2. After you've added a new title to your `essay-01.md` file, scroll down to the bottom of the file and type a commit message into the "Commit changes" text box.
3. Click the green "Commit changes" button to save your changes.
4. Head over to where you opened your "Essay In Progress" page in a different tab or window.
5. Wait a minute or two, then refresh the "Essay In Progress" page.
6. Once you refresh your site, you should see your new title displayed where "My Essay Title" used to be.
7. The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

You'll notice that `# My Essay Title` doesn't appear with a `#` in front of it on your actual website.
This is because the computer translates it into the appropriate code, so that it appears as a large title on your page, without displaying the `#` that you added on the back end.

Now that you've seen how the back end is translated into the front end of your website, you can continue to learn a few other features of Markdown:

{:#paragraphs}
### Paragraphs

Paragraphs in Markdown can be written exactly as you write them in Microsoft Word, but *without a tabbed first sentence* and *with a blank line in between paragraphs*.
In other words, you can string together sentences one after another as you are used to doing when you write papers or emails, and they will appear in a paragraph on the front end of the webpage.

*However*, be aware that **if you don't put an empty line *between* your paragraphs when you write them in your `essay-01.md` file, they will all join into one *massive* paragraph on your "Essay In Progress" page**.

For example, these two paragraphs have a blank line in between them, and will translate accordingly from the back end to the front end:

**Back end view (`essay-01.md`)**:

`Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent maximus ex vitae odio condimentum molestie. Cras porta, metus non tempus pellentesque, odio libero porttitor lectus, vel eleifend enim enim cursus nibh. Mauris aliquam dignissim nunc eget viverra.` 

`Duis in nisl in enim iaculis scelerisque. Ut congue ipsum nisi, nec ultrices nulla porta vel. In ultrices erat orci, in imperdiet dui tempor non. Nam placerat non ante nec viverra.`

**Front end view ("Essay In Progress")**: 

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent maximus ex vitae odio condimentum molestie. Cras porta, metus non tempus pellentesque, odio libero porttitor lectus, vel eleifend enim enim cursus nibh. Mauris aliquam dignissim nunc eget viverra. 

Duis in nisl in enim iaculis scelerisque. Ut congue ipsum nisi, nec ultrices nulla porta vel. In ultrices erat orci, in imperdiet dui tempor non. Nam placerat non ante nec viverra.

**But the following two sentences will merge into one paragraph when rendered on the front end, even though they are written on separate lines on the back end:**

**Back end view (`essay-01.md`)**:

```
Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
Praesent maximus ex vitae odio condimentum molestie.
```

**Front end view ("Essay In Progress")**: 

Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
Praesent maximus ex vitae odio condimentum molestie. 

**So, make sure to leave empty lines between your paragraphs, and between headings and paragraphs.**

### Now try it yourself

1. Click the pencil button at the top right of your `essay-01.md` file to open editing mode.
2. Underneath the new essay title that you just created, add two or three sentences of text (the subject can be anything, related or unrelated to your essay topic, this is just for practice).
3. Scroll down to the bottom of the file and type a commit message into the "Commit changes" text box.
4. Click the green "Commit changes" button to save your changes.
5. Head over to where you opened your "Essay In Progress" page in a different tab or window.
6. Wait a minute or two, then refresh the "Essay In Progress" page.
7. Once you refresh your site, you should see your new sentences.
8. The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

### Font styles

{:#italic}
To make a word or phrase *italic*, add one asterisk before and after that word or phrase, like this: `*example phrase*`.
The asterisks won't be visible on your webpage, but your text will appear italicized.

{:#bold}
To make a word or phrase **bold**, add two asterisks before and after that word or phrase, like this: `**example phrase**`.
Again, the asterisks won't be visible on your webpage, but your text will appear bold.

{:#hyperlinks}
### Hyperlinks

To link to another page or site, insert the link title (what you want displayed to the site visitors) into square brackets, followed by a URL in parentheses: 
`[GitHub Help](https://help.github.com/)` in your `essay-01.md` file will look like [GitHub Help](https://help.github.com/) on your "Essay In Progress" webpage.

{:#lists}
### Lists

You can create lists in two different ways:

A bullet list is created using a hyphen (`-`) in front of each bullet point:

- dog
- cat
- muffin

A numbered list is created using a number followed by a period (`.`) in front of each list item:

1. one
2. two
6. three
2. four

### Now try it yourself

1. Click the pencil button at the top right of your `essay-01.md` file to open editing mode.
2. Underneath the new sentences you just added, add some italic and bold text, a hyperlink, and either a bullet list or numbered list.
3. Scroll down to the bottom of the file and type a commit message into the "Commit changes" text box.
4. Click the green "Commit changes" button to save your changes.
5. Head over to where you opened your "Essay In Progress" page in a different tab or window.
6. Wait a minute or two, then refresh the "Essay In Progress" page.
7. Once you refresh your site, you should see your changes.
8. The updates may take a few seconds to a few minutes to appear, so hold tight and keep refreshing if you don't see them right away.

As you practice adding content to your `essay-01.md` file, you can delete much of the content that was pre-added to the file if you'd like, **except** for the frontmatter at the very top (looks like this): 
```
---
title: Essay 1
layout: about
permalink: /essay-01.html
---
```

Also **do not delete** the line of code that comes after the frontmatter, which looks like this: `{% raw %}{% include feature/nav-menu.html sections="Introduction;Conclusion;Notes" %}{% endraw %}`.
We'll discuss this line in more detail next week.

Otherwise, you're welcome to delete or simply ignore the other content already in the `essay-01.md` file for now.
You'll notice that there are some Markdown formatting options present in `essay-01.md` that we didn't cover in our Lab this week, but we will get to those next week.
