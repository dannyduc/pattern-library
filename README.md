# Pattern Requirements

This document will describe the structure of each pattern and its behaviour under various screen sizes.

---

## The Grid System

**Description**

- 12 columns
- Responsive, fluid
- Columns will be wrapped in a container .row
- Each column will have the class of .col-$
- Also create a .container class that wraps all content and centers it on the page. The container must be fluid in width.

**Responsive Behaviour**

- In smaller screen sizes (<1024px) the columns will have their gutter width halved
- In mobile sizes (<768px) all columns will get a 100% width

## Typography

**Elements**

- Headings
- Paragraphs
- Bold, em, strike, link
- Code blocks
- Lists
- Blockquotes

## Buttons

**Description**

- 2 styles: default, primary
- 3 sizes: small, default and large
- Styles for all HTML elements: `<a>, <button>, <input type="button">, <input type="submit">`

## Form Elements

**Elements**

- Inputs
- Radio and checkboxes (custom controls)
- Pre-made forms: sign-in, sign-up, contact

## Icons

**Description**

- Will use FontAwesome
- Styles for bordered icons
- Styles for square, rounded or circle border
- 3 different sizes: default, large, huge

## Feedback

**Description**

- 4 message boxes: information, success, error, warning

## Navigation

**Elements and Characteristics**

- Navbar
- Contains logo on the left side and menu on the right side
- The menu will be powered by the Superfish jQuery plugin

**Responsive Behaviour**

- At page load, the main menu will be cloned via jQuery into a responsive menu
- In mobile sizes (<768px) the main menu will be hidden, the logo moved to the center and the responsive menu will be displayed below the logo

## Animations

**Description**

- Will use the animate.css library by Dan Eden

## Tabs and Accordions

**Description**

- Custom controls

## Carousels

**Description**

- Will use the Cycle2 jQuery plugin

---

https://github.com/tutsplus/building-your-own-pattern-library-for-the-web

https://s3.amazonaws.com/cms-assets.tutsplus.com/uploads/users/71/courses/408/attachment/SourceFiles-BuildOwnPatternLibWeb.zip?AWSAccessKeyId=AKIAJGYHP2U3GKEIJIGQ&Expires=1409616871&Signature=adwvM0tiPHLlgqa66bB38rs88jQ%3D


    npm install grunt-contrib-sass
    
Gruntfile.js

	module.exports = function (grunt) {
    grunt.initConfig({
        sass: {
            dist: {
                files: [
                    {
                        expand: true,
                        cwd: 'sass',
                        src: ['*.scss'],
                        dest: 'css',
                        ext: '.css'
                    }
                ]
            }
        }
    });

    grunt.loadNpmTasks('grunt-contrib-sass');
    grunt.registerTask('default', ['sass']);
	};    
    

bower install
    
    
FontAwesome http://fontawesome.io/
FontAwesome Cheatsheet http://fontawesome.io/cheatsheet/
Bower http://bower.io/
Meet Bower: A Package Manager for the Web https://code.tutsplus.com/tutorials/meet-bower-a-package-manager-for-the-web--net-27774
    
Superfish jQuery Plugin
https://github.com/joeldbirch/superfish/
        
Animate.css
http://daneden.github.io/animate.css/
    
Cycle2 jQuery Plugin
http://malsup.com/jquery/cycle2/
    
    
Prism.js
http://prismjs.com/
Postable    
http://www.elliotswan.com/postable/