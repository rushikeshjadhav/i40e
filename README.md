# Build your kernel driver

In order to build any driver yourself, go on your docker host and use follwing shell commands to build it:

```
mkdir driver-i40e

cd driver-i40e

git clone https://github.com/xcp-ng/xcp-ng-build-env

git clone https://github.com/rushikeshjadhav/i40e

chown 1000 ./i40e/ -R

./xcp-ng-build-env/run.py -b 7.6 --build-local i40e/ --rm
```
