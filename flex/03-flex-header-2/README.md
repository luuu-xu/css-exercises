# Another common header style

We're starting to sneak in a little more CSS that you haven't seen yet. Don't worry about this for now; we just want things to look a little bit prettier, and this CSS will not interfere with your task.

For this one you will probably need to edit the HTML a little bit. Often with flexbox you need to add containers around things to make them go where you need them to go. In this case, you probably want to separate the items that go on the left and right of the header.

This is also the first example where you'll be nesting flex containers inside each other.

## Desired outcome
As with the last example, this one needs to be flexible in the middle, with items pushed to the left and right.

![png](./desired-outcome.png)

![gif](./desired-outcome.gif)

### Self Check
- Everything is centered vertically inside the header.
Yes, by adding .header {display: flex; align-items: center}.
And setting up .container-left,.container-right {display: flex; align-items: center}
- There is 8px space between everything and the edge of the header.
Yes, by setting .header {padding: 8px}
- Items are arranged horizontally as seen in the outcome image.
Yes, by setting .header,.container-left,.container-right {display: flex}
- There is 16px between each item on both sides of the header.
Yes, by setting .container-left,.container-right {gap: 16px}
- flex is used to arrange everything.
Yes. 

Checked with solutions. All correct.
Note: lists need to be set ul {pdding: 0; margin: 0} because The <ul> and <ol> elements have a top and bottom margin of 16px (1em)  and a padding-left of 40px (2.5em.)