_This document is looking at a specific collection on congress_




# Preamble

## [Python - Requests](https://requests.readthedocs.io/en/latest/)
> **Requests** is an elegant and simple HTTP library for Python, built for human beings.

### Blurb


### Useful Commands
import requests
r=requests.get('https://www.loc.gov/collections/?fo=json&at=results')
r.status_code

r.json()
r.headers['Content-Type']

## [Python JSON](https://docs.python.org/3/library/json.html)

### Blurb


### Useful Commands

# Comparisons

## [Library of Congress - Collections](https://www.loc.gov/collections/)

### To Infinity and Beyond

I recently had watched a [YouTube video](https://youtu.be/fG8SwAFQFuU?si=Eg1Ozdhur4K3w0aj), from someone I follow and the responses he got surprised me. Curated though they may be, I had assumed a bit of what he said was common knowledge, which really reveals some of my biases and preconceptions about common knowledge. I also don't have a leg to stand on, ask me about the names for **anywhere** in Barbados more than a mile from my home, and I *guarantee* I don't know it.

What's my point here? Ideas about the universe are fresh in my mind and so the collection entitled, [*Finding Our Place in the Cosmos: From Galileo to Sagan and Beyond*](https://www.loc.gov/collections/finding-our-place-in-the-cosmos-with-carl-sagan/about-this-collection/) really clicks with me.

The collection describes itself with the following words:
> A thematic collection exploring changing models of the universe through time, ideas of life on other words and Carl Sagan’s place in the tradition of science. It features manuscripts, rare books, celestial atlases, newspaper articles, sheet music and movie posters.

### Standard View Html

#### Pale Blue Dot *And Other Pixels*

People interact with the world mostly through sight, and having the images makes the experience as a user much more immersive. It's not just text, but actual pictures, which I assume is as good at it gets, excluding the real thing.

### JSON

#### Browser

#### Command Line


<!--

# Appendix

## Links to Consider
This section will be deleted, but will hold some links which may be used in the document

- [The Milky Way: One of the Many Galaxies](https://www.loc.gov/collections/finding-our-place-in-the-cosmos-with-carl-sagan/articles-and-essays/modeling-the-cosmos/the-milky-way-one-of-the-many-galaxies/)
   - Speaks to the size of milky way. I dig the scanned old [atlas](https://www.loc.gov/resource/g3180m.gct00292/?sp=6&r=-0.018,-0.11,1.288,0.633,0).


## Aspects to Compare about the Collection

This is not an exhaustive list, but should give some direction in what to look at

- What's generally interesting about the collection to you?
  - Have a general look, then breakdown by html and json in browser & command-line
- How is it structured?
  - Compare html and json, similarities and differences
- How was navigating the data
  - For html & json state in browser & command line: ease of use, similarities and differences
  - Note any idiosyncrasies for the three different methods
  - Note naming conventions
  - Note choices made in the organising, maybe consider why they were made and their likely trade-offs
- Note how you may want to use the data
  
-->
