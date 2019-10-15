# Creating Markup

* Test if there is any structured data already in your website
	* [Google Structured Data Testing Tool](https://search.google.com/structured-data/testing-tool#)
	* Make sure there are no errors

## Deciding on Type
* First and most important
* Can choose one of the [Things](https://schema.org/Thing)
* e.g. Creative Work
	* Article
	* Blog
* Check [Content Types](https://schema.org/Thing) on Google Guidelines
	* It has **Article** but **not Blog**
* Now use the Schema from schema.org

## Creating the Markup I
* If the Thing you want to add SD exists already as a data type in [Structured Data Markup Helper](https://www.google.com/webmasters/markup-helper/?hl=en_GB), use the SD Markup Helper to generate JSON-LD.
* Then [test](https://search.google.com/structured-data/testing-tool) the generated JSON-LD to make sure no errors occur or missing fields exist
	* if certain fields are missing, you can add them in the testing tool and check again

## Creating the Markup II (manually)
* 1 Way

	* Visit schema.org
	* Find Recipe schema (which doesn't exist in Google Markup Helper)
	* check all the options you can add
		* cookTime: the time it takes to actually cook in ISO 8601 duration format
	* copy **Example schema**, paste at the Google Testing Tool, edit the fields

* 2nd Way
	* Find example in Google data types

_Google AMP is a website publishing technology that lets you create web pages that load almost instantly on mobile phones._
