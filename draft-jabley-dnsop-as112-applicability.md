---
title: "Applicability Statement for the AS112 Project"
abbrev: "AS112 Applicability Statement"
category: info

docname: draft-jabley-dnsop-as112-applicability-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: "Operations and Management"
workgroup: "Domain Name System Operations"
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
  group: "Domain Name System Operations"
  type: "Working Group"
  mail: "dnsop@ietf.org"
  github: "ableyjoe/draft-jabley-as112-applicability"

author:
 -
    fullname: Joe Abley
    organization: Cloudflare
    email: jabley@cloudflare.com
    city: Amsterdam
    country: Netherlands
 -
    ins: W. Kumari
    name: Warren Kumari
    org: Google, Inc.
    street: 1600 Amphitheatre Parkway
    city: Mountain View
    state: CA
    code: 94043
    country: United States of America
    phone: +1 571 748 4373
    email: warren@kumari.net

normative:

informative:


--- abstract

The AS112 Project provides infrastructure that is used as a target for
DNS queries that it is not possible to answer in a useful way, such as
queries that relate to a private network that are sent to a public
server. From time to time IETF protocols specify use of the AS112
Project. This document provides an Applicability Statement for the
AS112 Project that aims to provide guidance for how and when the
AS112 Project should be used.


--- middle

# Introduction

Well, how about this?


# Terminology

{::boilerplate bcp14-tagged}

This document uses terminology related to the Domain Name System as
described in {{?RFC8499}}.

# Security Considerations

Make reference to the existing security guidance.

Provide guidance on when sinking queries with the AS112 project is appropriate, and when it is not. For example, note that causing queries to be redirected to AS112 servers can present privacy risks.

Note that protocols that intend to cause queries to be sent to AS112 servers should do so carefully, mindful that excessive traffic being sent to any destination can have the effect of denying service to both AS112 infrastructure and intermediate networks and systems.


# IANA Considerations

Give IANA directions about how to respond to requests from other documents that relate to AS112.

Note that since there are known cases of protocols that specify that queries for particular names in the ARPA domain be redirected to AS112 infrastructure, the IANA should start the process of becoming equipped to provision DNAME RRSets in the ARPA zone. Perhaps clarify that the provisioning process involves ancilliary systems and processes and is not simply a matter of support for the DNAME resource record type in the servers that serve the ARPA zone.

--- back

# Acknowledgments
{:numbered="false"}

These people helped. Yes.
