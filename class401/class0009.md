# Readings

## [Review: High-level HTTP](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)

### Local Processing

This is where we make a request on the browser

```

|http|://|www.example.com||:5000||/mainpage||?query=param&query2=param2|

```

### Resolve an IP

This (I think ) will try and find a response from the server?

### Establish a TCP Connection

Makes a connection from the client to the server

### Send an HTTP Request

This is where the request is found and it genereates a HTTP response.

### Tearing Down and Cleaning Up

At this time the client sends a FIN packet and the server responds with an ACK and sends a FIN.

## [Java HTTP Request example](https://www.baeldung.com/java-http-request)

### HttpUrlConnection

it allows to perform basic HTTP requests without using any additional libraries.

### Creating a request

You can create a connection instance using the openConnection() method.

```

URL url = new URL("http://example.com");
HttpURLConnection con = (HttpURLConnection) url.openConnection();
con.setRequestMethod("GET");

```

### Adding request parameters

```

Map<String, String> parameters = new HashMap<>();
parameters.put("param1", "val");

con.setDoOutput(true);
DataOutputStream out = new DataOutputStream(con.getOutputStream());
out.writeBytes(ParameterStringBuilder.getParamsString(parameters));
out.flush();
out.close();

```