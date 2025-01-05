## Google Analytics ID Based Subdomain Discovery

This script aims to find related domains or subdomains by searching for Google Analytics (GA) IDs on a given webpage. The process involves the following steps:

1. **Extract Google Analytics ID**: The script first retrieves the Google Analytics ID from the HTML source of the provided URL.

2. **Query Related Domains/Subdomains**: Once the GA ID is identified, the script sends requests to **BuiltWith** and **Hackertarget** to gather related domains or subdomains associated with that specific GA ID.


# Installation:


```
> git clone https://github.com/0xRupeshSardar/GoogleAnalyticsToURL.git
> cd GoogleAnalyticsToURL/
> go build 
```



```
>  ./GoogleAnalyticsToURL --url https://www.example.com
```

Or redirect output to a file (banner or information messages are sent to the error output):

```
>  ./GoogleAnalyticsToURL --url https://www.example.com 
```

You can also pass a file as input

```
>  cat url.txt | ./GoogleAnalyticsToURL 
```
OR

```
> GoogleAnalyticsToURL -ch < url.txt 
```

Or a single URL

```
>  echo https://www.example.com | ./GoogleAnalyticsToURL 
```
