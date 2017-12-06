# Welcome to MsPooka's Github page

<a href="Me and my human."><img src="http://www.lovethispic.com/uploaded_images/254892-Cute-Angry-Cat.jpg" title="Me and my human" /></a>

### Current Projects...


### Working on a website idea for a friend....

<img src="https://i.imgur.com/zclNU7cm.jpg" />
I hope this endeavor pans out for my friend.  If so, I'll build an e-commerce site for fresh farm meats. :)


### Bots, bots, bots.........
Its time to make a human-like conversation bot.  I setup a localhost Program O but I decided to try a more modern AI markup language.


<img src="https://i.imgur.com/p361k7o.png" />


So now I have gone with Dialogflow (Google API).....


Here is the VR/AR rig that I want to attach the bot to (Unity)....

<a href="https://imgur.com/B99MkS2"><img src="https://i.imgur.com/B99MkS2.png" title="source: imgur.com" /></a>


Now I need to find some way to bridge Unity text with Dialogflow....


So I spent like 15 hours trying to figure out why I was getting an certificate error...
```
ServicePointManager.ServerCertificateValidationCallback = (a, b, c, d) =>
		{
			return true;
		};
```


Took forever trying to parse a stupid string....
```
string answerText;
			answerText = outText;
			if (answerText != null) {
				string pattern = "speech\":\"";
				string pattern2 = "\"}";
				string[] results = Regex.Split(answerText, pattern);

				if (results[1] != null) {
					string[] finalanswer = Regex.Split(results[1], pattern2);
					Debug.Log(finalanswer[0]);
					fanswerText = finalanswer[0];
					if (onresponse != null) {
						onresponse();  //event action
					
					}
```



