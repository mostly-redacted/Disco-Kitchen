# Disco-Kitchen
Crestron control for Disco music and Disco ball with lights with 1 button press
This is a project me and my wife came up with.

THE IDEA:
She would play disco music while she cooked if she was feeling depressed. "It's hard to be sad with Disco music" she said.
Wouldn't it be fun to have a single button that played disco music, turned on a mirror ball and lights. It would be like having an instant happy button.
On remodeling our kitchen, I thought this through and realized I could do this.

This is based on Crestron, so at its basic it is in a version of C.
You need to have access to Creston SIMPL to install this.
One can use any generation processor and you do not need a touchscreen.
For the one button press this uses a CEN-RFGW-EX to communicate to a CEN-GWEXER button.

ECONONMY OF MEANS:
This is made of consumer and recycled parts. There is nothing commercial about this.
The amplifier 1 is controlled only by IR. No feedback to know which state it is in. You can use any home amplifier with IR control.
This can also be controlled by a 120 volt relay if there is no IR control and it is a really old amp.
For the kitchen amplifier 2, I am using a Clearone Converge 880TA. A discontinued generation 1 product. It has 4 amps inside each one that can be 8 ohm or 70 volt so you can use speakers you already have.
Being controlled via IP/TCP makes it a little easier. So this can be substituted for a modern LAN controlled amp.
The MP3 player is an IR controlled SD card reader. It is a no name product found on ebay.
2 8-Ohm speakers are used in my kitchen.

TIMING:
The main problem with consumer gear with only IR or relay control is having no ability to have feedback of when it is on.
Timing the lights, mirror ball and music to turn on simultaneously is the critical adjustment in your delays.

2 MODES:
The time it takes a consumer amplifier to power up makes the single button press a little tricky to time the music with the lights.
The CLW-EX has some options. In this program a long press is for when the system is off. It will take into account that the Pioneer amp I use takes 42 seconds to power up and pass audio.
This kind of ruins the one-button effect we are after.
That is MODE 1: Long press means turning on from full off. This is fine for yourself, but for the full effect we need instant on.
MODE 2: Prime the audio.
Long Press turns everything on. A short press of Off will only turn off the music and the lights. The main amplifier stays on ready to go.
Short press now will have the lights and music come on in about 1 second. Instant happy button.

MUSIC:
On button double tap advances to the next song
Off button double tap advances to previous song
The songs are not random. This MP3 player is a very simple thing. On power on the music starts. To make it time correctly, the power is sent to the IR and then Next is selected to start the song.
If not, then the song begins playing before the audio is ready. Going to the next song starts at the beginning.
