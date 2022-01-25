# A very common website feature

The goal of this exercise is to recreate a section that is found on many informational websites.

For this one you will need to edit the HTML a little bit too. We can't be making things _too_ easy for you. You'll want to add containers around the various elements so that you can flex them. Good luck!

## Desired outcome

![desired outcome](./desired-outcome.png)

### Self Check

- All items are centered on the page (horizontally, not vertically).
Yes, by setting .container-title,.container-content {display: flex; justify-content: center}
- The title is centered on the page.
Yes
- There is 32px between the title and the 'items.'
Yes, by setting .container-page {display: flex; flex-direction: column; gap: 32px}
- There is 52px between each item.
Yes, by setting .container-content {gap: 52px}
- The items are arranged horizontally on the page.
Yes
- The items are only 200px wide and the text wraps.
Yes, by setting every .items {width: 200px; display: flex; flex-flow: column wrap; align-items: center}
- The item text is centered.
Yes, by setting .text {text-align: center}

Cheked with solutions. All correct, but I solved it way too complicated. I added too many containers on the page by visualizing every area on the page, instead it could be done by regular methods like text-align or margin-bottom or max-width.