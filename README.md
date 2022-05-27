# Reason 1:
Its slow, incredibly slow, uses a lot of bandwidth and if you are using it for other purposes than testing a website, its useless.

Let me explain why its bad and why I switched to requests.

Most people use selenium, because they don't know about API's. Me too. But did you know you were at 3 clicks away from seeing the hidden part of a website?, enter inspect element, click on network and then Fetch/XHR mode. And now, you can see all the calls the website is making to their internal server.

- Why automating a login with selenium if you can do it 10x faster, without loading a whole driver?

But now you are asking yourself - how to use this API's, well use a python module called requests, and if you are using another language, a library that can make api calls. 

Here is a basic script showing an example of api call:

```python
import requests

# With the headers, we are indicating to the website that we are a normal comuter using chrome to not get detected as a bot
headers = { 
    "user-agent", "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.5005.61 Safari/537.36"
  }

response = requests.get('apiurl.com', headers=headers)
print(response.text) # this will showus the response the api made.

```
