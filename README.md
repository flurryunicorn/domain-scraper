## Simple Domain.com.au scraper

A very simple domain.com.au rental listing scraper to compare listings as there is no compare
option in domain. So this script pulls in `X` number of listing that helps you compare domain's
rental listing as coming to a new city it is a very handy thing to have.

<image-here>

### Disclaimer

Very irresponsible and hacky software ahead that works and does the job :).

## Steps

Each domain rental listing has a unique Id like `https://www.domain.com.au/12500140` redirects to

`https://www.domain.com.au/27a-arcadia-road-chester-hill-nsw-2162-12500140` but the id `12500140`
stays the same. So this script used that unique id to visit that page and scrape 10 fields out of it then save it as a csv which is a lot easy to compare than visiting 10-20 pages. You can do it following the steps below:

1. Add all your liked listing on `domain.com.au` in your shortlist. Yes you need to register and login.
1. Then run [this](https://gist.github.com/geshan/378be819646682c715e38a653c680401) super small script on `each` of your shortlist page to get the IDs you want to compare. (only tested on chrome)
1. Copy/replace the IDs to line no. 22-27, basically fill up the `listingIds` array correctly.
<image-here>
1. Then run the script as shown below.

### Run

`node index.js` gives out domain-rentals-{timestamp}.csv in the same directory with some fields for comparision like rent, no. of bedrooms, no. of bathrooms, no. of parking, available from etc.

### Tests

Would have been good to have them, it is just a useful hack. 

### Contributions

Yes of course, there are lots of things to improve. Any contribution/PR is really welcome.
