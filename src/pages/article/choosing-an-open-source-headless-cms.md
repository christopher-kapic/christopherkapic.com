---
layout: ../../layouts/Article.astro
id: article-1661785570397-giUUGBbC_
draft: true
medium: false
devto: false
title: Choosing an Open Source Headless CMS
author:
  - value: author-1660337033199-jpFG6u1fX
    label: Christopher Kapic
summary: Today, there are many options for CMSs, from traditional ones like
  Wordpress to many modern Headless CMSs. Use this framework to help get started
  in making your decision.
image: /cms/vs.png
tags:
  - netlify
  - netlifycms
  - cms
  - keystonejs
  - directus
publishDate: 2022-08-29T15:06:10.427Z
updateDate: 2022-08-29T15:06:10.433Z
---
## What is a CMS?

T﻿raditionally, a CMS and a website are hosted on the same server. Wordpress, for example, is a CMS and website combination in which the admin can log into the CMS to get editing privileges directly on the site. More recently, there has been the [JAMstack](https://jamstack.org/) trend, part of which is the introduction and proliferation of the [headless CMS](https://jamstack.org/headless-cms/).

## What does it mean to be headless?

### The webserver and the CMS are hosted separately.

I﻿nstead of hosting the website and the CMS on the same server, the site and CMS are separated. This has several pros and cons.

W﻿e'll start with the cons first.

## W﻿hat are the cons?

* U﻿sing a headless CMS requires a higher level of technical competence to get going. There are many competitive services which offer Wordpress hosting that require little technical savviness, but in choosing a headless CMS one necessarily must know how to host two servers, or outsource the CMS to a SaaS.
* O﻿ften, more custom development is required; you must know how to connect your site to your CMS.

## W﻿hat are the pros?

*﻿ If your CMS goes down, your site can still keep working. With options like [11ty](https://www.11ty.dev/), [Astro](https://astro.build/), [NextJS](https://nextjs.org/), and more for static site generation, your CMS only needs to run at build time. This gives you a lot more reliability, especially as modern serverless hosting options become more robust.
*﻿ 

![img](/cms/choose-a-cms.png)