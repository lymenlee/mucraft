---
published: true
layout: post
comments: true
title: GitHub: Clone, Set-Url, Push
date: "2018-06-11 22:59:56 -0400"
categories: GitHub
tag: Github, Git, DevOps	
---

## GitHub: Clone, Set-Url, Push

Sometimes you clone your own repo from GitHub on another machine and try to do quick updates on it, then you want to push back the changes. But when you try to get a `git push` running, you get an 403 error. How come? Well it's because when you clone your repo, you use the read-only URL provided on the repo page and your remote url is set to this read-only URL. Of course it won't let you log in and do push operation! Fortunately it's simple to address, just run below command:

```shell
git remote set-url https://yourusername@github.com/user/rego.git
```

Next time you try to do `git push`, you'll see the lovely password prompt. Enjoy and push more codes!


