### req

req is a very simple command line wrapper around Mikeal Roger's excellent [request](https://github.com/mikeal/request) library.


Usage:

    Usage: req [options] [method] uri

    Methods:
      Any valid HTTP method is supported. If unspecified, GET will be used.

    Options:
      -h, --headers      Headers to attach to the request in the form header=value                                                                                                                  
      -q, --querystring  Querystring parameters in the form param=value (these can also be passed as part of the URI)                                                                               
      -b, --body         The body of the request. If this is set to valid json, it will automatically set the json content-type. Can also attach the contents of the file using e.g. @uploadthis.txt
      -o, --output       File to write output to, otherwise will print text and json to screen and guess a filename for binaries                                                                    
      -u, --username     Username for basic auth                                                                                                                                                    
      -p, --password     Password for basic auth                                                                                                                                                    
      -f, --form         Similar to the body flag, but sends the data as x-www-formurlencoded                                                                                                       
      -v, --verbose      Output response headers and status codes   
