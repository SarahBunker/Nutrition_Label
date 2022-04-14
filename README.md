# Nutrition_Label
Recreating a Nutrition facts label from image.

Using [this](https://upload.wikimedia.org/wikipedia/commons/2/2b/FDA_Nutrition_Facts_Label_2006.jpg) image I attempted to recreate the Nutrition label using HTML and CSS. 

Assignment Restrictions and Guidance:
- only use one class
- Do not `div` and `span` elements
- strive to make it look as much like the original as possible without purchasing fonts
- font stack can use Franklin Gothic Heavy for the main heading
- Helvetica Black and Helvetica for the remaining fonts
- add Arial to the list
- let the browser supply a default font if necessary

Things I learned during this project.
- You can use multiple pseudo-classes element selectors in a combination selection.
- You can have multiple `tbody` elements in a table but only one `thead` and `tfoot`.
- Margins and Padding within tables are tricky.
- The CSS property `font-weight` has a lot more options then just bold. You can pick a specific value where `400` is normal weight and `700` is normal bold.
- You can have empty cells.
- You don't have to make a rowspan larger if you know the text is going to wrap over. It takes care of itself.
- Because this was the largest HTML and CSS project I have attempted to this point it helped to solidify a few topics that I had learned, but had to apply.
  - Tables
  - font-family
  - colspan
  - Using a lot of different kinds of CSS selectors

Things I want help with:

Currently my horizontal lines go the full distance across the table. I think this is because I used `border-collapse: collapse;`. I tried adding the following:
```css
table {
  ...
  border-collapse: separate;
  border-spacing: 20px, 0px;
}
```
Because in order to add spacing between cells you have to set it to `seperate` instead of collapse, but this didn't and it made it so the borders went into the cell so I couldn't create the large black lines for spacing.

I also had trouble with the indented lines haveing borders that go all the way to the edge of the screen. I am using padding to indent the text, but that doesn't affect the border, and margins are crazy in tables, so I didn't get that to work either.
