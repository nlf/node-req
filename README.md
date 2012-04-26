### req

req is a very simple command line wrapper around Mikeal Roger's excellent [request](https://github.com/mikeal/request) library.


Usage:

    req [method] uri


Method is optional and will default to GET if not specified. URI is required (obviously).

Additional supported flags are..

    -h/--headers
        add the given header to the object passed to request, ie: -h content-type=text/plain
    -o/--options
        add the given option to the object passed to request, ie: -o encoding=binary
    -q/--query
        add the given query to the querystring object passed to request, ie: -q search=turtles
    -f/--file
        use the given file as the body in the request
    -d/--data
        use the data as the body in the request (note that both of these attempt to guess a valid content-type)
    -v   
        verbose. will console.log the arguments object before it sends the request.
