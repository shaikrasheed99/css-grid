# CSS Grid

Grid offers a grid-based layout with rows and columns, with which we can design web pages without taking help of floats and positioning.

# CSS Properties covered in this example

* `display: grid` - defines a container to be able to follow grid layout.
    ```javascript
    .container {
        display: grid;
    }
    ```

* `grid-template-columns` - defines the number of columns in grid layout.
    ```javascript
    .container {
        grid-template-columns: 1fr 1fr 1fr; // three column with 30% of width
        grid-template-columns: 30% 30% 30%; // three column with 1fr of width
        grid-template-columns: repeat(3, 1fr); // three column with 1fr of width help of repeat function
    }
    ```

* `grid-template-rows` - defines the number of rows.
    ```javascript
    .container {
        grid-template-rows: 1fr 1fr 1fr; // three rows with 30% of height
        grid-template-rows: 30% 30% 30%; // three rows with 1fr of height
        grid-template-rows: repeat(3, 1fr); // three rows with 1fr of height help of repeat function
    }
    ```

* `grid-auto-rows` - defines the height of rows.
    ```javascript
    .container {
        grid-auto-rows: 200px; // assign the fixed height to all the rows
        grid-auto-rows: minmax(200px, auto); // height would be adjusted based on the content inside it but initial height of 200px
    }
    ```

* `grid-gap` - applies the spacing between items.
    ```javascript
    .container {
        grid-gap: 10px; // applies 10px of gap to the row and column 
        grid-gap: 10px 20px; // applies 10px of gap to the row and 20px to the column 
        grid-row-gap: 10px; // applies 10px of gap only to the row
        grid-column-gap: 10px; // applies 10px of gap only to the column
    }
    ```

* `justify-items` - defines the alignment of all the items in horizontal direction.
    ```javascript
    .container {
        justify-items: start; // align to left
        justify-items: end; //align to right
        justify-items: center; // align in center
        justify-items: stretch; // adjust the items to the screen
    }
    ```

* `align-items` - defines the alignment of all the items in vertical direction.
    ```javascript
    .container {
        align-items: start; // align to top
        align-items: end; // align to bottom 
        align-items: center; // align in center
        align-items: stretch; // adjust the items to the screen
    }
    ```

* `grid-column` - define the start and end values to the column of an item.
    ```javascript
    .item {
        grid-column: 1 / 3; // shorthand to define both start and end values
        grid-column-start: 3; // define the column start value of an item
        grid-column-end: 3; // define the column end value of an item
    }
    ```

* `grid-row` - define the start and end values to the row of an item.
    ```javascript
    .item {
        grid-row: 1 / 3; // shorthand to define both start and end values
        grid-row-start: 3; // define the row start value of an item
        grid-row-end: 3; // define the row end value of an item 
    }
    ```

* `justify-self` - defines the alignment of the item in horizontal direction.
    ```javascript
    .item {
        justify-self: start; // align to left
        justify-self: end; //align to right
        justify-self: center; // align in center
        justify-self: stretch; // adjust the items to the screen
    }
    ```

* `align-self` - defines the alignment of the item in vertical direction.
    ```javascript
    .item {
        align-self: start; // align to top
        align-self: end; // align to bottom 
        align-self: center; // align in center
        align-self: stretch; // adjust the items to the screen
    }
    ```

* `grid-template-areas` - define layout based on the area names.
    ```javascript
    .container {
        grid-template-areas: 
            "area area area area"
            "area area area area";
    }
    ```

* `grid-area` - define particular area name to the item.
    ```javascript
    .item {
        grid-area: area;
    }
    ```

Built this website by following [The Net Ninja](https://www.youtube.com/playlist?list=PL4cUxeGkcC9itC4TxYMzFCfveyutyPOCY) youtube playlist.