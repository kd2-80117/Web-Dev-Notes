### 1. What is flexbox and it's properties?
Flexbox stands for flexible box. It handles layout efficiently, aligns items and uses space inside the flex container.
        
Parent container properties are:
        
        1. display:flex;
        2. flex-direction: row (default value)/ column/ row-reverse/ column-reverse;
            row stacks flex items horizontally left to right.
            column stacks flex items vertically top to bottom.
            row-reverse stacks flex items horizontally right to left.
            column-reverse stacks flex items vertically bottom to top.
        3. flex-wrap: nowrap(default) / wrap / wrap-reverse;
        4. flex-flow: row nowrap(default);
            short hand property for flex-direction and flex-wrap.
        5. justify-content: flex-start(default)/flex-end/center/space-around/space-between;
            It arranges flex items around it's main axis horizontally (if row) and vertically(if column) and distributes the space between items according to the property.
        6. align-items: stretch(default)/flex-start/flex-end/center/baseline;
            It aligns items on it's cross axis vertically (if row) and horizontally(if column).
        7. align-content: stretch(default)/flex-start/flex-end/space-around/space-between/center;
            It determines spacing between item lines. If one line then no use.
        
        Child (flex items) properties are:
        1. order: -1/0(default)/1;
            By default flex items are in source code order. It helps to change the order of item.
        2. align-self: auto/flex-start/flex-end/center/(default);
            works same as align-items but aligns the particular item it overrides align-items value.
        3. flex-shrink:
        4. flex-grow: 1(default)/any positive number;
            It increases size of that item. Negative number not allowed.
        5. flex-shrink: 1(default)/any positive number;
            It decreases size of that item. Negative number not allowed.


### 2. What is grid and it's properties?
    Grid is 2 dimensional layout system. It efficiently arranges items into rows and columns.
    Parent container properties are:
    1. display:grid;
    2. grid-template-row: fr 2fr 50% 3em;
        it sets how many rows we want and their size. We can use different units like em,%,px or fr fractional unit which divides the space into fractions.
        repeat(3,2fr); repeat function will create 3 rows of size 2fr, it reduces the code.
    3. grid-template-column: fr 2fr 50% 3em;
        it sets no of columns and it's size.
    4. grid-template: fr 2fr 50% 3em / fr 2fr 50% 3em;
        short hand property for template rows and column. First value is for row / second value for column.
    5. grid-gap:10px 15px;
        short hand property for row and column gap.
    6. justify-items
    7. align-items
    8. justify-content
    9. align-content

    Child (grid items) properties are:
    1. grid-area: auto auto / auto auto;
        short hand property for grid-row-start grid-column-start/ grid-row-end grid-column-end
    2. justify-self: start/end/center/stretch;
        Aligns grid item inside cell.

        
### 3. Difference between grid and inline-grid?
Grid creates block container and takes whole width of screen and inline-grid is inline which takes width of it's size.


### 4. Difference between flexbox and grid?
flexbox is one dimensional. It is use for menu or linear designs.
Grid is two dimensional and is use when row and columns are required.