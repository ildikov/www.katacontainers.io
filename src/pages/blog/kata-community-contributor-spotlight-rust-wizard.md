---
templateKey: blog-post
title: Contributor Spotlight Series - Ya'nan Li
author: Ya'nan Li, Ildiko Vancsa
date: 2026-08-19T01:32:05.627Z
category:
  - value: category-6-wjkXzEM2
    label: Features & Updates
---

This Contributor Spotlight mini series features the winners of the Kata Containers 4.0 Contributor Awards. In this article the spotlight is on Ya'nan Li, the Kata community’s Rust Wizard.

Ya’nan is a Software Engineer at Ant Group based in China and a contributor to Kata Containers since the end of 2022. In the 4.0 release cycle Ya’nan was a quiet force of nature, and a patient listener with a powerful voice. He works with speed and precision, which is how he became one of the key pillars of recreating the Kata runtime in Rust.

![alt text](/img/Yanan_Li.jpg)

I asked him a few questions to learn a bit more about his journey and involvement in the project:

# How long have you been contributing to Kata Containers, and what drew you to the project?
I submitted my first Pull Request to Kata Containers in October 2020 and have been actively contributing since December 2022.

In fact, I've been following Kata Containers ever since its launch in 2017. I've long had a deep interest in container runtimes, lightweight virtualization, and workload isolation, and I was always looking for an opportunity to jump in and contribute.

In 2022, Ant Group and Alibaba Cloud contributed the Rust-based Kata shim to the community, coinciding with the release of Kata Containers 3.0. At the time, the Rust runtime was still evolving rapidly—there was a lot of ground to cover in terms of core features and ecosystem maturity, as well as significant feature and behavior parity to achieve with the existing Go runtime. Our internal team needed more engineers to work on runtime-rs, and I was fortunate to step up and join the development and maintenance effort.

# What areas of the project do you contribute to?
My primary focus is on code development. I mainly work on feature development, bug fixes, and day-to-day maintenance for runtime-rs and the agent, pushing to continuously mature these capabilities while improving their stability and maintainability.

# What is one contribution you are particularly proud of and why?
As part of the drive toward Kata Containers 4.0, our team accomplished a lot of critical work. One contribution I'm particularly proud of is my involvement in building out runtime-rs capabilities for [Confidential Containers (CoCo)](https://confidentialcontainers.org) scenarios.

I primarily led the adaptation of runtime-rs for TDX, Non-TEE, and agent policy, and worked alongside other community developers to set up the Non-TEE CI. These efforts significantly improved runtime-rs capabilities in CoCo scenarios and helped drive ongoing feature and behavior alignment with the Go runtime. Establishing the Non-TEE CI, in particular, not only enabled continuous automated validation for critical CoCo paths, but also laid a solid foundation to prevent regressions during the long-term evolution of runtime-rs.

The task was far more complex than initially expected. It wasn't just about runtime-rs itself—it required coordinating interactions across multiple components, including the agent, agent policy, CoCo, and CI. Seemingly subtle behavior differences could easily break the entire test pipeline, demanding continuous debugging, validation, and refinement.

At the same time, this was a quintessential community effort. While I focused on TDX, Non-TEE, and agent policy, bringing support for other TEE platforms (like AMD SEV-SNP and IBM Secure Execution) and constantly refining the broader CI framework relied on the collective effort of fellow maintainers and contributors. What gives me the greatest sense of accomplishment isn't just delivering a single feature, but working together with the community to mature these capabilities into a cornerstone of Kata Containers 4.0.

# What has surprised you most about the Kata Containers community?
What has surprised me most is how deeply the Kata Containers community embodies a culture of true open collaboration.

Kata Containers sits at the intersection of container runtimes, virtualization, guest agents, security, confidential computing, and cloud-native tech. A single issue often spans across multiple domains like the runtime, hypervisor, agent, and CI pipelines.

What made the deepest impression on me is that when complex issues arise, people don't treat them as someone else's problem just because they fall outside their own module or company's scope. Instead, folks naturally come together to analyze, discuss, and solve them as a team. Often, discussion on a single PR draws active involvement not just from the immediate maintainers, but also from other contributors jumping in to help debug, suggest ideas, or validate fixes.

The same applies to newcomers. Community members are patient in answering questions, thorough with code reviews, and quick to provide constructive feedback. The focus of every discussion is always on how to make the project better, never on who raised the issue or who owns the code. I believe it's this open, trusting, and shared-responsibility culture that makes Kata Containers not just a fantastic open source project, but an incredible community to learn in and contribute to over the long run.

# What are you most excited about in the project right now?
What excites me most is seeing Kata Containers continuously expand its use cases while drawing in new technical directions and fresh community perspectives.

While Kata originally focused on security isolation in standard cloud-native environments, we are now seeing an explosion of exploration around AI workloads, confidential computing, and Agent Sandboxes. These emerging workloads bring brand-new requirements that drive the ongoing evolution of Kata's core architecture.

For me, the most exciting part isn't any single feature, but watching how the community tackles these new challenges together—like advancing support for accelerators like GPUs to meet the practical demands of Agentic AI and Confidential AI, all while maintaining a lightweight footprint and strong isolation. At the same time, there's great work happening to boost Sandbox boot speed and refine state save/restore capabilities. I'm eager to see more developers and organizations join in on these initiatives to keep pushing the project forward.

# What advice would you give to someone just getting started?
My advice is simple: Stay curious, get your hands dirty, and don't be afraid to take that first step.

When you're starting out, don't worry about reading every line of source code or understanding every implementation detail right away. Start by understanding what problems Kata Containers solves and where it fits, then follow the official docs to get it up and running yourself. A lot of architectural concepts will naturally click once you see them in action.

When you're ready to contribute, don't feel like you need to start with a massive feature. Fixing a bug, improving documentation, adding a test case, or even refining an error message are all genuinely valuable contributions. In fact, many long-time contributors started with something just that small.

Finally, don't hesitate to ask questions. The Kata Containers community is always open to discussion and eager to help new contributors grow. Stay engaged, embrace review feedback with an open mind, and keep learning—you'll find your understanding of the project deepening with time. Open source contribution is a marathon, not a sprint. Start small, stick with it, and you'll grow right alongside the project.

Check out Ya’nan’s [GitHub profile](https://github.com/Apokleos) to learn more about his work, and don’t hesitate to join the [Kata Slack](https://join.slack.com/t/katacontainers/shared_invite/zt-16w1u6usn-sK871qbMxVN8KsCP5Gr56A) to talk to him and fellow project maintainers and contributors.

# About Kata Containers
If you would like to learn more about the project and get involved check out the [website](https://www.katacontainers.io) for more information or [download the code](https://github.com/kata-containers) and start to experiment with the runtime. If you are already evaluating or using the software please fill out the [user survey](https://openinfrafoundation.formstack.com/forms/kata_containers_user_survey) and help the community improve the project based on your feedback.
