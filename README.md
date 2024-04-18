# example-pq-safe-x509
A Repository to hold example x509 objects with PQ-Safe Algorithms


The x509 Objects (certs/csrs/ocsp/ctl) in this repo were created using the OQS Provider
https://github.com/open-quantum-safe/oqs-provider from the Open Quantum Safe project.

This, however, means that these x509 objects will be parseable with standard OpenSSL or other x509 clients
which haven't been updated to recognise the PQ-Safe algorithms.

Currently they are using dilitium2/3, however as per FIPS-204 internet draft, they will need to be updated
to the revised ML-DSA-44/64 OIDS when they have been confirmed.
https://csrc.nist.gov/pubs/fips/204/ipd
