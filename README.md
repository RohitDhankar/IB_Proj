# IB_Proj
IB_Proj  . files $rc


(py27infoBOT) dhankar@dhankar-VPCEB44EN:~/infoPROJ$ 
(py27infoBOT) dhankar@dhankar-VPCEB44EN:~/infoPROJ$ python
Python 2.7.13 |Continuum Analytics, Inc.| (default, Dec 20 2016, 23:09:15) 
[GCC 4.4.7 20120313 (Red Hat 4.4.7-1)] on linux2
Type "help", "copyright", "credits" or "license" for more information.
Anaconda is brought to you by Continuum Analytics.
Please check out: http://continuum.io/thanks and https://anaconda.org
>>> 
>>> print (u'360\B0'.encode('utf-8'))
360\B0
>>> 
>>> print (u'aa\B0'.encode('utf-8'))
aa\B0
>>> 
>>> 
>>> print (aa\B0.encode('utf-8'))
  File "<stdin>", line 1
    print (aa\B0.encode('utf-8'))
                                ^
SyntaxError: unexpected character after line continuation character
>>> 
>>> print ("aa\B0".encode('utf-8'))
aa\B0
>>> 
>>> print ("aa%".encode('utf-8'))
aa%
>>> 
>>> print ("aa%".encode('latin-1'))
aa%
>>> 
>>> print ("aa\B0".encode('latin-1'))
aa\B0
>>> 
>>> print ("aa\B0".encode('latin-1'))
aa\B0
>>> 
>>> print ("360° Degree".encode('latin-1'))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc2 in position 3: ordinal not in range(128)
>>> 
>>> 
>>> print ("360° Degree".encode('utf-8'))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc2 in position 3: ordinal not in range(128)
>>> 
>>> 
>>> print ("360° Degree".encode('utf-8').encode("ascii", "ignore"))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc2 in position 3: ordinal not in range(128)
>>> 
>>> print ("360° Degree".encode("ascii", "ignore"))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc2 in position 3: ordinal not in range(128)
>>> 
>>> 
>>> print ("360Degree".encode("ascii", "ignore"))
360Degree
>>> 
>>> print ("360° Degree".encode("ascii")
... 
... 
... quit()
  File "<stdin>", line 4
    quit()
       ^
SyntaxError: invalid syntax
>>> 
>>> print ("360° Degree".encode("ascii"))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc2 in position 3: ordinal not in range(128)
>>> 
>>> 
>>> print ("360° Degree".decode("ascii"))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
UnicodeDecodeError: 'ascii' codec can't decode byte 0xc2 in position 3: ordinal not in range(128)
>>> 
>>> print ("360° Degree".decode("latin-1"))
360Â° Degree
>>> 
>>> print ("360° Degree".decode("latin-1").decode("utf-8"))
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "/home/dhankar/anaconda2/envs/py27infoBOT/lib/python2.7/encodings/utf_8.py", line 16, in decode
    return codecs.utf_8_decode(input, errors, True)
UnicodeEncodeError: 'ascii' codec can't encode characters in position 3-4: ordinal not in range(128)
>>> 
>>> print ("360° Degree".decode("latin-1").encode("utf-8"))
360Â° Degree
>>> 
>>> 
>>> 
