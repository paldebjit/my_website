---
title: Verification and Reliability
summary: " "
#Research related to hardware verification and hardware reliability
#tags:
#- Deep Learning
date: 2021-08-01

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: ""
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

#### System-on-Chip (SoC) Validation ####
System-on-Chips (SoCs) constitutes the primary backbone of modern embedded computing devices including many safety-critical applications e.g., autonomous vehicles, health care systems. The presence of any undetected bugs in these systems would have aberrant cost both in terms of safety and reliability and can cause loss of property or life.  Hence, SoC validation is a crucial task to ensure the functional correctness of an SoC. The sheer size, presence of hundreds of concurrently executing heterogeneous IPs, vertical integration of SoC components e.g., hardware/firmware/software to realize multiple functionality, and application-level relevance of components present a new spectrum of validation challenges that have rendered the traditional microprocessor validation paradigm moot in the context of SoC validation. The challenges include observability enhancement and debug and diagnosis under the constraint of vertical integrations, identifying high-quality verification artifacts among others. In industrial practice, SoC validation is a manual, unsystematic, and ad hoc process that heavily relies on the expertise and the creativity of the validator. Consequently, there is an urgent need to develop scalable and efficient algorithms of industrial relevance to address this massive ongoing challenge of SoC validation.

In my research, we made contributions to both post-silicon and pre-silicon validation of SoCs, with highly impactful contributions to next-generation post-silicon SoC validation. We use top-down analysis, a higher level of abstraction, and application relevance as the key ideas to automate post-silicon observability enhancement for industrial scale SoCs. We scaled observability to designs that are more than 300$\times$ the size of designs that have been presented in the academic literature so far. Our observability enhancement solution can be applied at the netlist-level, behavioral level ([ICCAD'15](/publication/iccad-2015), [TCAD'20a](/publication/tcad-2020-2)), and at the system-wide application level ([DAC'18](/publication/dac-2018)) to select high-quality signals that are most beneficial for post-silicon debug and diagnosis. We apply a feature engineering based machine learning technique on the observed signal data to develop an automatic, scalable, and efficient post-silicon debug and diagnosis solution. The key idea is to learn the correct and erroneous design behavior automatically from trace data without prior design knowledge. We believe our debugging solution can automate post-silicon debug and diagnosis, where manual debugging is the norm. 

The quality of SoC verification and validation heavily depends on the quality of verification artifacts e.g., assertions. To automate and expedite identification of high-functional coverage assertions that are useful for regression analysis, localization, etc., we have also developed a comprehensive ranking scheme for assertions ([TCAD'20b](/publication/tcad-2020-1/), [ASP-DAC'19](/publication/aspdac-2019/), [VLSID'16](/publication/vlsi-2016/)). The key idea is to identify assertions that capture important design behaviors by analyzing the design source code.

Our SoC validation solutions are scalable and efficient. We consistently show orders of magnitude speedup improvements over the state-of-the-art while objectively improving quality of results. We have shown that going forward application-level analysis is the key to scale post-silicon validation to industrial scale SoCs. Our proposed validation solutions can plug into the existing industrial validation process to introduce automation in the current unsystematic, ad hoc, manual settings with multiple order of magnitudes of benefit.

#### Hardware Reliability Estimation ####
Due to the continuous technology scaling and lowering of operating voltages, modern computer systems are highly vulnerable to soft errors induced by the high-energy particles. Soft errors can corrupt program outputs leading to silent data corruption or a Crash. To protect computer systems against such failures, architects need to precisely and quickly identify vulnerable program instructions that need to be protected. Traditional techniques for program reliability estimation either use expensive and time-consuming fault injection or inaccurate analytical models to identify the program instructions that need to be protected against soft errors. In this research ([DATE'21](/publication/date-2021/)), we present a graph learning-assisted model for fast, accurate, and transferable soft-error induced instruction vulnerability estimation. We leverage a synergy between static analysis and data-driven statistical reasoning to automatically learn signatures of instruction-level vulnerabilities and their propagation to program outputs using a fine-grain error propagation information from the bit-level program graphs of a set of realistic benchmarks. 
