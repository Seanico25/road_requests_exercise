# Introduction

## Taking a peek at the dataset

i. **Public-facing webpages** (Library of Congress collections portal)
   
 a.
   **Header:**
   - at the top left side of the page there is the logo of the Library of Congress which is a clickable link to the home page.
   - a search bar at the top right with a dropdown menu (to help filter through a particular collection)
   - navigation menu

**Body:** 
- Page title (e.g. Digital Collections)
- carousel slider with the collection's featured content
- filter to sort the collections by (title, date, etc...)
- view option to change the how the content is displayed to the user
- each collection is displayed in a container that displays the collection name, title, a breif description, and how many items are in that collection
- side bar panel with additional filter links to other parts of the collection to refine the search results
- page numbers
- an option to change how many items are displayed on the page at a time 

**Footer:** 
- reasources, contact information, social media links and copy right logo

  ------

ii. **A specific collection**

a.  **Header:**
   - at the top left side of the page there is the logo of the Library of Congress which is a clickable link to the home page.
   - a search bar at the top right with a dropdown menu (to help filter through a particular collection)
   - navigation menu

**Body:** 
- Page title (e.g. 10th-16th Century Liturgical Chants)
- Two hyperlink headings one that displays the collection items and the other tells you about the collection 
- filter to sort the collections by (title, date, etc...)
- view option to change the how the content is displayed to the user
- each collection is displayed in a container that displays the format of the item, the title/ name of item, a breif description, date, contributor, and reasources to view more about that particular item
- side bar panel with additional filter links to other parts of the collection to refine the search results (e.g. you can filter to items dated from 1400 to 1499)
- page numbers
- an option to change how many items are displayed on the page at a time 

**Footer:** 
- reasources, contact information, social media links and copy right logo
------

2. **API -- same thing in a different format! Just add ?fo=json&at=results**

i. - ?fo=json&at=results returns the page content stored in an array called results
- they're 40 objects (0-39) in this array with nested objects and key-value pairs
    - an exmaple of these array is description: [_] when expanded shows 0: array that contains a string shown in the body of the about this collection page
- keys represents different aspects of the collection
- expanding 0: {...} shows there are a list of objects and key value pairs where each object represents a specific attribute or item of the collection and its corresponding value shows the associated data ( e.g count: 55)
- the full URL is given to where a photo is located is shown in this view, whereas in the normal webpage view the photo is shown
- the use of boolean values are shown, an example of this is "access_restricted: false" it shows you what is accessible to the public 
- timestamps of when the data was last edited
- the data is presented hierarchically, where each object represents an individual item from the collection.
- Within these objects, key-value pairs describe various attributes of the collection items.  
   
ii.
- they're 25 objects (0-24) in this array with nested objects and key value pairs
- the layout format is identical to the above mentioned with minor chaanges such as less objects 
I 
-----


## Solo Exercise








