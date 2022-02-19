+++
author = "Loris Scandurra"
title = 'My lunilo.live journey'
date = "2021-03-08"
description = 'I talk about my first startup experience'
disableComments = true
+++

On the 10th of November 2020, a friend added me to a group call to discuss a startup idea. It was my friend, a guy I didn't know yet, and me in the group call. The guy I didn't know, named Luzius, had the idea to bring local artists, entertainers, comedians, performers to the digital age. He had this idea because of the Corona restrictions. Not only restaurants and shops were hit hard by this but also performers. They couldn't perform in front of big crowds or any crowds anymore.  
So the idea was to give them a platform to perform live. YouTube and Twitch don't address this kind of artist because you need a huge following to survive on those platforms. So our idea was to put a paywall for the live performances. So we started the project with high hopes and dreams. The name of the platform was lunilo.live.

## The Start

I started programming the platform. I was in charge of the whole backend and frontend development. We wanted to go live with our platform as quickly as possible to get first reactions and feedback. So to save time, we used solutions like AWS IVS for the live streaming part. This way, we already had a streaming backend. The rest of our backend programmed using node.js with apollo-server, a GraphQL framework. For the database, we were using MongoDB Atlas. And the frontend was realized using Vue.js. Frontend and backend were containerized and ran on the Google Cloud Kubernetes Platform.<br>I programmed all of this in my spare time, so in the evening and on the weekend. Because we wanted to go to market quickly, we took all possible shortcuts. Still, we paid attention not to create any big road blocks if we needed to scale rapidly in the future.

## Our first artist

My team members were busy looking for artists interested in doing a live stream on our platform and preparing everything around the platform and live stream. They were the sale and the product owner of the team.  
We had many artists interested in a platform like that, but none of them were ready to take on the risk of being the first to try such a format on our new platform. Too big was the fear of disappointing fans with a terrible stream experience or a format that doesn't work online. So we searched for artists prepared to take this risk and go live with us.  
In January, we found an artist couple willing to go this way with us. Their name Schreiber vs. Schneider. They just published their new book and wanted to do a reading. So we had our first artists ready to perform, and the date of the event was Valentines' Day, the 14. February.

## The deadline

Now we had two weeks to provide an MVP. Because they wanted to do a first test event on the 6. February. So the pressure was there to deliver. I worked like crazy those two weeks. I stayed up late almost every night to progress the code. On the 5th of February, we tested the platform and did a production deployment. We still had many changes to our product, so we pulled an all-nighter and finished just in time for the test event.  
The test event went smoothly, and everybody participating in the test was satisfied with the result. We even got [mentioned](https://www.badenertagblatt.ch/aargau/baden/bad-zurzach-geheimnissen-der-liebe-auf-der-spur-schreiber-schneider-kommen-in-die-stuben-ihrer-zuhoerer-ld.2095750) on a local news site. With this, we proved that our platform works, and we could proceed with the event on the 14th of February.

## Our first real live stream

Before our first live stream on the 14th of February, we improved the user interface. We also implemented a one-way chat for the audience to interact with the artist. We also advertised the event on different channels. We sold over 100 tickets for the event, which was quite a surprise for us and the artists. The 14th came along, and we delivered a live stream with no significant hiccups. A small number of people had an issue watching the live stream. However, we later found out they were still using Internet Explorer (Internet Explorer should be banned from the Internet). All in all, it was a major success on our site and for the artists.

## The End

Sadly, this was the last live stream I participated in as a member of lunilo. We split up because of differences in the founding team. Now only one team member remains to advance the platform.  
All in all, it was a positive experience for me, and we sold tickets and had a successful live stream on the platform. I took my learnings from it and will approach the next big idea with more experience.