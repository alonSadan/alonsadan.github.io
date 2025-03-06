### 1. **Display** Properties
Defines how an element is displayed in the layout.

- **`display: block;`**: Element takes up the full width of its container (e.g., `<div>`).
- **`display: inline;`**: Element only takes up as much width as its content (e.g., `<span>`).
- **`display: inline-block;`**: Acts like `inline` but allows setting width and height.
- **`display: flex;`**: Enables Flexbox layout, allowing you to align child elements in a flexible way.
- **`display: grid;`**: Enables CSS Grid layout, allowing for two-dimensional layouts.

---

### 2. **Flexbox** Properties
A powerful layout mode to control alignment, spacing, and distribution of elements within a container.

- **`flex-direction`**: Defines the main axis of the flex container.
  - `row`: Aligns items horizontally (default).
  - `column`: Aligns items vertically.

- **`justify-content`**: Aligns items along the main axis (horizontal in `row`, vertical in `column`).
  - `flex-start`: Items align to the start of the container.
  - `flex-end`: Items align to the end of the container.
  - `center`: Items align to the center.
  - `space-between`: Items spread out with space between them.
  - `space-around`: Items have space around them.

- **`align-items`**: Aligns items along the cross axis (vertical in `row`, horizontal in `column`).
  - `flex-start`: Items align to the start of the cross axis.
  - `flex-end`: Items align to the end of the cross axis.
  - `center`: Items align to the center.
  - `stretch`: Items stretch to fill the container.

- **`gap`**: Sets spacing between flex items (works like `margin` but only between items).

---

### 3. **Positioning** Properties
Control where an element is placed on the page.

- **`position: static;`**: Default position, follows the natural flow of the document.
- **`position: relative;`**: Positions the element relative to its normal position. You can use `top`, `right`, `bottom`, `left` to adjust it.
- **`position: absolute;`**: Positions the element relative to the nearest positioned ancestor (non-static). Removes it from the document flow.
- **`position: fixed;`**: Positions the element relative to the viewport. Stays in place when scrolling.
- **`position: sticky;`**: Switches between `relative` and `fixed` depending on scroll position.

---

### 4. **Box Model Properties**
Defines the space around elements, including margins, borders, padding, and content.

- **`width`** and **`height`**: Set the size of the content area.
- **`padding`**: Space inside the element, between the content and the border.
  - **Example**: `padding: 1rem;` applies 1 rem of padding on all sides.
  - **Shorthand**: `padding: 1rem 2rem;` sets 1 rem top/bottom and 2 rem left/right.

- **`border`**: Defines the border around the padding and content.
  - **Example**: `border: 1px solid black;` adds a black border.

- **`margin`**: Space outside the element, between the border and surrounding elements.
  - **Example**: `margin: 1rem;` applies 1 rem of margin on all sides.
  - **Shorthand**: `margin: 1rem 2rem;` sets 1 rem top/bottom and 2 rem left/right.

- **`box-sizing`**:
  - `content-box`: Width and height include only the content (default).
  - `border-box`: Width and height include padding and border, making layout calculations easier.

---

### 5. **Alignment Properties**
Used to align elements within containers.

- **`text-align`**: Aligns inline text content within a block element.
  - `left`, `center`, `right`: Aligns text accordingly.
  
- **`vertical-align`**: Aligns inline elements or table cells vertically within their container.
  - Common values: `top`, `middle`, `bottom`.

---

### 6. **Spacing and Sizing with `rem` and `em`**
Relative units that scale with font size.

- **`rem` (Root EM)**: Relative to the root font size (`<html>` element). Consistent across the page.
  - **Example**: `1rem` is usually 16px if the root font size is 16px.
- **`em`**: Relative to the font size of the element itself. Useful for spacing that scales with element font size.
  - **Example**: `1em` equals the current font size of the element.

---

### 7. **CSS Grid** (Basic Overview)
A layout system that divides a container into rows and columns.

- **`display: grid;`**: Enables CSS Grid layout.
- **`grid-template-columns`**: Defines column structure.
  - **Example**: `grid-template-columns: 1fr 1fr;` creates two equal columns.
- **`grid-template-rows`**: Defines row structure.
  - **Example**: `grid-template-rows: auto 1fr;` creates rows with specified heights.
- **`gap`**: Sets spacing between grid items.

---

### Quick Reference Summary

| Property                  | Function                                                   |
|---------------------------|------------------------------------------------------------|
| **display**               | Defines how an element is displayed (e.g., `block`, `flex`). |
| **flex-direction**        | Controls main axis direction in Flexbox (`row` or `column`). |
| **justify-content**       | Aligns items along the main axis (e.g., `center`, `space-between`). |
| **align-items**           | Aligns items along the cross axis (e.g., `center`, `stretch`). |
| **position**              | Sets the element’s positioning (`static`, `relative`, `absolute`). |
| **padding**               | Space inside the element, between content and border.      |
| **margin**                | Space outside the element, between border and other elements. |
| **width** / **height**    | Sets the size of the content area.                         |
| **box-sizing**            | Controls how width and height are calculated (`border-box` preferred). |
| **text-align**            | Aligns inline content horizontally within a block.         |
| **gap**                   | Sets space between items in Flexbox or Grid containers.    |