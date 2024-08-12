SHELL := /bin/bash

orig:
	v=$$(dpkg-parsechangelog --show-field Version); \
	tar czf ../opencpn-sglock-amd64_$${v/-*/}.orig.tar.gz sglock Makefile
