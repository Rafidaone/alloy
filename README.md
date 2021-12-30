# Alloy Proxy
A web proxy for use in combating web filters.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/titaniumnetwork-dev/alloy/tree/master)

this is a modifide vershion of alloy that i made to use in my school it pritends to be schoology and it has a thing to prevent smart ass's from looking at your screen for the url


## Running locally

```sh
git clone https://github.com/titaniumnetwork-dev/alloyproxy.git
cd alloyproxy
npm start
```


## Options in config.json
```json
{
    "port": "80",
    "ssl": false,
    "prefix": "/web/",
    "localAddresses": [],
    "blockedHostnames": ["192.168.1.254"]
}
```

`"port": "8080"` = Sets HTTP server port of web proxy.

`"ssl": "false"` = Sets HTTP server SSL.

`"prefix": "/web/"` = Sets the overall prefix of the web proxy.

`"localAddresses": [ "0.0.0.0" ]` = Allows you to choose which IP to make the request from. If there are multiple IP's then the IP chosen will be randomized.

`"blockedHostnames": [ "example.org", "example.com" ]` = If the hostname of the proxy URL matches any of the URL hostnames listed in the array, the request to the server will be cancelled.
