---
layout: page
title: About
permalink: /about/
---


Hi, I’m Dakota McKay, and ever since I first learned how make [European 4-in-1]({{ site.baseurl }}{% post_url 2023-02-12-european_4_in_1 %}) in <abbr title="" id="yearsMail">August 2022</abbr>, I have been fascinated with chainmail. I first discovered non-armor weaves in December and decided to learn how to make more. On <abbr title="" id="yearsBlog">January 25, 2023</abbr> I decided to start uploading the weave samples/projects I made to this website, and ever since then I have been showcasing a new weave/project weekly.

I hope you enjoy the showcased <abbr title="" data-tippy-content="Check out the <b><a href=&quot;{{site.baseurl}}/gallery/&quot;>Gallery</a></b>">weaves/projects</abbr>, have fun seeing the chainmail, or even <abbr title="" data-tippy-content="Check out the <b><a href=&quot;{{site.baseurl}}{{site.glossary_page}}&quot;>Glossary</a></b> or <b><a href=&quot;{{site.baseurl}}{{site.tag_page}}#tutorial&quot;>Tutorial Posts</a></b>">learn</abbr> a thing or two. Please feel free to [reach out]({{ site.baseurl }}/contact/) if you enjoy the content, learned anything, or just want to say hello.

<!-- Dynamically set the number of years I have been making chainmail on page load -->
<script>
    const startMail = new Date('2022-08-27T13:00:00');
    const startBlog = new Date('2023-01-25T12:00:00');
    const now       = new Date();
    let yearsMail = ((now - startMail) / (1000*60*60*24*365.25)).toFixed(1);
    let yearsBlog = ((now - startBlog) / (1000*60*60*24*365.25)).toFixed(1);
    document.getElementById('yearsMail').setAttribute('data-tippy-content', `${yearsMail} years ago`);
    document.getElementById('yearsBlog').setAttribute('data-tippy-content', `${yearsBlog} years ago`);
</script>
