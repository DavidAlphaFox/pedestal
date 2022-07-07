# Servlet Filters

This sample shows how to use Servlet Filters and new Jetty Handlers
within your Pedestal services.
The sample specifically applies a gzip filter to the service configuration
of Jetty. To check on the encoding of the server's response,
hit with curl, requesting compression:

`curl -vv --compressed http://localhost:8080`

You'll observe in the return headers:

`Content-Encoding: gzip`

## Getting Started

1. Start the application: `lein run-dev` \*
2. Go to [localhost:8080](http://localhost:8080/) to see: `Hello World!`
3. Read your app's source code at src/gzip/service.clj. Explore the docs of functions
   that define routes and responses.
4. Run your app's tests with `lein test`. Read the tests at test/gzip/service_test.clj.
5. Learn more! See the [Links section below](#links).

\* `lein run-dev` automatically detects code changes. Alternatively, you can run in production mode
with `lein run`.

## Configuration

To configure logging see config/logback.xml. By default, the app logs to stdout and logs/.
To learn more about configuring Logback, read its [documentation](http://logback.qos.ch/documentation.html).

## Links
* [Other Pedestal examples](http://pedestal.io/samples)

License
-------
Copyright 2014-2019 Cognitect, Inc.

The use and distribution terms for this software are covered by the
Eclipse Public License 1.0 (http://opensource.org/licenses/eclipse-1.0)
which can be found in the file epl-v10.html at the root of this distribution.

By using this software in any fashion, you are agreeing to be bound by
the terms of this license.

You must not remove this notice, or any other, from this software.
