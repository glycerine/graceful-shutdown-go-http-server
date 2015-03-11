# graceful-shutdown-go-http-server

This code has been extracted, slimmed to the bare essentials, and modified slightly from the original. The original source code is from Richard Crowley's go-tigertonic project, located at https://github.com/rcrowley/go-tigertonic.

This is just the essentials to get a gracefully-stoppable web-server. Go Tigertonic provides a wealth of other features that we don't require.

We also allow setting the timeouts for reads on the webserver, which is highly useful, in fact critical, for rapid testing. When your tests create and destroy web servers quickly, use this project and set the timeout parameter on your calls to NewCustomHttpServer() to something small; e.g. <= 500 msec to avoid long test-shutdown times.

Copyright (c) 2015 Jason E. Aten, Ph.D.

Copyright (c) 2013 Richard Crowley.

License: 2-clause BSD, see LICENSE file.
