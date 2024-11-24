## Coffee Scraper

This will be a service that will periodically run and scrap coffee roasters.

This will be a service that is kicked off by something else and will return
back a JSON of everything that's pertinent/needed

## What will the normalize data look like

* Roaster
* Roast Level
* Variety
* Process
* Country of Origin
* Elevation
* Tasting Notes
* Date Added
* Description
* Picture of bag
* Availbles sizes, and price
* Link to the actual website buy it from

## Roasters?

| Roasters | Support Added |
| -------- | ------------- |
| Onxy | N/A |
| Sey | N/A |
| S&W | N/A |

More Roasters to Come

## Scraping

Onyx uses shopify and there is a `all.atom` that will give you all the
coffee/accessories and stuff in a HTML formatted file. Need to parse
it using something like `BeautifulSoup`

S&W There is a API with JSON data with everything we will need

## Language

What language do we want to use here, do we want `Python`, `JS`, `JAVA`,
`GOLANG`, or `RUST`

I think either Rust or Golang would work best here,

This service will not actually write directly to a database, but will become
a Rest API endpoint that will hit and return a JSON.

Will hitting it return a JSON with all the roasters it can, or will it just
take a Roaster as a request and return the information related to that?

Another service will eventually call for each supported roaster, get the
data then put it into a database

## What are we going to do with this

Eventually, what will happen if this will then just populate a website, and we
would be grouped.

What would it be grouped by? Roaster, Process, Country of Origin, Elevation,
Tasting Notes, Variety, Roast Level

Then we will continue on adding more and more roasters

Eventually we will add a Reccomender System, "You like x why don't you try these
coffee they are similar", "You like Roaster Y, These other Roasters have Similar
Coffee" coffee_scraper

