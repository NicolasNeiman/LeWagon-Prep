
# HTML : The 2-hour landing page

##### Table of Contents
1. [A good landing page](#a-good-landing-page)
2. [HTML](#html)
    - [Philosophy](#philosophy)
    - [Skeleton](#skeleton)
        - [Head](#head)
        - [Body](#body)
3. [CSS](#css)
    - [Enable CSS](#enable-css)
    - [CSS Syntax](#css-syntax)
    - [Id and Selector](#id-and-selector)
    - [Class - simple classes](#class---simple-classes)
    - [Class - combined classes](#class---combined-classes)
4. [Bootsrap](#bootstrap)

## A good landing page

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

HTML code will be written between 2 html tags

HTML Structure v1 :

```html
<html>


</html>
```

Then within those tags we will have 2 main tags for the 2 part of the code:
- head : link to the design and all the "intelligence of the page"
- body : what needs to be displayed

HTML Structure v2 :
```html
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

The **title** of the page is not actually displayed on the page but is used for instance by google.

A lot of assets used by 3rd parties (Facebook, Google, WhatsApp ??)

#### Body

##### Core syntax

```html
<element attr="sthg"> ... </element>
```

##### Keywords
- tags (opening and closing tags)
- tag content
- attributes
- attributes' value

Exemple :
```html
<a href="http://lewagon.org" target="_blank">
    Le Wagon
</a>
```
- tag name : a
- content of the tag : the text "Le Wagon"
- attributes:
    - href with value "http://lewagon.org" : this is the redirection address
    - target with value "_blank" this attribute is used to open the page in a new tab

##### Some commmon tags

- titles : h1, h2, h3 ...
- paragraph : p
- emphasize : em or strong
- list : ul (unordered list = bullet points) or ol (ordered list with numbers). each items uses li (list item)
- image : no closing tag

Tips : cool icons : https://nucleoapp.com/free-icons

##### The div tag

- height and width + padding + margin
- border-radius

## CSS

### Enable CSS

Link to CSS file is in the head of the HTML file.

```html
<link rel="stylesheet" href="style.css">
```

### CSS Syntax

```css
selector {
    property1: value1;
    property2: value2;
}
```

How to find nice colors ? -> coolors.co </br>
How to find nice fonts  ? -> fonts.google.com </br>
Then to use google font it is more convinient to use a link to the font on google's server rather than download the font and store it in our project :
```html
<link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@1,600&family=Open+Sans:wght@300;400&display=swap" rel="stylesheet">
```
font-family: 'Montserrat', sans-serif; </br>
font-family: 'Open Sans', sans-serif; </br>


### Id and selector

Give tags and ID and then define properties for this ID in the CSS :

#### HTML
```html
<img src='logo.png' id="logo">
``
#### CSS

```css
#logo{
    width: 40px;
}
```

### Class - simple classes

Id are meant to be used for unique elements
If we want to reuse design class we use classes

#### HTML

```html
<img src='paul.png' id="staff">
```

#### CSS

```css
.staff{
    border-radius : 50%;
}
```

### Class - Combined classes

```html
<img src='paul.png' id="staff shadow">
```

#### CSS

```css
.staff{
    border-radius : 50%;
}

.shadow{
    box-shadow : 5px 5px 3 px black;
}
```

## Bootstrap












