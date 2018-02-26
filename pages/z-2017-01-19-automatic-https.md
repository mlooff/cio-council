---
layout: blog
body-class: home
title: Blog - Automatic HTTPS Enforcement for New Executive Branch .Gov Domains
blog-date: January 19, 2017
blog-author: Eric Mill
blog-title: Automatic HTTPS Enforcement for New Executive Branch .Gov Domains
permalink: /2017/01/19/automatic-https-enforcement-new-executive-branch-gov-domains/
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
HTTPS is a necessary baseline for security on the modern web. Non-secure HTTP connections lack integrity protection, and can be used to attack citizens, foreign nationals, and government staff. HTTPS provides increased confidentiality, authenticity, and integrity that mitigate these attacks.

In June 2015, the White House required all new federal web services to <A HREF="https://https.cio.gov/#guidelines">support and enforce HTTPS connections over the public internet</A>, and for agencies to migrate existing web services to HTTPS by the end of calendar year 2016. GSA’s Office of Government-wide Policy has supported the growth of HTTPS in the federal government by providing a <A HREF="https://pulse.cio.gov/">public HTTPS</A> monitoring dashboard and <A HREF="https://https.cio.gov/">thorough policy guidance and technical assistance</A>.

Federal agencies have made very significant progress towards that goal, to the point that <A HREF="https://18f.gsa.gov/2017/01/04/tracking-the-us-governments-progress-on-moving-https/">federal use of HTTPS</A> now outpaces the private sector.

This year, GSA will be taking another significant step forward in making secure communication the default for federal web services by automatically enforcing HTTPS in modern web browsers for newly issued executive branch .gov domains and their subdomains.

As new executive branch domains are registered, the <A HREF="https://www.dotgov.gov/">DotGov</A> program will submit them to web browsers for “<A HREF="https://https.cio.gov/hsts/#hsts-preloading">preloading</A>.” After submission, it can take up to three months before preloading takes effect in modern web browsers. The change will be introduced to dotgov customers when they register a new domain under the Executive Branch, and will not affect existing or renewed domains.

Once preloading is in effect, browsers will strictly enforce HTTPS for these domains and their subdomains. Users will not be able to click through certificate warnings. Any web services on these domains will need to be accessible over HTTPS in order to be used by modern web browsers.

GSA provides <A HREF="https://https.cio.gov/">extensive guidance</A> on HTTPS deployment to agencies, and encourages .gov domain owners to obtain low cost or <A HREF="https://https.cio.gov/certificates/#what-kind-of-certificate-should-i-get-for-my-domain%3f">free certificates</A> trusted by the general public. In our experience, more expensive certificates do not offer more security value to service owners, and automatic deployment of free certificates can significantly improve service owners’ security posture.

GSA plans to introduce this HTTPS preloading change in the spring of 2017. DotGov domain customers will be notified by the Gov Domain Registrar via email 30 days before the change goes in effect.

For questions about this new GSA policy, agencies can email the <A HREF="mailto:feedback@cio.gov">team at CIO.gov</A>.

For more information on preloading, please read 18F’s blog post on the first preloaded .gov domains, and GSA’s HTTPS policy support article on the topic.

Some important notes:

-Executive agencies do not have to do any work to be in compliance, other than ensuring that HTTPS is supported on their web services deployed to any newly issued .gov domains.
-This change only affects clients that support <A HREF="https://https.cio.gov/hsts/">HTTP Strict Transport Security (HSTS)</A>, which is generally limited to modern web browsers. Specialized HTTP clients (such as cURL or HTTP standard libraries) should generally not be affected by default.
-This change will affect all subdomains of newly registered executive .gov domains. This includes intranet websites, if they are deployed to subdomains of publicly registered .gov domains. Using plain HTTP for intranet websites is not secure and is discouraged, but can still be achieved by using private domain names that only resolve inside the intranet.

For more information and technical guidance on HTTPS and HSTS, GSA has provided <A HREF="https://https.cio.gov/">detailed guidance</A>:

-<A HREF="https://https.cio.gov/faq/">General FAQ</A> on HTTPS: What HTTPS does and doesn’t do, and how it relates to DNSSEC.
-<A HREF="https://https.cio.gov/hsts/">HTTP Strict Transport Security</A>: What HSTS does, and how to use it.
-<A HREF="https://https.cio.gov/certificates/">Certificates</A>: Best practices and recommendations around the use of inexpensive or free certificates.

Additionally, GSA’s DigitalGov University and 18F teams have partnered to produce three detailed video presentations on HTTPS:

-<A HREF="https://www.youtube.com/watch?v=d2GmcPYWm5k">An Introduction to HTTPS</A> (basic, a general introduction for anyone)
-<A HREF="https://www.youtube.com/watch?v=rnM2qAfEG-M">Implementing HTTPS</A> (advanced, more technical detail)
-<A HREF="https://www.youtube.com/watch?v=X5H8JRULDOo">Migrating to HTTPS</A> (advanced, focused on HSTS, certificates, and mixed content)

