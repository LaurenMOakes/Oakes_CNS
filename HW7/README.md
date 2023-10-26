1/c Lauren Oakes

Computer and Network Security 

26 OCT 23

## Exploit Summary - http api/storage Remote Root
This exploit is a critical security vulnerability that enables an attacker to gain unauthorized remote access to a target system like a web server using encrypted http on port 443. The exploit targets an http API used for storage, potentially found on various web services and applications and allows an attacker to achieve root-level access to the target system, which grants them full control and privileges over the server by not validating one of the user inputs. Using root access you can execute arbitrary commands, manipulate or exfiltrate sensitive data, and establish persistence on the compromised server. This exploit will work on systems with Unitrends Backup (UB) before version 10.0.0. To mitigate the risk associated with this vulnerability, it is crucial for system administrators to apply patches and updates promptly, as security patches are often released to address such vulnerabilities.

## Exploit CVE Info
CVE-2017-12478
CWE-287	Improper Authentication
Base Score - 9.8 critical

These descriptions show how dangerous this vulnerability is (very) and what category it falls under (improper authentication) so that cyberseucirty professionals can better detemrine how to prioritze and organize their resources in order to best defend their systems. Like this exploit should be a high priority to patch because of its high ranking and associated potential threats from improrer user access.

