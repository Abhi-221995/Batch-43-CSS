# Box Sizing in CSS

The `box-sizing` property defines how the total width and height of an element are calculated, including or excluding padding and borders.

## Values of `box-sizing`

| Value         | Description                                                                                               |
| ------------- | --------------------------------------------------------------------------------------------------------- |
| `content-box` | Default value. The width and height properties include only the content. Padding and border are excluded. |
| `border-box`  | The width and height properties include content, padding, and border.                                     |
| `inherit`     | Inherits the `box-sizing` value from its parent element.                                                  |

## Why Use `box-sizing: border-box`?

Using `box-sizing: border-box` makes layout calculations easier because padding and borders are included in the element's total width and height. This ensures that the specified dimensions are respected without requiring manual adjustments.

## Example

```css
/* Default behavior: content-box */
.element-content-box {
  width: 200px;
  padding: 10px;
  border: 5px solid black;
  box-sizing: content-box;
}

/* Better behavior: border-box */
.element-border-box {
  width: 200px;
  padding: 10px;
  border: 5px solid black;
  box-sizing: border-box;
}



---------------------------------------------------------------------------------------------------------------


# CSS Grid Properties

## Container Properties

| Property                | Description                                                             |
| ----------------------- | ----------------------------------------------------------------------- |
| `display: grid`         | Defines an element as a grid container.                                 |
| `grid-template-rows`    | Specifies the number and sizes of the rows. Example: `100px auto 1fr`.  |
| `grid-template-columns` | Specifies the number and sizes of the columns. Example: `1fr 2fr`.      |
| `grid-template-areas`   | Names grid areas for placement of items using `grid-area`.              |
| `grid-gap` or `gap`     | Sets the spacing between rows and columns.                              |
| `justify-items`         | Aligns grid items along the horizontal axis (`start`, `center`, `end`). |
| `align-items`           | Aligns grid items along the vertical axis.                              |
| `justify-content`       | Aligns the entire grid horizontally.                                    |
| `align-content`         | Aligns the entire grid vertically.                                      |

## Item Properties

| Property       | Description                                                                   |
| -------------- | ----------------------------------------------------------------------------- |
| `grid-row`     | Specifies the row start and end positions. Example: `grid-row: 1 / 3;`.       |
| `grid-column`  | Specifies the column start and end positions. Example: `grid-column: 2 / 4;`. |
| `grid-area`    | Places an item into a named area defined by `grid-template-areas`.            |
| `justify-self` | Aligns a single grid item horizontally.                                       |
| `align-self`   | Aligns a single grid item vertically.                                         |
```
