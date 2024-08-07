# Iowans of Things events website

## Steps for creating a new event page

1. Pull latest code down from git and make a branch. (Or use web editing tools on github to make a new branch.)
1. Change category tag on previous event from "next" to "past".
1. Add new file to "_posts" with today's date and the name of the event.
1. Copy front matter to new file
  a. Update the category tag to "next" and update the `title:` and `permalink:` fields.
  a. The date: field should be today's date. It's the date the post was published, not the date of the event.
1. Create new banner image. New image goes in assets/images
1. Add link to banner image for the event.
1. Add date, time, location information
1. Add summary paragraph.
1. Ensure the <!--more--> tag gets added. This tells the website where to clip the post for the main page.
1. Add event highlights.
1. Copy icon.
1. Copy who should come section.
1. Add event agenda.
1. Add Reserve your spot section. (Copy embedded link from Microsoft Forms)
1. `<br /><br />` spacing forces extra vertical space between elements.
1. Add sponsors section. New sponsors' logos go in the assets/images directory.
1. Commit changes and push to github. (workflow is the same on web or computer)
1. Create a pull request with your changes and assign a reviewer.
1. You should be able to see the deploy preview from netlify at the link on the PR.
