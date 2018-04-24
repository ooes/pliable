
![Alt testimg](https://github.com/gutierr3z/pliable_flex/raw/master/images/hero_bg.png)

# Pliable CSS

It's a brandable responsive layout structure (HTML/CSS) for a page that just needs a header at the top, content centered, and footer at the bottom.  Pliable is meant to be used when you want to keep things simple.  But can also work well with heavy libraries like Bootstrap.  

## Getting Started

There are two steps in order to apply Pliable to a project.

### 1) Link to pliable.css

We assume that you are using a /css folder in your project.  If so, download the /pliable folder into your /css folder.  The file structure should now look like this:

```
your-project/css/pliable/
```
Next, your HTML file (index.html) needs to link to the /pliable/pliable.css.  In the head tag add the link tag:

```
<link href="css/pliable/pliable.css" rel="stylesheet">
```

Now you are set to write your HTML.

### 2) Code HTML Tags

Pliable expects three top level tags as siblings; `<header>`, `<main>`, and `<footer>`.  We assume these will be the children of the body tag.

```
<body>
    <header></header>
    <main></main>
    <footer></footer>
</body>
```
Each of these tags needs to have in them two nested tags before any content.  We suggest these to be `<section>` tags but can be any block tag.  Pliable just expects two nested levels, does not look for specific types of tags.  

```
<body>
    <header>
        <section>
            <section>
                // content
            </section>
        </section>
    </header>
    <main>
        <section>
            <section>
                // content
            </section>
        </section>
    </main>
    <footer>
        <section>
            <section>
                // content
            </section>
        </section>
    </footer>
</body>
```
Now Pliable should take effect and you can start to add your content.

### Colors!

Out of the box, Pliable is very colorful.  We use colors to see the different sections and tags that are being affected by CSS.  Some of these section/tags are just structural and wont normally been seen.  But in order to debug or tweak attributes like paddings and margins, you might want to give these elements colors or borders in order to see what you are doing.  Pliable also includes a list of classes that will apply a border color to an element in order to debug.
```
<div class="red">my content</div>
```
All these color settings are inside the debugging files which need to be commented out before you apply your own brand or look and feel.  

#### Turning off the Debugging Colors

Inside the pliable.css, comment out the pliable.base.debug.css import:
```
/* @import url( 'pliable.base.debug.css' ); */
```
This will turn all Pliable background colors off (transparent).  Border class colors applied to tags inline need to be removed manually.

## File and Code Structure

## License

[MIT](LICENSE)