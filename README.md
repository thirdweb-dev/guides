# Guides

We're gonna use this repo to track what guides we're working on and which ones do we plan to work on in the future.

These guides will live in [thirdweb.com/portal/guides](https://thirdweb.com/portal/guides).

If you want to write a guide, you can check the issues on this repo and pick one, or create a new issue with the topic you want to write about.

## How to create an issue

1. Use the name of the guide on the title of the issue.
2. Add a description on what the guide will contain.
3. Add why do you think you/we should write about this topic.
4. Add images/text showing people asking for this topic if you have them.
5. Add labels to your issue (see next section).

## Labels

### Topic
One or multiple:
- **nft-collection** - Guides related to the NFT Collection module, check [here](https://thirdweb.com/portal/guides/nft-collection).
- **drop** - Guides related to the Drop module, check [here](https://thirdweb.com/portal/guides/drop).
- **bundle** - Guides related to the Bundle module, check [here](https://thirdweb.com/portal/guides/bundle).
- **market** - Guides related to the Market module, check [here](https://thirdweb.com/portal/guides/market).
- **token** - Guides related to the Token module, check [here](https://thirdweb.com/portal/guides/token).
- **pack** - Guides related to the Pack module, check [here](https://thirdweb.com/portal/guides/pack).

If your guide doesn't use any modules, use:
- **general** - For guides not related to any of the previously mentioned modules, check [here](https://thirdweb.com/portal/guides/general).

### Language
- **typescript**
- **python**
- **go**

## How to write a guide

Explain step by step what users need to do to get the same results you're getting. Remember there's multiple OSs that people can use (Windows, MacOS, Linux) or maybe different package managers (npm, yarn) so be mindful of that.

If you are working with code, provide code snippets that people can copy and paste into their code.

If you are showing people how to do something, add screenshots and be explicit on where people should click or what should they do.

When you start writing the guide, move that guide issue to the **"In progress"** tab.

## How to format your guide

### Metadata

This is the first thing you need to add on the top of your .mdx file, this is the template we're using for now, with one of our existing guides as example:

```md
---
title: Create an NFT Gated website
author: "Jake Loo"
authorAvatar: "/assets/portal/authors/jake-loo.jpeg"
authorTwitter: "https://twitter.com/jake_loo"
draft: false
tags: [nft-collection, mint, access]
summary: "NFTs can be used as a membership, in this guide we'll show you how to setup a website that restricts content based on owning your NFT."
image: "/assets/portal/guides/thumbnails/3.jpg"
date: "2021-11-15"
updated: ""
featured: false
---
```

- **title**: The title of your guide.
- **author**: Your name
- **authorAvatar**: A picture (you can send it separetely, but it's good if it follows this format beforehand)
- **authorTwitter**: Link to your Twitter.
- **draft**: If it's a draft or not (defaults to *true*)
- **tags**: An array of tags, one of the tags should be one of the labels, the rest you choose.
- **summary**: Short explanation about what your guide is about.
- **image**: Thumbnail for your guide.
- **date**: Day that the guide was posted (we'll update this the day that it gets actually posted)-
- **updated**: If the guide is ever updated with new info or updated code, we'll modify this (defaults to *""*)
- **featured**: If we like your guide enough, we'll also feature it so more people can see it (defaults to *false*)

### Guide

- **Headings**: We use h2 and h3 for the table of contents, you can add an h2 using `##` and an h3 using `###`
- **Dividers**: Use `---` to add a divider.
- **YouTube videos**: First, import this library on the top of your file (under metadata)
```js
import Youtube from "mdx-embed";
```

and then you can embed the video with:

```js
<YouTube youTubeId="<!-- youtube id here -->" />
```
- **Images**: Images should have this structure for the imports: `![<!-- Alt text -->](/assets/portal/guides/<!-- Guide slug -->/<!-- image name -->.(png/jpg...))`
- **Links**: 
  - External: `[Check my Twitter](https://twitter.com)`
  - Internal: `[Check our dashboard](/dashboard)`
- **Bold** and *Italics*: Use them to emphasize so the text doesn't look bland. Use it with: `**bold**`, `*italics*`.
- **Code**: Use this for file names, package names, etc. Enclose the text in backticks.  ``hello.py``
- **Code blocks**: You can embed code snippets with whatever language you want, to do so, place a triple backtick in one line, followed by the language you want to use, then the code block, and three more backticks at the end.

` ```javascript ` // triple backticks followed by the language name

You can also add a file title to the code block by writing if after the language name and a colon.

` ```javascript:index.js ` // triple backticks, language name, colon and file name

This will add the title of the file to the rendered markdown on the portal.

- **React components**: If you want to use custom React components for your guide, that's totally possible, but let's first discuss why and how.

## Handing out the guide

When you have finished writing the guide, send an email to <nacho@thirdweb.com> or a message to nachoiacovino#4022 on [Discord](https://discord.com/invite/thirdweb).

In this message, you should add a zipped file with two things inside:
- `<-- Guide slug -->.mdx`
- `<-- Guide slug -->` folder with the images you are using in the guide inside. The name of the images should be the same name you referenced them with `<!-- image name -->` before.



