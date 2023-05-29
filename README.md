# Bazel-Project
Projects using Bazel


# Web Enumeration Automator

## Dependencies

* Python 3.8
* Nmap
* curl
* wfuzz

```
sudo apt-get install nmap
sudo apt-get install curl
sudo apt-get install wfuzz
```
### Troubleshooting wfuzz
```
pip3 install pycurl --upgrade
```

```
bazel run //webexploits:main <target IP> [nikto,durbuster,curl, wfuzz]
```
