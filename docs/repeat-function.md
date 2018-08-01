>*If you want create a lot of columns with the same dimensions it will be really boring if we have to create let's say 12 columns instead of that we have a function who can make your work more faster.*

## Repeat function
<p data-height="265" data-theme-id="0" data-slug-hash="LBdjBZ" data-default-tab="css,result" data-user="Luctst" data-pen-title="Repeat function" data-preview="true" class="codepen">See the Pen <a href="https://codepen.io/Luctst/pen/LBdjBZ/">Repeat function</a> by Lucas Tostée (<a href="https://codepen.io/Luctst">@Luctst</a>) on <a href="https://codepen.io">CodePen</a>.</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

1. By default we can in `grid-template-rows` and `grid-template-columns` simply add a columns or a row by adding a new parameter with a unit like this, `grid-template-columns: 1fr 1fr 1fr`, but there is a better way to do that.
2. If all your columns will be the same you can use the `repeat()` function who can help to avoid DRY.
3. The `repeat()` function need two parameters, the first parameter will be the number of columns you need, the second parameter is the size of yours columns.
4. So in our container above it would be like that, `grid-template-columns: repeat(3,1fr)`.
5. This method can be very helpful if you have a lot of columns with the same size, notice that it also work with `grid-template-rows`.

## Current errors
This is a list of the main errors that you can meet:
> **Note:** I'm not a wizard there is maybe some issue that you notice above so fell free to open an issue in the [github repo](https://github.com/luctst/learn-css-grid) if you find a new error not mentioned above.