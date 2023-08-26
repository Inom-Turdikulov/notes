---
canonicalUrl: https://www.youtube.com/watch?v=R5ON3iwx78M
date: '2023-08-22'
tags:
- research
- inbox
---

# The Magic of LRU Cache (100 Days of Google Dev)

Here’s a common problem that I’m sure you’ve run into: It’s time to load a new bitmap for your apps’ social media stream, or whatever, but you're out of memory.  You can’t load in the new bitmap, without first destroying one of the existing bitmaps already in memory. But, which one should you get rid of?

Well, as Colt McAnlis, points out, you could learn 60 years of history of Cache replacement algorithms; that’ll help.. or, you could just use Android’s LRUCache container.

This container keeps a list of objects, and ranks them based upon how many times they’ve been accessed. When it’s time to evict one of them (to make space for a new object) the LRUCache already knows which ones to get rid of. All done without you having to worry about any of it.

100 Days of Google Dev / 100 developer videos over 100 days / GoogleDev100

Watch more Android Performance Patterns here: http://goo.gl/4ZJkY1
Join the G+ Community here : http://goo.gl/g7mxmI
Subscribe to the Google Developers channel here: http://goo.gl/mQyv5L