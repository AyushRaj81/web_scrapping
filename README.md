# web_scrapping
. In this project, the aim was to extract links related to YouTube from the Openin app website.
The project involved a number of steps, including sending HTTP requests to the website, parsing the HTML content, and filtering the relevant links.

To start, the requests library was used to send HTTP requests to the Openin app website. The HTTP response was then retrieved and the HTML content was extracted. Once the HTML content was obtained, it was parsed using the beautifulsoup4 library. This involved identifying the relevant HTML tags and attributes to extract the desired data.

The beautifulsoup4 library provides a number of useful methods for navigating and searching HTML content. In this project, the find_all method was used to extract all the links on the Openin app website. This method returns a list of Tag objects that match the specified search criteria. The Tag objects represent different elements in the HTML content, such as links, text, or images.

Once the relevant Tag objects were identified, the next step was to filter out the links that were not related to YouTube. This involved using the re library to search for links that contained the YouTube domain name. The re library provides a number of powerful tools for working with regular expressions. Regular expressions are a way of specifying patterns that can be used to match strings of text.

## For finding of valid link of youtube from multiple link i use this code: 

 youtube_pattern = r'(?:https?://)?(?:www\.)?(?:youtube\.com|youtu\.be)/(?:watch\?v=)?([a-zA-Z0-9_-]{11})'
 url_string = str(href)
 match = re.match(youtube_pattern, url_string)

In this project, regular expressions were used to search for links that contained the YouTube domain name. The re library provides a number of useful methods for working with regular expressions, including search and findall. The search method is used to find the first occurrence of a pattern in a string, while the findall method is used to find all occurrences of a pattern in a string.

Once the relevant links were identified and filtered, the final step was to store the data in a structured format. For this project, the csv library was used to create a CSV file that contained the relevant links. CSV stands for Comma Separated Values and is a common file format used for storing and exchanging data.

The csv library provides a number of useful methods for working with CSV files. To write data to a CSV file, the writerow method is used to write a single row of data to the file. In this project, each row of data contained a single link related to YouTube.

One of the key benefits of web scraping is the ability to automate the process of data collection. In this project, the use of Python libraries such as requests, beautifulsoup4, re, and csv allowed for the efficient extraction, filtering, and storage of relevant links. Without web scraping, collecting this data would have been a time-consuming and manual process.

Here in this project i just scraped only 100 links but we can stract as much as we can.

if you want to get in touch and discuss about this project here is my link: Ayushraj21042002@gmail.com
