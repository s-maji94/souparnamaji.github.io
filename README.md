# Souparna Maji Portfolio

This is a Hugo website based on the HugoBlox Academic CV theme.
https://github.com/HugoBlox/theme-academic-cv

HugoBlox has a complete set of "blox" used to customize your site. Here are some helpful instructions about HugoBlox in general:
https://docs.hugoblox.com/

## (one-time) Fork the repository
Create a copy of this repository under your own username so you can control the repository settings. Detailed instructions here:
https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo#forking-a-repository

You may choose your preferred name of the repository.  If you choose to name the repository `<username>.github.io`, where
`<username>` is your own username, the site will be published at `<username>.github.io`. If you choose any other repository name,
the url will be `<username>.github.io/<repository-name>`.

## (one-time) Set up GitHub Pages publishing
GitHub does not automatically start publishing your webpage, you must configure it to be on. There is already a custom
workflow in the repository that has been set up called "Deploy Hugo site to Pages", but it needs to be enabled. You do not
need to create a new workflow. Detailed instructions are here about enabling the workflow:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow

After completing this step, you should be able to view your webpage in the browser based on your username and repository name
as described in the previous step.

## (one-time) Configuration a custom domain name (optional)
Details about configuring a custom domain name are here: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## (one-time) Setting up a development environment
You may edit the site by either installing GitHub Codespaces in the browser, or by setting up an environment locally. More
instructions are here: https://docs.hugoblox.com/getting-started/install-hugo/

## Helpful tips on customizing the webpages
Most of the site content is set up using Markdown. Info about Markdown here: https://gohugo.io/content-management/formats/#markdown
One helpful tip is that if you are trying to put a line break between two lines, end the first line in Markdown with a double space.
### Navigation Menu
The pages that show up on the navigation bar can be customized in `config/_default/menus.yaml`. In particular, the "Hobbies"
and "Media" page already exist, but are not available in the menu because they are commented out. Remove the `#` that are on
lines 34-39 to uncomment those lines and those pages will appear in the navigation menu.

### Bio / Homepage
The starting point for the structure of this site is in `content/_index.html`. Some content is found there, but a lot of
the content is pulled from your author profile at `content/authors/admin/_index.html`.  The bio pic is pulled from
`content/authors/admin/avatar.[jpg|png]`, so if you'd like a new picture, rename your new photo to be `avatar` and replace
the photo in that folder.

### Experience
The initial structure of the page is defined in `content/experience.md`. Content details are pulled from `content/authors/admin/_index.html`.
The "Read More" links point to pages that are defined in the `content/experience` directory.

### Research
This page is defined in `content/research.md`. Photos are from `content/research/img`.

### Teaching
This page is defined in `content/teaching.md`. The "Read More" links reference pages in the `content/experience` directory.

### Talks
Defined in `content/taks.md`

### Publications
Page layout is defined in `content/publications.md`. The articles are found in their respective directory, in
`content/peer-reviewed`, `content/policy-articles`, `content/popular-articles`. To replace the image for the publication,
find the appropriate folder for the article/paper, and replace the featured.[jpg|png] image. Must be named "featured".

### Awards & Grants
Defined in `content/awards-and-grants.md`

### Service
Defined in `content/service.md`

### CV
Defined in `content/cv.md`.  The CV it references is found in `static/uploads`.

### Hobbies
Defined in `content/hobbies/_index.md`. Automatically uses content in the subfolders in `content/hobbies`. Images in each
subfolder must be called `featured`.

### Media
Defined in `content/media.md`
