## A stripped down html template

This is a stripped down html webbased template based on [RStudio DT] (http://rstudio.github.io/DT).

Proceeding from here

    git clone https://github.com/einarhjorleifsson/template_DT.git
    mv template_DT your_title
    cd your_title
    rm -rf .git
    git init
    
And then modify:

- `include/before_body.html`

    <li><a href="./">Home</a></li>
    <li><a href="section01.html">Section 1</a></li>
    <li><a href="section02.html">Section 2</a></li>
    <li><a href="section03.html">Section 3</a></li>
    <li><a href="section04.html">Section 4</a></li>
    <li><a href="section05.html">Section 5</a></li>
    ...
    <li><a href="https://github.com/einarhjorleifsson/template_DT" title="View Source on Github"><i class="fa fa-github fa-lg"></i></a></li>



### How did I get here?

    git clone https://github.com/rstudio/DT.git
    mv DT template_DT
    cd template_DT
    rm -rf .git
    git init
    git add *
    git add .gitignore
    git add .nojekyll
    git commit -m 'seeding'
    rm 00*
    rm copy*
    rm DT-doc.Rproj
    rm -r libs/datatables*
    rm -r libs/htmlwidgets
    rm -r libs/jquery
    rm -r libs/nouislider
    rm -r selectize
    git commit -a -m 'simplified'

Then some manual non-coded editing.

And then ...

    git remote add origin git@github.com:einarhjorleifsson/template_DT.git
    git push -u origin master
