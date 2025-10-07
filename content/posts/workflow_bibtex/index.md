---
title: "My Research Workflow: How Do I Manage My References with BibTeX"
date: 2025-10-07
lastmod: 2025-10-07
tags: ["LaTex","BibTex","research","paper","writing","workflow"]
author: ["Chaoyue Fei"]
description: "This post demonstrates how to manage references in LaTeX documents using BibTeX."
summary: "This post demonstrates how to manage references in LaTeX documents using BibTeX."
showToc: true
disableAnchoredHeadings: false
---


Typically, the file `references.bib` contains the BibTeX entries for all the papers I have collected.


## How to add new paper in the bib file

I recommend using [Google Scholar](https://scholar.google.com/) to find the paper and obtain the BibTeX citation.

> Tools like [Zotero](https://www.zotero.org/) and [Mendeley](https://www.mendeley.com/) are useful for reference management, but I find Google Scholar to be the most straightforward option, as it minimizes the risk of errors compared to scrapers.

For instance, I would like to search for the paper titled "Text2Robot: Evolutionary Robot Design from Text Descriptions.":

1. search the paper

<img src="./assets/CleanShot 2025-10-07 at 14.55.46@2x.png" alt="CleanShot 2025-10-07 at 14.55.46@2x" />

2. click `Cite` and then select `BibTex`

<img src="./assets/CleanShot 2025-10-07 at 14.56.41@2x.png" alt="CleanShot 2025-10-07 at 14.56.41@2x" />

3. Copy the BibTex to the `references.bib` file:

```bash
@inproceedings{ringel2025text2robot,
  title={Text2robot: Evolutionary robot design from text descriptions},
  author={Ringel, Ryan P and Charlick, Zachary S and Liu, Jiaxun and Xia, Boxi and Chen, Boyuan},
  booktitle={2025 IEEE International Conference on Robotics and Automation (ICRA)},
  pages={5789--5797},
  year={2025},
  organization={IEEE}
}
```

Less is more, just keep it simple.
