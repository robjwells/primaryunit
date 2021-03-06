---
title: "Skype’s emoji cache"
slug: skype-emoji-cache
date: 2017-12-19T11:31:00
---

Skype, a 117MB application (as of right now, on macOS at least), keeps a 340MB stash of emojis on your computer. What?

Clearing some space on my SSD today, I notice that Skype’s Application Support folder takes up over 600MB.

<p class="full-width">
    <img
        src="/images/2017-12-19-skype-application-support.png"
        alt="A screenshot of Daisy Disk showing Skype’s Application Support folder taking up 603.6MB"
        class="no-border"
        width=720
        height=540
        />
</p>

The Upgrade subfolder contains 230MB of old Skype versions, with the oldest dating back to late 2012. That’s a little odd, to keep a five-year-old version around, but fine.

<p>
    <img
        src="/images/2017-12-19-skype-upgrade.png"
        alt="A screenshot showing Skype’s Upgrade folder, containing five previous versions, with the oldest dating back five years."
        />
</p>

How far we’ve come: Skype today is over five times the size it was five years ago.

Drilling down into the robjwells subfolder we find emo\_cache\_v2, accounting for nearly all the 370MB size of its parents. What’s inside? 5,138 emojis and animations. Here’s a taste:

<p>
  <video
    controls
    muted
    preload="none"
    playsinline
    poster="/images/2017-12-19-skype-animation.jpg"
    src="/images/2017-12-19-skype-animation.mp4"
    >
  </video>
</p>

Except that, unlike the super-low-quality version above, the original is 2.4MB and has a delightful reggae soundtrack to accompany its 17-second length.

5,000 of these things. There’s even a Forrest Gump one!

And you’d think “cache” means that “you sent this before, you might need it again” — but as far as I can remember I’ve only ever sent “standard” emojis on Skype. 🤷‍♀️

<div class="flag">
  <p><b>Postscript:</b> If you delete all the mp4 and png files in that directory and then relaunch Skype, it will refill it — but with 3.5MB of animated png emojis.</p>
  <p><b>Post-postscript:</b> I changed the title to remove the emoji as some feed-reading services (like Feed Wrangler, the one I use), couldn’t handle
  🤦‍♀️. Oh well 🤦‍♂️. (And, funnily enough, BBEdit doesn’t handle the “emoji + zero width joiner + modifier” as a single character. Unicode is hard.)</p>
</div>
