# bounty-targets
Bug Bounty Program Target Domain List
=====================================

This is a hand-crafted list of domain names that were searched out by hand after
referring to the bug bounty web application portals operated by the commercial
entities [HackerOne](https://hackerone.com) and [BugCrowd](https://bugcrowd.com).

When a wildcard is encountered in the target list such as "*.host.dom" various
DNS subdomain enumeration techniques are used to expand it into multiple subdomain
entries. DNS records which correspond to identical IP addresses are avoided; this 
includes both singular and round robin resources.  

Use of the "www" host for any domain is also prevented when possible. There are 
several "www" hostnames included in the list, but only because it was impossible
to achieve full IP address coverage without it.  Basically, this is an 
exceptional case that usually only happens when both "host.dom" and "www.host.dom" 
resolve to different numeric addresses and no other subdomain resolves to the 
address for "www.host.dom". The idea behind all this is that the "www." string can
be programatically prepended to all host names since there may be host names 
formatted like this: "www.sub.host.dom". 
