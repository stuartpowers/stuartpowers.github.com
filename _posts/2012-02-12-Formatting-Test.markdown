---
layout: post
title: Formatting Test...
excerpt: taking a peak at this
---

{% highlight python %}
for i,p in enumerate(pages):
    root = lxml.html.fromstring(p)
    for l in root.iterlinks():
        if l[1] == 'href':
            if l[0].text and l[2].startswith('/app/id') and l[2].endswith('/'):
                print '%s' %i +'\t'+ 'http://iphoneapplicationlist.com%s' %l[2]+'\t'+l[0].text.encode('utf-8','replace') + '\t',
                id = ''.join(l[2].split('/')[-2][3:])
                print 'http://itunes.apple.com/WebObjects/MZStore.woa/wa/viewSoftware?id=%s&mt=8' %id
{% endhighlight %}



