>


<p align="center">
This script try to get related domains / subdomains by looking at Google Analytics IDs from a URL. First search for ID of Google Analytics in the webpage and then request to <b>builtwith</b> and <b>hackertarget</b> with the ID.
</p>
<br/>
<hr/>

**Note**: It does not work with all websites. It is searched by the following expressions: 

```
->  "www\.googletagmanager\.com/ns\.html\?id=[A-Z0-9\-]+"
-> GTM-[A-Z0-9]+
->  "UA-\d+-\d+"
```


## Installation:


```
> git clone https://github.com/Josue87/AnalyticsRelationships.git
> cd AnalyticsRelationships/
> go build -ldflags "-s -w"
```


### GO


```
>  ./analyticsrelationships --url https://www.example.com
```

Or redirect output to a file (banner or information messages are sent to the error output):

```
>  ./analyticsrelationships --url https://www.example.com > /tmp/example.txt
```

You can also pass a file as input

```
>  cat file.txt | ./analyticsrelationships 
```
OR

```
> analyticsrelationships -ch < file.txt 
```

Or a single URL

```
>  echo https://www.example.com | ./analyticsrelationships 
```


## Examples

### GO

Without redirection:

![image](https://user-images.githubusercontent.com/16885065/118682807-0e571c00-b801-11eb-8da2-d9e3d3c1d555.png)


An example with a file:

![image](https://user-images.githubusercontent.com/16885065/123318287-57506d80-d52f-11eb-89d8-cf0a3f8ab4ee.png)


# Disclaimer!

This is a PoC. The author is not responsible for any illegitimate use.
