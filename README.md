## Welcome to GitHub Pages

🚀 🐼 weee

yes

For now, this is a copy of the template repo for the Just The Docs jekyll theme, with some tweaked colors, and the template editted to call MathJax for latex Rendering.

You can use the [editor on GitHub](https://github.com/pmarsceill/test-jtd/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

Github's parser makes `\(\)` and `\[\]` finicky:

Double dollar notation for display mode `$$x^2_i  \times \beta $$`: 
$$x^2_i \times \beta $$

Slash bracket display mode `\[x^2_i + u_u  \times \beta \]`: 
\[x^2_i + u_u  \times \beta \]

Slash bracket display mode `\\[x^2_i + u_u \times \beta \\]`: 
\\[x^2_i + u_u  \times \beta \\]


Inline latext how you doin? `\(x^3\)` \(x^2\)    ; `\\(x^4\\)` \\(x^4\\)   ;  `$x^5$` $x^6$

### Editting a theme to enable mathJax

Prepend the following to the beginning of the  \_includes/head.html file from the jekyll theme. 

```html
<!--renders latex-->
    <script src='https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML' async></script>

    <!--The following is used to allow the math to wordwrap.-->
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            CommonHTML: { linebreaks: { automatic: true } },
            "HTML-CSS": { linebreaks: { automatic: true } },
            SVG: { linebreaks: { automatic: true } },
            TeX: {extensions: ["enclose.js"]},
            tex2jax: {
            inlineMath: [['$','$'], ['\\(','\\)']],
            processEscapes: true
            }
        });
    </script>
```

Using the default Minima theme, you can find the file to copy over and modify [here](https://github.com/jekyll/minima/blob/master/_includes/head.html)

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/pmarsceill/test-jtd/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
