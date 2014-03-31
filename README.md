RGF - DEV BRANCH
===

Sending data to Graphite via REXX Socket API on z/OS. 

If your site has the ported tools activated within USS it's recommended to use 'curl' for sending data to Graphite. If you don't have (or are not allowed) curl you can try compiling 'netcat for z/OS'.

One can also use the native REXX SOCKET API to 'talk' to a graphite server (essentially just netcatting).

The function in this repository does just that.

###usage example

    /*REXX*/
    toGraphite('my.key', 123, '192.168.1.5', '2003')
    
    
Will send value 123 for key 'my.key' to the Graphite server at 192.168.1.5

###todo

* Proper error handling
* read server/port data from config file?


###Contribute
If you're a __*System z*__ idiot like me feel free to contribute. Please use the DEV branch for your pull-requests :)
