# get_all_links_from_a_website_python

The code uses the `requests` library to send an HTTP GET request to the GitHub website (https://github.com/) and then uses `BeautifulSoup` to parse the HTML content of the web page. It extracts and prints the href attributes of all anchor (`<a>`) tags on the page.

Here's how the code works:

1. It imports the `requests` library to make HTTP requests and the `BeautifulSoup` library to parse HTML.

2. It defines the URL as 'https://github.com/'.

3. It sends an HTTP GET request to the specified URL using `requests.get(url)` and stores the response in the `reqs` variable.

4. It creates a `BeautifulSoup` object called `soup` to parse the HTML content of the response. The `'html.parser'` argument specifies the parser to use.

5. It initializes an empty list called `urls` to store the href attributes of anchor tags.

6. It iterates over all anchor (`<a>`) tags found in the parsed HTML content using `soup.find_all('a')`.

7. For each anchor tag, it retrieves the href attribute using `link.get('href')` and prints it to the console.

This code will print out the href attributes of all anchor tags on the GitHub homepage. It essentially extracts and displays the URLs that are linked to from the page. If you want to further process or filter these URLs or perform other actions with them, you can modify the code accordingly.
