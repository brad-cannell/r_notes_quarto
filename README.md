# Brad's R Notes - Quarto Version

This repository is for a [Quarto](https://quarto.org/) version Brad Cannell's R Notes. This repository is primarily intended to be helpful to me, but even better if you find it useful too! This version of my R Notes replaces the previous [Bookdown version](https://brad-cannell.github.io/r_notes/). 

Why am I doing this (as opposed to just keeping notes locally)?       
* Better organized (e.g., chapter structure and search).      
* Easy access -- just click on the bookmark on web browser.      
* Practice using Quarto.      
* Might help with R4Epi -- This can be sort of a sandbox for developing before I add things to R4Epi.    

## Useful websites:

-   [Quarto book documentation](https://quarto.org/docs/books/)

## Rendering

We can render the files by clicking the Render button in RStudio. To render the HTML and PDF files at the same time, type `quarto render` into the terminal. 

````
```{bash}
quarto render
```
````

You can also render Quarto files with a native R code chunk.

- The input argument: The input file or project directory to be rendered (defaults to rendering the project in the current working directory).

- The output_format argument: Target output format (defaults to "html"). The option "all" will render all formats defined within the file or project.

````
```{r}
#| Render with R
#| eval: false
quarto::quarto_render(output_format = "all")
```
````

## Publishing to GitHub pages

[This article is great](https://quarto.org/docs/publishing/github-pages.html). After committing, and making sure you are on the main branch, type `quarto publish gh-pages` in the terminal.

````
```{bash}
quarto publish gh-pages
```
````

## Publishing to Netlify

[This article is great](https://quarto.org/docs/publishing/netlify.html). After committing, and making sure you are on the main branch, type `quarto publish netlify` in the terminal.

````
```{bash}
quarto publish netlify
```
````

## Where to publish

I've used Netlify in the past and have been happy with it. However, I'm not sure that it is necessary or efficient to add the extra layer of using Netlify in GitHub Pages will work just as well. Why introduce a third site into the mix if we don't have to? For now, I may just stick with GitHub Pages.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
