---
title: Security Analysis
summary: " "
#Research related to hardware security asset protection
#tags:
#- Deep Learning
date: 2021-09-15

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: 
#Photo by rawpixel on Unsplash
  focal_point: Smart

links:
#- icon: twitter
#  icon_pack: fab
#  name: Follow
#  url: https://twitter.com/georgecushen
#url_code: ""
#url_pdf: ""
#url_slides: ""
#url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example
---

#### Trojan Detection in Third-Party IP ####
<p align="justify">
Most modern microelectronic systems are designed through
a System-on-Chip (SoC) architecture, which realizes system
functionality within a single substrate by integration and
coordination of pre-designed hardware blocks (referred to as
``Intellectual Properties'' or ``IP''s). In current practice, the
IPs are procured from a complex, globally distributed supply
chain of third-party IP (3PIP) vendors distributed across the globe. However, the global complex supply chains involved in 3PIP development and delivery make it difficult to ensure the quality and trustworthiness of 3PIPs. A key problem is the vulnerability of these IPs to hardware Trojans, i.e., malicious circuitry intended to subvert the security and integrity of the system. In this ongoing research, we are developing a comprehensive Trojan detection framework based on formal methods for certification of 3PIPs against Trojans. Our approach is flexible, e.g., the
same methodology can be used to detect a spectrum of Trojans
in arbitrary 3PIPs. Our approach works on hardware designs at both
RTL and gate-level netlists enabling early trust verification of
procured 3PIPs before layout and synthesis. A key feature of
our methodology is quantifiable assurance, i.e., if our methodology does
not detect a Trojan, it provides a mathematical certification
stipulating the absence of the Trojan. Consequently, the approach 
enables an SoC integration team to use 3PIPs procured
from an untrusted third-party vendor with confidence that it
does not contain malicious circuitry.
</p>

#### Automatic Generation of Security Assertions ####
<p align="justify">
Modern SoCs contain numerous IPs that participate in complex operations, communications, and co-ordinations with each other to deliver the expected functionality. Various security assets often govern all these features that worth protecting from adversaries. Due to feature diversity, customization, and convoluted interactions among hardware IPs, the SoC can suffer from various security vulnerabilities that allow an adversary to perform unauthorized access, execute malicious modifications, or/and influence the confidentiality and availability of the security assets in the field. The increasing SoC design complexity and shrinking time-to-market make it more challenging to ensure security within the limited verification and solution scope. In this ongoing research, we are developing a comprehensive automatic security assertion generation framework for RTL on top of <a href="http://goldmine.csl.illinois.edu" target="_blank">GoldMine</a> to formally describe the design's expected behavior in the context of protecting security assets. Our objective is twofold -- to automatically identify various security assets in the design automatically based on the design and user-specified asset list and to use the gathered knowledge about security assets to generate useful security assertions. In this process we use a rule-based inferencing system to automatically prune portions of the design that are irrelevant in the security context, thereby constraining the assertion miner's search space. This approach can aid security verification by providing a comprehensive list of security properties which is otherwise a daunting task to develop.
</p>