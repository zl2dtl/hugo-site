---
title: "Server testing"
layout: page
date: 2025-11-22
draft: false
---

Nothing thrilling at all with this one, but if it's visible after 5:40pm on 23/11/25 NZST then I have successfully implemented a much more automated workflow. This means I can write as much as I want, and literally push one button which runs a .bat script that pushes it to Github after prompting me only for a commit message. My server then has another script which hopefully runs every 20 minutes past the hour (3 times an hour, at :00, :20, and :40) if I wrote it correctly that should delete the old directory and automagically pull the updated copy from Github. 

That's all for now, this is just a test of my automation.

Update 6:22pm, the server-side cronjob isn't running. Must have scripted it wrong somehow. I'm honestly more inclined to make a comically large physical update button at this point... The upside is now everything is technically automated, or at least I have to think less and I can just run two scripts to upload a new update. 

Edit 12:12am 20/03/2026: I set this up but last time I needed to update something I ran the script on the server manually. So I have no idea if it works. I'll leave my latest post just pushed to the repo and in a few hours I'll see if it's up. Should update every 10 minutes in theory. Also, now I just write in VS Code so I can use the git commit button because I'm a blog writer not a tech guy... 