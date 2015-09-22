# SoundOnHover
##Play Audio on :hover
Play Audio on :hover
We're going to use HTML5 here, no Flash. We'll need an audio element with both MP3 (WebKit, IE) and OGG (Firefox, Opera).

<audio controls preload="auto">
	<source src="audio/beep.mp3" controls></source>
	<source src="audio/beep.ogg" controls></source>
	Your browser isn't invited for super fun audio time.
</audio>
We're using jQuery in this demo to make selecting things and events easier, but the .play() function is native. You probably wouldn't show the audio element, that's for demo purposes only, just remove the control attribute to not show anything.

#1.One <audio> for all menu items
.play() won't force the audio clip to start over unless it's finished first, not very smooth.

#2.One <audio> for all menu items, with pause
.pause() ing first should stop it and then play new sound but it actually makes it worse somehow. Sounds get chopped off but not restarted.

#3.Cloned <audio>, one for each menu item
Smoothest but not perfect.


