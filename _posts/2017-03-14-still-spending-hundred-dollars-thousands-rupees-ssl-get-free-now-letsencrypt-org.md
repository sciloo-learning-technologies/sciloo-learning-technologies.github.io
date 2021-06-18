---
id: 444
title: 'Still spending hundred dollars or thousands rupees on SSL &#8211; Get it free now on letsencrypt.org'
date: 2017-03-14T01:34:46+05:30
author: admin@sciloo.com
layout: post
guid: https://sciloo.com/?p=444
permalink: /2017/03/14/still-spending-hundred-dollars-thousands-rupees-ssl-get-free-now-letsencrypt-org/
colormag_page_layout:
  - default_layout
dsq_thread_id:
  - "5629474761"
categories:
  - Startups
  - technology
tags:
  - encryption
  - security
  - SSL
---
Companies always thrive to satisfy their customers and it becomes more important in the online business where huge numbers of online frauds are being reported daily. These can range starting from the data theft to the money theft to hacking the complete websites.

Online experience should be safe for our users and SSL encryption is one major step towards this goal. It gives assurance to your customers that their data is safe from hackers and eavesdroppers.

But if you see, setting up SSL is a costly affair. People are spending 100s $ and 1000s ₹ on SSL certificates and setup cost. See the screenshot below for one such SSL certificate pricing for the Indian market. It becomes more costly if you need separate SSL certificates for each of your subdomains.

<img loading="lazy" class="alignnone wp-image-445 size-large" src="http://sciloo.com/wp-content/uploads/2017/03/sslratesgodaddy-1024x516.png" alt="" width="800" height="403" /> 

People have the basic notion in their mind that setting up SSL for their website is a tedious task and it belongs to experts. But letsencrypt.org has changed this perception by providing the SSL for the free and available provision of an easy setup either through the [command line](http://github.com/certbot/certbot) or plugins (example [wp-encrypt](http://wordpress.org/plugins/wp-encrypt/) for WordPress). You can have free SSL certificates for all your subdomains absolutely free.

There are plentiful resources on using the command line.

please be an explorer and join the dots you find on the way to make a clear picture. This is the best way to learn.

Setting up the SSL on a web server requires certain technicalities such as modifying the vhosts file to add redirection code for HTTP to HTTPS. Then adding the paths to the certificates downloaded from letsencrypt.org.  The web server should also be listening on 443 port to make SSL work. wp-encrypt plugin can do most of the work itself such as downloading certificates to the local path and then the user has to follow the steps above.

As of now, this certificate expires every 90 days after which you have to renew it &#8211; either manually from the command line (automate it using cron job, etc.) or automatically using the plugin.

Search engines worldwide especially [google have started giving more importance to the links with https](http://webmasters.googleblog.com/2014/08/https-as-ranking-signal.html) (having SSL layer) protocol, it becomes necessary to switch to SSL, the sooner the better.

One interesting thing about these certificates is they are accepted in all the browser and gets A rating on ssl [test benchmarks](http://www.ssllabs.com/ssltest/). Check the sample report below. Please share your thoughts on the topic in the comment section.<img loading="lazy" class="alignnone wp-image-447" src="http://sciloo.com/wp-content/uploads/2017/03/ssltest.png" alt="" width="800" height="290" />

See the [growth](http://letsencrypt.org/stats/) of certificates issued by letsencrypt.org over the past few years below. It is growing ~5 M new certificates per month and ~1 M new domains per month.

<img loading="lazy" class="alignnone wp-image-448" src="http://sciloo.com/wp-content/uploads/2017/03/growth.png" alt="" width="800" height="383" /> 

[1] help &#8211; http://letsencrypt.org/docs/