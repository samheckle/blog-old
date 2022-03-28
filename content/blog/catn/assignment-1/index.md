---
title: 'a generated narrative device'
date: "2022-01-30"
description: "sketch #1 documentation"
---

[link to code](https://github.com/theheckle/catn/tree/master/assignment-1)

## Premise -- Two Sentence Horror

On reddit there exists a subreddit called [Two Sentence Horror](https://www.reddit.com/r/TwoSentenceHorror/top/?t=month) that takes in a title and a body to create a short story that is within two sentences. Basically what I did was create a horror generator that separates these basic parts to create a new story.

## Some Outputs

“Dad…,the man that’s been standing outside my window is gone,” I whispered shakily into the phone. 

I squeezed my eyes shut and told myself it was all in my head, but the slimy footprints staining the carpet the next morning made it clear I would never be allowed to forget what I've done.

----

As I was falling asleep, my girlfriend asked if she could be blunt with me, and groggily I said "Yes." 

The other thing I've learned is that it's super hard to hold a cat down with one hand while holding a melonballer in the other.

----

I tightened my legs around him, letting out a shudder of delight, and gazed deeply into his eyes as I brought my mouth down to his. 

“She’s my half-sister now” I said as I dropped my axe

----

## Using the Reddit API

I created this in JavaScript using a Node.js backend. Specifically the tools I used were this integration of [snoowrap](https://github.com/not-an-aardvark/snoowrap/blob/master/src/README.md) which allows me to use a JS port of the python based api. 

From there, I had to create an authorization token to allow the REST requests to go through using the [reddit dev app console](https://www.reddit.com/prefs/apps)

I created my own environment file to host these variables. Then I got to work using the call and parsing the data returned from the "hot" posts on the particular subreddit I wanted. This will be continuously updated if I choose eventually to host this somewhere.