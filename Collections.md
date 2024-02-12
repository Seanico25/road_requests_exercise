# My Findings on "American Colony in Jerusalem, 1870-2006" Collection
## The Normal Webpage view 
The website is structured to provide a comprehensive overview of the American Colony in Jerusalem collection. It features a clean and accessible layout, designed for easy navigation. Users can explore various sections such as an overview of the collection, its significance, and the types of materials included. The site utilizes both text, images, and  audio to showcase highlights and key items from the collection, allowing for an engaging and educational experience. The Library of Congress platform ensures visitors have access to a wealth of resources and tools to further their research or interest in the subject. This specific page can be found from this link to [American Colony in Jerusalem, 1870 to 2006](https://www.loc.gov/collections/american-colony-in-jerusalem/).

In addition, it also provides the following materials and information:
-   Collection spans from 1786 to 2007, focusing on the American Colony in Jerusalem.
-   Includes 16,600 items like manuscripts, photos, and diaries.
-   Documents life in Jerusalem and the Colony's impact on its social and religious life.
-   Provides insights into the Middle East's complex history through personal accounts and visual archives.
------
## The JSON format
The information regarding "American Colony in Jerusalem, 1870-2006" Collection is found listed under "['results'],[29]" of [the main collections view](https://www.loc.gov/collections/american-colony-in-jerusalem/about-this-collection/). Navigating the JSON format of the collection contrasts sharply with the user-friendly web interface, marked by an absence of visual aids and a minimalist text-centric presentation. This method inundates users with raw data, making it challenging to locate specific items due to the need to navigate through numerous textual elements and hyperlinks. Although the structure becomes more apparent, facilitating an understanding of the data organization, the utility of interacting with the JSON format seems limited mainly to those seeking a deeper comprehension of the data architecture, rather than a general exploration.

------
## The Request format  

Software strictly adheres to its instructions, which can result in both highly effective or problematic outcomes depending on the precision of those instructions. The ease of using JSON in Python, or any programming language, hinges on familiarity with the necessary commands to achieve a specific aim. My experience revealed a mix of frustration and satisfaction; frustration from the learning curve and satisfaction once mastery was achieved, underscoring the efficiency of tasks requiring repetition for those with the necessary skills. This format was accessed through the use of [Python Anywhere](https://www.pythonanywhere.com/). It would not have been at all possible to learn how to access a specific collection without the help and collaboration of my peers. 

See below the code used to access this collection:
````Python
import requests
r=requests.get('https://www.loc.gov/collections/?fo=json&at=results')
r.status_code
import json
j=json.loads(r.text)
print(json.dumps(j,indent=2))
print(j.keys())

def explore_json_structure(data, seen_values=None):
    if seen_values is None:
        seen_values = set()
    if isinstance(data, dict):
        if len(data) == 1:
            key, value = next(iter(data.items()))
            return {key: explore_json_structure(value, seen_values)}
        else:
            return {key: explore_json_structure(value, seen_values) for key, value in data.items()}
    elif isinstance(data, list):
        if len(data) > 1:
            return [explore_json_structure(data[0], seen_values)]
        else:
            return [explore_json_structure(item, seen_values) for item in data]
    else:
        if data not in seen_values:
            seen_values.add(data)
            return "VALUE"
        else:
            return "..."


j_struct = explore_json_structure(j)
print(json.dumps(j_struct, sort_keys=True, indent=2))

j_struct['results'][0]['aka']
j['results'][29]['aka']
['http://www.loc.gov/collections/american-colony-in-jerusalem/about-this-collection/', 'http://www.loc.gov/collections/acj/', 'http://lccn.loc.gov/mm2004085137', 'http://www.loc.gov/item/mm2004085137/', 'https://hdl.loc.gov/loc.mss/collmss.ms000020', 'https://hdl.loc.gov/loc.mss/collmss.ms00020x']
