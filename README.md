# Full-Width TopBar

Making the first row of any page stretch across the entire viewport makes applications look slicker. Here is some CSS to make this happen

## Version 
1.0 - initial

# Setup

## Application Setup
1. Check the *Enable Style Sheet* checkbox in the application properties

## Page Setup
1. Drag any control to a page
2. Add the class "stadium-top-bar" to the classes property

## Options / Notes
1. Dragging a *Menu* control into the first row will cause that menu to be shown integrated with the top bar (use *LeftToRight* display)
2. The position of the profile icon can be adjusted in the [*top-bar-variables.css*](top-bar-variables.css) file (see below)
3. Adding the class "fixed-top-bar" to the control will cause the top bar to remain fixed at the top of the page while the remaining content will scroll
4. When the first control on the page is a *Flexbox* control, you can additionally add the class "split-flex" to that flexbox control to make the last element in that control display on the right-hand side of the top bar

# Styling
The background color can be changed using the two CSS files in this repo

## Applying the CSS

**Stadium 6.6 or higher**
1. Create a folder called "CSS" inside of your Embedded Files in your application
2. Drag the two CSS files from this repo [*top-bar-variables.css*](top-bar-variables.css) and [*top-bar.css*](top-bar.css) into that folder
3. Paste the link tags below into the *head* property of your application
```html
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/top-bar.css">
<link rel="stylesheet" href="{EmbeddedFiles}/CSS/top-bar-variables.css">
``` 

![](images/ApplicationHeadProp.png)

**Versions lower than 6.6**
1. Copy the CSS from the two css files into the Stylesheet in your application

## Customising CSS
1. Open the CSS file called [*top-bar-variables.css*](top-bar-variables.css) from this repo
2. Adjust the variables in the *:root* element as you see fit
3. Overwrite the file in the CSS folder of your application with the customised file

## CSS Upgrading
To upgrade the CSS in this module, follow the [steps outlined in this repo](https://github.com/stadium-software/samples-upgrading)
