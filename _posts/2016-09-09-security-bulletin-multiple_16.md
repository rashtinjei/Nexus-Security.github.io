---
title: 'Security Bulletin: Multiple vulnerabilities in IBM Java Runtime affect Rational Directory Server (Tivoli) & Rational Directory Administrator'
date: 2019-12-17T01:40:00+01:00
draft: false
---

#### Dec 3, 2019 7:00 pm EST | [Low Severity](https://www.ibm.com/blogs/psirt/category/severity-low/)

CVEID:   CVE-2019-1552 DESCRIPTION:   OpenSSL has internal defaults for a directory tree where it can find a configuration file as well as certificates used for verification in TLS. This directory is most commonly referred to as OPENSSLDIR, and is configurable with the --prefix / --openssldir configuration options. For OpenSSL versions 1.1.0 and 1.1.1, the mingw configuration targets assume that resulting programs and libraries are installed in a Unix-like environment and the default prefix for program installation as well as for OPENSSLDIR should be '/usr/local'. However, mingw programs are Windows programs, and as such, find themselves looking at sub-directories of 'C:/usr/local', which may be world writable, which enables untrusted users to modify OpenSSL's default configuration, insert CA certificates, modify (or even replace) existing engine modules, etc. For OpenSSL 1.0.2, '/usr/local/ssl' is used as default for OPENSSLDIR on all Unix and Windows targets, including Visual C builds. However, some build instructions for the diverse Windows targets on 1.0.2 encourage you to specify your own --prefix. OpenSSL versions 1.1.1, 1.1.0 and 1.0.2 are affected by this issue. Due to the limited scope of affected deployments this has been assessed as low severity and therefore we are not creating new releases at this time. Fixed in OpenSSL 1.1.1d (Affected 1.1.1-1.1.1c). Fixed in OpenSSL 1.1.0l (Affected 1.1.0-1.1.0k). Fixed in OpenSSL 1.0.2t (Affected 1.0.2-1.0.2s).CVSS Base score: 2.9CVSS Temporal Score: See: https://ift.tt/2DFVDUX for the current score.CVSS Vector: (CVSS:3.0/AV:L/AC:H/PR:N/UI:N/S:U/C:N/I:L/A:N) [...read more](https://www.ibm.com/blogs/psirt/security-bulletin-vulnerability-in-openssl-affects-ibm-cloud-pak-system-cve-2019-1552/)

  
  
from IBM Product Security Incident Response Team https://ift.tt/2YUflpM