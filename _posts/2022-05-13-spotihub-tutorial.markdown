---
layout: single
title:  "SpotiHub Tutorial"
date:   2022-05-13 18:00:04 +0020
header:
  overlay_image: /assets/images/blog/spotihub/SpotiHub-Banner.png
  overlay_color: "#000"
  overlay_filter: "0.7"
categories:
  - SpotiHub 
  - Projects

tracked-untracked-playlist-gallery:
  - url: /assets/images/blog/spotihub/SpotiHub-Untracked-Playlist-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Untracked-Playlist-Tutorial-768x514.png
    alt: "Untracked Playlist"
    title: "Untracked Playlist"
  - url: /assets/images/blog/spotihub/SpotiHub-Tracked-Playlist-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Tracked-Playlist-Tutorial-768x514.png
    alt: "Tracked Playlist"
    title: "Tracked Playlist"

merging-a-branch-gallery:
  - url: /assets/images/blog/spotihub/SpotiHub-Switch-Branch-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Switch-Branch-Tutorial-768x514.png
    alt: "Switch Branch"
    title: "Switch Branch"
  - url: /assets/images/blog/spotihub/SpotiHub-Merge-Branch-1-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Merge-Branch-1-Tutorial-768x514.png
    alt: "Initialise Merge"
    title: "Initialise Merge"
  - url: /assets/images/blog/spotihub/SpotiHub-Merge-Branch-2-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Merge-Branch-2-Tutorial-768x514.png
    alt: "Confirm Merge"
    title: "Confirm Merge"
  - url: /assets/images/blog/spotihub/SpotiHub-Commits-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Commits-Tutorial-768x514.png
    alt: "View Commit List"
    title: "View Commit List"

pull-request-gallery:
  - url: /assets/images/blog/spotihub/SpotiHub-Pull-Request-1-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Pull-Request-1-Tutorial-768x514.png
    alt: "Create a Pull Request"
    title: "Create a Pull Request"
  - url: /assets/images/blog/spotihub/SpotiHub-Pull-Request-2-Tutorial-2048x1370.png
    image_path: /assets/images/blog/spotihub/SpotiHub-Pull-Request-2-Tutorial-768x514.png
    alt: "Check the status of a PR"
    title: "Check the status of a PR"
---
This post is intended to teach you how to use SpotiHub. 

For more information about the project go to the [SpotiHub blog post](/2022/05/13/introducing-spotihub.html). Be sure to first check out the interactive tutorial in [SpotiHub](http://spotihub.com) itself. This blog post is meant as reference when you finished the interactive tutorial.

## Introduction

In this tutorial you will learn how to use SpotiHub to manage your own playlists and collaborate with friends to create playlists together. We will cover these topics:

*   [Overview of the SpotiHub Homepage](#overview)
*   [Fork a playlist](#forking)
*   [Create a new branch](#branching)
*   [Create a commit](#committing)
*   [Merge a branch back into main](#merging)
*   [Open a Pull Request](#pull-request)

These are the same topics, that are also covered by the interactive tutorial

## Overview of the SpotiHub Homepage

Let's first take a look at the SpotiHub homepage when you log in.

![SpotiHub Homepage]({{ '/assets/images/blog/spotihub/SpotiHub-Homepage-Tutorial-1200x803.png' | absolute_url }})

The SpotiHub homepage with tracked playlists and the tutorial

We can see an overview of all our playlists in two representations: big images in the main section and a searchable list on the side. If you have not completed the tutorial you should see in the bottom left corner. Also notice the green dot next to the first playlist. This dot indicates, that this playlist is tracked by SpotiHub. It appears once you create the first commit in the playlist. We can also see the difference between a tracked and an untracked playlist when we inspect the playlist details by either clicking one of the playlist covers or a playlist in the list. There is another difference, depending on whether it is your own playlist or the playlist of a friend, but we will look into that later.

{% include gallery id="tracked-untracked-playlist-gallery" caption="Untracked and tracked playlist. (Click to enlarge)" %}

The untracked playlist only allows you to create your first commit. The tracked playlist shows you the current branch in the pill shaped button (_main_), next the most recent commit (_Initial Commit_) and an action bar. We will go through a typical usage scenario to learn more about each of these actions.

## Forking a Playlist

In this example we want to work on a friends playlist, so we need to create our own fork. Our fork allows us to make changes to the playlist without affecting the original. Don't worry, once we are happy with our playlist will propose an update to the original playlist!

When we view the details of a friends playlist we can create a fork by clicking on the green "Fork" button by the playlist title. You will be redirected to your own fork automatically.

{% include figure image_path="/assets/images/blog/spotihub/SpotiHub-Fork-Playlist-Tutorial-1200x803.png" alt="Fork a playlist by clicking the Fork button" caption="Fork a playlist by clicking the Fork button." %}

## Creating a Branch

Next up we are going to create a new branch. Branches are essentially lightweight copies of our playlist where we can try out new songs. Once we are sure we want to permanently keep these songs we can merge them into our main playlist. If we are unhappy with our changes we can easily switch back to our main branch which is still in our previous state.

To create a branch we click on the "New Branch" button and enter a branch name in the input field. You can come up with any name you like, like "Summer Additions" or "Music from Vacation".

Afterwards we click "Create" to create and check out the new branch. We can see the branch name in the pill shaped button by the playlist description.

{% include figure image_path="/assets/images/blog/spotihub/SpotiHub-Create-Branch-Tutorial-1200x803.png" alt="Create a branch by selecting the New Branch tab, entering a name and clicking create." caption="Create a branch by selecting the New Branch tab, entering a name and clicking create." %}

## Committing

Now it's time to make some modifications to your playlist by adding new songs!

You add Songs on Spotify like you always do, either by opening the Spotify App on your phone or laptop, or on the web by clicking on the "Open in Spotify" Link under the playlist title.

SpotiHub doesn't automatically refresh the playlist so we need to reload the page if we made any external changes.

Afterwards we can see newly added songs in the list of songs with a green highlight on the left of the row. This indicates, that these song were newly added and have not been saved by a commit yet. If you remove songs they are highlighted in red.

Now it's time to make our first commit. Commits are essentially save points for your playlists. You always need to create a commit when you switch a branch or create a Pull Requests, otherwise your changes won't be saved. We must click on the "New Commit" tab and enter a commit message. This is the place where you can come up with creative ways to describe your changes to the playlist. For example: "Added my favourite song from when I was visiting Colombia :)"

Now we can press "Commit" to commit our changes. We can see that the green indicator next to the song disappears and our commit message shows up at the top of the page.

{% include figure image_path="/assets/images/blog/spotihub/SpotiHub-Create-Commit-Tutorial-1200x803.png" alt="Create a commit by selecting the New Commit tab, entering a commit message and clicking Commit." caption="Create a commit by selecting the New Commit tab, entering a commit message and clicking Commit." %}


## Merging a branch

As we mentioned before, the changes we made live on a separate branch of the playlist. This allows us to try out different music without changing our main playlist.

But when we are happy with our new additions, we need to merge these changes back to our main branch. To achieve this we first need to checkout the main branch. We can go to the "Switch Branch" tab and select the main branch. Then we click "Switch" to check it out. In your official Spotify App you will always see the version of the playlist, that is currently checked out.

Now our playlist looks like when we forked it, before we made any changes ourselves.

In order to see our changes we need to merge the branch we created earlier. We select the "Merge Branch" tab and select the name of the branch we created earlier. After click "Merge" we will be redirected to a new page.

Here we can see how our playlist will look once we're done merging. Merging means that we add all the commits, so the save points, that we created on a different branch, on top of our current branch.

Once we're happy with the result we merge the branch by clicking "Merge". If we're unhappy we can go back, switch to our branch, make changes to the playlist and create a new commit on top of the old commit. After we merged we will see a Merge Commit by the playlist description, which was created by SpotiHub. When we click on it we can see all the commits that have been created on this playlist.

{% include gallery id="merging-a-branch-gallery" caption="Steps for merging a branch." %}

## Creating a Pull Request

Now we have all our updates on our main branch of our playlist. But how great would it be if the original creator could also benefit from our changes!

We can create a Pull Request to propose our changes to the original playlist creator, so he can decide to merge our changes to his own playlist.

We go to the "Create Pull Request" tab and select the "SpotiHub/main" branch.

Now we only need to click "Create" and we can see that our Pull Request is in state _open_. Once the creator has merged the PR we will see our changes on his playlist.

{% include gallery id="pull-request-gallery" caption="Opening a Pull Request." %}

## Merging the Upstream

One bonus feature, that is not covered by the interactive tutorial (yet) is the possibility to merge new changes of the original playlist into our fork. When the original creator adds new commits to his playlist a "Merge Upstream" tab will appear where you can merge his changes into your own fork.

{% include figure image_path="/assets/images/blog/spotihub/SpotiHub-Merge-Upstream-Tutorial-1200x803.png" alt="Merge new commits of the upstream playlist." caption="Merge new commits of the upstream playlist." %}

## Conclusion

Now it's time to go back to [SpotiHub](http://spotihub.com) to create more playlists! Checkout the [Announcement Blog Post](/2022/05/13/introducing-spotihub.html), if you haven't already. If you have any questions or comments please reach out at [hello@spotihub.com](mailto:hello@spotihub.com). For any bugs or issues please use [issues@spotihub.com](mailto:issues@spotihub.com).