---
title: "Neurofit W.S.I.B Assessment App"
excerpt: "A Computer Vision Based Motion Capture for Assessing Whether W.S.I.B workers are ready to go back to work."
header:
    video:
        id: s8_5_Kmhq9E
        provider: youtube
    teaser: assets/images/NeurofitLogo.png

sidebar:
  - title: "Role"
    text: "Integration Developer"
  - title: "Responsibilities"
    text: "Research, Pipeline Integration, Frontend Implementation, Build Deployment"
  - title: "Tools Used"
    text: "Unity, C#, Pytorch, Python"
---

# Overview

As part of the C.E.W.I.L(Co-operative Education and Work-Integrated Learning Canada) Tech For Good Program, I worked with Neurofit, A Company working to equip healthcare professionals with virtual therapy tools to track real-time progress.

Working as a team of three, the task given to us was to create a visual motion capture system that could test and meet specific criteria on the W.S.I.B(Workplace Safety and Insurance Board), making them capable of assessing worker health at home, rather than having them come into the office for assessment.

## Research

We began by looking up similar implementations and libraries used, first looking into the computer vision side of things and then how it could be integrated into unity.

We discovered google media pipe gave us access to this in a pre-built form, and decided we would use this as our starting point.


## Development and Deployment

My primary responsibility was supporting the lead developer and designer through frontend implementation and system integration within Unity. This involved translating the design specifications into functional UI components and ensuring a smooth user experience throughout the assessment workflow.

A key technical challenge was bridging the Python-based computer vision pipeline with the Unity application. Rather than relying on the Python process to launch automatically in the background, I implemented a command line trigger where Unity explicitly activated and managed the connection lifecycle by initiating, monitoring, and terminating the Python process as needed. This gave us greater control over error handling and made the system more robust for end users running the application outside a development environment.

To prepare the pipeline for distribution, I packaged the Python motion capture components into a standalone executable, removing the dependency on users having a Python environment installed. This was integrated into the final Unity build process, resulting in a single deployable application suitable for at-home use by W.S.I.B. workers without requiring any technical setup on their part.


## Takeaways

This project was my first experience integrating a computer vision system into a production-facing application, through this, I learned a lot about getting a product from a working research prototype to a deployable product. Wrapping the Python pipeline into an executable and coordinating it with Unity reinforced how much engineering effort goes into reliability and ease-of-use once you move past a proof of concept.

Working as a team of three meant having the opportunity to perform multiple tasks across different fields such as User Experience, Frontend, and Pipeline Integration. This cross-functional exposure sharpened my ability to work across the stack and communicate technical trade-offs with teammates focused on different parts of the system.

Although we did not create a production ready product, working on this project gave me a lot of insight into how the process works and the best practices in a building a client facing product.





