# Text-preprocessing

##### extracting the html links from text
```
import re
text = '<p>Contents :</p><a href="https://w3resource.com">Python Examples</a><a href="http://github.com">Even More Examples</a>'
urls = re.findall('http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+', text)
print("Original string: ",text)
print("Urls: ",urls)

```
Output: 
  Original string:  @bbcmtd Wholesale Markets ablaze http://t.co/lHYXEOHY6C
  Urls:  ['http://t.co/lHYXEOHY6C']
  
##### extracting the twitter user names from text 

```
import re
twitter_username_re = re.compile(r'@([A-Za-z0-9_]+)')

```
##### Special Characters in string literals
```
from string import punctuation
set(punctuation)
```
