# Inserting JSON-LD
**You can add structured data in several ways:**

* Create the JSON-LD as we have done, and insert it into the HTML code.
* Using a plugin which takes care of creating and inserting the code
	* Schema Pro for Wordpress
	* DuracellTomi's Google Tag Manager for WordPress
* Using **Google Tag Manager** to insert our JSON-LD. We will look at this as the preferred way to insert JSON-LD into our pages.

There is one other method that is not recommended, simply because only Google will be able to see this markup.

* Using Google Data Highligher to markup a page, but be aware that this markup will only be visible to Google

## Google Tag Manager
_Google Tag Manager ID => "GTM-M6GC6K7"_

* Admin
* Install Tag Manager
	* one script goes in the head, another in the body

* If you have more than one sites, use at least 1 container/site

* Every time the page loads, the code looks at your accound for tags that needs to be triggered

## Tags and Triggers
* Create a tag, that contains the JSON-LD
	* New
	* Custom HTML
	* Insert JSON-LD
		* Paste the code from [script helper](https://yoa.st/json/) 
	* Click on Support document write
	* Save (No trigger)

* We need to tell Tag Manager when that tag needs to be triggered
	* Click on Triggers
	* New (Page View)
	* Choose Page View > All Page Views

To link them, go back to the created Tag:

* Triggering
* Choose the Trigger that just created
* Now Tag ---> Firing Triggers (Page View)
* Submit
* Publish
* Preview
* Go to your website
	* Shows in the preview what is being used


## Variables
instead of having 100 different JSON-LD with same structure

e.g.
the headline and url will be automaticallly pulled from the web page

How to take Article name from the webpage **h1** directly:
* Tag Manager
* Variables
* New (Title)
* DOM Element
	* CSS Selector
	* h1
	* Save

every time the h1 is found in the page, the title will have the content of h1

* Back to Tag

From
```
"name": "Hello World"
```
to
```
"name": "{{Title}}"
```