# JSON -LD

* **You can use examples provided by google and edit them, or use generator tools**

* JSON-LD is the code used to pass the meta data (structured data) to the search engines.

* It is Javascript

* It uses **name/value** pairs. We've seen this earlier when looking at the properties of different "things". Each property (name) has a value.

* JSON uses some "reserved" names which you can easily spot because they start with an **@**

* @context & @type are the two you will see over and over when working with structured data.

## @context
* Since we will be using the schema.org vocabulary, the @context will always have a value of http://schema.org
* Specifies the format of the meta data. We are telling the search engines that the following JSON-LD uses the meta data structure from schema.org

## @type
* part of the schema (from schema.org) that we want to define.

* e.g. @type can be an article, recipe, restaurant, offer, price, rating, etc.

* Once you define the @type for a thing, you then define the properties and values (for that type) that you want to include in your markup

### Example
```
<script type="application/ld+json"
{
	"@context": "http://schema.org",
	"@type": "Product",
	"aggregateRating": {
		"@type": "AggregateRating",
		"bestRating": "100",
		"ratingCount": "24",
		"ratingValue": "87"
	}
}
</script>
```