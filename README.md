# OldTweetDeck
Returns old TweetDeck, for free!
Currently no easy way to install, but you can download this repo and load it as unpacked extension in Chrome/Edge/Opera/any chromium browser.
![Screenshot](https://lune.dimden.dev/9713d947d56.png)  

## Info
New TweetDeck was renamed to XPro and now requires Blue subscription. But currently you can still `tweetdeck_version=legacy` cookie to get old TweetDeck back without any subscriptions required. First thought would be just to set that cookie when you install extension, but I'm 100% sure this will most likely stop working soon when they find out. So I've made this extension to actually replace files with my own hosted ones. This way it will work even if they completely remove old TweetDeck from their servers.

## Transparent disclaimer
This extension will use files hosted on my own server (dimden.dev). This technically grants me access to add anything I want to TweetDeck code any time I want. I don't have any interest in doing anything malicious, but still, use at your own risk.  
You might be asking, why not just include all files within extension itself (like [OldTwitter](https://github.com/dimdenGD/OldTwitter) does), well I [tried](https://github.com/dimdenGD/OldTweetDeck/commit/043529289ce85d5017bcc158d0e26a7df0ed4de3) and it's impossible due to use of `eval` / `new Function` in TweetDeck code. Manifest v3 extensions are not allowed to use `eval` / `new Function` because of new stupid policies.