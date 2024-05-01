---
layout: single
title:  "Introducing Kraggl"
date:   2022-03-16 17:30:52 +0020
categories: kraggl projects
header:
  overlay_image: /assets/images/blog/kraggl/kraggl-header.png
  show_overlay_excerpt: false
  overlay_color: "#000"
  overlay_filter: "0.7"
---

This project took us 45 hours, 23 minutes and 36 seconds. 
At least that's what my time tracking tool tells me. 
Granted, this calculations omits the countless ideas, thoughts and talks Annika and I had since starting this project ten days ago. 
How much time did I spend programming the backend? 
Well, I can't trace that back now. 
With so much to do and so little time, I didn't waste it creating new specific time entries for every task.
And how much time got lost in my calculation, because I forgot to start the timer or was just to absorbed in my work to really care about it? 
Unfortunately there is no way of finding out now. 
But at least we created a new tool, that may or may not avoid this loss of data in the future. 
And it's called **[Kraggl](https://kraggl.lichtblau.io)**...

## Why Kraggl?

Everyone should try time tracking for their work (at least if you listen to [CGPGrey](https://www.reddit.com/r/CGPGrey/) on his Podcast show [Cortex](https://www.relay.fm/cortex), but no one really likes to do it. 
It's tedious work remembering to start a timer when you sit down for work and even worse creating a new one when you switch to another task. 
However, if you use **[Glo Boards](https://www.gitkraken.com/glo)** as your project management tool, you are in luck my friend. 
With the help of Kraggl, we can reduce the burden of accurate time tracking. 
Kraggl directly connects your Glo Boards to your **[Toggl](https://toggl.com)** account, taking away the pain of starting, stopping and categorising your time entries. 

## How does it work?

After signing up for Glo Boards with your GitKraken account and creating a Toggl account you can head over to Kraggl and start connecting them. 
Of course you can also link to existing accounts if you already have them. 
After logging into Kraggl with your GitKraken account you have to enter your Toggl API token. 
The token can be found at the bottom of your Toggl profile page. 
After successfully connecting both accounts, a list of your existing Glo Boards is displayed. 
If you don't have any boards, go ahead and create one in the Glo Boards web app.

{% include figure image_path="/assets/images/blog/kraggl/kraggl1-768x461.png" alt="In the Board Overview you can see how much time you spent on a project." caption="In the Board Overview you can see how much time you spent on a project." %}

To start tracking a board, click on its name and select _⚙️Settings_ on the next page.
After flipping the switch you can choose which columns should be tracked and if you want to use the chatbot. 
The chatbot will comment a _Time Summary_ in your tracked Glo Board cards. 
To correctly categorise the time entries on this board select a Toggl project. 
Lastly we need to set up a webhook in the Glo Board app to notify Kraggl about changes. 
Now your set-up is all done and you don't have to worry about starting and stopping your timers, as long as you use the Glo Board app to manage your tasks.

{% include figure image_path="/assets/images/blog/kraggl/kraggl2-768x191.png" alt="Browse your cards or click _⚙️Settings_ to enable tracking." caption="Browse your cards or click _⚙️Settings_ to enable tracking." %}

Voilà, if you drag a card into a tracked column your Toggl timer starts running. 
Move it into an untracked column and it stops. 
If you enabled the chatbot you can find a summary of the time spent on a card in its comments, after you move it to an untracked column.

{% include figure image_path="/assets/images/blog/kraggl/kraggl3-768x254.png" alt="Kraggl automatically creates and updates comments with a summary of the time you spent on the card." caption="Kraggl automatically creates and updates comments with a summary of the time you spent on the card." %}

## Outlook

Unfortunately we didn't have time to integrate all of our ideas yet. 
But the work on Kraggl isn't over. Our next task is to integrate _Pause Labels_. 
They automatically stop a timer if assigned to a card, even if the card is currently in a tracked column. 
As soon as you remove the label the timer continues. As of now Kraggl is mostly optimised for single users. 
Adding team functionalities will be another powerful improvement. 
If you have any ideas, big or small, feel free to comment below or head over to [GitHub](https://github.com/mlichtblau/kraggl/issues) and create a feature request.

## Development

If you want to check out the code for Kraggl it is open sourced on [GitHub](https://github.com/mlichtblau/kraggl). 
Feel free to contribute! We use a simple Javascript Express server that consumes the Glo Board and Toggl APIs and provides the interface for the user. 
The database is a SQLite database, that we consider moving to a document store like MongoDB. 
If you have any comments or suggestions feel free to contact us. We are looking forward to hear from you.

_We hope you like it_,

Marius Lichtblau ([mlichtblau](http://github.com/mlichtblau), [@lichtblau](https://twitter.com/lichtblau))

Annika Baldi ([bisbaldi](http://github.com/bisbaldi))

[YouTube](https://youtu.be/uk9bi9fxvlo)