# E-mail-Scraper

This code is a web-scraping script that finds all emails on a given website. It starts by asking for a target URL for the user to enter. It then uses the BeautifulSoup library to scrape the contents of the URL, looking for any email addresses.

It uses regular expressions to find any valid email addresses in the response text. It then looks for any links on the page and adds them to a queue of URLs to be scraped. If a link is a relative path, it combines it with the base URL and appends it to the queue. It then loops through all the URLs in the queue, printing out each URL as it is processed and finding any emails within each page. Finally, it prints out all the emails that it found throughout its scraping.

The code above is a web crawler that finds and prints emails found on a website.

First, the user_url input is taken from the user, and stored in the urls deque.

Then, the scraped_urls and emails sets are declared.

The count variable is used to ensure the while loop doesn't run indefinitely.

Once the while loop runs, the url is taken from the deque and stored in the url variable.

The parts variable splits up the url into components, including the scheme and the netloc.

The base_url variable is created using the scheme and netloc components of the url.

The path variable is created using the url minus the '/'.

Then, the response variable sends a get request to the url.

The new_emails variable uses the re module to find all emails in the response text.

The emails set is then updated with the new_emails set.

The BeautifulSoup module is then used to parse the response text.

The for loop then finds all href attributes and stores them in the link variable.

If the link starts with '/', the base_url is added to the link.

If the link does not start with 'http', the path is added to the link.

If the link is not in the urls or scraped_urls set, it is added to the urls deque.

The KeyboardInterrupt exception is used to ensure the program exits if the user presses ctrl-c.

Lastly, the for loop prints all emails stored in the emails set.

# Wath I learn in the process

This project has helped to strengthen my Python coding abilities.

Learn how to extract data from websites using web scraping and analyze it using data mining techniques.

I learned how to use regular expressions to match patterns in email addresses.
