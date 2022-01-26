# The Holy Grail of Layout

In this last flexbox exercise you're going to recreate an incredibly common website layout. It is so common that it is often called the [Holy Grail](https://www.google.com/search?q=holy+grail+layout&tbm=isch&sclient=img) layout... and with flexbox it is actually pretty easy to pull off.

As with the previous exercise, we've left a little more for you to do.

### Hints
- You will need to change the flex-direction to push the footer down.
- You will need to add some divs as containers to get things to line up correctly. 
- `flex-wrap` will help get the cards aligned correctly.

## Desired outcome

![desired outcome](./desired-outcome.png)

The number of cards lined up in that section will change based on the width of your screen, so don't stress about getting _exactly_ a 2x3 or 3x2 grid.

On a smaller screen it will look like this:

![smaller](./desired-outcome-smaller.png)

### Self Check
- The header text is size 32px and weight 900.
Yes, by setting  .header {font-size: 32px; font-weight: 900}
- The header text is vertically centered and 16px from the edge of the screen.
Yes, by setting .header {display: flex; align-items: center; padding-left: 16px}
- The footer is pushed to the bottom of the screen (the footer may go _below_ the bottom of the screen if the content of the 'cards' section overflows and/or if your screen is shorter).
Yes, by setting up .header, .content, .footer under body and set .body {display: flex; flex-direction: column}
- The footer text is centered horizontally and vertically.
Yes, by setting .footer {display: flex; justify-content: center; align-items: center}
- The sidebar and cards take up all available space above the footer.
Yes, by setting up .sidebar, .cards under .content and setting .content {display: flex}
- The sidebar is 300px wide (and it doesn't shrink).
Yes, by setting .sidebar {width: 300px; flex-shrink: 0}
- The sidebar links are size 24px, are white, and do not have the underline text decoration.
Yes, by adding ul {list-style-type: none; margin: 0; padding: 0}, and setting a {font-size: 24px; text-decoration: none; color: #eee}
- The sidebar has 16px padding.
Yes, by setting .sidebar {padding: 16px}
- There is 32px padding around the 'cards' section.
Yes, by setting up .cards area to colloect all cards.
And setting .cards {gap: 30px; padding: 50px}
- The cards are arranged horizontally, but wrap to multiple lines when they run out of room on the page.
Yes, by setting .cards {display: flex; flex-wrap: wrap}
And also setting .card {width: 300px; max-height: 300px; min-height: 200px}

Checked with solutions. 
!!!Important mistake: how to make footer to stay at the bottom of the page when browser window is tall enough but when the browser window is too short the footer stays outside of the view?
By setting up areas: header, content, footer.
And then setting header and footer to a fixed height, then setting body {display: flex; flex-direction: column} and setting !!!.content {flex: 1}