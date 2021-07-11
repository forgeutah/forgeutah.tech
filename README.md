<h1 align="center">
  Forge Utah Foundation Website
</h1>

We use [Hugo](https://gohugo.io/documentation/) static site builder along with the [Doks Theme](https://getdoks.org/).


## Quick Start

### Setup

* Install NPM
* Checkout this repo and CD into the directory
* run `npm install`
* Start the local demo server with `npm run start`

### Add New Meetup

Use command `hugo new community/meetups/my-new-meetup/index.md -k meetups`

It will create the file specified and create all the metadata fields necessary for a meetup:

```
---
title: "My New Meetup"
date: 2021-07-10T18:25:14-06:00
meetupLink:
banner:
logo:
chairs:
- clintberry
locationSponsor:
  name: Weave
  link: https://getweave.com
  logo: weave.jpg
foodSponsor:
  name: Weave
  link: https://getweave.com
  logo: weave.jpg

draft: true
---
```

Change the fields as needed

### Add New People

We reference people in several places on the site. For example, a chair of a meetup is a reference to a person, and an author
of a blog post can reference a person. For ease of re-use and updating we store all references to people in `data/people.json`. 
Every person is stored with an ID reference (just use \[\[firstname]]\[\[lastname)]]). Then you can reference that ID in metadata
and it will auto populate with correct info.

```
---
...
chairs:
- clintberry
...
---
```

### Add New Blog Post

`hugo new blog/name-of-my-post.md`




