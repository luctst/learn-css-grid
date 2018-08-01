>*We saw in the last section how to positions our elements with the `grid-column` and `grid-row` instructions but let's now see a second way of positioning elements in our grid with the `grid-template-areas`.*

The `grid-template-areas` instruction allow you to create your layout directly in css it's a really powerful instruction. We will use in this example the same grid than the last section.

## Grid-template-areas
<p data-height="265" data-theme-id="0" data-slug-hash="ejMeRy" data-default-tab="css,result" data-user="Luctst" data-pen-title="grid-template-areas" data-preview="true" class="codepen">See the Pen <a href="https://codepen.io/Luctst/pen/ejMeRy/">grid-template-areas</a> by Lucas Tostée (<a href="https://codepen.io/Luctst">@Luctst</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

1. `grid-template-areas` allow you to create the layout directly in your css, you should write exactly the same number of columns and lines or it doesn't work.
2. Once your layout is create on your container you have to create a link between the elements that you want place and the `grid-template-areas` for this we will use the `grid-area` instruction.
3. With `grid-area` we will create a key that we will use in our layout to position our elements.
4. Let's see an example, for our `header` we will use the key `h`, so in our CSS it should be `.header { grid-area: h; }` by this way the key is create. we must do the same with the key of your choice for all the elements.
5. Finally in our `.container` we can use:
```css
.container {
    grid-template-areas:
    ". . h h h h h h h h h ."
    "m c c c c c c c c c c c"
    ". . f f f f f f f f f .";
}
```
the `.` in our code indicate that we want a blank to this place.





## Current errors
This is a list of the main errors that you can meet:
> **Note:** I'm not a wizard there is maybe some issue that you notice above so fell free to open an issue in the [github repo](https://github.com/luctst/learn-css-grid) if you find a new error not mentioned above.