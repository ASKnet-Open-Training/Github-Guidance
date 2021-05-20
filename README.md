# #ASKnet Github-Guidance

This repository includes a guide to help with using Github.This guide was created at one of the worldwide #ASKnet programs, which is about helping people to help themselves.  With Github or Git in the background, actions/projects or ideas can be documented wonderfully and archived in historical versions.This guide is from the beginning as a git repository about a git repository :)

## --===<({   [Github Guidance Here](https://asknet-open-training.github.io/Github-Guidance)   })>===--

There you find all information about how to use Github and get support

Some important informations:
1. Working with you GitHub account issues.
2. Creating repository and forking existing repository.
3. Using issues for communicating tasks.
4. Handling merges and merges conflicts.
5. Mastering other collaboration features of the platform

## Feedback

If you want to give us feedback, feel free to write us: [Give a Feedback](https://github.com/ASKnet-Open-Training/Github-Guidance/issues/new)

## Developers

The guide consists of Markdown files that are rendered as HTML pages using jekyll and Github Actions.

If you have a suggestion or even concrete content incl. screenshots, feel free to [write us an issue](https://github.com/ASKnet-Open-Training/Github-Guidance/issues/new).

If you already know the basics of Git and Markdown, feel free to write content yourself. Here you can learn how to edit content. There are two methods to get to the right place you want to edit.

### Method 1 Get to the content via the HTML page (easier)

With this method, only already created manuals can be edited and no new ones can be created. To find the desired content, it is best to switch to the HTML page and search for the desired page there: https://asknet-open-training.github.io/Github-Guidance/

Then browse to your desired page and you'll find an `Edit this page on GitHub` link at the bottom of each page. Clicking on it will take you to the exact Markdown file you want to edit.

![Edit this page](assets/images/readme-edit-this-page.png)

Once you have reached the Markdown file, you can use the pen button to go into edit mode and change the content. Afterwards, the change is saved as a commit or a change suggestion is made in the form of a pull request. How a [commit](https://asknet-open-training.github.io/Github-Guidance/pages/github-repo/file-save/) works or a [pull request](https://asknet-open-training.github.io/Github-Guidance/pages/github-repo/pull-request-create/) is made, you can find out [in this guide](https://asknet-open-training.github.io/Github-Guidance/) ;)

![Edit file.png](assets/images/readme-edit-file.png)

### Method 2 Use the Git Repository (advanced)

With method 2 you can not only edit instructions, but also create them yourself and upload images.

You can go through the Git repository and mainly all the content for the guide can be found in two directories:

- assets -> [images](https://github.com/ASKnet-Open-Training/Github-Guidance/tree/main/assets/images)
- [pages](https://github.com/ASKnet-Open-Training/Github-Guidance/tree/main/pages)

You can ignore the other directories or files.

![Folders for the guide](assets/images/readme-folders-for-the-guide.png)

### Pages

In the [pages](https://github.com/ASKnet-Open-Training/Github-Guidance/tree/main/pages) directory you will find all pages sorted into the subfolders corresponding to the main points of the guide (e.g. github-account, github-repo or github-issues).

In the desired folder you can either edit pages or create new pages.

To create a page you have to create a new Markdown file. You can use any name, but it must **not** contain special characters or spaces. At the end of a file must be `.md`

Example: `image-upload.md`

The following information must be entered at the top of the file:

```
---
layout: default
title: Upload images to Repo
parent: Github Repository
nav_order: 7
---
```

Then save the page with a commit.

### Images

#### Where are the images located

All images are uploaded to the [images](https://github.com/ASKnet-Open-Training/Github-Guidance/tree/main/assets/images) directory. This directory is located in the parent directory `assets`. 

The name of an image should be descriptive and not e.g. ~~IMG_345345345.jpg~~. It is recommended to use the name of the main topic (e.g. github-repo, github-account or github-isses) at the beginning and after `-` the name of your new manual.

Example: `github-repo` `-` `create-new-repo` `.png` ([View images folder and upload images](https://github.com/ASKnet-Open-Training/Github-Guidance/tree/main/assets/images))

**Important:** Do not use spaces or special characters in file names and do not upload images that are too large. Otherwise the entire repository would become too big.

Alternatively, you are welcome to [write us an issue](https://github.com/ASKnet-Open-Training/Github-Guidance/issues/new) and upload your desired image there. You just have to tell us on which page the image should be displayed ;)

#### Insert image into Markdown file

You can use the usual Markdown standards. Then the full URL including `https://...` must be used.

```
![ASKnet Logo](https://raw.githubusercontent.com/ASKnet-Open-Training/Github-Guidance/main/assets/images/partner-asknet-logo.jpg)
```

This works, but isn't very flexible and a very long URL. Better are relative links.

##### Why are relative links better?

This guide should be flexibly usable (e.g. without internet connection) and freely expandable. You can even use this guide on your computer without having access to the internet.

Now we come to the relative links. The alternative are, as we have already learned, permalinks with a fixed URL. If images are now included with a permalink, then these images are not loaded from your local computer or your fork, but always from the main repository on Github in the internet. If we now use relative links instead, then the images and all content will always be loaded from your repository, no matter where it is. Whether on your computer or your new fork repository.

The code to include an image looks like this. You can ignore the cryptic characters `}`, `[`, `|`, etc. Just look at the path to your image: `assets/images/partner-asknet-logo.jpg`.

```
![ASKnet Logo]({{ 'assets/images/partner-asknet-logo.jpg' | relative_url }})
```

## Partners and Funder

| r0g_agency | ASKnet | BMZ |
| :--------: | :----: | :-------: |
|[![r0g_agency Logo](assets/images/partner-r0g-logo.png)](https://openculture.agency/)|[![#ASKnet Logo](assets/images/partner-asknet-logo.jpg)](https://github.com/ASKnet-Open-Training) | [![BMZ Logo](assets/images/founder_BMZ.jpg)](https://www.bmz.de/en/) |
| [Official Website](https://openculture.agency/) | [Official Website](https://github.com/ASKnet-Open-Training) | [Official Website](https://www.bmz.de/en/) |

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
