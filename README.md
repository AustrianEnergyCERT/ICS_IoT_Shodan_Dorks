# ICS and IoT Shodan Dork collection

## Who
Austrian Energy CERT (AEC) is the Computer Emergency Response Team (CERT) for the Austrian energy industry. For more information please see: https://www.energy-cert.at/en/

## What is a ‘dork’
Usually the term is used in the context of web search engine queries using advanced search operators so find information. In our case it refers to search terms and operators for searching Shodan.io. Simply said, you can paste the dork into	the search field of the Shodan web-interface and should be able to get results.

## Motivation
Why did we publish this dork-list?
First of all, this information is already public.
Services connected to the Internet are already sending out their banner to anybody how asks 	for them. There are also already publicly available presentations out there which contains lists of dorks to search for and find ICS and/or IoT devices. What was missing so far, at least to our	knowledge, is a central place to find quality assured dorks in an easy to use format. We are trying to fill the gap with this project.

A community can move faster together.
We hope to find a few people who are willing to help in improving this list. By improving we mean correct errors, for example in vendor attribution, make it more complete by adding dorks and additional information or find and improve inefficient/error-prone dorks.

## Disclaimer
The list is not perfect. There is no guarantee that a dork only returns the searched for ICS or IoT devices. Use the search results with care and make your own validation. If you find errors or inconsistencies in the list, please remember that we are happy to accept help and input to make this list better.

## Format
It is a standard .csv file (delimiter: ";") following this structure:

Column | Description
------------ | -------------
Vendor | If the vendor is known and the attribution is somewhat stable, the vendor name is listed in this column.
Product | If the product is known and the attribution is somewhat stable, the product is listed in this column.
Comment | Any generic comment, which might be helpful.
Dorks | Shodan search term, also called “dork”. You can paste the content of this column into the search field of the Shodan web-interface. In case you want to script the searches or use them with the command-line interface of Shodan, you are on your own when it comes to escaping, quotation and so on. Satisfying all possible scripts, interpreters and tools is beyond the scope of this project.

#### Explanation of “Generic” vendor or product:
If an attribution to a specific vendor or product is not reasonable "Generic" is set. An example for a not reasonable attribution to a vendor is the dork “tag:ics”, this tag is assigned by Shodan if there are enough indicators to Shodan, that the responding service has to be categorized as in Industrial Control System. This happens fully unrelated to a specific vendor producing the gear/software behind the service
