# Getting Started
To get started, first clone this template by clicking on the Green button labeled [`Use this template`][use].

To install all the requirements simply:
```bash
pip install -r requirements.txt
```

## Creating pages
To create new pages, just add new markdown files to the [docs folder] of the repository and edit them.  
MkDocs will then turn those into static HTML pages once you [build](#build-pages) or [deploy](#deploy-to-github) the pages.

The template also has some pre-made settings for your convenience to help you with creating documentation much easier.  
In the [mkdocs.yml] will you find many settings that you can alter. Please check the comments and the links they have for more info.

It also contains some extensions that might be useful including:

- Admonition
- CodeHilite
- ToC
- [PyMdown Extensions]

You're free to add, edit or remove any extension at your own discretion, but keep in mind that some expansions might cause compatibility issues with others or require to be downloaded first.  
For that, alter the `requirements.txt` if you also deploy pages using GitHub Actions.

## Linking images and media
The paths are relative to the current document (the path it's in). To ensure accurate rendering on the web and/or PDF,
kindly refrain from using file paths that begin with a slash when linking any media. Any `.md` file that is not named
`index.md` will be mapped to a file named `index.md` placed in a folder with the original `.md` file. For example,
a file called `game.md` in the docs folder will become `/game/index.md` once deployed. Keep this in mind when
referencing media.