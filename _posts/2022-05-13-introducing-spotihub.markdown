---
layout: single
title:  "Introducing Spotihub"
date:   2022-05-13 17:45:38 +0020
categories: spotihub projects
---
About 4 years ago, I was looking for my first serious side project, besides working as a working student and doing my bachelors degree at Hasso-Plattner-Institute. Not with the intention of gaining a big user base or earn money, but rather to create something useful to me personally, that could also be a playground for me to try out and learn new things.

Back in school I was always proud of my iTunes music catalog and playlist collection, which I transferred to Spotify with a heavy heart when I replaced my beloved iPod Classic with an iPhone as my primary music listening device. I am not sure how many playlists I had back then, but currently there are more than 250 in my Spotify library. The feature I enjoyed most, when I switched to a streaming service, was the ability to star my friends playlist, which was so much easier than recreating them in my own iTunes library. And I had always the most recent version!

Unfortunately, soon managing my own playlists using the Spotify apps and "liking" other playlists to add them to my library felt very limiting. As a software engineer I was used to managing projects with version control systems like git and collaborating with my peers using central repository hubs like GitHub. This is were I drew my inspiration for a similar collaborative experience for creating playlists, which became SpotiHub.

## Something Technical

If you are only interested what SpotiHub can do, jump to the [Features](#features).
{: .notice}

On September 26, 2018 I started with my first version of the SpotiHub backend. Since then I worked on it on and off (rewriting it multiple times) with some other projects squeezed in between (see [Kraggl](http://kraggl.com){:target="_blank"}). I can say I definitely learned a lot. To understand git in more detail, I implemented big parts of git in Swift using the excellent [Building Git](https://shop.jcoglan.com/building-git){:target="_blank"} by James Coglan. It helped me implement the algorithms in TypeScript, that SpotiHub uses today! I started out with a REST API, which I replaced with an Apollo Server GraphQL backend in a later rewrite. I tried out patterns in the backend like Inversion of Control and Dependency Injection and learned how to build a frontend with Angular, Angular Material and Apollo Client. I also added a CD pipeline with GitHub Actions, Docker images published in the GitHub container registry and dev and production deployments. Most recently I even added simple monitoring dashboards using DataDog. I can already say, that the 225 hours and 16 minutes I tracked on this project have been worth it, even if it stays a niche product.

## Features

Now I want to showcase some of the features and use cases I imagined when developing SpotiHub. For a detailed introduction on how to use this features please checkout the Tutorial **(TODO(mlichtblau) link to Tutorial)**

### Manage versions of your own Playlists

Sometimes it is useful to have multiple versions of one playlist and be able to easily switch between these versions. Sure you could copy the playlist and make some changes to your copy but then you have another playlist cluttering up your Spotify apps even though in theory it's still the same playlist.

One example of this is my summer playlist. I would like to have one giant playlist where I add my new favourite songs every summer. But to be honest there will always be songs, that we just cannot listen to anymore after we heard them too often. Of course I can delete those, but then they are gone forever. SpotiHub lets me create branches for every single summer, where I can build on the version from last summer and delete as many songs as I like. And when I want to listen to the version from the summer three years ago to bath in nostalgia I can just switch back to my old branch and the playlist will be like I left it back then. Similarly I can switch back to the current version whenever I like.

### Make suggestions to other playlists

Wouldn't it be great if you could make suggestions to your friends playlists but letting them control which songs they would really like to add or remove? If your friends also use SpotiHub, you can fork your friends playlist to make some changes, like adding and removing songs. When you are happy with your changes you can open a Pull Request to suggest these changes to the original creator. The creator now has the chance to merge your changes into the original playlist.

### Keep your own modified version of another playlist

But what happens if the creator doesn't like your changes? You can just keep your version of the playlist and treat it like your own. And when there are new additions to the original playlist you can just merge them back into your own version without loosing your own modifications. Everyone wins!

## Try it out!

If you are interested head to [SpotiHub](http://spotihub.com){:target="_blank"} to try it out! I encourage you to do the tutorial to learn how to use all of SpotiHub's features or checkout the **Tutorial Link** blog post. If you have any questions or comments please reach out at [hello@spotihub.com](mailto:hello@spotihub.com). For any bugs or issues please use [issues@spotihub.com](mailto:issues@spotihub.com).