#Responsive Grid

###What is this

This is a personal pet project aiming to develop my own SASS responsive grid. It is more of a learning project and a personal tool than a future grid framework, there are plenty of good ones out there already.

The index.html file serves as demo and documentation.

###How-to use

####Css Classes

You can use the 12 columns grid out of the box with the grid.css file (minified).

The system is pretty basic in itself :

+	Encapsulate any fluid row in `.row` class, they have a max width of 1196px by default for a 100% width row, use the `.row--full` class
+	Columns are set with the `.column-` class plus the number of column it spans, like this `.column-2` to span two columns
+	You can offset columns by adding the class `.offset-by-` plus the number of columns you want to offset it with `.offset-by-i`, like `.offset-by-2`
+	You can hide/display rows; columns or anything with the `no-mobile` and `mobile-only` classes, which use a media query for a default breakpoint of 640px

####Sass Mixins

There's also the option of using sass mixins to avoid adding non-semantic classes, you can find them in grid.mix.scss with comments to explain each mixin.

####Customize

There are a few things you can customize :

+	The max width of the grid (default : 1196 px)
+	The gutter size at said full width (default : 16 px)
+	The number of columns (default : 12)
+	The basic mobile breakpoint (default : 640px)

You can have the grid suit your needs by setting the scss variables at the top of the `grid.scss`.
To build the `grid.css` file simply use the following command in your terminal of choice (you need SASS installed):

	sass --scss --style compressed grid.scss grid.css
	
####Support

This is in no way a responsive framework, and it is not meant to be cross-browser compatible. It is just a lightweight starting point mostly used for small projects and prototypes.  
If you need a more advanced framework, there are plenty out there such as (among others) :

+    [Bootstrap](http://getbootstrap.com/)
+    [1140px](http://www.1140px.com/)
+    [Susy](http://susy.oddbird.net/)
+    [The Semantic Grid System](http://semantic.gs/)

Or just build your system according to the layout and design needs of the project.

####Credit

For anyone who'd wish to use or modify this code, it is licensed under the [MIT License](http://mit-license.org).

