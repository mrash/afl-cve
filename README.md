# afl-cve
A collection of vulnerabilities discovered by the AFL fuzzer (afl-fuzz)

## Introduction
`afl-cve` is a collection of known vulnerabilities that can be attributed to the
AFL fuzzer [afl-fuzz](http://lcamtuf.coredump.cx/afl/). All vulnerabilities in
this list either already have a CVE assigned, or a CVE has been requested from a
[CVE Numbering Authority](https://cve.mitre.org/cve/cna.html#participating_cnas).

## Why is This Necessary?
Because CVE descriptions are not generally being written to mention AFL as the
tool that enabled particular bugs to be found. This is primarily due to the fact
that CVE descriptions do not require the underlying discovery tool or technique
to be disclosed. Nor should it necessarily - many security researchers have their
own methods, and it might hurt the vulnerability reporting process if researchers
were required to disclose such techniques. Further, most security researchers do
acknowledge AFL in some form (twitter post, afl-users mailing list, etc.) when
it finds a bug, and `afl-cve` attempts to track this more formally.

Also, the `afl-fuzz` website does a great job of tracking *bugs* found by AFL.
But not all bugs get assigned a CVE, and hence there is a need to specifically
track those that do because having a CVE is at least a tacit acknowledgment of
potential exploitability. So, the bugs AFL has found are therefore frequently
*important* for anyone concerned about security.

## Fuzzing Revisited
AFL has discovered a huge number of bugs in all sorts of projects from compilers
to image processing libraries. AFL seems to be succeeding where other fuzzers have
failed, or at least not been generally embraced or made operational by the security
community for whatever reason. Another way to see this is to try to determine which
fuzzer has the most CVE's. Is there a different fuzzing project that comes close to
AFL in terms of the number of vulnerabilities found? It would be instructive to see
which fuzzer comes in second place and by how much.

## The Vulnerabilities
This is likely a partial list, but please send a pull request or contact me below
to include any CVE that is not included below:

| Project / Software | CVE Number | Metasploit |
| ------------------ | ---------- | ---------- |
| bash | [CVE-2014-6277](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-6277) | NA |
| bash | [CVE-2014-6278](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-6278) | [scanner](https://github.com/rapid7/metasploit-framework/blob/master/modules/auxiliary/scanner/http/apache_mod_cgi_bash_env.rb),[exploit1](https://github.com/rapid7/metasploit-framework/blob/master/modules/exploits/multi/http/apache_mod_cgi_bash_env_exec.rb),[exploit2](https://github.com/rapid7/metasploit-framework/blob/master/modules/exploits/multi/http/cups_bash_env_exec.rb) |
| libjpeg | [CVE-2013-6629](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2013-6629) | NA |
| libpng | [CVE-2014-9495](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9495) | NA |
| BIND | [CVE-2015-5477](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5477) | NA |
| BIND | [CVE-2015-5722](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5722) | NA |
| BIND | [CVE-2015-5986](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5986) | NA |
| Xerces-C | [CVE-2015-0252](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0252) | NA |
| Xerces-C | [CVE-2016-0729](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-0729) | NA |
| Xerces-C | [CVE-2016-4463](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4463) | NA |
| ImageIO | [CVE-2015-5781](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5781) | NA |
| ImageIO | [CVE-2015-5782](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5782) | NA |
| libtiff | [CVE-2014-8127](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8127) | NA |
| libtiff | [CVE-2014-8128](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8128) | NA |
| libtiff | [CVE-2014-8129](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8129) | NA |
| libtiff | [CVE-2014-8130](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8130), [Debian Advisory](https://security-tracker.debian.org/tracker/CVE-2014-8130) | NA |
| firefox | [CVE-2014-1564](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-1564) | NA |
| firefox | [CVE-2014-1580](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-1580) | NA |
| firefox | [CVE-2014-8637](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8637) | NA |
| flash | [CVE-2015-0329](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0329) | NA |
| flash | [CVE-2015-0323](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0323) | NA |
| mutt | [CVE-2014-9116](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9116) | NA |
| clamav | [CVE-2015-1463](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1463) | NA |
| clamav | [CVE-2015-2170](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2170) | NA |
| clamav | [CVE-2015-2221](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2221) | NA |
| clamav | [CVE-2015-2222](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2222) | NA |
| X.org | [CVE-2015-1802](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1802) | NA |
| X.org | [CVE-2015-1803](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1803) | NA |
| X.org | [CVE-2015-1804](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1804) | NA |
| libwmf | [CVE-2015-0848](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0848) | NA |
| libwmf | [CVE-2015-4695](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4695) | NA |
| libwmf | [CVE-2015-4696](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4696) | NA |
| tidy | [CVE-2015-5522](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5522) | NA |
| tidy | [CVE-2015-5523](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5523) | NA |
| patch | [CVE-2014-9637](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9637) | NA |
| openssl | [CVE-2015-1788](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1788) | NA |
| openssl | [CVE-2015-0288](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0288) | NA |
| openssl | [CVE-2015-3193](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3193) | NA |
| gnutls | [CVE-2014-8564](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8564) | NA |
| libmspack | [CVE-2014-9556](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9556) | NA |
| libmspack | [CVE-2014-9732](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9732) | NA |
| libmspack | [CVE-2015-4467](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4467) | NA |
| libmspack | [CVE-2015-4468](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4468) | NA |
| libmspack | [CVE-2015-4469](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4469) | NA |
| libmspack | [CVE-2015-4470](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4470) | NA |
| libmspack | [CVE-2015-4471](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4471) | NA |
| libmspack | [CVE-2015-4472](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4472) | NA |
| Qt | [CVE-2015-1858](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1858) | NA |
| Qt | [CVE-2015-1859](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1859) | NA |
| Qt | [CVE-2015-1860](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1860) | NA |
| unace | [CVE-2015-2063](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2063) | NA |
| ARJ | [CVE-2015-2782](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2782) | NA |
| t1utils | [CVE-2015-3905](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3905) | NA |
| Android (libstagefright) | [CVE-2015-1538](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1538) | NA |
| Android (libstagefright) | [CVE-2015-1539](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1539) | NA |
| Android (libstagefright) | [CVE-2015-3824](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3824) | NA |
| Android (libstagefright) | [CVE-2015-3826](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3826) | NA |
| Android (libstagefright) | [CVE-2015-3827](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3827) | NA |
| Android (libstagefright) | [CVE-2015-3828](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3828) | NA |
| Android (libstagefright) | [CVE-2015-3829](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3829) | NA |
| antiword | [CVE-2014-8123](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8123) | NA |
| ArduinoJson | [CVE-2015-4590](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4590) | NA |
| CUPS | [CVE-2014-9679](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9679) | NA |
| Cap'n Proto | [CVE-2015-2310](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2310) | NA |
| Cap'n Proto | [CVE-2015-2312](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2312) | NA |
| libtasn1 | [CVE-2015-3622](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3622) | NA |
| libtasn1 | [CVE-2016-4008](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4008) | NA |
| UnRTF | [CVE-2014-9274](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9275) | NA |
| UnRTF | [CVE-2014-9275](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9275) | NA |
| unzip | [CVE-2015-1315](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1315), [Debian Advisory](https://security-tracker.debian.org/tracker/CVE-2015-1315) | NA |
| unzoo | [CVE-2015-1845](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1845), [Red Hat Advisory](https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2015-1845) | NA |
| unzoo | [CVE-2015-1846](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1845), [Red Hat Advisory](https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2015-1846) | NA |
| Ghostscript | [CVE-2015-3228](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1845), [Red Hat Advisory](https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2015-3228) | NA |
| GnuPG | [CVE-2015-1606](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1606) | NA |
| GnuPG | [CVE-2015-1607](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1607) | NA |
| libksba | [CVE-2014-9087](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9087) | NA |
| Microsoft Windows | [CVE-2014-6355](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-6355) | NA |
| Microsoft Windows | [CVE-2015-0061](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0061) | NA |
| NTP | [CVE-2015-7855](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-7855) | NA |
| NTP | [CVE-2016-7434](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-7434) | NA |
| libxml2 | [CVE-2015-7941](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-7941) | NA |
| libxml2 | [CVE-2015-8035](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8035) | NA |
| libxml2 | [CVE-2015-8241](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8241) | NA |
| libxml2 | [CVE-2015-8242](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8242) | NA |
| libxml2 | [CVE-2015-8317](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8317) | NA |
| libxml2 | [CVE-2016-4658](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4658) | NA |
| libxml2 | [CVE-2016-5131](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5131) | NA |
| PuTTY | [CVE-2015-5309](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5309) | NA |
| PowerDNS | [CVE-2015-5311](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5311) | NA |
| PHP | [CVE-2015-0232](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0232) | NA |
| pngcrush | [CVE-2015-2158](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2158) | NA |
| dpkg | [CVE-2015-0860](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0860) | NA |
| PCRE | [CVE-2015-8380](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8380) | NA |
| LHA for UNIX | [CVE-2016-1925](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-1925) | NA |
| libXfont | [CVE-2015-1803](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1803) | NA |
| libXfont | [CVE-2015-1804](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1804) | NA |
| imlib2 | [CVE-2014-9771](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9771) | NA |
| imlib2 | [CVE-2016-3994](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-3994) | NA |
| jq | [CVE-2015-8863](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8863) | NA |
| Botan | [CVE-2015-5726](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5726) | NA |
| Botan | [CVE-2016-2194](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-2194) | NA |
| Botan | [CVE-2016-2195](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-2195) | NA |
| Botan | [CVE-2016-2196](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-2196) | NA |
| dosfstools | [CVE-2015-8872](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8872) | NA |
| dosfstools | [CVE-2016-4804](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4804) | NA |
| Expat | [CVE-2016-0718](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-0718) | NA |
| libarchive | [CVE-2015-8915](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8915) | NA |
| libarchive | [CVE-2015-8916](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8916) | NA |
| libarchive | [CVE-2015-8917](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8917) | NA |
| libarchive | [CVE-2015-8918](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8918) | NA |
| libarchive | [CVE-2015-8919](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8919) | NA |
| libarchive | [CVE-2015-8920](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8920) | NA |
| libarchive | [CVE-2015-8928](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8928) | NA |
| libarchive | [CVE-2015-8921](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8921) | NA |
| libarchive | [CVE-2015-8922](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8922) | NA |
| libarchive | [CVE-2015-8923](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8923) | NA |
| libarchive | [CVE-2015-8924](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8924) | NA |
| libarchive | [CVE-2015-8925](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8925) | NA |
| libarchive | [CVE-2015-8926](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8926) | NA |
| libarchive | [CVE-2015-8927](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8927) | NA |
| libarchive | [CVE-2015-8929](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8929) | NA |
| libarchive | [CVE-2015-8930](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8930) | NA |
| libarchive | [CVE-2015-8931](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8931) | NA |
| libarchive | [CVE-2015-8932](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8932) | NA |
| libarchive | [CVE-2015-8933](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8933) | NA |
| libarchive | [CVE-2015-8934](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8934) | NA |
| libarchive | [CVE-2016-5844](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5844) | NA |
| libarchive | [CVE-2016-1541](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-1541) | NA |
| libarchive | [CVE-2016-8687](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8687) | NA |
| libarchive | [CVE-2016-8688](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8688) | NA |
| libarchive | [CVE-2016-8689](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8689) | NA |
| libiberty | [CVE-2016-2226](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-2226) | NA |
| libiberty | [CVE-2016-4487](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4487) | NA |
| libiberty | [CVE-2016-4488](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4488) | NA |
| libiberty | [CVE-2016-4489](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4489) | NA |
| libiberty | [CVE-2016-4490](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4490) | NA |
| libiberty | [CVE-2016-4491](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4491) | NA |
| libiberty | [CVE-2016-4492](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4492) | NA |
| libiberty | [CVE-2016-4493](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4493) | NA |
| libiberty | [CVE-2016-6131](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6131) | NA |
| OpenBSD | [CVE-2016-6239](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6239) | NA |
| OpenBSD | [CVE-2016-6240](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6240) | NA |
| OpenBSD | [CVE-2016-6241](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6241) | NA |
| OpenBSD | [CVE-2016-6242](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6242) | NA |
| OpenBSD | [CVE-2016-6243](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6243) | NA |
| OpenBSD | [CVE-2016-6244](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6244) | NA |
| OpenBSD | [CVE-2016-6245](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6245) | NA |
| OpenBSD | [CVE-2016-6246](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6246) | NA |
| OpenBSD | [CVE-2016-6247](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6247) | NA |
| collectd | [CVE-2016-6254](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6254) | NA |
| libidn | [CVE-2016-6261](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6261) | NA |
| libidn | [CVE-2016-6263](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6263) | NA |
| w3m | [CVE-2016-9422](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9422) | NA |
| w3m | [CVE-2016-9423](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9423) | NA |
| w3m | [CVE-2016-9424](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9424) | NA |
| w3m | [CVE-2016-9425](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9425) | NA |
| w3m | [CVE-2016-9426](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9426) | NA |
| w3m | [CVE-2016-9427](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9427) | NA |
| w3m | [CVE-2016-9428](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9428) | NA |
| w3m | [CVE-2016-9429](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9429) | NA |
| w3m | [CVE-2016-9430](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9430) | NA |
| w3m | [CVE-2016-9431](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9431) | NA |
| w3m | [CVE-2016-9432](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9432) | NA |
| w3m | [CVE-2016-9433](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9433) | NA |
| w3m | [CVE-2016-9434](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9434) | NA |
| w3m | [CVE-2016-9435](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9435) | NA |
| w3m | [CVE-2016-9436](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9436) | NA |
| w3m | [CVE-2016-9437](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9437) | NA |
| w3m | [CVE-2016-9438](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9438) | NA |
| w3m | [CVE-2016-9439](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9439) | NA |
| w3m | [CVE-2016-9440](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9440) | NA |
| w3m | [CVE-2016-9441](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9441) | NA |
| w3m | [CVE-2016-9442](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9442) | NA |
| w3m | [CVE-2016-9443](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9443) | NA |
| w3m | [CVE-2016-9622](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9622) | NA |
| w3m | [CVE-2016-9623](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9623) | NA |
| w3m | [CVE-2016-9624](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9624) | NA |
| w3m | [CVE-2016-9625](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9625) | NA |
| w3m | [CVE-2016-9626](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9626) | NA |
| w3m | [CVE-2016-9627](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9627) | NA |
| w3m | [CVE-2016-9628](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9628) | NA |
| w3m | [CVE-2016-9629](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9629) | NA |
| w3m | [CVE-2016-9630](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9630) | NA |
| w3m | [CVE-2016-9631](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9631) | NA |
| w3m | [CVE-2016-9632](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9632) | NA |
| w3m | [CVE-2016-9633](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9633) | NA |
| libical | [CVE-2016-5823](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5823) | NA |
| libical | [CVE-2016-5824](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5824) | NA |
| libical | [CVE-2016-5825](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5825) | NA |
| libical | [CVE-2016-5826](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5826) | NA |
| libical | [CVE-2016-5827](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-5827) | NA |
| GNU ed | [CVE-2017-5357](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5357) | NA |
| Irssi | [CVE-2017-5356](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5356) | NA |
| JasPer | [CVE-2016-8690](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8690) | NA |
| JasPer | [CVE-2016-8691](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8691) | NA |
| JasPer | [CVE-2016-8692](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8692) | NA |
| JasPer | [CVE-2016-8693](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8693) | NA |
| JasPer | [CVE-2016-8884](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8884) | NA |
| JasPer | [CVE-2016-8885](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8885) | NA |
| JasPer | [CVE-2016-8886](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8886) | NA |
| JasPer | [CVE-2016-8887](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8887) | NA |
| JasPer | [CVE-2016-9387](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9387) | NA |
| JasPer | [CVE-2016-9388](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9388) | NA |
| JasPer | [CVE-2016-9389](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9389) | NA |
| JasPer | [CVE-2016-9390](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9390) | NA |
| JasPer | [CVE-2016-9391](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9391) | NA |
| JasPer | [CVE-2016-9392](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9392) | NA |
| JasPer | [CVE-2016-9393](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9393) | NA |
| JasPer | [CVE-2016-9394](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9394) | NA |
| JasPer | [CVE-2016-9395](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9395) | NA |
| JasPer | [CVE-2016-9396](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9396) | NA |
| JasPer | [CVE-2016-9397](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9397) | NA |
| JasPer | [CVE-2016-9398](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9398) | NA |
| JasPer | [CVE-2016-9399](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9399) | NA |
| JasPer | [CVE-2016-9557](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9557) | NA |
| JasPer | [CVE-2016-9560](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9560) | NA |
| JasPer | [CVE-2017-5502](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5502) | NA |
| JasPer | [CVE-2017-5501](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5501) | NA |
| JasPer | [CVE-2017-5500](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5500) | NA |
| JasPer | [CVE-2017-5499](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5499) | NA |
| JasPer | [CVE-2017-5498](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5498) | NA |
| JasPer | [CVE-2017-5503](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5503) | NA |
| JasPer | [CVE-2017-5504](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5504) | NA |
| JasPer | [CVE-2017-5505](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5505) | NA |
| Adobe Reader DC | [CVE-2016-4198](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-4198) | NA |
| Adobe Reader DC | [CVE-2016-6969](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6969) | NA |
| Adobe Reader DC | [CVE-2016-6978](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-6978) | NA |
| OpenCV | [CVE-2016-1516](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-1516) | NA |
| OpenCV | [CVE-2016-1517](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-1517) | NA |
| WavPack | [CVE-2016-10169](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-10169) | NA |
| WavPack | [CVE-2016-10170](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-10170) | NA |
| WavPack | [CVE-2016-10171](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-10171) | NA |
| WavPack | [CVE-2016-10172](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-10172) | NA |
| mp3splt | [CVE-2017-5665](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5665) | NA |
| mp3splt | [CVE-2017-5666](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-5666) | NA |
| ImageMagick | [CVE-2016-8677](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8677) | NA |
| ImageMagick | [CVE-2016-8678](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8678) | NA |
| ImageMagick | [CVE-2016-8862](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8862) | NA |
| ImageMagick | [CVE-2016-8866](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8866) | NA |
| ImageMagick | [CVE-2016-9556](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9556) | NA |
| ImageMagick | [CVE-2016-9559](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-9559) | NA |
| GraphicsMagick | [CVE-2016-7449](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-7449) | NA |
| GraphicsMagick | [CVE-2016-8682](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8682) | NA |
| GraphicsMagick | [CVE-2016-8683](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8683) | NA |
| GraphicsMagick | [CVE-2016-8684](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-8684) | NA |

## Contact
All updates to the above list of CVE's are managed through any of three methods:
github issues tracking, email contact (michael.rash_AT_gmail.com), or reaching me
through Twitter ([@michaelrash](https://twitter.com/michaelrash)).
