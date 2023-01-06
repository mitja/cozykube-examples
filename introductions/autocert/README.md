# Autocert Introduction Examples

This folder contains examples for the [autocert introduction](https://cozykube.com/autocert/). Check the tutorial in this introduction for a description how to use these examples.

## Notes

- the client runs curl every 5 seconds and presents its certificate and checks that the server certificate is valid
- the server runs Nginx which is configured to use the certificates and check the validity of client certificate
- the *certwatch.sh* script of the nginx server watches for file changes on the certs and reloads nginx if the certificate files have been changed. It is linked in the *entrypoint.sh*. The certificates are changed due to periodic renewal performed by autocert.

## Acknowledgements

The examples are just copies of the nginx and curl examples from the original [autocert examples](https://github.com/smallstep/autocert/tree/master/examples) which are published under the same license as autocert (Apache 2.0 license). I copied them here to have a complete repo for all the examples.