# Requests Exercise

I chose the "America Singing: Nineteenth-Century Song Sheets" for this exercise.

## JSON Variables
* "access_restricted" which is set to false across the entire page, indicating that all items in this collection are accessible
* "aka"(links that open the particular item)
* campaigns(unsure)
* "digitized", set to true across the collection
* "extracted_timestamp"(unsure)
* "group"(unsure) which contains "hassegments" set to false across collection
* "id"(url)
* "image_url"(urls containing the image)
* "index"
* "item" which contains "format", "genre", "language", "medium", "notes"(item description, "repository", "rights","source_collection"), and "subjects"
* "title"
*  "language"
*  "mime_type"(image formats?)
*  "online_format"
*  "original_format"(contains "other_title")
*  "partof"(collections?)
*  "resources"(contains "files", "image", "url")
*  "shelf_id"(subdirectory of url)
*  "subject"(contains subject, "timestamp", "title")
*  "type"(contains type and "url")

### Browser JSON View Visual Differences
Each collection item is identified by "number:"(0:, 1:) and is segmented into several variables which provide details about the item. 

### Python Console JSON View Visual Differences
* Each collection item is identified by braces("{}") and is segmented into several variables which provide details about the item.
  * Variables that contain multiple variables/items use square brackets"[]"

#### General Thoughts/Observations
* Most of the information provided in the code is hidden from the user's view and also repeats multiple times for e.g title and language
* Browser JSON View is much easier to read than the Python JSON view since it is collapsible and laid out cleaner
* Some variable names do not fully convey their purpose especially since all information is now visible from the user's view

