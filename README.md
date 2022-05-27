# Reason 2:
Its slow, incredibly slow, uses a lot of bandwidth and if you are using it for other purposes than testing a website, its useless.

Let me explain why its bad and why I switched to requests.

Most people use selenium, because they don't know about API's. Me too. But did you know you were at 3 clicks away from seeing the hidden part of a website?, enter inspect element, click on network and then Fetch/XHR mode. And now, you can see all the calls the website is mkeing to their internal server.

- Why automating a login with selenium if you can do it 1Ox faster, without loading a whole driver?

But now you are asking yourself - how to use this API's, well use a python module called requests, and if you are using another language, a library that can make api calls. 

Here is a basic script showing an example of api call:

```python
import requests

headers = {"user-agent", ""}

requests.get('apiurl.com', headers=headers

```
