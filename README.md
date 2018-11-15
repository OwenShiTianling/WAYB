#!/usr/bin/python
import re
line="Cats are smarter than dogs."
matchObj=re.match(r'(.*) are (.*?) than (.*?)',line,re.M|re.I)
if matchObj:
 print(matchObj.group(1),"are much",matchObj.group(2),"than",matchObj.group(3))
