doxygen-bootstrapped
====================

This is my fork of doxygen-bootstrap containing a handful of tweeks and fixes.

# Changes
* Added styling for the `memtitle` class (was using default Doxygen styling before)
* Added link to "Project Name" in navbar
* Added class list and class index to navbar

# How to Integrate (from Velron/doxygen-bootstrapped)

To integrate this into your own project tell your doxyfile to use these 4 files in the HTML section (see the example site for an example of each file):

* HTML_HEADER=header.html
    * Adds a Bootstrap navbar
    * Wraps the content in a Bootstrap container/row
* HTML_FOOTER=footer.html
    * Closes the extra divs opened in the header.html
* HTML\_EXTRA_STYLESHEET=customdoxygen.css
    * Adds additional styling such as a sticky footer   
* HTML\_EXTRA_FILES=doxy-boot.js
    * Where the magic happens to augment the HTML with bootstrap
