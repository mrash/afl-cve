# afl-cve
A collection of vulnerabilities discovered by the AFL fuzzer (afl-fuzz)

## Introduction
`afl-cve` is a collection of known vulnerabilities that can be attributed to the
AFL fuzzer [afl-fuzz](http://lcamtuf.coredump.cx/afl/). All vulnerabilities in
this list either already have a CVE assigned, or a CVE has been requested from a
[CVE Numbering Authority](https://cve.mitre.org/cve/cna.html#participating_cnas).

## Why is This Necessary?
Because CVE descriptions are not generally being written to mention AFL as the
tool that enabled particular bugs to be found. his is primarily due to the fact
that CVE descriptions do not require the underlying discovery tool or technique
to be disclosed. Nor should it necessarily - many security researchers have their
own methods, and it might hurt the vulnerability reporting process if researchers
were required to disclose such techniques. Further, most security researchers do
acknowledge AFL in some form (twitter post, afl-users mailing list, etc.) when
it finds a bug, and `afl-cve` attempts to track this more formally.

## Fuzzing Revisited
AFL has discovered a huge number of bugs in all sorts of projects from compilers
to image processing libraries. Many of these bugs have been assigned a CVE number,
and this is at least a tacit acknowledgment of potential exploitability. So, the
bugs AFL has found are therefore frequently *important* for anyone concerned about
security. AFL seems to be succeeding where other fuzzers have failed, or at least
not been generally embraced or operationalized by the security community for
whatever reason. Another way to see this is to try to determine which fuzzer has
the most CVE's. Is there a different fuzzing project that comes close to AFL in
terms of the number of vulnerabilities found? It would be instructive to see
which fuzzer comes in second place and by how much.

## The CVE's
This is likely a partial list, but please send a pull request or contact me below
to include any CVE that is not included below:

| Project / Software | CVE Number | Metasploit |
| ------------------ | ---------- | ---------- |
| bash | [CVE-2014-6277](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-6277) | NA |
| bash | [CVE-2014-6278](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-6278) | [scanner](https://github.com/rapid7/metasploit-framework/blob/master/modules/auxiliary/scanner/http/apache_mod_cgi_bash_env.rb),[exploit1](https://github.com/rapid7/metasploit-framework/blob/master/modules/exploits/multi/http/apache_mod_cgi_bash_env_exec.rb),[exploit2](https://github.com/rapid7/metasploit-framework/blob/master/modules/exploits/multi/http/cups_bash_env_exec.rb) |
| libjpeg | [CVE-2013-6629](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2013-6629) | NA |
| libpng | [CVE-2014-9495](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-9495) | NA |
| BIND | [CVE-2015-5477](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-5477) | NA |
| Xerces-C | [CVE-2015-0252](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-0252) | NA |
| ImageIO | [CVE-2015-5781](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-5781) | NA |
| ImageIO | [CVE-2015-5782](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-5782) | NA |
| libtiff | [CVE-2014-8127](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-8127) | NA |
| libtiff | [CVE-2014-8128](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-8128) | NA |
| libtiff | [CVE-2014-8129](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-8129) | NA |
| firefox | [CVE-2014-1564](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-1564) | NA |
| firefox | [CVE-2014-1580](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-1580) | NA |
| firefox | [CVE-2014-8637](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-8637) | NA |
| flash | [CVE-2015-0329](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-0329) | NA |
| flash | [CVE-2015-0323](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-0323) | NA |
| mutt | [CVE-2014-9116](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-9116) | NA |
| gnutls | [CVE-2014-8564](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-8564) | NA |
| clamav | [CVE-2015-1463](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-1463) | NA |
| X.org | [CVE-2015-1803](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-1803) | NA |
| X.org | [CVE-2015-1803](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-1803) | NA |
| libwmf | [CVE-2015-0848](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-0848) | NA |
| libwmf | [CVE-2015-4695](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-4695) | NA |
| libwmf | [CVE-2015-4696](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-4696) | NA |
| tidy | [CVE-2015-5522](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-5522) | NA |
| tidy | [CVE-2015-5523](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-5523) | NA |
| patch | [CVE-2014-9637](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-9637) | NA |
| openssl | [CVE-2015-1788](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2015-1788) | NA |
| gnutls | [CVE-2014-8564](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2014-8564) | NA |

## Contact
All CVE updates are managed through any of three methods: github issues tracking, email
contact (michael.rash_AT_gmail.com), or reaching me through
Twitter ([@michaelrash](https://twitter.com/michaelrash)).
