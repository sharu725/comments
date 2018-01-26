---
layout: none
description: This is a demo of CSS Grid Layout.
article: /css-grid/
---

<html lang="en">
<head>
   <meta charset="UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1">
    <title>{{demo.title}}</title>
    <meta name="description" content="{{demo.description}}" />
    <!-- <link rel="stylesheet" href="/css/demo.css"> -->
    <style>
   

body {
    font-family: Helvetica, sans-serif;
}   

.wrapper {
    display: grid;
    grid-gap: 20px;
    grid-template-columns: 1fr 1fr 1fr;
    color: white;
    font-size: 30px;
 }

header, aside, article, footer {
    grid-column: span 4;
    min-height: 100px;
    padding: 20px;
} 

header {
    background: #4574ba;
}

aside {
    background: #e7e61c;
}

article {
    background: #46b749;
}

footer {
    background: #323232;
}



@media only screen and (min-width: 600px) {
    header {
        grid-column: 1 / 4;
        grid-row: 1 / 2;
        align-items: center;
        
    }

    aside {
        grid-column: 3 / 4;
        grid-row: 2 / 4;
        
    }

    article {
        grid-column: 1 / 3;
        grid-row: 2 / 3;
        
    }

    footer {
        grid-column: 1 / 3;
        grid-row: 3 / 4;
        
    }

    
}

@media only screen and (min-width: 800px) {
    header {
        grid-column: 1 / 4;
        grid-row: 1 / 2;
    }

    aside {
        grid-column: 1 / 2;
        grid-row: 2 / 4;
    }

    article {
        grid-column: 2 / 4;
        grid-row: 2 / 3;
    }

    footer {
        grid-column: 2 / 4;
        grid-row: 3 / 4;
    }

}



</style>
</head>
<body>
    <div class="wrapper">
        <header>Header</header>
        <article>Article</article>
        <aside>Aside</aside>
        <footer>Footer</footer>
    </div>
    
    <p>Resize the window to see the changes in the positions of <strong>aside</strong> item.</p>
    <a class="btn" href="{{page.article}}">Back to article</a>
    
<script src="/demo/css-polyfills.min.js"></script>
</body>


</html>




