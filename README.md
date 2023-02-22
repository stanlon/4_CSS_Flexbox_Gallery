# CSS Flexbox Photo Gallery

Objective: Use Flexbox to build a responsive photo gallery webpage.

- Flexbox helps design a webpage so that it looks good on any screen size.


Notes:
- To use Flexbox, give an element a display property of flex. 
- This will make the element a flex container. 
- Any direct children of a flex container are called flex items.

- Flexbox has a main and cross axis. The main axis is defined by the flex-direction property, which has four possible values:
    1. row (default): horizontal axis with flex items from left to right
    2. row-reverse: horizontal axis with flex items from right to left
    3. column: vertical axis with flex items from top to bottom
    4. column-reverse: vertical axis with flex items from bottom to top

- The flex-wrap property determines how your flex items behave when the flex container is too small. 
    - Setting it to wrap will allow the items to wrap to the next row or column.
    - nowrap (default) will prevent your items from wrapping and shrink them if needed.

- The justify-content property determines how the items inside a flex container are positioned along the main axis, affecting their position and the space around them.

- The align-items property positions the flex content along the cross axis. 
    - In this case, with your flex-direction set to row, your cross axis would be vertical.

- Images may become distorted. This is because the images have different aspect ratios.  
    - Use the object-fit property to determine how images should behave.
    - Use the object-fit property and set it to cover. 
    - This will tell the image to fill the img container while maintaining aspect ratio, resulting in cropping to fit.

- The gap CSS shorthand property sets the gaps, also knowns as gutters, between rows and columns. 
    - The gap property and its row-gap and column-gap sub-properties provide this functionality for flex, grid, and multi-column layout.
    - You apply the property to the container element.



- The ::after pseudo-element creates an element that is the last child of the selected element. 
    - You can use it to add an empty element after the last image. 
    - If you give it the same width as the images it will push the last image to the left when the gallery is in a two-column layout.
    - Right now, it is in the center because you set justify-content: center on the flex container.
    - Must use ::after on container element.
    - Then use content property set to an empty string.
    - And need to set the width property.

    

