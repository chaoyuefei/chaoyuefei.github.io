---
title: "My Research Workflow: How to Enable Embedded Video in Beamer Presentations"
date: 2025-06-05
lastmod: 2025-06-05
tags: ["LaTex","Beamer","video","presentation","workflow"]
author: ["Chaoyue Fei"]
description: "This post demonstrates how to embed a video in a Beamer presentation using LaTeX."
summary: "This post demonstrates how to embed a video in a Beamer presentation using LaTeX."
showToc: true
disableAnchoredHeadings: false
---

## Motivation
In my research workflow, I love LaTeX for its code-controlled typesetting, cross-platform, and version control nature. If it is possible, all my writing work is done in LaTeX. Even for presentations, I prefer using Beamer, a LaTeX class for creating slides. However, one limitation of Beamer is that it does not support embedding videos directly. This post shows the workflow I use to embed a video in a Beamer presentation PDF file using the `movie15` package, along with the tool `pymypress` that I use for presenting it.

## Prerequisites
To embed a video in a Beamer presentation, you need to have the following tools installed:
- **LaTeX Environment**
- **[pymypress](https://github.com/Cimbali/pympress)**: a simple yet powerful PDF reader designed for dual-screen presentations.

## LaTeX Code
Here is a minimal example of how to embed a video in a Beamer presentation using the `movie15` package. You can include the call-up image as a placeholder for the video, which will be displayed when the video is not playing.

```latex
\documentclass{beamer}
\usepackage{movie15}

\begin{document}
\begin{frame}
  \begin{center}
    \includemovie[attach=false,autoplay,text={%
        \includegraphics{fig/call-up.png}%
      }]{0.4\linewidth}{0.3\linewidth}{fig/test.mp4}
  \end{center}
\end{frame}
\end{document}
```

## Presentation
To present the Beamer slides with the embedded video, you can use `pympress`. It allows you to play the video directly within the PDF presentation.

To run `pympress`, simply execute the following command in your terminal:

```bash
pympress your_presentation.pdf
```
This will open your Beamer presentation in a dual-screen mode, allowing you to control the slides and play the video seamlessly as illustrated in the video below.
![pympress demo 1](demo1.gif)
![pympress demo 2](demo2.gif)

## Conclusion
`movie15` plus `pympress` provides a powerful way to embed videos in Beamer presentations. It is easy yet powerful, and should be used in all platforms including Windows, macOS, and Linux.
