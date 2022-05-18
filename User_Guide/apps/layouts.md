
# App Layouts




#### Layout options


Layout components are the only components that can go directly onto the page root. You can also nest them within other layout components. They provide a structure for the content that you put within them.

![screenshot.1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.1.jpg?width=508&name=screenshot.1.jpg) 

The two main layout options are the Flex Layout and Grid Layout. Both conform to standard CSS Flex and Grid behaviour. Flex allows you to create a horizontal or vertical line of content and to align the content within the space as well as the space between the content items. The Grid Layout allows you to customise a grid display with a set number of columns and rows along with custom spacing between those columns and rows. By default, the row height will be set at the maximum height needed to accommodate the content in any one grid row. If you have a particularly tall piece of content in one row, but do not want the other rows to have the same height, simply increase the 'Weight' value on the row containing the tall content.
 

#### Repeating Layouts


A repeating layout takes a table in a datastore and replicates each line of data in that table according to a base design.
First, place a repeating layout onto the page (this can be on the page root or nested within another layout component). Next, select your table from the datastore in the Repeating Layout Properties panel and choose your display preference. Block will render each item one after the other in a vertical line. Grid will create a grid layout, for which you can customise the number of columns and the gaps between the rows.

![screenshot.5](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.5.jpg?width=545&name=screenshot.5.jpg) 

Next, create your base design. Simply drag a component into the repeating layout, for instance a card. You can then add variables from the Repeating Layout context wherever there is a variable sign (x). You will see that the variables from Context are the same as your table headers. This is because the generated layout will take the value from each line of your data in the column with the chosen header. In the Design view, you will see a preview of the first line of your data set and how it will look when it is rendered.

![screenshot.4](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.4.jpg?width=602&name=screenshot.4.jpg) 

Click on the Preview button to see all the data rendered. 

![screenshot.2](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.2.jpg?width=602&name=screenshot.2.jpg) 

Above you can see a card component within a repeating layout that is pulling data from a table in a datastore. It is then rendering both of the chosen variables: the name of the fruit and it's price.

![screenshot.3](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.3.jpg?width=341&name=screenshot.3.jpg) 

 

#### Filtering Repeating Layout Content

Content in Repeating Layouts can be filtered by toggling the Filter content option in the Repeating Layout Properties panel. First, choose which column to filter your content by (for example, this may be a category tag in a table of blogs). You can then choose whether to apply an initial filter and what you would like the 'Show all' option text to be (by default this is 'All Resources').

![screenshot.6](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.6.jpg?width=282&name=screenshot.6.jpg) 

Below you can see the filter button in the top right. As you can see, the data has been filtered to only show the desired fruit.

![screenshot.8-1](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.8-1.jpg?width=688&name=screenshot.8-1.jpg) 

If you want to only display a segment of your table data to the end user without giving them the option to change what they see, simply apply an initial filter and toggle the 'Hide filter' option.

![screenshot.7](https://docs.toca.io/hs-fs/hubfs/book%20of%20toca%20images/book%20of%20toca%20updated%20images%20(13.10.21)/Apps/layouts/screenshot.7.jpg?width=290&name=screenshot.7.jpg) 

 
