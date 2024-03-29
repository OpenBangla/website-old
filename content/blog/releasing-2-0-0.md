---
title: "ওপেনবাংলা কিবোর্ড ২.০.০ - প্রকাশিত!"
date: 2020-10-01
author: Muhammad Mominul Huque
---

প্রায় ২ বছর পর আপনাদের কাছে ওপেনবাংলা কিবোর্ডের ২.০.০ সংস্করণ এনে দিতে পেরে আমরা খুবই আনন্দিত। তবে আগেই বলে দিতে চাই, এযাবতকালে ওপেনবাংলা কিবোর্ডের অন্যতম বড় রিলিজ হতে চলেছে এটি!
<!--more-->

পারফরম্যান্সের দিকে লক্ষ্য রেখে এবারে লেআউট হ্যান্ডলিং কোড [সম্পূর্ণ নতুন করে][107] লেখা হয়েছে। এখন ওপেনবাংলা কিবোর্ডের অভ্র ফনেটিক অন্যান্য অভ্র ফনেটিক ইমপ্লেমেন্টেশন থেকে অনেক দ্রুত। ওপেনবাংলা কিবোর্ডের [অভ্যন্তরীণ লেআউট ফরম্যাট][143] পরিবর্তন করা হয়েছে এবং ব্যবহারকারীর ডেটা ফাইল সেভ করার স্থান বদলানো হয়েছে। এখন ওপেনবাংলা কিবোর্ড ব্যবহারকারীর ডেটা ফাইল [XDG Base Directory specification][xdg] অনুযায়ী সেভ করে। পূর্ববর্তী সংস্করণের ব্যবহারকারীদের সুবিধার জন্য ডেটা মাইগ্রেশন সুবিধা যোগ করা হয়েছে। ওপেনবাংলা কিবোর্ড ইন্সটল করার পর টপবার চালালেই স্বয়ংক্রিয়ভাবে ব্যবহারকারীর ডেটা নতুন স্থানে ও নতুন ফরম্যাটে পরিবর্তন করে নেবে।

ওপেনবাংলা কিবোর্ডের ইন্সটলেশন পদ্ধতি খুবই সহজ করা এই সংস্করণের রোডম্যাপে অন্যতম চাওয়া ছিল আমাদের। [Bintray](https://bintray.com/) এর সহায়তায় উবুন্টু, ডেবিয়ান, ফেডোরা, আর্চ লিনাক্সের বিভিন্ন সংস্করণের জন্য আমরা প্যাকেজ বিতরণ করছি এবং প্যাকেজগুলো GPG signed করা তাই নিরাপত্তাও এখন সর্বোচ্চ! ইন্সটলেশন পদ্ধতি দেখতে [এখানে ভিজিট করুন।](https://openbangla.github.io/install/)

ওপেনবাংলা কিবোর্ডের ফিচারগুলোর ওপর নজর রেখে তৈরি করা হয়েছে এই চমৎকার ওয়েবসাইটটি। একজন নতুন ব্যবহারকারী যেন প্রথমেই ওপেনবাংলা কিবোর্ড সম্পর্কে ভাল ধারনা পেতে পারেন সেই দিকটি আমরা বিবেচনা করেছি।

### অভ্র ফনেটিক
এবারের সংস্করণ অভ্র ফনেটিকের সাজেশন [প্রায় ১.২ গুন দ্রুততার সাথে][3] প্রদর্শন করবে ব্যবহারকারীর সামনে। সাথে সাজেশন লিস্টে ব্যবহারকারীর লেখা ইংলিশ শব্দও অন্তর্ভুক্ত থাকবে।
{{< figure src="/images/blog/phonetic-english.png" >}}

সাজেশন লিস্ট প্রদর্শনকালে অ্যারো কী চাপলে হঠাৎ ওপেনবাংলা কিবোর্ড [ক্রাশ হবার ত্রুটির][123] সমাধান করা হয়েছে। এছাড়াও কিছু বিশেষ ক্ষেত্রে অটো কারেক্ট সাজেশন ও অন্যান্য সাজেশনের ক্রমবিন্যাস বদলে যাবার ত্রুটিও ঠিক করা হয়েছে।
### ফিক্সড কিবোর্ড লেআউট (প্রভাত, জাতীয়, ইত্যাদি)
এখন প্রভাত কিংবা অন্যান্য ফিক্সড কিবোর্ড লেআউটে লিখলে সম্ভাব্য শব্দ সমূহের সাজেশন লিস্ট প্রদর্শন করবে:
{{< figure src="/images/blog/fixed-suggestion.png" >}}

এছাড়া [যফলা লেখার ত্রুটি][117], [ব্যাক স্লাশ(\\) কী কাজ না করা][98] ত্রুটির সমাধান করা হয়েছে।
এবারের সংস্করণে লেআউটের **AltGr** এবং **Shift AltGr** লেয়ার কিবোর্ডের **ডানপাশের Alt** এবং **Shift** + **ডানপাশের Alt** কী [চেপে টাইপ করা][152] যাবে। পূর্ববর্তী সংস্করণে শুধু Ctrl + Alt এবং Shift + Ctrl + Alt কী চেপে টাইপ করার ব্যবস্থা ছিল। 

ওপেনবাংলা কিবোর্ডের সাথে বিতরণ করা লেআউটগুলো এখন [আকারে ৫৮% ছোট][143]। এখন আলফা নিউমেরিক কীগুলোও AltGr লেয়ারে টাইপ করা যাবে। ব্যবহারকারীর সিস্টেম লেআউট Qwerty না হয়ে অন্য লেআউট হলে ওপেনবাংলা কিবোর্ড দিয়ে সে কীবোর্ডের মাধ্যমে লেখার [সক্ষমতা যোগ করার কাজ][143] সম্পূর্ণ হয়েছে, এবং তা অভ্র ফনেটিক ও ফিক্সড কীবোর্ড লেআউট উভয়ের জন্যই প্রযোজ্য!
### ইউজার ইন্টারফেস
ওপেনবাংলা কিবোর্ডের এবারের সংস্করণে ইউজার ইন্টারফেসে অনেক পরিবর্তন আনা হয়েছে:
{{< figure src="/images/blog/user-interface.png" width=98% link=/images/blog/user-interface.png >}}

গুগলের জনপ্রিয় ম্যাটেরিয়াল ডিজাইন আইকনসেট ব্যবহার করা হয়েছে। পূর্ববর্তী সংস্করণে এলোমেলোভাবে ছড়িয়ে থাকা সেটিংস্‌গুলো এখন সব একসাথে নতুন সেটিংস্‌ ডায়ালগে পাওয়া যাবে। লেআউট ভিউয়ার ডায়ালগ নতুন করে ডিজাইন করা হয়েছে, ফলশ্রুতিতে এখন ব্যবহারকারী ইচ্ছেমতন ভিউয়ার ডায়ালগ বড় করে দেখতে পারবেন।
{{< figure src="/images/blog/topbar-moving.gif" >}}

টপবারে এখন আইকন বাটনে ক্লিক করেই টপবার সরানো যাবে সাথেসাথেই এক্সট্রা ইনফর্মেশনের মেনুও পাওয়া যাবে। তাই টপবার এখন আগের তুলনায় বেশ ছোট। টপবারের প্রতিটি বাটন এখন টুলটিপের সাহায্যে দেখিয়ে দিবে তার কাজের বর্ণনা। এছাড়াও টপবার সরাতে গেলে হঠাৎ সেটি উইন্ডো ম্যানেজারের [কিছু বিশেষ অংশে আটকে][153] যাবার [ত্রুটিরও সমাধান][171] রায়েছে।

ওপেনবাংলা কিবোর্ডের নতুন সংস্করণ সম্পর্কে আরও বিস্তারিত জানতে [চেঞ্জলগ দেখুন।](https://github.com/OpenBangla/OpenBangla-Keyboard/blob/master/CHANGELOG.md#200)

### যারা কন্ট্রিবিউট করেছেন (বর্ণানুক্রমে)
* [Adyel Ullahil Mamun](https://github.com/Adyel)
* [Ahmad Hasan Mubashshir](https://github.com/ahmubashshir)
* [Muhammad Mominul Huque](https://github.com/mominul)
* [Sammay Sarkar](https://github.com/bdeshi)


[xdg]: https://specifications.freedesktop.org/basedir-spec/latest
[107]: https://github.com/OpenBangla/OpenBangla-Keyboard/pull/107
[3]: https://github.com/OpenBangla/riti/pull/3
[123]: https://github.com/OpenBangla/OpenBangla-Keyboard/issues/123
[117]: https://github.com/OpenBangla/OpenBangla-Keyboard/issues/117
[98]: https://github.com/OpenBangla/OpenBangla-Keyboard/issues/98
[152]: https://github.com/OpenBangla/OpenBangla-Keyboard/issues/152
[143]: https://github.com/OpenBangla/OpenBangla-Keyboard/pull/143
[153]: https://github.com/OpenBangla/OpenBangla-Keyboard/issues/153
[171]: https://github.com/OpenBangla/OpenBangla-Keyboard/pull/171
