# Schema Tools & Examples

### Schema Generators

* [schemaapp](https://www.schemaapp.com)
* [technicalseo](https://technicalseo.com/tools/schema-markup-generator/)

### Examples
_always validate the JSON-LD with Google testing tool_

* Organization (doesn't exist at Google Markup Helper)
	* helps you build your brand. This can enhance your SERP entry, but can also contribute to your knowledge graph entry
	* Things to include: name, logo, social profile & contact information

	* Google Guideline: None. When talking about this type, it refers us to [schema.org](https://schema.org/Organization)

* Product
	* For a product or service. Not a software product(there is another type for that).
	* [Google Guidelines](https://developers.google.com/search/docs/data-types/product)
	* [Schema](https://schema.org/Product)

* Event
	* To add multiple dates (that appear in google rich snippet): you can create an array of events [event1, event2]

* Course
	* The best thing to do is to grab the JSON-LD from Google site

* Local Business
	* [schema.org](https://schema.org/LocalBusiness)
	* Lots of More Specific Types
	* Standard Hours / Late Night Hours / All-Day Hours / Seasonal Hours
	* If you already have your local business [Google Markup Helper](https://www.google.com/webmasters/markup-helper/)

* Review
	* Exist at [Google Data Types](https://developers.google.com/search/docs/data-types/review-snippet)
	* Can help to build the Knowledge card 
	* Multiple reviews should be accompanied by an aggregate rating.
		* multiple reviews must be in an array of "review" : 
	```
	"review": [
		{"@type": "Review", ...},
		{"@type": "Review", ...},
	]
	```

* Software Application

* Breadcrumps
	* [Google Data Type](https://developers.google.com/search/docs/data-types/breadcrumb)
```
{
"@context": "https://schema.org",
"@type": "BreadcrumbList",
  "itemListElement": [{
    "@type": "ListItem",
    "position": 1,
    "name": "Books",
    "item": "https://example.com/books"
  },{
    "@type": "ListItem",
    "position": 2,
    "name": "Authors",
    "item": "https://example.com/books/authors"
  },{
    "@type": "ListItem",
    "position": 3,
    "name": "Ann Leckie",
    "item": "https://example.com/books/authors/annleckie"
  }]
}
```

* SiteLinks SearchBox
	* [Google Data Type](https://developers.google.com/search/docs/data-types/sitelinks-searchbox)
```
"potentialAction": {
	"@type": "SearchAction",
	"target": "http://ezseonews.com/?s={search_term_string}",
	"query-input": "required name=search_term_string"
}
```

