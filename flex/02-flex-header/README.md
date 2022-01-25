# A Basic Header

Use flexbox rules to create this very common webpage header style. The benefit to using flex here is that everything should be _flexible_. Check out the two screenshots below to get an idea of how it should scale with your screen. Besides flex rules, you'll also want to add some rules for margin and padding. (Hint: `ul`s have some default margin/padding that you will need to deal with.)

## Desired Outcome

narrow:
![narrow](./desired-outcome-narrow.png)

wide: 
![wide](./desired-outcome-wide.png)

### Self Check
- There is space between all items and the edge of the header (specific px amount doesn't matter here).
Yes, by adding .header {padding: 8px}
- Logo is centered vertically and horizontally.
Yes, by adding .header {display: flex justify-content: space-between}, and .logo {align-self: center}
- list-items are horizontal, and are centered vertically inside the header.
Yes, by adding ul {display: flex;}, and .header {align-items: center}
- left-links and right-links are pushed all the way to the left and right, and stay at the edge of the header when the page is resized.
Yes, by adding ul {padding: 0px} 
- Your solution does not use floats, inline-block, or absolute positioning.
Yes.

Checked with solutions. The links from ul could be spaced out by either adding margin to the li; or adding ul {display: flex; gap: 8px}