
A good landing page
- clear value proposition
- clean design
- call-to-action : be able to measure performance
- crm first milestone

Many services to create your landing page without coding

But we will code it from scratch using :
- HTML : structure (markup language)
- CSS : Bootstrap and Material Design (2 famous CSS libraries)
- javascript : animations when the user interact with the page


## HTML

### Philosophy
Tag the content for the Browser to apply default rules. For instance H1 is bigger than H2. CSS will allow us to override those rules to apply our own formatting.

### Skeleton
HTML code will be written between 2 html tags :

```
<html>


</html>
```

Then within those tags we will have 2 main tags for the 2 part of the code:
- head : link to the design
- body : what needs to be displayed

```
<!DOCTYPE html>
<html>
  <head>
    <!-- Intelligence (meta-data) -->
  </head>

  <body>
    <!-- Stuff to display-->
  </body>
</html>
<!-- end of file -->
```

#### Head

The *title* of the page is not actually displayed on the page but is used for instance by google.

A lot of assets used by 3rd parties (Facebook, Google, WhatsApp ??)

#### Body

Core syntax :

<element attr="sthg"> ... </element>
Keywords :
- tags (opening and closing tags)
- attributes

Exemple :
```
<a href="http://lewagon.org" target="_blank">
    Le Wagon
</a>
```
- tag name : a
- content of the tag : the text "Le Wagon"
- attributes:
    - href with value "http://lewagon.org" : this is the redirection address
    - target with value "_blank" this attribute is used to open the page in a new tab

Some commmon tags :
- titles : h1, h2, h3 ...
- paragraph : p
- emphasize : em or strong
- list : ul (unordered list = bullet points) or ol (ordered list with numbers). each items uses li (list item)
- image : no closing tag

Tips : cool icons : https://nucleoapp.com/free-icons


## CSS

### Enable CSS
Link to CSS file is in the head of the HTML file.
<link rel="stylesheet" href="style.css">

### CSS Syntax
selector {
    property1: value1;
    property2: value2;
}

How to find nice colors ? -> coolors.co
How to find nice fonts  ? -> fonts.google.com
Then to use google font it is more convinient to use a link to the font on google's server rather than download the font and store it in our project :
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@1,600&family=Open+Sans:wght@300;400&display=swap" rel="stylesheet">
font-family: 'Montserrat', sans-serif;
font-family: 'Open Sans', sans-serif;


### The div tag

- height and width + padding + margin
- border-radius

### Id and selector

Give tags and ID and then define properties for this ID in the CSS :

#### HTML

<img src='logo.png' id="logo">

#### CSS

#logo{
    width: 40px;
}

### Class - simple classes

Id are meant to be used for unique elements
If we want to reuse design class we use classes

#### HTML

<img src='paul.png' id="staff">


#### CSS

.staff{
    border-radius : 50%;
}

### Class - Combined classes

<img src='paul.png' id="staff shadow">


#### CSS

.staff{
    border-radius : 50%;
}

.shadow{
    box-shadow : 5px 5px 3 px black;
}













