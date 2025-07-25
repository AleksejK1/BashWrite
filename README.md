# BashWrite - [demo](https://raycc51.github.io/BashWrite/)

![screenshot](screenshot.png)

Single, pure bash script to make your blog.

You can find more information on the [demo](https://raycc51.github.io/BashWrite/) site.

Inspired by [bashblog](https://github.com/cfenollosa/bashblog)

## Features

- No dependencies
- Support extended Markdown with [mattcone/markdown-guide](https://github.com/mattcone/markdown-guide)
- Darkmode
- Tags
- Recent posts
- Pinned posts
- RSS
- Github Pages

### Limits

- Hard to customize
- [Markdown to html converter](https://github.com/RayCC51/md2html) is not perfect - [bug list](https://raycc51.github.io/BashWrite/posts/markdown/md4html-bug.html)

## Quick start

### Install

1. Download `bw.sh` - [Release page](https://github.com/RayCC51/BashWrite/releases).
2. Open `bw.sh`, edit settings and save the file.
3. Open *terminal*, and run `./bw.sh b`
4. Then your blog will be generated!

### Write new posts

1. Write a markdown file in *write/*.
2. The markdown file should start with [frontmatter](https://raycc51.github.io/BashWrite/posts/frontmatter.html)
    ```
    ---
    title: My new post
    description: Write description of this post.
    date: 2025-02-05
    lastmod: 2025-05-02
    tags: tags seperated by a whitespace
    draft: false
    pin: 1
    banner: image.png
    ---
    ```
3. Save your file and run `./bw.sh b`

### Remove posts

1. Remove a markdown file in *write/*
2. Run `./bw.sh b`
3. The script will delete files and links.

## Commands

- `./bw.sh h` : Show help dialog.
- `./bw.sh b` : Build the blog.
- `./bw.sh r` : Force a rebuild.

## About directory structure

### Download from repo

- bw.sh
- .github/ - Download this folder if you want to use Github Pages.

### Automatically generated: Do not edit these files

- backup/
- checksum/ - Checksum list to compare the diffrence of files.
- posts/
- tags/
- 404.html
- all-posts.html - List of every posts.
- all-tags.html - List of every tags.
- index.html
- robots.txt
- rss.xml
- style.css
- sitemap.xml

### Create these folders yourself, and work only within these folders

- write/ - Write your markdowns in this folder. You can also add assets needed for the posting.
- assets/ - Add any assets in this folder.

## Contributing

1. I am always welcome to any issues pointing out my English spelling or grammar since I am not very good at English.
2. There are no specific contributing rules. Feel free to leave issues or send pull requests, and I will handle them accordingly.
