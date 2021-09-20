```diff
- This repository is a deliverable for my current training as a front-end developer, do not take it into account. -
```
___
# What's Reservia?
Reservia is a website that allows you to plan your vacation, you can find accommodation and activities in the city of your choice according to filters (themes, budget, atmosphere, etc.).
___
My job is to turn a mockup into a website, not to make a functional website, so this website is only the front-end part of the project, and probably won't go further than that.
## What technologies have I used?
I was forced not to use a framework so it's just html and css without a framework.

I use flex and grid to have a fairly flexible website, then I use media queries with breackpoints:
- 1630px
- 810px

For the star system, I use the data-attributes so that I don't have to put a different class for each star.
```html
<div class="stars-count" data-stars="4">
  <i class="fas fa-star"></i>
  <i class="fas fa-star"></i>
  <i class="fas fa-star"></i>
  <i class="fas fa-star"></i>
  <i class="fas fa-star"></i>
</div>
```
And I retrieve them via the css to be able to color the stars according to the attribute.
```css
.stars-count[data-stars="1"] > i:nth-child(-n+1),
.stars-count[data-stars="2"] > i:nth-child(-n+2),
.stars-count[data-stars="3"] > i:nth-child(-n+3),
.stars-count[data-stars="4"] > i:nth-child(-n+4),
.stars-count[data-stars="5"] > i:nth-child(-n+5) {
    color: var(--blue-d);
}
```
