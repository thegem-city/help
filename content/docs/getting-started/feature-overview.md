+++
title = "Feature Overview"
description = "An overview of some of the core features and concepts."
date = 2022-11-03T08:20:00+00:00
updated = 2022-11-03T08:20:00+00:00
draft = false
weight = 13
sort_by = "weight"
template = "docs/page.html"

[extra]
lead = "An overview of some of the core features and concepts."
toc = true
top = false
+++

## The Local Timeline

The local timeline is a feed of posts and activity from the accounts on <a href="https://thegem.city/">thegem.city</a>. It does not include posts and activity from other servers.

<a href="https://thegem.city/">thegem.city</a> is just one of many fediverse servers and because they all communicate with each other, posts and updates can come in from all over the place.

The local timeline can be found here: <a href="https://thegem.city/web/public/local">https://thegem.city/web/public/local</a>.

## The Federated Timeline

The federated timeline is a feed of posts and activity from <a href="https://thegem.city/">thegem.city</a> as well as all of the servers that <a href="https://thegem.city/">thegem.city</a> receives posts from.

When a user on <a href="https://thegem.city/">thegem.city</a> follows or interacts with an account on another server, that server will send updates for that remote account to this server. The federated timeline is sort of link a window into all of the public posts and activity from servers across the fediverse.

The federated timeline can be found here: <a href="https://thegem.city/web/public">https://thegem.city/web/public</a>

## The Fediverse

The fediverse is the collection of all of the servers that implement the activitypub protocol and are connected to one another. This term is used pretty casually to reference how all of the accounts on different servers can interact with each other.

See more:

* <a href="https://activitypub.rocks/">activitypub.rocks</a>
* <a href="https://en.wikipedia.org/wiki/Fediverse">en.wikipedia.org/wiki/Fediverse</a>

## Mentions

Mentioning other accounts is as simple as referencing their @username in the content of your message.

For example:

> Hey @nick@thegem.city, anything fun this weekend?

When that happens, the post will both link to that account, and that account will get a notification that they were mentioned.

## Post Visibility

On Mastodon, and as a part of the activitypub spec, posts and activity can have different levels of visibility.

* ***Public*** posts can be seen by everyone and are proactively pushed to all of your followers and other servers that are connected to thegem.city.
* ***Unlisted*** posts can be seen by everyone but are not proactively pushed to all of your followers.
* ***Followers only*** posts are only seen by your followers and are proactively pushed to servers that your followers are on.
* ***Mentioned people only*** posts are only seen by people that you specifically mention in your post. They are pushed to the servers that those accounts are located on, but do not appear in the public timeline.

The visibility of a post can be toggled when creating a new post. A post's visibility cannot be changed once it is created.

It is generally accepted that Mastodon nor implementations of the activitypub spec are not a replacement for secure direct messaging. Messages are not encrypted and the content of messages are usually stored in plain text. If you want to communicate securely with another account, you should use the proper tools and services to do so. Mastodon, and by extention this server, is not that tool.

## Boosts

When you boost a post, you a forwarding it to all of your followers.

Boosting posts is the best way to spread a post or activity. The account that created the original post will be notified and all of your followers will see their post and a small reference to your account for boosting it.

## Favorites

Posts can be favorited (starred, liked, etc.). Favoriting a post will notify the account that created the original post, but it will not notify any other accounts that have seen the post.

Think of favoriting a post as a way of giving someone a thumbs up. It's just for you and them.

