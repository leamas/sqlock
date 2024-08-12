SHELL := /bin/bash

orig:
	v=$$(dpkg-parsechangelog --show-field Version); \
	tar czf ../opencpn-sglock-arm64_$${v/-*/}.orig.tar.gz sglock Makefile
