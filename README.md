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

### Run

Use following command for all:
```
bazel run //webexploits:main <target IP> nikto dirbuster curl wfuzz
```

For just nmap:
```
bazel run //webexploits:main <target IP>
```

For dirbuster (will run nmap first):
```
bazel run //webexploits:main <target IP> dirbuster
```

For curl (will run nmap first):
```
bazel run //webexploits:main <target IP> curl
```

For wfuzz (will require hostname):
```
bazel run //webexploits:main <target hostname> wfuzz
```
