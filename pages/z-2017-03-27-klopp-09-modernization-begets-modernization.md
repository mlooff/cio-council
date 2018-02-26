---
layout: blog
body-class: home
title: Blog - Part 9 - Modernization Begets Modernization
blog-date: March 27, 2017
blog-author: Rob Klopp, CIO, SSA
blog-title: Part 9 - Modernization Begets Modernization
permalink: /2017/03/27/modernizing-federal-it-part-9-modernization-begets-modernization/
background-image: /assets/img/grey.background.png
hero-text:  News & Updates
hero-byline:
hero-button-text: 
hero-button-link: 
banner-heading: 
banner-text: 
banner-button-text: 
banner-button-link: 
---
<BR>
<I>This is the 9th in a series describing how the Social Security Administration is working towards a more
modern IT infrastructure. </I>
*<A HREF="https://www.cio.gov/2015/12/10/modernizing-federal-it-part-1-catching-up-and-jumping-ahead/">Part 1: Catching Up and Jumping Ahead</A><BR>
*<A HREF="https://www.cio.gov/2016/01/19/modernizing-federal-it-part-2-the-gravity-of-ip/">Part 2: The Gravity of Inetellectual Property</A><BR>
*<A HREF="https://www.cio.gov/2016/03/07/modernizing-federal-it-part-3-teasing-apart-the-problem/">Part 3: Teasing Apart the Problem</A><BR>
*<A HREF="https://www.cio.gov/2016/03/21/modernizing-federal-it-part-4-building-a-modern-data-foundation/">Part 4: Building a Modern Data Foundation</A><BR>
*<A HREF="https://www.cio.gov/2016/05/23/modernizing-federal-it-part-5-modernizing-software-architecture/">Part 5: Modernizing Software Architecture</A><BR>
*<A HREF="https://www.cio.gov/2016/11/07/modernizing-federal-it-part-6-agility-and-evolving-a-minimal-viable-product/">Part 6: Agility and Evolving a Minimal Viable Product</A><BR>
*<A HREF="https://www.cio.gov/2016/11/22/modernizing-federal-it-part-7-what-does-a-modern-application-look-like/">Part 7: Modernizing Federal IT Part 7 What Does a Modern Application Look Like</A><BR>
*<A HREF="https://www.cio.gov/2017/01/09/modernizing-federal-it-part-8-the-proof-is-in-the-pudding-disability-case-processing-system-2-dcps2-goes-live/">Part 8: Modernizing Federal IT Part 8: The Proof is in the Pudding, Disability Case Processing System 2 (DCPS2) goes Live</A><BR>
*<A HREF="https://www.cio.gov/2017/03/27/modernizing-federal-it-part-9-modernization-begets-modernization/">Modernization begets Modernization</A>
<BR><BR>

In several of the previous blogs on IT Modernization, I mentioned the SSA’s DCPS2 product program, which aims to modernize a very old legacy green-screen application. In this post, I’d like to share what comes next as one IT modernization program begets another.

The DCPS2 product provides a modern application for determining whether a claimant is eligible for disability benefits.

The application is comprised of three components that work together to support our case workers. The simplest component performs case management: allowing new cases to be introduced, assigned, tracked, and closed. The most complex component performs case processing. Here case workers perform the bulk of the investigation, requesting and analyzing evidence against legislative and regulatory guidelines to make a determination. The third component is also complex as it provides automated quality assurance tests to ensure that the case worker has applied the guidelines accurately. Note that these complex components are very SSA-specific and unavailable off-the-shelf.

After a case is processed by DCPS2, if the claim is denied, the case could be passed to an adjudication process handled by another organization within the SSA: ODAR. The entire process from DCPS2-to-ODAR takes time and, given the human judgements along the way, the process requires review and oversight all along the way.

Here is the surprise. While not every step in the process is exactly the same, the basics: case management, evidence gathering and analysis, and quality assurance, are common across the DCPS2 and the ODAR business processes. As a result, the agency has started a program to modernize the entire disability determination process end-to-end by leveraging the modern DCPS code base into the ODAR business process. This means that a disability case will be processed consistently by a single application from inception through to a final adjudicated close.

This is very significant. Within a modern end-to-end process, there are major efficiencies to be had. We estimate that between 20% and 50% of the DCPS2 code may be reused to modernize the ODAR process. Even at the lower end of the range this leverage will accelerate modernization of this critical process by a year and reduce costs as we go.

Disability determination is one of the core parts of the agency mission. Congress oversees this part of our mission and constantly, rightfully, pushes us to process disability claims as fast as possible. By leveraging our first modern application, we aim to quickly develop a tightly integrated, end-to-end, bespoke business application that will extend to incorporate new technology and continuously improve business outcomes. It will do this at less cost and in the near term.
