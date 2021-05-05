Using Grid

https://learncssgrid.com/

Grid Container:
    To start using Grid, we need to specify a Grid Container by using the css property display: grid;
    This will make all direct children Grid items

Creating the Grid:
    Creating the grid, we need to specify the Rows and Columns that the Grid will contain.
    
    Create Rows
        We can create rows with css using grid-template-rows: x x x...
        When making rows you can use different values ex: px % em rem fr etc.
    
    Create Columns
        We can create rows with css using grid-template-columns: x x x...
        When making columns you can use different values ex: px % em rem fr etc.
    
    Create Rows/Columns with Repeat()
        Instead of having to type out the size of each row or column, we can shorten the code and use repeat(x, value);
        This allows us to set x to the number of rows/columns we want, and the value to the different values used.
    
    Create Gaps
        We can space the grid sections apart using the css grid-gap: x;
        This allows us to use the different size values to space apart the grid on rows and/or columns.
    
    Placing Items on the Grid
        When the grid is created and we have created the rows and columns, we can now specify where to place the items on our page on that grid
        We would use the following css lines to place each item
            grid-row-start: x;
            grid-row-end: x;
            grid-column-start: x;
            grid-column-end: x;
        The start is using the row/column the item will start in
        The End will fill the item in the rows/columns needed up to that 'x' value
        Example, using a grid with 3 rows 4 columns, using grid-row-start: 2; grid-row-end: 4;
            This will start that item in grid row 2 and span to fill in row 2 and 3 stopping at 4 which is the end of the grid.
        We can shorten the code grid-row/column-start/end with grid-row/column: x / y;
            this will use the same as above in one line instead of 2 the 'x' defines the start posistion, and 'y' defines the end position which needs to be y+1
        We can then shorten the code even further from having 2 lines of grid-row and grid-column by using grid-area: a / b / x / y;
            this will combine grid-row/column into one line with start and end values.
            'a' is the row start, 'b' is the column start, 'x' is row end, 'y' is column end
        We can also specify a more defined grid using grid-template-areas: with names of the sections repeated for each row/column they should be in 
            this is an example of the grid-template-area
            grid-template-area: nav nav nav
                                header header header
                                left right right
                                left right right
                                footer footer footer
            With this example, it states that the nav section will be in row 1 and column 1-3, header will be in row 2 column 1-3, left will be in row 3-4 column 1, right will be in row 3-4 column 2-3, and footer will be in row 5 column 1-3.
            we would also use the grid-template, grid-template-row/column css settings to specify the size of these sections
            we would then just apply the named area of the grid to the item it reponds to by using either grid-row/column-start/end or useing grid-row/column and the named section
            ex nav {grid-row: nav;}