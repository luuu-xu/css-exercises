# A common 'modal' style
This one is another very common pattern on the web. The solution to this one is _simple_... but it might not be immediately obvious to you. You'll need to edit the HTML a bit to get everything where it needs to be.

### A hint
Depending on how you approach this one, you might need to revisit the `flex-shrink` property to keep a flex item from getting smashed.

## Desired outcome

![desired outcome](./desired-outcome.png)

### Self Check

- The blue icon is aligned to the left.
Yes, by setting .modal {display: flex}
- There is equal space on either side of the icon (the gaps between the icon and the edge of the card, and the icon and the text, are the same).
Yes, by adding .modal {gap: 16px}
- There is padding around the edge of the modal.
Yes, by adding .modal {padding: 16px}
- The header, text, and buttons are aligned with each other.
Yes, because these are all under .container-content {display: flex; flex-direction: column}
- The header is bold and a slightly larger text-size than the text.
Yes, by setting .header {font-size: larger; font-weight: bold}
- The close button is vertically aligned with the header, and aligned in the top-right of the card.
Yes, by setting .container-title {display: flex; justify-content: space-between}

Checked. Correct. 
But it could be easier. I created areas icon and container-content and set display to flex, which is correct way to make sure icon and texts are separeted and icon doesn't get shrinked. But then I created areas within container-content to container-title, text and container-buttons, set displat to flex and flex-direction to column. Instead, it doesn't have to be flex, because header, text and button are already block elements so they are separeted. Though setting container-title is right for putting title and close-button into one area. But I could've just indenting .close-button under .header, that way I dont't need to create container-title at all and also set displat to flex.
