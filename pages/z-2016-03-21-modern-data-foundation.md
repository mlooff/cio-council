---
layout: blog
body-class: home
title: Blog - Modernizing Federal IT Part 4 - Building a Modern Data Foundation
blog-date: March 21, 2016
blog-author: Rob Klopp, CIO, SSA
blog-title: Modernizing Federal IT Part 4 - Building a Modern Data Foundation
permalink: /2016/03/21/modernizing-federal-it-part-4-building-a-modern-data-foundation/
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
modern IT infrastructure. </I><BR>
*<A HREF="https://www.cio.gov/2015/12/10/modernizing-federal-it-part-1-catching-up-and-jumping-ahead/">Part 1: Catching Up and Jumping Ahead</A><BR>
*<A HREF="https://www.cio.gov/2016/01/19/modernizing-federal-it-part-2-the-gravity-of-ip/">Part 2: The Gravity of Inetellectual Property</A><BR>
*<A HREF="https://www.cio.gov/2016/03/07/modernizing-federal-it-part-3-teasing-apart-the-problem/">Part 3: Teasing Apart the Problem</A><BR>
*<A HREF="https://www.cio.gov/2016/03/21/modernizing-federal-it-part-4-building-a-modern-data-foundation/">Part 4: Building a Modern Data Foundation</A><BR>
*<A HREF="https://www.cio.gov/2016/05/23/modernizing-federal-it-part-5-modernizing-software-architecture/">Part 5: Modernizing Software Architecture</A><BR>
*<A HREF="https://www.cio.gov/2016/11/07/modernizing-federal-it-part-6-agility-and-evolving-a-minimal-viable-product/">Part 6: Agility and Evolving a Minimal Viable Product</A><BR>
*<A HREF="https://www.cio.gov/2016/11/22/modernizing-federal-it-part-7-what-does-a-modern-application-look-like/">Part 7: Modernizing Federal IT Part 7 What Does a Modern Application Look Like</A><BR>
*<A HREF="https://www.cio.gov/2017/01/09/modernizing-federal-it-part-8-the-proof-is-in-the-pudding-disability-case-processing-system-2-dcps2-goes-live/">Part 8: The Proof is in the Pudding, Disability Case Processing System 2 (DCPS2) goes Live</A><BR>
*<A HREF="https://www.cio.gov/2017/03/27/modernizing-federal-it-part-9-modernization-begets-modernization/">Part 9: Modernization begets Modernization</A><br>
  *<A HREF="https://www.cio.gov/2017/04/14/part-10-modernizing-with-a-buy-or-a-build/">Part 10: Modernizing with a Buy or Build</A><BR>
<BR><BR>

In this post we will consider how to develop a modern data architecture to underpin the modernization of your code base. 

Systems developed before the year 2000 were often built on application-specific data models. Today we build applications that more-or-less adhere to an enterprise data model. This move from modeling data in an application context, which created stovepipes, into data modeled into an enterprise context is what we consider the foundation of a modern data architecture.

Systems developed even earlier, before 1990, were built before relational databases became the norm. The legacy of these systems is data that is not normalized and that uses application-specific keys to identify records. Normalizing these stovepipes into a subject-oriented enterprise model requires a fair amount of effort, but the result is data that is integrated and easy-to-use. Easy-to-use translates into reduced software development costs and integrated translates into better business applications.

Note that there are lots of applications built pre-1990 that were semi-modernized and semi-normalized to run in relational databases but that were not re-architected into a modern subject-oriented, enterprise context. So while they are relational they are not modern and there is a technical debt still to be paid.

There is a great example of this at the SSA. Our original systems were tape-based; there was no direct access storage available for files as large as our. As a result all of our systems were developed to process file sequentially. Every night we read in 500 reels of tape and wrote out 500 updated reels. When direct access storage devices (DASD in mainframe-speak) came along there was no file system that could support putting all of this data online, so we built one from scratch. Since we could not afford to rewrite all of the applications we just passed on this technical debt and built an API that let the original code “believe” that it was still talking to tape.

Please note that this theme, we did not have the budget for a rewrite so we passed on the debt, reoccurs throughout this series on IT modernization. The fact of this technical debt and of the inability to fund the effort to retire that debt makes the argument for the President’s $3.1B IT Modernization Fund (more here) which we strongly support.

Back to the SSA story. Now we have sequential processes lashed to a proprietary file system that mimics tape but provides the performance enhancement of reading from disk. Many years later when databases were conventional we decided to retire the technical debt associated with running on our own file system, so we built an API that masked the previous API from “seeing” that data was now stored in an RDBMS and retired our home-grown file system (or very nearly retired it… Sigh). The end result is data stored in a relational database is an un-integrated application-specific context, sort-of normalized, that still looks like tape to the legacy business applications. These efforts to retire some technical debt without the ability to execute a proper modernization program represent what can be done around the edges and I suspect that most Federal agencies have similar stories and similar legacy systems.

With this background in place, at the SSA we are starting on a “data first” approach to modernization. While data changes, the rate of change is much slower than the rate software changes. We want to develop a stable foundation before we start modernizing the code base so we are building a new data architecture with an enterprise-wide customer subject area that will pull all of the data we store about our customers into an integrated whole. This project started a year ago and will deploy into production in December 2016.

Data first and a modern data foundation seems to be the right starting point. In the next posts we will consider several options on how to leverage this start and to begin modernizing the code base.
