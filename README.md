## Why this extension

When using some website, for example, 
job list, video list, 
and they are sorted by updated time,
and most time,
you don't want to see the same thing again and again,
but they can be updated at any time.

And here comes this extension.

## How to implement

1. Checking if current page is the page you want to check.
2. Get the list data's identifier, for example, video id, job id from the HTML.
3. Check if the identifier is in the local storage / database.
4. If it is, hide it, or mark it as read.
5. If it is not, add it to the local storage / database.

## Code design

1. Storage using service / repository pattern, in case the storage changes from local storage to database.
2. Target website logic using strategy pattern, implement the logic in different class for different website.