# hello-world
scraping e-commercial site with python and BeautifulSoup
A question about scraping information, with python bs4, from an international e-commerce marketplace.
I’m __scraping__ the site: https://www.thedetoxmarket.com/products/organic-lavender-soap?_pos=2&_sid=fc64927ad&_ss=r
This is a site that changes the prices depending on the country one selects as being in. If I select (as an example) Austria or Venezuela, the prices will be different on the site - but not in the scrape. When I want to get the price information, no matter what country I put as my location, it scrapes the prices for the US location.
Here is the code, that i wrote for the scrape:
```
price = soup.find('div', class_ = 'apercu-medium-19 pb-3 mt-3 mb-1' ).text.strip()
print(price)
```
Here is the code from the site:
```
<div class="price d-none d-lg-block">
<div class="text-left">
<div class="apercu-medium-19 pb-3 mt-3 mb-1" style="visibility: visible;">
€‌8.95
</div>
</div>
</div>
```
How can I scrape in such a way that the prices will reflect the location I selected?
