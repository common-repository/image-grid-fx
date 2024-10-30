=== Image Grid FX ===
Contributors: flashxml
Tags: images, photos, widget, post, plugin, posts, sidebar, free, flash, grid, imagegrid, gallery, thumb, thumbs, xml, as3, photo, image, tooltip, effects, zoom, roll, over, out, background, columns
Requires at least: 2.8.0
Tested up to: 3.0.1
Stable tag: trunk

A stylish and fully customizable Image Grid. Fully XML customizable without any Flash knowledge. And it's free!

== Description ==

The Image Grid FX can be embedded in any website for free without even using Flash. It can have an overall width and height up to 1680 x 1050 pixels. It supports an unlimited number of rows and columns, thus an unlimited number of images. You can have the option to go to an URL or to enlarge the image when clicking a thumb. Both the description and tooltip have CSS formatted text. External PNGs (changeable) for next/previous buttons. The images border and spacing are configurable too. Enlarging effects are provided.

== Installation ==

Make sure your Wordpress version is greater than 2.8 and your hosting provider is using PHP5.

1. There are two files to download: [WordPress Plugin](http://downloads.wordpress.org/plugin/image-grid-fx.zip "Image Grid FX Plugin") (that you have to install and activate) & [Free archive](http://www.flashxml.net/free/download/image-grid.zip "Image Grid FX")
2. Create a new folder inside your **wp-content** folder called **flashxml**, inside this folder create a new one called **image-grid-fx** and copy the content of the **free archive** there
3. If you copied the **free archive** to a location different than the one above, go to **Image Grid FX** from the **Settings** tab in your **WordPress Dashboard** and update the path accordingly
4. Add `[image-grid-fx][/image-grid-fx]` where you want the Flash to show up in your post/page
5. If you want to make the Image Grid FX part of your theme, edit the template files and add `<?php imagegridfx_echo_embed_code(); ?>` where you want it to show up
6. Go to [FlashXML.net](http://www.flashxml.net/ "Free Flash Components") and [customize your Image Grid FX](http://www.flashxml.net/image-grid.html "Image Grid FX") using the Live Demo. Generate the `settings.xml` text and use it to overwrite `wp-content/flashxml/image-grid-fx/settings.xml`
7. To use your own images, upload them to `wp-content/flashxml/image-grid-fx/images/` and update the `wp-content/flashxml/image-grid-fx/images.xml` file accordingly

= Additional settings file =

To embed the Image Grid FX more than once, you will need another settings file and (probably) another set of images. Let's assume your new file is called `settings2.xml`. Add `[image-grid-fx settings="settings2.xml"][/image-grid-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the file name as **the first argument** of the `imagegridfx_echo_embed_code()` function call (for example `<?php imagegridfx_echo_embed_code("settings2.xml"); ?>`).

= No Flash support text =

To support visitors without Adobe Flash Player, you can provide alternative content by adding the text between `[image-grid-fx]` and `[/image-grid-fx]`. If you made the Flash part of your theme, add the text as **the second argument** of the `imagegridfx_echo_embed_code()` function call (for example `<?php imagegridfx_echo_embed_code("","Alternative content"); ?>`).

= If you have PHP4 =

To make it work with PHP4, add `[image-grid-fx width="600" height="300"][/image-grid-fx]` where you want the Flash to show up in your post/page. If you made the Flash part of your theme, add the width and height as **the third and fourth argument** of the `imagegridfx_echo_embed_code()` function call. Don't forget to provide your own width and height values, since 600 and 300 are just examples.

= Getting rid of the FlashXML.net label =

To remove the FlashXML.net label from the top-left corner you'll need to buy the [paid package](http://www.flashxml.net/image-grid.html "Image Grid FX"). Once you'll do that, simply use the SWF file from the paid package to overwrite the SWF file from the `wp-content/flashxml/image-grid-fx/` folder.

== Screenshots ==

1. The Live Demo on [FlashXML.net](http://www.flashxml.net/image-grid.html "Image Grid FX") is the utility that helps easily customize your Image Grid FX to fit all your needs.