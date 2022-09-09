---
layout: ../../layouts/Article.astro
id: article-1661785570397-giUUGBbC_
draft: false
medium: true
devto: true
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

* ﻿If your CMS goes down, your site can still keep working. With options like [11ty](https://www.11ty.dev/), [Astro](https://astro.build/), [NextJS](https://nextjs.org/), and more for static site generation, your CMS only needs to run at build time. This gives you a lot more reliability, especially as modern serverless hosting options become more robust.
* T﻿here are far more options for site customization - you have the freedom to connect any framework to any CMS. For sites that require custom development, this freedom can be essential.
* H﻿osting options are more compelling when you enter the JAMstack world. Instead of a traditional webserver setup, using tools like Netlify, Vercel, CockroachDB, Planetscale, any of the myriad of frontend frameworks, and more can allow you to create an incredible and unique experience to your customers.

## How do I know which CMS to choose?

![Choose a CMS diagram (explained in article)](/cms/choose-a-cms.png)

U﻿ltimately, there are more options to consider than those which I can cover here. For a more comprehensive breakdown, I recommend that you check out [JAMstack.org's comparison](https://jamstack.org/headless-cms/).

T﻿hat being said, if open-source is important to you, be it for privacy or avoiding vendor lock-in, my three favorites are [Directus](https://directus.io/) (I am a contributor), [KeystoneJS](https://keystonejs.com/), and [NetlifyCMS](https://www.netlifycms.org/) (not *technically* a headless CMS, but still worth considering).

## D﻿irectus

D﻿irectus is... really cool. It can connect with your currently-existing database, provides a GraphQL API, is extensible, can be hosted in a serverless environment (Google Cloud Run), and is a pleasure to use.

## K﻿eystoneJS

K﻿eystone is in many ways similar to Directus, except it uses a more developer-first approach to the database schema. You write a file that compiles into a Prisma configuration. This is nice in theory, but it makes using the same database as your currently-existing database more difficult. However, that may not be a problem since the idea of a headless CMS is to divorce the CMS from the website infrastructure anyway. Like Directus, it too can be hosted in a serverless environment (even Netlify).

## N﻿etlifyCMS

O﻿f this group, NetlifyCMS is certainly the oddball. Instead of connecting to a database and potentially a storage bucket, NetlifyCMS connects with your git repository. Using a service like Netlify, a new build of your site is created every time a piece of content is updated. For something like a blog, where content is read far more than it is updated, and the content is updated only by admin users, NetlifyCMS is a good choice. The best part about NetlifyCMS is that it can easily be used for site templates. Most starter sites I create use NetlifyCMS because users can simply deploy to Netlify and call it good.

N﻿etlifyCMS is *not* good for websites with content that must be updated by regular users (comments should not be handled by NetlifyCMS, for example).

## H﻿ow to choose?

E﻿ssentially, I argue the best simplification for how to choose is this:

1. D﻿o non-admin users update any "server-side" state in your site? If not, go with NetlifyCMS.
2. D﻿o you want to connect to your existing database? If so, go with Directus.
3. I﻿f neither of the above apply, choose between Directus and KeystoneJS. You'll probably want Directus, but there may be edge cases in which Keystone is better (or, you might just have a preference for whatever reason).

U﻿ltimately, there are many options for your choice of CMS, and the right one might not be here. This is just a framework I have decided upon after doing lots of research for my own projects and learning which CMS options work best for most of my needs.