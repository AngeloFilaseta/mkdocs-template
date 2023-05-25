[use]: https://github.com/Andre601/mkdocs-template/generate

[MkDocs]: https://www.mkdocs.org/

[squidfunk]: https://github.com/squidfunk
[MkDocs Material Theme]: https://github.com/squidfunk/mkdocs-material

[facelessuser]: https://github.com/facelessuser
[PyMdown Extensions]: https://github.com/facelessuser/pymdown-extensions/

[Netlify]: https://netlify.com

[mkdocs.yml]: https://github.com/Andre601/mkdocs-template/blob/master/mkdocs.yml
[docs folder]: https://github.com/Andre601/mkdocs-template/blob/master/docs
[workflow]: https://github.com/Andre601/mkdocs-template/blob/master/.github/workflows/deploy.yml

[LICENSE]: https://github.com/Andre601/mkdocs-template/blob/master/LICENSE

[gh-pages]: https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

# MkDocs Material Template
This is a template repository for anyone that wants to use the MkDocs Material Theme.

## Getting Started
To get started, first clone this template by clicking on the Green button labeled [`Use this template`][use].

To install all the requirements simply:
```bash
pip install -r requirements.txt
```

### Creating pages
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

## Build Pages
To build pages (locally) can you use the `mkdocs build` command in your prefered command prompt.  
Note that for the successful execution of this command you have to...

- ...be in the folder that contains the `mkdocs.yml`
- ...have Python 3.7 installed
- ...have MkDocs and all required dependencies such as Material for MkDocs installed.  
Note that Material for MkDocs automatically downloads MkDocs and also certain extensions such as the [PyMdown Extensions].

MkDocs would now build the HTML in the defined configuration folder for you to use.

## Deploy to GitHub
If you want to publish the pages on GitHub Pages can you use the [premade workflow][workflow] for this.  
This workflow will setup Python, download Material for MkDocs and all its dependencies and deploy the pages to the `gh-pages` branch to then be viewable under `<username>.github.io/<repository>` (unless you defined a specific CNAME through a CNAME file in the [docs folder]).

Note that in order for this to work will you need to have a `gh-pages` branch already made.

## License

This template is served under the MIT license.  
Read the [LICENSE] file for more info.  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

### Credits
This repository started from [Andre601/mkdocs-template](https://github.com/Andre601/mkdocs-template).
