# Rendering

You can render the website locally by running `quarto render` in the terminal. The website is then rendered in the folder ./docs. See the current version by opening ./docs/index.html.

# Personalisation

### Edit the following files to alter the respective tabs

| File | Role |
|---------------------------------|---------------------------------------|
| `./_quarto.yml` | Meta information for the website |
| `./index.qmd` | Welcome page |
| `./pages/research.qmd` | Research tab |
| `./pages/presentations.qmd` | Talks and Presentations tab |
| `./pages/teaching.qmd` | Teaching tab |
| `./css/theme.css`. | Base color in `$primary_color`, background color in `$body-bg`, link color in `$link-color`. |

### Files to provide:

| File                       | Role                               |
|----------------------------|------------------------------------|
| ./images/Picture.png       | Your welcome page picture          |
| ./images/favicon.png       | Your favicon (browser tab picture) |
| ./content/presentation.pdf | Your Presentation                  |
| ./content/poster.pdf       | Your Poster                        |

### Write your CV:

Fill in you CV information in `./content/cv/`, specifically the sections in `./content/cv/sections/` and compile the main LaTeX file `./content/cv/cv.tex` with `xelatex` or `LuaLaTeX`. The file `./content/cv/cv.pdf` is then automatically included in the rendered website.
You can alter the main color sceme of your cv in line 18 of `./content/cv/cv.tex`. 

**Tips:** Modify the content as you wish. Add more tabs, links, etc. and look for inspiration to other academics' personal websites.

# Publishing

You can publish through multiple providers as `quarto pub` or `git pages`. For `github pages`, go to `Settings -> Pages` in your repository, activate and set the `Build and Deploy` informtation to the `master` branch and the folder `docs`. After writing to the git repository, the page updates in the next minutes.

# Google Indexing

You have to index your Website on Google. This ensures that it can be found if, e.g., *Your Name* is searched. For this, you have to upload an invisible page (see `_quarto.yml` line 18) to prove the ownership of the website. See also the [Google instruction](https://developers.google.com/search/docs/crawling-indexing).
