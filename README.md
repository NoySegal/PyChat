# PyChat
A Python chat application

### Prerequisites
This version of the code runs successfully on Windows 10 and Ubuntu-18.04. Should also compile on other variants of linux and Windows. Other operating systems are currently not supported.

### How to use:
* Download all files. You'll also need Python 3 interpreter installed. (Download Python 3 from [here](https://www.python.org/downloads/))
* Fire up server:

```python
python3 server.py
```

* Fire up client/s:

```python
python3 client.py
```

Once a server is running, it will accept clients which can send and receive messages simultaneously. Command-line style.

### Example:

#### Server-side:
```
$ py server.py
> Accepted new connection from 127.0.0.1:41202 username: tester1
> Accepted new connection from 127.0.0.1:41203 username: tester2
> Received message from tester1: Hello
> Received message from tester2: How are you?
```

#### client 1:
```
$ py client.py
> Username: tester1
> tester1 >> Hello
> tester1 >>
> tester2 > How are you?
> 
```

#### client 2:
```
$ py client.py
> Username: tester2
> tester2 >>
> tester1 > Hello
> How are you?
> tester2 >>
```
