# Ohmyfood - Online meal ordering website (Part 1)

![Ohmyfood project thumbnail](src/images/readmethumbnail.jpg)

The concept of Ohmyfood is to order meals online. Users should be able to compose their own menu and reduce their waiting time in restaurants because their menus are prepared in advance. This project is a two phases project. In the first place, the goal is to develop a site offering four restaurants menus. Secondly, the online reservation and menu composition functions will be implemented.

<details open>
<summary>Table of contents</summary>

1. [Overview](#overview)
    - [About the project](#about-the-project)
    - [Links](#links)
2. [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
    - [Usefull resources](#usefull-resources)
3. [Authors](#authors)
</details>

## Overview

### About the project

#### Pages content
##### Header
- A header must be on all pages
- On home page, it contains the brand logo
- On menu pages, there should also be a back button to the home page 

##### Home page
- The user must be able to see the location of the restaurants. In phase 2, he will be able to choose it.
- The user must be able to see the four menus in the shape of a card and be redirected to the menu page after a click.

##### Menu pages
- There should be four pages each offering the menu of a restaurant

##### Footer
- The footer is the same for all pages.
- When you click on “Contact” link, a forwarding to an email address is made.

#### Graphic effects and animations

##### Buttons
- Background color should slightly lighten and the shadow be more visible when hovering.
- The "like" button should gradually fill up when on click. For this first version, the effect can appear on hover.

##### Home page
- A loading spinner must appear for 1 to 3 seconds when you arrive on the home page, cover the entire screen, and use CSS animations (no library).

##### Menu pages
- The dishes should appear gradually with a slight shift in time, either one by one, or by group "Entrées", "Plat" and "Desserts".
- In phase 2, visitors can add the dishes they want to their order by clicking on them. This brings up a small checkbox to the right of the dish. This checkbox should slide from right to left. For this first version, the effect can appear on hover on desktop instead of the click. If the title of the dish is too long, it should be trimmed with ellipsis.

#### Compatibility
- The website must be developped using a mobile-first approach
- It must be responsive with a free layout on tablet and desktop.

### Links
Mobile mockup (Home page): [Here](src/mockup/accueil.png)  
Mobile mockup (La palette du goût): [Here](src/mockup/menu-lapalettedugout.png)   
Mobile mockup (La note enchantée): [Here](src/mockup/menu-lanoteenchantee.png)  
Mobile mockup (À la française): [Here](src/mockup/menu-alafrançaise.png)  
Mobile mockup (Le délice des sens): [Here](src/mockup/menu-ledelicedessens.png)  
Live Site: [Here](https://desireebesnard.github.io/DesireeBesnard_3_08092021/)  

## My process

### Built with
- Semantic HTML5
- Font Awesome (icons)
- SCSS (Sass)
- Flexbox and CSS Grid
- Mobile-first workflow

### What I learned

#### Write better structured code and faster with Sass

##### Install sass (Linux)
> sudo apt install nodejs
> npm -g install sass

##### 7-1 Sass Architecture
```
sass/
|
|– utils/
|   |– _variables.scss           # Sass Variables
|   |– _mixins.scss              # Sass Mixins
|   |– _animations.scss          # Keyframes Animation
|
|– base/
|   |– _base.scss                # Reset/normalize
|   |– _typography.scss          # Typography rules
|
|– layouts/
|   |– _header.scss              # Header
|   |– _main-description.scss    # Presentation of the company
|   |– _main-restaurants.scss    # Restaurant cards layout
|   |– _main-menu.scss           # Menu layout
|   |– _footer.scss              # Footer
|   |– _mediaqueries.scss        # Media queries
|
|– components/
|   |– _button.scss              # Button
|   |– _spinner.scss             # Loading spinner
|
 – main.scss                     # Main Sass input file
```

##### Mixins
```
@mixin box-shadow {
    box-shadow: 1px 2px 15px 0px rgb(0 0 0 / 15%);
}
//The mixin is included into the current context using the @include at-rule
@include box-shadow;
``` 

##### Improve code maintainability with Sass variables

#### Create graphic effects
##### Linear Gradient on svg
##### CSS transition
##### Create more complex animations with the @keyframes CSS rule

#### Ensure the graphic consistency of a website (Media queries for tablets and desktop)

### Continued development
- Build the site using a framework such as React to create components and avoid redundancies (cards)

### Useful ressources
- 

## Authors
- Website - [Désirée Besnard](https://github.com/DesireeBesnard)
- MockUp - [OpenClassRooms](https://openclassrooms.com/fr/)