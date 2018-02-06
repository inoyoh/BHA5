---
layout: post
title: "Github Troubleshooting: Page builds failing"
author: sota
date: 2018-02-06-20:30:00
categories: general github
tags: github troubleshooting
---

![Failing builds](/images/failing_builds.png)
## So, your commits in `_posts` are not reflecting in the `bha5.bioclub.org` page?
You check the commits in `BioClub/BHA5` and there's a small red X?

That's probably because your **Builds are failing**!

### *But why are my builds failing?* It's usually because you have a **syntax error** in your code.

Syntax errors happens when there is something incomprehensible by the computer in your code written by you.

Common mistakes among markdown are:

- A general typo in the meta header

- Not having a space after Header pounds `#Bad Example` `# Good Example`

- Once you open a quote you MUST close it! [Example](https://github.com/BioClub/BHA5/commit/e38eb1240c9e0cb4735a14bc1997247b17b5a816)


There are more causes of a bad build. Happy debugging! *Add your cause of a failed build here too!*
