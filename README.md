# conlleval.py

conlleval.py is originally contributed by spyysalo. 
The original code has some limitations. 
 - not support utf-8 (especially CJK)
 - not support program level Python API
 
This forked version is just re-factored version of the original. 

Check original connlleval.py at [here](https://github.com/spyysalo/conlleval.py)
 

# Typical Usauage
```python

from conlleval import measure_performance

# the target file is placed in the same directory as name of '__out.txt'
# the file should be 
# - '\t' seperated
# - no character (r'^$' in regular expressoin') symbol should be used as sentence boundary
# 
# the result is python dictionary object

result = measure_performance('__out.txt', delimiter='\t', boundary=r'^$')
print result 
```
