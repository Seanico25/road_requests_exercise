# Road Requests Exercise

> The collection I chose was "Civil War", the link to it in webpage format is:
https://www.loc.gov/collections/civil-war
>The link to the JSON version of the webpage is:
https://www.loc.gov/collections/civil-war/?fo=json&at=results


## 1. JSON Format

On the JSON version of the webpage, results is shown with a nested arrow containing a total of 25 results numbered 0-24. Within each numbered result, is the metadata of the individual collection entries. This information is all text, and under the id heading contains a link to the collection referenced in the numberedd result. For example: number "1:" links to page http://www.loc.gov/item/2002719396/ showing a photo titled "Black soldier seated with pistol in hand, watch chain in pocket".
This collection features 19,797 items available online, _however_ only the first 25 entries are shown on the results page in JSON.

## 2. Normal WebPage

On the normal web page, the list of items on the collection is diplayed with an image, and text with a title and a short description on the right hand side of the page. On the left hand side is a list data types you can use to refine your search, such as, date, online format, original format, contributor etc. Unlike the JSON format, you can access multiple pages of content, with up to 25 items per page.

## 3. Command-line View

In the command-line view  after inputting the command "print(json.dumps(j,indent=2))", the results page from the JSON format is printed. _However_, all the metadata that was nested in that format is now printed in it's entirety with curly brackets( {} ) to represent the nested parts and square brackets( [] ) to encapsulate the data contained. This string extends for several screens in a continous stream which would generally require careful parsing to be understandable, or a side by side comparison with the JSON formate page to give you a better idea of the data being shown.
