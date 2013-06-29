#Responsive Grid - Learning Experiment

###What is this

This is a personal pet project aiming to develop my own SASS based responsive grid system. It is more of a learning project and a personal tool than a future grid framework, there are plenty of good ones out there already.

The index.html file gives  a few examples.

###How-to use

####Css Classes

You cans use the 12 column grid out of the box with the grid.css file.

The system is pretty basic in itself :

+	Encapsulate any fluid row in `.row` class, for a 100% width row, use the `.row--full` class
+	Columns are set with the `.column-` class plus the number of column it spans (written in letters), like this `.column-two` to span two columns
+	You can offset columns by adding the class `.offset-by-` plus the number of columns you want to offset it with `.offset-by-number`, like `.offset-by-two`
+	You can hide/display rows; columns or anything with the `no-mobile` and `mobile-only` classes

####Sass Mixins

There's also the option of using sass mixins to avoid adding non-semantic classes, you can find them in grid.mix.scss.

####Customize

There are a few things you can customize :

+	The max width of the grid (default : 1196 px)
+	The gutter size at this full width (default : 16 px)
+	The number of columns (default : 12)
+	The basic mobile breakpoint (default : 640px)

You can have the grid suit your needs by setting the scss variables at the top of the `grid.scss` file, just don't forget to set the last column correctly like indicated in the comments.

###Credits

Started with [HTML5 Reset](http://html5reset.org), heavily influenced by every grid framework I've used so far, mainly [1140 CSS Grid](http://cssgrid.net).
Built with [Compass](http://compass-style.org) using [Codekit](http://incident57.com/codekit/).

###Copyright

For anyone who'd wish to use or modify this code, it is licensed under the [MIT License](http://mit-license.org).

