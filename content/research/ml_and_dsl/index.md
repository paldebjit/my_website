---
title: Application of ML
summary: " "
#An example of using the in-built project page.
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

#### Application of ML in Pre-Silicon Verification ####
<p align="justify">
The quality of design verification is as good as the verification artifacts. There are multiple such artifacts, including tests, assertions, checker modules. It takes many months to develop such well-crafted artifacts for high-quality verification. In this research, (<a href="/publication/tcad-2020-1" target="_blank">TCAD'20b</a>, <a href="/publication/aspdac-2019" target="_blank">ASP-DAC'19</a>) we applied machine learning for generating assertions automatically for hardware designs and implemented a prototype tool called <a href="http://goldmine.csl.illinois.edu" target="_blank">GoldMine</a>. Assertion generation refers to the automation of the manual, tedious, ad-hoc, and incomplete process of writing assertions. The principle of GoldMine is simple but powerful. We guide machine learning algorithms by statically analyzing the state space of the system. The domain knowledge of the static analysis algorithms and formal verification could be leveraged as an oracular, iterative mechanism to direct the learning process. This interaction between a statistical inductive inference engine and a static analysis engine could be used repeatedly to generate assertions that surpass manual assertions in quality.
</p>

<p align="justify">
One of the key tasks of verification is root causing and debugging. However, root causing and debugging are often performed in an unsystematic and ad hoc way under aggressive time-to-market schedules and incur disproportionate costs. In this research, (<a href="/publication/vlsi-2016" target="_blank">VLSID'16</a>) we extend the GoldMine principle and develop an automatic bug localization technique in RTL. Our technique is based on identifying statistically relevant common symptoms across failing simulation trace through data mining, and mapping these back to the corresponding execution paths in the RTL source code.
</p>

#### Application of ML in Post-Silicon Validation ####
<p align="justify">
Post-silicon validation is a crucial component of contemporary System-on-Chip (SoC) validation and debugging. It is performed in an unsystematic and ad hoc way under aggressive time-to-market schedules. An expensive component of post-silicon validation is application-level use-case validation. In this activity, a validator exercises various target usage scenarios of the system (e.g., for a smartphone, playing videos, or surfing the Web, while receiving a phone call) and monitors for failures (e.g., hangs, crashes, deadlocks, overflows, etc.). However, it is tedious and error-prone to investigate such failure traces containing traces from multiple concurrently executing on-chip components. In this research, (<a href="/publication/dac-2018" target="_blank">DAC'18</a>, <a href="/publication/corr-abs-2021" target="_blank">CoRR'21</a>) we have developed an automatic, scalable, and efficient post-silicon debug and diagnosis solution by applying feature engineering-based machine learning techniques on the failure traces. The idea is to learn the correct and erroneous design behavior automatically from trace data without prior design knowledge. We believe our debugging solution can automate post-silicon debug and diagnosis, where manual debugging is the norm.
</p>

#### Application of ML in Hardware Resiliency ####
<p align="justify">
Progressive technology scaling and lowering operating voltages have made current and future computer systems more susceptible to high-energy particles induced soft errors (i.e., transient hardware faults). Traditionally, soft error estimation approaches primarily focus on fault injection (FI) campaigns and analytical models. Given realistic program contains billions of instructions, FI incurs a long time to achieve statistically significant results. Alternatively, analytical models can identify vulnerable instructions fast but are inaccurate and suffer from scalability. Recently, ML methods are increasingly used to estimate instruction vulnerability. However, each of these methods suffers from high accuracy loss, small training datasets, and requires time-consuming retraining for unseen programs making them in-feasible for realistic program vulnerability estimation. In this research, (<a href="/publication/date-2021" taregt="_blank">DATE'21</a>) we have developed GLAIVE, an inductive graph learning assisted model that is scalable to large programs containing millions of instructions, can quickly and accurately estimate instruction vulnerability, and can be transferred to unseen programs without retraining.
</p>

#### Application of ML in FPGA QoR Estimation ####
<p align="justify">
Modern heterogeneous FPGA architectures incorporate a variety
of hardened blocks, such as DSP blocks and carry blocks, to boost the performance of arithmetic-intensive designs. Since one can configure hardened blocks in different ways, a variety of datapath patterns can be mapped into these blocks. Existing high-level synthesis (HLS) tools, such as Vivado HLS, often fail to capture many such operation mapping patterns, leading to limited resource usage and delay estimation accuracy. In this research, (<a href="/publication/iccad-2020" target="_blank">ICCAD'20</a>) we propose to exploit graph-neural networks (GNN) to learn operation mapping patterns automatically. We apply GNN models that are trained on microbenchmarks directly to realistic designs through inductive learning. Our learned model can effectively infer various valid mapping patterns on both microbenchmarks and realistic designs. Furthermore, we leverage the proposed framework to improve the accuracy of delay estimation in HLS.
</p>

#### Application of ML in Trojan Detection in IP ####
<p align="justify">

</p>


