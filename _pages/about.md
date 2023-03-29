---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hi! I am a third year PhD student at Robotics Institute of Carnegie Mellon University, advised by Prof. [Deva Ramanan](https://www.cs.cmu.edu/~deva/). I did my undergrad in Computer Science and Maths at Cornell University and served as college symbol bearer (top 5 of the college). My current research focuses on computer vision and learning, especially robustness to distribution shifts (continual/lifelong vision) and data-efficient adaptation with multi-modalities.

<!-- My research interest includes neural machine translation and computer vision. I have published more than 100 papers at the top international AI conferences with total <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=DhtAFkwAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>). -->

# 🔥 News
- *2023.02*: [Multimodality Helps Unimodality: Cross-Modal Few-Shot Learning with Multimodal Models](https://linzhiqiu.github.io/papers/cross_modal/) accepted by CVPR'23.
- *2022.09*: [LECO: Continual Learning with Evolving Class Ontologies](https://linzhiqiu.github.io/papers/leco/) was accepted by NeurIPS'22. Check out the [website](https://linzhiqiu.github.io/papers/leco/) and [slides](/papers/leco/LECO.pdf) for a quick overview!
- *2022.06*: [The 1st CLEAR Challenge](http://clear-benchmark.github.io) was hosted on CVPR'22 [2nd Workshop on Open World Vision](https://www.cs.cmu.edu/~shuk/vplow.html). Check out the [slides](/papers/clear/clear_cvpr.pdf) for a quick overview!
- *2021.09*: [The CLEAR Benchmark: Continual LEArning on Real-World Imagery](http://clear-benchmark.github.io) accepted by NeurIPS'21 (Datasets and Benchmarks Track). 
- *2020.06*: Best Paper Nomination at CVPR'20 for [Visual Chirality](https://linzhiqiu.github.io/papers/chirality/)!
<!-- - *2020.06*: &nbsp;🎉🎉 Best Paper Nomination at CVPR'20 for [Visual Chirality](https://linzhiqiu.github.io/papers/chirality/)! -->

# 📝 Publications 
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2023</div><img src='papers/cross_modal/images/neuro.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Multimodality Helps Unimodality: Cross-Modal Few-Shot Learning with Multimodal Models**

**Zhiqiu Lin**\*, [Samuel Yu\*](https://scholar.google.com/citations?user=gxRDkLMAAAAJ&hl=en), [Zhiyi Kuang](https://www.linkedin.com/in/zhiyikuang/), [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), [Deva Ramanan](https://www.cs.cmu.edu/~deva/)

[Website](https://linzhiqiu.github.io/papers/cross_modal/) \| [Arxiv](http://arxiv.org/abs/2301.06267) \| [![](https://img.shields.io/github/stars/linzhiqiu/cross_modal_adaptation?style=social&label=Code+Stars)](https://github.com/linzhiqiu/cross_modal_adaptation)
- We propose a simple cross-modal adaptation method for multimodal models that repurposes information from other modalities (e.g., class names and audio clips) as additional training samples.
- For CLIP, it achieves SOTA few-shot adaptation performance even with a simple **linear probe**, and consistently improves prior art such as prompting, adapter, and weight ensembling.
- Audiovisual experiments with AudioCLIP suggest that one can learn a better dog **visual** classifier by **listening** to them bark.

</div>
</div>
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NeurIPS 2022</div><img src='papers/leco/images/teaser.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**LECO: Continual Learning with Evolving Class Ontologies**

**Zhiqiu Lin**, [Deepak Pathak](https://www.cs.cmu.edu/~dpathak/), [Yu-Xiong Wang](https://yxw.web.illinois.edu/), [Deva Ramanan\*](https://www.cs.cmu.edu/~deva/), [Shu Kong\*](https://aimerykong.github.io/)

[Website](https://linzhiqiu.github.io/papers/leco/) \| [Arxiv](https://arxiv.org/abs/2210.04993) \| [NeurIPS'22 Talk](/papers/leco/LECO.pdf)
- A practical lifelong vision benchmark motivated by real-world dataset versioning issues, e.g., Mapillary 1.2 to 2.0.
- Simple but effective solutions such as joint training, semi-supervised learning, and learning-with-partial-labels to address inconsistent annotation (both coarse-grained and fine-grained).

</div>
</div>
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NeurIPS 2021 (Datasets and Benchmarks)</div><img src='images/clear/icon_text.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**The CLEAR Benchmark: Continual LEArning on Real-World Imagery**

**Zhiqiu Lin**, [Jia Shi](https://www.linkedin.com/in/elvishelvisshi/), [Deepak Pathak\*](https://www.cs.cmu.edu/~dpathak/), [Deva Ramanan\*](https://www.cs.cmu.edu/~deva/)

[CLEAR Wiki](https://linzhiqiu.gitbook.io/the-clear-benchmark/) \| [NeurIPS Paper Site](http://clear-benchmark.github.io) \| [Arxiv](https://arxiv.org/abs/2201.06289) \| [CVPR'22 Talk](/papers/clear/clear_cvpr.pdf)
- The first continual benchmark for visual recognition with natural distribution shifts over a decade!
- CLEAR has a 10- and 100-classes version ([download links](https://linzhiqiu.gitbook.io/the-clear-benchmark/)), similar to the famous CIFAR-10 and CIFAR-100 benchmarks.
- [1st CLEAR challenge](https://www.aicrowd.com/challenges/cvpr-2022-clear-challenge) was hosted on June 19th, 2022. We have 79 participants from 21 different countries and regions signed up for the challenge!

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR 2020 (Best Paper Nomination)</div><img src='images/chirality/mirror.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Visual Chirality**

**Zhiqiu Lin**, [Jin Sun](http://www.cs.cornell.edu/~jinsun/), [Abe Davis](http://abedavis.com), [Noah Snavely](http://www.cs.cornell.edu/~snavely/)

[Website](https://linzhiqiu.github.io/papers/chirality/) \| [Arxiv](https://arxiv.org/abs/2006.09512) \| [Video](https://www.youtube.com/watch?v=gc5IvTozU9M) \| [![](https://img.shields.io/github/stars/linzhiqiu/digital_chirality?style=social&label=Code+Stars)](https://github.com/linzhiqiu/digital_chirality)
- How does reflection change what we learn from images? Despite widespread use in data augmentation, people had not looked closely at this question before our work.

<!-- [**Project**](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=DhtAFkwAAAAJ&citation_for_view=DhtAFkwAAAAJ:ALROH1vI_8AC) <strong><span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span></strong>
- Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->
</div>
</div>

- [QPyTorch: A Low-Precision Arithmetic Simulation Framework](https://arxiv.org/abs/1910.04540).
 [Tianyi Zhang](https://tiiiger.github.io), **Zhiqiu Lin**, [Guandao Yang](https://www.guandaoyang.com), [Chris De Sa](http://www.cs.cornell.edu/~cdesa/), **NeurIPS 2019 Workshop @ EMC2** \| [![](https://img.shields.io/github/stars/Tiiiger/QPyTorch?style=social&label=Code+Stars)](https://github.com/Tiiiger/QPyTorch)
- [What.Hack: Engaging Anti-Phishing Training Through a Role-playing Cyber Defense Simulation Game](https://dl.acm.org/doi/abs/10.1145/3290605.3300338).
 [Zikai Alex Wen](https://www.cs.cornell.edu/~zkwen/), **Zhiqiu Lin**, Rowena Chen, [Erik Andersen](http://www.cs.cornell.edu/~eland/), **CHI 2019**

# 🎖 Honors and Awards
- *2020.06* Best Paper Nomination at CVPR'20 for [Visual Chirality](https://linzhiqiu.github.io/papers/chirality/)!
- *2020.05* Graduated Summa Cum Laude in Computer Science and Mathematics from Cornell University, and served as college symbol bearer (top 5 of the college).
<!-- - *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  -->

# 📖 Educations
- *2020.09 - (now)*, PhD student, Carnegie Mellon University. 
- *2016.09 - 2020.06*, Undergraduate, Cornell University.

# 💬 Invited Talks
- *2022.06*, I presented [CLEAR Benchmark](https://linzhiqiu.gitbook.io/the-clear-benchmark/) on [CVPR'22 2nd Workshop on Open World Vision](https://www.cs.cmu.edu/~shuk/vplow.html). 
<!-- - *2021.03*, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet.  \| [\[video\]](https://github.com/) -->

# 💻 Services
- Organizer: CVPR’22 VPLOW Workshop (Challenge Track)
- Reviewer: ECCV, CVPR (Outstanding reviewer), ICCV, NeurIPS, ICML.
- Teaching (CMU): [Learning-based Image Synthesis](https://learning-image-synthesis.github.io/sp22/) and Advanced Computer Vision
- Teaching (Cornell): Advanced Machine Learning, Cornell Tech Pre-Master Program, Functional Programming, Algorithm Analysis, Data Structures, Computer Vision