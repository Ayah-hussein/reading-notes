

# CSS Layout Techniques
There are several basic techniques to use in your CSS to create multi-column layouts. What follows is are demonstrations of the barebones techniques needed.

layouts: 

**Two Column Layouts**
Two column layouts on the web are very common for basic sites. Generally, they consist of a header, footer and then two columns in the content area. One column is for the main content while the other is a sidebar.

The essential CSS code for a centered 2 column layout with the CSS on the left is as follows.

body {
 text-align: center; /* This is a hack for older browsers to center the page */
}

#container {
  margin: 0 auto;    /* This centers the page in modern browsers */
  text-align: left;  /* This is a hack for older browsers to center the page */
  width: 960px;      /* This sets our total page width */
}

#header {
  width: 960px;      /* This sets the header to stretch the full page width */
}

#navigation li {
  display: inline;   /* Make our navigation display in a line */
}

#content {
  float: right;      /* This causes the content to move to the right */
  width: 700px;      /* We need to set the width whenever we float an element */
}

#sidebar {
  float: left;       /* This causes the sidebar to move to the left */
  width: 260px;      /* We need to set the width whenever we float an element */
}

#footer {
  clear: both;       /* This makes sure that the footer clears both the sidebar and content floats */
  width: 960px;      /* This sets the footer to stretch the full page width */
}
Here are the key points to consider for this layout:

The header and footer are set to 960 pixels so they stretch the entire width.
The content and sidebar have their widths set. The total adds up to 960px.
The sidebar is floated to the left, the content to the right.
The footer is set to clear floats on both sides so that it sits below the content and sidebar.

**2 Column Demos**
Two column layout with sidebar on the left
View HTML
View CSS
Two column layout with sidebar on the right
The only difference here is in the floats in the CSS. We tell the content to float to left and the sidebar to the right.

View HTML
View CSS
Three Column Layout
A three column layout generally consists of a main content area in the middle and a sidebar on both the right and left sides.

Below is the basic CSS code for a 3 column layout.

body {
  text-align: center;  /* This is a hack for older browsers to center the page */
}

#container {
  margin: 0 auto;      /* This centers the page in modern browsers */
  text-align: left;    /* This is a hack for older browsers to center the page */
  width: 960px;        /* This sets our total page width */
}

#header {
  width: 960px;        /* This sets the header to stretch the full page width */
}

#navigation li {
  display: inline;     /* Make our navigation display in a line */
}

#content {
  float: left;         /* This causes the content to move to the left */
  width: 560px;        /* We need to set the width whenever we float an element */
}

#sidebar-left {
  float: left;         /* This causes the sidebar to move to the left
                          It's going to appear to the left of the content because 
                          we declared it first in our HTML page */
  width: 200px;        /* We need to set the width whenever we float an element */
}

#sidebar-right {
  float: right;        /* This causes the sidebar to move to the right */
  width: 200px;        /* We need to set the width whenever we float an element */
}

#footer {
  clear: both;         /* This makes sure that the footer clears both the sidebar and content floats */
  width: 960px;        /* This sets the footer to stretch the full page width */
}


**3 Column Demo**
Three column layout with sidebar on the right and left
View HTML
View CSS
Three Column Unbalanced Layout
The standard three column layout can be easily modified to have the sidebars both on one side to create and unbalanced feel.

Below is the basic CSS code for a 3 column unbalanced layout.

body {
  text-align: center;  /* This is a hack for older browsers to center the page */
}

#container {
  margin: 0 auto;      /* This centers the page in modern browsers */
  text-align: left;    /* This is a hack for older browsers to center the page */
  width: 960px;        /* This sets our total page width */
}

#header {
  width: 960px;        /* This sets the header to stretch the full page width */
}

#navigation li {
  display: inline;     /* Make our navigation display in a line */
}

#content {
  float: left;         /* This causes the content to move to the left 
                          It's going to appear to the left of the content because 
                          we declared it first in our HTML page */
  width: 560px;        /* We need to set the width whenever we float an element */
}

#sidebar-one {
  float: left;         /* This causes the sidebar to move to the left */
  width: 200px;        /* We need to set the width whenever we float an element */
}

#sidebar-two {
  float: left;        /* This causes the sidebar to move to the left */
  width: 200px;        /* We need to set the width whenever we float an element */
}

#footer {
  clear: both;         /* This makes sure that the footer clears both the sidebar and content floats */
  width: 960px;        /* This sets the footer to stretch the full page width */
}
**3 Column Demo**
Three column layout with sidebar on the right and left
View HTML
View CSS
Two Column Stretch Layout
For lack of a better term, I'm calling this type of layout a "stretch" layout. Basically this type of layout is still centered and has a certain width, but the backgrounds of each section stretch to the edge of the page.

Below is the basic CSS code for a 2 column stretch layout.

body {
  text-align: center;  /* This is a hack for older browsers to center the page */
}

.centerLayout {        /* We use a class for this since we're using it in several places */
  margin: 0 auto;      /* This centers the page in modern browsers */
  text-align: left;    /* This is a hack for older browsers to center the page */
  width: 960px;        /* This sets our total page width */
}

#navigation li {
  float: left;         /* Floating also makes our navigation display in a line */
}

#content {
  float: left;         /* This causes the content to move to the left */
  width: 700px;        /* We need to set the width whenever we float an element */
}

#sidebar {
  float: left;         /* This causes the sidebar to move to the left */
  width: 260px;        /* We need to set the width whenever we float an element */
}

#footer {
  clear: both;         /* This makes sure that the footer clears both the sidebar and content floats */
}

the key points to consider for this layout:

In the past, we've wrapped everything with a container and centered that container.
This time, we leave the main elements (header, navigation, footer) on the outside, and don't declare their widths. This means they stretch to fit the page width.
Immediately inside each of these main divs, we add a new div with the class, centerLayout.
We use that class to center the inner parts in the normal manner.