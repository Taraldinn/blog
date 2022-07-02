## গিট কি এবং কেন ? (What is Git?)

---
title: গিট কি এবং কেন ? (What is Git?)
published: true
date: 2022-06-10 22:28:47 UTC
tags: GitGitHUb,git,GitGitHub,GitHub
canonical_url: https://blog.aldinn.com/what-is-git/?utm_source=rss&utm_medium=rss&utm_campaign=what-is-git
---

 ![Git & Github](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMjAwIiBoZWlnaHQ9IjYzMCI+PHJlY3Qgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSI+PGFuaW1hdGUgYXR0cmlidXRlTmFtZT0iZmlsbCIgdmFsdWVzPSJyZ2JhKDE1MywxNTMsMTUzLDAuNSk7cmdiYSgxNTMsMTUzLDE1MywwLjEpO3JnYmEoMTUzLDE1MywxNTMsMC41KSIgZHVyPSIycyIgcmVwZWF0Q291bnQ9ImluZGVmaW5pdGUiIC8+PC9yZWN0Pjwvc3ZnPg==)

[আগের পর্ব](https://blog.aldinn.com/git-and-github-complete-mastery-%e0%a6%97%e0%a6%bf%e0%a6%9f-%e0%a6%8f%e0%a6%a8%e0%a7%8d%e0%a6%a1-%e0%a6%97%e0%a6%bf%e0%a6%9f-%e0%a6%b9%e0%a6%be%e0%a6%ac-%e0%a6%95%e0%a6%ae%e0%a6%aa%e0%a7%8d%e0%a6%b2/ "আগের পর্ব")

```
Git কি এবং কেন গিট এত পপুলার? 
```

[Git](https://git-scm.com/ "Git ")হচ্ছে পৃথিবির সব থেকে পপুলার ভার্শন কন্ট্রোল সিস্টেম ।কোন ভার্শন কন্ট্রোল সিমপ্লি আমাদের কোড এর চেইঞ্জেস গুলা রেকর্ড রাখে সময়ের সাথে সাথে একটি ডেটাবেজে, যার নাম রিপোজিরিটি(Repository) হিসেবে সর্ব পরিচিত । [git](https://git-scm.com/ "Git ")এর মাধ্যমে আমারা আমাদের প্রজেক্ট হিস্টরি চেক করতে পারি ,আমরা দেখতে পারি কে কি চেইঞ্জ করেছে ,কতটুকু চেইঞ্জ করেছে , কখন করেছে এবং কেন করেছে । যদি আমাদের প্রজেক্ট এ কোন গোলমাল পাকিয়ে ফেলি তাহলে আমরা সিমপ্লি আমাদের কোড এর আগের ভার্শন এ চলে যেতে পারব জাস্ট একটা কমান্ড এর মাধ্যমে।

<video id="video-2639-2" width="640" height="360" preload="metadata" controls="controls"><source type="video/mp4" src="https://res.cloudinary.com/aldinn/video/upload/v1654900716/blog/git_01_igcqqh.mp4?_=2"></source><a href="https://res.cloudinary.com/aldinn/video/upload/v1654900716/blog/git_01_igcqqh.mp4">https://res.cloudinary.com/aldinn/video/upload/v1654900716/blog/git_01_igcqqh.mp4</a></video>

যদি আমরা একই প্রজেক্ট অনেকজন মিলে করি এবং আমাদের প্রজেক্ট এ যদি কোন গিট অথবা ভার্শন কন্ট্রোলিং সিস্টেম ইউজ না করি তাহলে আমাদেরকে একই প্রজেক্ট অনেক গুলো ফোলন্ডরের কপি করতে হবে লাইক ভার্সন ১.০০ এর জন্য একটা ১.০.১ এর জন্য একটা এইভাবে অনেক গুলো ফোন্ডারের কপি করতে হবে যেটা মোটেও কোন ইফিসিয়েন্ট কাজ নাহ । আর সেটা যদি মাল্টিপল ডেভলপার অথবা প্রোগ্রামার একই প্রজেক্ট এ কাজ করেন তাহলে ভার্সন আর কোড ম্যানেজমেন্ট আর বেশি ঝামেলার হয়ে যায়

<video id="video-2639-3" width="640" height="360" preload="metadata" controls="controls"><source type="video/mp4" src="https://res.cloudinary.com/aldinn/video/upload/v1654900715/blog/git_02_eyhlcz.mp4?_=3"></source><a href="https://res.cloudinary.com/aldinn/video/upload/v1654900715/blog/git_02_eyhlcz.mp4">https://res.cloudinary.com/aldinn/video/upload/v1654900715/blog/git_02_eyhlcz.mp4</a></video>

এখন আপনি প্রজক্ট মার্জ করতে গেলে অথবা প্রজেক্ট শেয়ার করতে গেলে আপনার টিমমেট এর সাথে তাহলে আপনাকে ইমেইল অথবা অন্য কোন ম্যাকানিজম ব্যাবহার করতে হবে যেটি সফটওয়্যার ইঞ্জিনিয়ারিং মোটেও সুখকর নয় । ঠিক এই জায়গায় গিট আমাদের এই কাজ গুলো করে । আমাদের এইসব প্রব্লেম গুলো সল্ভ করে ।

ভার্শন কন্ট্রোল সিস্টেম এর মাধ্যমে আমরা দুইটা কাজ করতে পারি

- Track History
- Work Together 

![git](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxMDI0IiBoZWlnaHQ9IjYxOCI+PHJlY3Qgd2lkdGg9IjEwMCUiIGhlaWdodD0iMTAwJSI+PGFuaW1hdGUgYXR0cmlidXRlTmFtZT0iZmlsbCIgdmFsdWVzPSJyZ2JhKDE1MywxNTMsMTUzLDAuNSk7cmdiYSgxNTMsMTUzLDE1MywwLjEpO3JnYmEoMTUzLDE1MywxNTMsMC41KSIgZHVyPSIycyIgcmVwZWF0Q291bnQ9ImluZGVmaW5pdGUiIC8+PC9yZWN0Pjwvc3ZnPg==)

আবার ভার্শন কন্ট্রোল সিস্টেম দুই প্রকার

1. সেন্ট্রালাইজড 
2. ডিস্ট্রিবিউটেড 

#### সেন্ট্রালাইজড সিস্টেম

![git](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxOTIwIiBoZWlnaHQ9IjEwODAiPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxhbmltYXRlIGF0dHJpYnV0ZU5hbWU9ImZpbGwiIHZhbHVlcz0icmdiYSgxNTMsMTUzLDE1MywwLjUpO3JnYmEoMTUzLDE1MywxNTMsMC4xKTtyZ2JhKDE1MywxNTMsMTUzLDAuNSkiIGR1cj0iMnMiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiAvPjwvcmVjdD48L3N2Zz4=)

সেন্ট্রালাইজড সিস্টেম এ সকল টিম মেম্বার একটি সেন্ট্রাল সার্ভারে কানেক্ট থাকে যাতে তারা লেটেস্ট কোড এর আপডেট পায় এবং তাদের চেইঞ্জেসটা সকল এর সাথে শেয়ার করার জন্য । [Subversion](https://subversion.apache.org/ "Subversion"), [Microsoft Foundation Server](https://azure.microsoft.com/en-us/services/devops/server/ "Microsoft Foundation Server") এই সিস্টেম এর একটি উদাহরন ।

![](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxOTIwIiBoZWlnaHQ9IjEwNzkiPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxhbmltYXRlIGF0dHJpYnV0ZU5hbWU9ImZpbGwiIHZhbHVlcz0icmdiYSgxNTMsMTUzLDE1MywwLjUpO3JnYmEoMTUzLDE1MywxNTMsMC4xKTtyZ2JhKDE1MywxNTMsMTUzLDAuNSkiIGR1cj0iMnMiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiAvPjwvcmVjdD48L3N2Zz4=)

সেন্ট্রালাইজড সার্ভার এর সমস্যা হল কোন ভাবে সার্ভার ডাউন বা সার্ভার এর সাথে ডিস্কানেক্ট হয়ে গেলে আমরা আর কোলাবোরেট করতে পারব নাহ আর কোড এর স্ন্যাপশট গুলো সেন্ড করতে পারব নাহ । মানে কোন সিঙ্গেল ফেইলুর হলেই আমাদের কোডিং অফ রাখতে হতে পারে । সার্ভারে অনলাইনে আসা পর্যন্ত আমাদের অপেক্ষা করতে হবে ।

#### ডিস্ট্রিবিউটেড সিস্টেম 

ডিস্ট্রিবিউটেড সিস্টেম এ আমাদের আবার এই সমস্যা নেই । প্রত্যেক টিম মেম্বার এর লোকাল মেশিন এ তাদের প্রজেক্ট হিস্ট্রি থাকে ফলে আমরা লোকালি সব কোড স্ন্যাপ্সহট গুলো লোকালি স্টোর করতে পারি ।

![](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxOTIwIiBoZWlnaHQ9IjEwODAiPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxhbmltYXRlIGF0dHJpYnV0ZU5hbWU9ImZpbGwiIHZhbHVlcz0icmdiYSgxNTMsMTUzLDE1MywwLjUpO3JnYmEoMTUzLDE1MywxNTMsMC4xKTtyZ2JhKDE1MywxNTMsMTUzLDAuNSkiIGR1cj0iMnMiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiAvPjwvcmVjdD48L3N2Zz4=)

যদি আমাদের সার্ভার অফলাইনে থাকে তাও আমরা আমাদের প্রজেক্ট ডিরেkটলি সবার সাথে সিংক্রোনাইজ করতে পারি । [Git](https://git-scm.com/ "Git ")& [Mercurail](https://www.mercurial-scm.org/ "Mercurail ")এই সিস্টেম এর উদাহরন

![](data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxOTIwIiBoZWlnaHQ9IjEwODAiPjxyZWN0IHdpZHRoPSIxMDAlIiBoZWlnaHQ9IjEwMCUiPjxhbmltYXRlIGF0dHJpYnV0ZU5hbWU9ImZpbGwiIHZhbHVlcz0icmdiYSgxNTMsMTUzLDE1MywwLjUpO3JnYmEoMTUzLDE1MywxNTMsMC4xKTtyZ2JhKDE1MywxNTMsMTUzLDAuNSkiIGR1cj0iMnMiIHJlcGVhdENvdW50PSJpbmRlZmluaXRlIiAvPjwvcmVjdD48L3N2Zz4=)

এই সব গুলোর মোড [গিট](https://git-scm.com/ "গিট ")পৃথিবির সব থেকে জনপ্রিয় ভার্শন কন্ট্রোলিং সিস্টেম । কেননা ইহা

1. ফ্রি
2. ওপেন সোর্স 
3. সুপার ফাস্ট 
4. স্কেলেবল
5. সবচেয়ে সহজ ব্রাঞ্চিং এন্ড মার্জিং 

পৃথিবির ৯০% এর বেশি সফটওয়্যার ডেভলপমেন্ট হয়েছে গিট ইউজ করে । তাই প্রায় সব জব ডেস্ক্রিপশন এ গিট মাস্ট এড থাকে । যদি আপনি একটু জব খুজতেসেন অথবা জব করার পরিকল্পনা আছে তাহলে আপনি অবশ্যি গিট আপনার স্কিল বাকেট এ এড করতে হবে হবে সুতরাং দেরী নাহ করে আজই শিখা শুরু করে দিতে পারেন ।

[পরবর্তী পোস্ট](https://blog.aldinn.com/using-git/ "পরবর্তী পোস্ট")

রিসোর্স সমুহ:

1.  [official Git project site](https://git-scm.com/) 
2.  [ProGit book](http://git-scm.com/book)
3.  [Git command list](https://git-scm.com/docs)
4. [on-demand training courses](https://skills.github.com/)
5. [on-demand training courses](https://skills.github.com/)
6. [online Git course](https://www.pluralsight.com/courses/code-school-git-real)
7. [Top 30 Git Commands You Should Know To Master Git CLI | by Tara Prasad Routray | Level Up Coding (medium.com)](https://medium.com/gitconnected/top-30-git-commands-you-should-know-to-master-git-cli-f04e041779bc)
8. [Git commands nobody has told you. Git plays an important role in our… | by Svetloslav Novoselski | Apr, 2022 | Bootcamp (medium.com)](https://medium.com/design-bootcamp/git-commands-nobody-has-told-you-cd7025bea8db)

The post [গিট কি এবং কেন ? (What is Git?)](https://blog.aldinn.com/what-is-git/) appeared first on [Aldinn Rocks](https://blog.aldinn.com).