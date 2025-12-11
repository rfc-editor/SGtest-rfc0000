---
title: SVGs in RFCs
docname: draft-editorial-rswg-svgsinrfcs-04
venue:
  group: RSWG
  type: Editorial Stream Working Group
  mail: rswg@rfc-editor.org
  arch: https://mailarchive.ietf.org/arch/browse/rswg/
  github: "alexisannerossi/id-svgsinrfcs"
  latest: "https://github.com/alexisannerossi/id-svgsinrfcs/blob/main/svgsinrfcs.md"
stand_alone: true
v: 3
obsoletes: 7996
ipr: trust200902
kw: Internet-Draft
cat: info
submissionType: editorial
keyword:
 - SVG
author:
  -
    ins: A. Rossi
    name: Alexis Rossi
    organization: RFC Series Consulting Editor
    email: rsce@rfc-editor.org
  -
    ins: N. Brownlee
    name: Nevil Brownlee
    organization:
    email: nevil.brownlee@gmail.com
  -
    ins: J. Mahoney
    name: Jean Mahoney
    organization: RFC Production Center
    email: jmahoney@staff.rfc-editor.org
  -
    ins: M. Thomson
    name: Martin Thomson
    organization:
    email: mt@lowentropy.net

normative:


informative:
  RFC7996:
  SVG:
    author:
      org: W3C
    title: Scalable Vector Graphics
    target: https://www.w3.org/TR/SVG/
  WAI:
    author:
      org: W3C
    title: W3C Accessibility Standards Overview
    target: https://www.w3.org/WAI/standards-guidelines/

--- abstract

This document sets policy for the inclusion of SVGs in the definitive versions of RFCs and relevant publication formats. It contains policy requirements from RFC 7996 and removes all requirements related to using a specific SVG profile or specific implementation code. It also makes the RFC Publication Center (RPC) responsible for implementation decisions regarding SVGs.

--- middle

# Introduction

This document sets policy for the inclusion of SVGs (Scalable Vector Graphics) in the definitive versions of RFCs and relevant publication formats. It contains policy requirements taken from {{RFC7996}} and removes all requirements related to using a specific SVG profile or specific implementation code.

SVG has been developed by W3C, the World Wide Web Consortium {{SVG}}.

The RFC Publication Center (RPC) is responsible for making SVG tooling and implementation decisions. They may want to use the content of {{RFC7996}} as a starting point for those decisions, but they are not bound by {{RFC7996}} and they may change elements of the implementation as needed to support the RFC authoring community as long as those changes are aligned with the policy requirements in this document.

# Policy Requirements

SVG tooling and implementation decisions are made or overseen by the RPC, and must adhere to the policy requirements in this document.

* SVGs may be included in RFCs to help explain a concept more clearly, but should not be the only representation of that concept. A good faith effort should be made to assure that descriptions of concepts - which might include protocols, formats, or system architectures - are fully represented in the text of the RFC. At minimum, SVGs should be consistent with the text.
* SVGs must not include animation or interactive features. SVGs should include only limited reactive design elements (scaling, dark/light mode, and perhaps minor adjustments to allow for variations in display technology). The intent of this is to ensure that the diagram's meaning is not altered.
* Images and diagrams in RFCs should be successfully rendered and understood by the widest audience possible. To that end, the RPC may prohibit the use of SVG features that are known to lack support on common devices, that do not render on small or low-resolution screens, or that could make diagrams less comprehensible for any significant readership. This includes:
  * SVGs must not contain pointers to external resources.
  * SVGs must not contain executable script.
  * SVGs should be as accessible as possible to people with visual disabilities, including those who have color blindness, those who need to scale or change fonts, and those who use screen reading software. The RPC will refer to the W3C Accessibility Guidelines {{WAI}} when making decisions regarding accessibility.
* Authors may include multiple versions of images or diagrams in rfcxml.  Publication formats should present the versions best suited to each format.  In many cases, that will be an SVG.
* SVG vocabulary and implementation may change over time. Changes are not required to remain backwards-compatible, although maintaining compatibility where possible is encouraged.

The RPC is authorized to place constraints on SVG usage in RFCs for both technical and editorial reasons
in order to ensure that published RFCs meet the above policy
and to provide consistency across the RFC series.
The RPC must document the acceptable usage of SVGs, and all changes to tooling or implementation decisions must be widely communicated to the RFC author community using mailing lists or other means.

# Implementation Guidance

The RPC is expected to solicit community input before making decisions and to publicly explain their reasoning.

Documentation produced by the RPC should describe what technical and editorial constraints apply to SVGs
and provide RFC authors with guidance on how to produce diagrams that meet these constraints.

The RPC's implementation should strive to allow SVGs produced by widely used drawing tools.
Where possible, implementation decisions should focus on specifying what is disallowed, rather than attempting to specify exactly what is allowed.

The RPC should periodically review and revise their practices.

# Security Considerations

This document has no security considerations.


# IANA Considerations

This document has no IANA actions.


--- back
