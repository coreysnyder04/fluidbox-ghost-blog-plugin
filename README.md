# What is this? 
This is a [fluidbox](http://terrymun.github.io/Fluidbox/demo/index.html) integration for the [Ghost.org Blogging Platform](https://ghost.org/) that I've developed. 
By adding a single line to the footer section in the Ghost Admin Panel, it adds additional functionality to the default casper theme. 
When you click on an image, either standalone or in a gallery, it will pop a modal to reveal a larger view of that image. 
It is customizable via a configuration object.

## Features
 * Both stand-alone and gallery images are clickable. This doesn't include images added via markdown mode. 
 * Auto-dismiss on scroll
 * Ability to use image as back-drop
 * Ability to show captions in modal
 * Ability to navigate images with arrow keys. 

## Demo
Video Demo: https://youtu.be/bBOP9-Rpeuk

Live Demo: You can see this live on my site now using the default casper theme: http://coreysnyder.me/test-page-for-my-gallery-fluidbox/

## How to use
Drop this line into your site-footer section in the ghost admin panel
```html
  <script async src="https://cdn.jsdelivr.net/gh/coreysnyder04/fluidbox-ghost-blog-plugin@0.1.0/fluidbox-ghost-blog-plugin.min.js"></script>
```

### Customization
Currently you can customize two different things by adding this above that script:

```html
<script>
    window.fluidboxGhostConfig = {
      theme: 'image-backdrop', // Options: light, dark, image-backdrop, hsla(262, 100%, 82%, 0.6)
      showCaption: true, // Sets whether to capture the caption and show it below the image when expanded
    }
</script>
```

## Versioning 
Updates to Ghost Casper theme which change the HTML affecting images might break this integration. To combat this I will release versions which align with the versions of casper.  

