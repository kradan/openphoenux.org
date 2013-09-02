openphoenux.org
===============

_website draft for the next generation open source hardware mobile phone_

Thanks for checking out this website draft for openphoenux.org!

Every feedback is highly appreciated. My biggest question: Is this design able to attract non nerds? If not, what should change?

To parse update index.html call:
$ ./parse index
You also can use any file sitting in ./include/ instead. (In future versions .inc and .html suffix will be tolerated.)

New includes can be added with
<!-- include:name -->

Add new menu entries on the left or on top with
<!-- top:name Title -->
<!-- left:name Title -->

Comment includes or menu entries with # after <!--

This will wrap following around the content of name so will be hidded until the menu entry is clicked:
 <div id="title" class="tab top">
  <a href="#title" class="menu top">Title</a>
  <div class="content hidden">
   [<name> is included here]
  </div>
 </div>

If you add new images, thumbnails are created using imagemagick (convert) automatically. You need to install that. (Will add a option to disable thumbnailing in the future.)

Implemented MARKUP so far:
.p 		paragraph
.p.left		paragraph with class=left
.p#contact	paragraph with id=contact
.h[1..X]	headline 
*		unordered list element (<ul></ul> are added automatically)
.li		unordered list element (<ul></ul> are added automatically)
.img[<|=|>] filename
.img[<|=|>] filename Title
.img[<|=|>] filename Title -> URL
.gallery[<|>|=] [list of image files without path]
(Comments are not implemented yet, but in the queue.)

New features will be added when needed. I am open for any suggestion!

AUTHOR
-------

kardan <kardan@riseup.net>

THANKS
------

To everybody who worked on the the OpenMoko series and especially to Nikolaus Schaller and his team for the amazing engagement and investment for the GTA04!
