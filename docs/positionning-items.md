>*When we create a grid we see that our elements moves one after each other like an inline element, let's see how to move our elements as we want in our grid.*

## Positionning elements
For this example we will use this grid:
```css
.container {
    display: grid;
    grid-gap: 3px;
    grid-template: repeat(12,1fr) / 40px auto 40px;
}
```
<p data-height="265" data-theme-id="0" data-slug-hash="oMqGYG" data-default-tab="css,result" data-user="Luctst" data-pen-title="positionning elements" data-preview="true" class="codepen">See the Pen <a href="https://codepen.io/Luctst/pen/oMqGYG/">positionning elements</a> by Lucas Tostée (<a href="https://codepen.io/Luctst">@Luctst</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

1.  Once your grid is create you maybe want to positioning some elements in a different order, in css grid it's very easy to move the elements in our grid here is the first solution.
2. To move our elements we will use `grid-column` and `grid-row`.
3. The `grid-column` instruction is a shorthand for `grid-column-start` and `grid-column-end` who takes two parameters, the first define where the element should start and the second where he should end on the column line.
4. It works exactly the same for `grid-row`.
5. So the `.header, .content, .footer` class will be in our css `grid-column: 2 / -1;` this instruction will place our three divs at the second column and goes to the last column in the grid because of the `-1`.
6. For our `menu` div, we now have three columns who are placed along the horizontal axis because we played with the `grid-column` instruction, but we now want that our `menu` div will stretch to fill all the row in our grid, so the instruction will be `grid-row: 1 / -1;`. So once again our div should now start at the first row of our grid and ending at the last row in our grid.

## Current errors
This is a list of the main errors that you can meet:
> **Note:** I'm not a wizard there is maybe some issue that you notice above so fell free to open an issue in the [github repo](https://github.com/luctst/learn-css-grid) if you find a new error not mentioned above.