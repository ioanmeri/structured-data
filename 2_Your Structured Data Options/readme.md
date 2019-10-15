# Options for Adding Structured Data

To add structured data to a page, we need to know two things:

1. **What information needs to be included** — comes from what's called a taxonomy. The taxonomy defines the specific vocabulary we need to use.

1. **How to include it** — that is decided by the "syntax" or code we use to define the structured data

In this course:

1. Syntax: JSON-LD (there are other syntaxes like micro data and micro formats)

2. Taxonomy: schema.org

We look up what needs to be included on schema.org, and then create the code using JSON-LD. 

## Why Schema.org?

* Google, Bing, Yahoo! and Yandex standardized it
* Google recommends it

## Why JSON-LD?

* JSON for Linked Data
* is Javascript code that you insert into the head section of a web page.
	* JSON-LD does not require HTML to exist

### JSON-LD advantages
* not bound to the content of the web page. It does not need to be embedded in amongst the HTML tags of your page, like other syntaxes. No HTML codes.

* No need to have access to the backend of your to edit and implement JSON-LD. Google Tag Manager can be used.

### Putting it all together
When you want to add structured data to a web page, we: 

1. Decide what type of web page it is.
2. Find that "Type" over at Schema.org, which then tells us the information we can (and need to) include.
3. Using JSON-LD, create the code that defines the structured data.
4. Insert the code into our web page.


# Google guidelines
* Follow the [guidelines](https://developers.google.com/search/docs/guides/sd-policies)
* Some things have required properties that need to be included in the JSON-LD to make markup valid.
* [Content-types](https://developers.google.com/search/docs/data-types/product) examples
	* Follow content-type specific guidelines
	* Properties
		* check required fields