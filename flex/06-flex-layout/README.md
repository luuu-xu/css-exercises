# An entire page!

Flexbox is useful for laying out entire pages as well as the smaller components we've already been working with. For this exercise, we're leaving you with a little more work to do, with some things you may not have encountered yet. It's perfectly acceptable to google things you're unsure of!

### Hints
- You may want to search something like `CSS remove list bullets`.  We've done this for you in previous examples, but not here. Yay learning.
- We've added `height: 100vh` to the `body`... this makes the body exactly the same height as the viewport. To stick the footer to the bottom you will need to use flex and change the direction to column.

## Desired Outcome
![desired outcome](./desired-outcome.png)

### Self Check

- The header is at the top of the page, the footer is at the bottom, and they stay in place if you resize your screen.
Yes, by setting body {display: flex; flex-direction: column; justify-content: space-between}
- The header and footer have padding.
Yes, by adding .header,.footer {padding: 16px}
- The links in the header and footer are pushed to either side.
Yes, by setting .header,.footer {display: flex; justify-content: space-between}
- There is space between the links in the header and footer.
Yes, by setting ul {display: flex; gap: 20px}
- The footer has a light gray background (`#eeeeee`).
Yes.
- The logo, input and buttons are centered in the screen.
Yes, by setting .content {align-self: center; display: flex; flex-direction: column; align-items: center}
- The buttons have an appropriate amount of padding.
Yes, by setting button {padding: .5em 1em}
- There is space between the logo, input and buttons.
Yes, by setting .content {gap: 8px}

Checked with solutions. Correct.
But I set body {justify-content: center} to make the content (logo, input, buttons) to be centered vertically, instead, it should set .content {justify-content: center}