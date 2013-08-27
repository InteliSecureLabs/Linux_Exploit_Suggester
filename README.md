Linux_Exploit_Suggester
=======================

Linux Exploit Suggester; based on operating system release number.

This program run without arguments will perform a 'uname -r' to grab the Linux Operating Systems release version, 
and return a suggestive list of possible exploits.  Nothing fancy, so a patched/back-ported patch may fool this script.

Additionally possible to provide '-k' flag to manually enter the Kernel Version/Operating System Release Version.

This script has been extremely useful on site and in exams.  Now Open-sourced under GPLv2.

Sample Output
==============
<pre>
$ perl ./Linux_Exploit_Suggester.pl -k 3.0.0

Kernel local: 3.0.0

Possible Exploits:
[+] semtex
   CVE-2013-2094
   Source: www.exploit-db.com/download/25444/‎
[+] memodipper
   CVE-2012-0056
   Source: http://www.exploit-db.com/exploits/18411/
[+] perf_swevent
   CVE-2013-2094
   Source: http://www.exploit-db.com/download/26131
</pre>

<pre>
$ perl ./Linux_Exploit_Suggester.pl -k 2.6.28

Kernel local: 2.6.28

Possible Exploits:
[+] sock_sendpage2
   Alt: proto_ops    CVE-2009-2692
   Source: http://www.exploit-db.com/exploits/9436
[+] half_nelson3
   Alt: econet    CVE-2010-4073
   Source: http://www.exploit-db.com/exploits/17787/
[+] reiserfs
   CVE-2010-1146
   Source: http://www.exploit-db.com/exploits/12130/
[+] pktcdvd
   CVE-2010-3437
   Source: http://www.exploit-db.com/exploits/15150/
[+] american-sign-language
   CVE-2010-4347
   Source: http://www.securityfocus.com/bid/45408/
[+] half_nelson
   Alt: econet    CVE-2010-3848
   Source: http://www.exploit-db.com/exploits/6851
[+] udev
   Alt: udev &lt;1.4.1    CVE-2009-1185
   Source: http://www.exploit-db.com/exploits/8478
[+] do_pages_move
   Alt: sieve    CVE-2010-0415
   Source: Spenders Enlightenment
[+] pipe.c_32bit
   CVE-2009-3547
   Source: http://www.securityfocus.com/data/vulnerabilities/exploits/36901-1.c
[+] exit_notify
   Source: http://www.exploit-db.com/exploits/8369
[+] can_bcm
   CVE-2010-2959
   Source: http://www.exploit-db.com/exploits/14814/
[+] ptrace_kmod2
   Alt: ia32syscall,robert_you_suck    CVE-2010-3301
   Source: http://www.exploit-db.com/exploits/15023/
[+] half_nelson1
   Alt: econet    CVE-2010-3848
   Source: http://www.exploit-db.com/exploits/17787/
[+] half_nelson2
   Alt: econet    CVE-2010-3850
   Source: http://www.exploit-db.com/exploits/17787/
[+] sock_sendpage
   Alt: wunderbar_emporium    CVE-2009-2692
   Source: http://www.exploit-db.com/exploits/9435
[+] video4linux
   CVE-2010-3081
   Source: http://www.exploit-db.com/exploits/15024/
</pre>
