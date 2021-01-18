<script src="https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
<script>mermaid.initialize({startOnLoad:true});</script>

<div class="mermaid">
    graph TD
    A[Client] --> B[Load Balancer]
    B --> C[Server01]
    B --> D[Server02]
    E --> F
    F --> E
    G --> A
</div>

<div class="mermaid">
graph LR
    A[Start] --> B{Is it?};
    B -->|Yes| C[OK];
    C --> D[Rethink];
    D --> B;
    B ---->|No| E[End];
</div>

<div>
graph TD
    A[Start] --> B{Is it?};
    B -->|Yes| C[OK];
    C --> D[Rethink];
    D --> B;
    B ---->|No| E[End];
</div>
{: .mermaid}

[More info about mermaid syntax](https://mermaid-js.github.io/mermaid/#/flowchart)


## Welcome to GitHub Pages

🚀 🐼 weee :confused: asdf :unamused:


$$\textcolor{red}{\text{Hello!}}$$

Hello!
{: .text-red-200 }
Font sdds
{: .text-blue-200 }
Beep


<article markdown="block">
And this is a test of how default article rendering works here

And another paragraph hopefully
</article>

<aside markdown="block">
# Testing things this is too big

Here is something more reasonable.
- heloo
- hulloo
- beep beep
</aside>

more change more rendder

Change this again to force a re-render

yes




With mermaid declaration:

```mermaid
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
```

without:

```
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
```

Yeh


~~~plantuml
!define ICONURL https://raw.githubusercontent.com/tupadr3/plantuml-icon-font-sprites/v2.1.0
skinparam defaultTextAlignment center
!include ICONURL/common.puml
!include ICONURL/font-awesome-5/gitlab.puml
!include ICONURL/font-awesome-5/java.puml
!include ICONURL/font-awesome-5/rocket.puml
!include ICONURL/font-awesome/newspaper_o.puml
FA_NEWSPAPER_O(news,good news!,node) #White {
FA5_GITLAB(gitlab,GitLab.com,node) #White
FA5_JAVA(java,PlantUML,node) #White
FA5_ROCKET(rocket,Integrated,node) #White
}
gitlab ..> java
java ..> rocket
~~~





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

You need to have a blank line before the equation in $$$$ or github's jekyll stuff will think you actually want an inline equation. ... Bad design choice imo.

Inline test 1 $$x^2_i + u_u  \times \beta$$

Inline test 2 \\(x^2_i + u_u  \times \beta\\)

Inline test 3 $x^2_i + u_u  \times \beta$

Inline test 4 $$ \left\{ x^2_i + u_u  \times \beta \right\}$$

Inline test 5 $\left\{ x^2_i + u_u  \times \beta \right\}$

Inline test 6 $$\{ x^2_i + u_u  \times \beta $$

Inline test 7 $\{ x^2_i + u_u  \times \beta $


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
