The following is the SuperTux [[Meeting logs|meeting log]] for Tuesday, March 2, 2004.

<pre>
Mar 02 20:50:45 ---	wolfman8k has changed the topic to: supertux is GotM - Official IRC Meeting starts at 20:00 GMT - err today, 10 minutes left
Mar 02 20:51:28 *	tobgle misses neoneurone and blacksheep ^^
Mar 02 20:51:41 <tobgle>	and Bill, of course ;)
Mar 02 20:51:56 <wolfman8k>	i am still optimistic that they will make it in time for the meeting :D
Mar 02 20:52:06 <tobgle>	hope so :)
Mar 02 20:52:38 <tobgle>	Bill is possibly preparing another ./ post at the moment ;)
Mar 02 20:52:55 <wolfman8k>	haha
Mar 02 20:54:35 <wolfman8k>	5 minutes to go by my watch...
Mar 02 20:55:15 <tobgle>	exactly Â°!
Mar 02 20:55:30 *	tobgle is so damn nervous
Mar 02 20:56:12 <tobgle>	did you checkout supertux lately?
Mar 02 20:59:01 <tobgle>	wolfman8k: one minute to go ;)
Mar 02 20:59:29 <virus>	.
Mar 02 20:59:33 <wolfman8k>	yeah, i checked out cvs a few days ago. after you made some big update and i waited 24 hours. and i also checked out grumbels level editor
Mar 02 20:59:48 <wolfman8k>	10...9...8...7...6...5...4...
Mar 02 20:59:48 <tobgle>	wolfman8k: you should make a cvs up again!
Mar 02 20:59:52 <wolfman8k>	3...2...
Mar 02 20:59:53 <wolfman8k>	1...
Mar 02 20:59:55 <wolfman8k>	time
Mar 02 20:59:56 <tobgle>	The sessions starts!
Mar 02 21:00:07 <tobgle>	err, session
Mar 02 21:00:13 <tobgle>	hello everybody!
Mar 02 21:00:16 <wolfman8k>	:D
Mar 02 21:00:24 <Gislan>	hi :)
Mar 02 21:00:55 <tobgle>	grumbel: wake up!
Mar 02 21:01:10 <virus>	.
Mar 02 21:01:14 *	wolfman8k pours tux-style ice cubes over grumbel
Mar 02 21:01:23 <grumbel>	buh
Mar 02 21:01:42 *	tobgle waits for upcoming questions
Mar 02 21:02:03 <wolfman8k>	is there like a topic or a plan for tonights meeting?
Mar 02 21:02:05 <grumbel>	tobgle: when can we expect a 0.6 release?
Mar 02 21:02:06 <paroneayea>	alright
Mar 02 21:02:08 <paroneayea>	hey, I'm back
Mar 02 21:02:09 <grumbel>	0.0.6
Mar 02 21:02:16 <tobgle>	grumbel: when it's ready, sir!
Mar 02 21:02:29 <a-rdel>	how many people are working on it ? 
Mar 02 21:02:31 <paroneayea>	I'm willing to contribute my skill as a graphic artist to the project...
Mar 02 21:02:35 <tobgle>	grumbel: I'd guess this happens untikl friday ;)
Mar 02 21:03:08 paroneayea paxed Mar 02 21:03:21 <grumbel>	paroneayea: any graphics done by you to show?
Mar 02 21:03:35 <paroneayea>	absolutely.  Check out www.lingocomic.com
Mar 02 21:03:39 <grumbel>	http://pingus.seul.org/~grumbel/tmp/supertux-endscreen.jpg
Mar 02 21:03:57 <paroneayea>	the site design is somewhat bland... but the comic itself I think shows my artistic abilities
Mar 02 21:04:11 <tobgle>	a-rdel: we have an active maintainer (well, that's me) , two to three patch senders, and grumbel is wants to be an artists, but you know, he should show skills first *kidding
Mar 02 21:04:23 <wolfman8k>	grumbel: smells of yoshi's island :)
Mar 02 21:04:28 <a-rdel>	i would offer my services but i only really work with 3d :) i came to scope out a 'typical' linux game project hehe  
Mar 02 21:04:30 -->	maxy (~martin@217-162-190-250.dclient.hispeed.ch) has joined #supertux
Mar 02 21:04:48 <wolfman8k>	a-rdel: maybe you can help me with this other game project then ;)
Mar 02 21:05:03 <tobgle>	heh
Mar 02 21:05:17 <a-rdel>	wolfman8k : which project is it ? 
Mar 02 21:05:18 <paroneayea>	oh, awesome looking screenshot, grumbel
Mar 02 21:05:32 <paroneayea>	or, prospective screenshot :)
Mar 02 21:05:44 <wolfman8k>	a-rdel: maybe we should talk about this somewhere else.... can i pm you?
Mar 02 21:05:51 <grumbel>	paroneayea: are you any good at animation?
Mar 02 21:05:51 <tobgle>	you guys should checkout the CVS, if you want to contribute stuff
Mar 02 21:05:56 *	msd is back after 5h 29m 47s: maths
Mar 02 21:06:21 <tobgle>	what we need in the first place is ...
Mar 02 21:06:23 <paroneayea>	grumbel: well.... I haven't ever tried.  But I never tried comics until I just sat down and did one either
Mar 02 21:06:44 <a-rdel>	wolfman8k go for it ;)
Mar 02 21:06:50 <tobgle>	artists for good graphics and musics.
Mar 02 21:07:07 <wolfman8k>	should development be focused now purely on milestone 1, or should we also start thinking about post-milestone 1?
Mar 02 21:07:22 <grumbel>	for this month only milestone1
Mar 02 21:07:28 <tobgle>	milestone 1 is a step in the way to post milestone productions
Mar 02 21:07:30 <grumbel>	everything else just confuses me ;)
Mar 02 21:07:37 <tobgle>	me too :)
Mar 02 21:07:39 <paroneayea>	something I was thinking about.... are we going to do a mini-tux and a larger tux, like in Mario bros?
Mar 02 21:07:54 paroneayea paxed Mar 02 21:08:05 <wolfman8k>	yeah, i think that's a big question
Mar 02 21:08:06 <grumbel>	paroneayea: most likly yes
Mar 02 21:08:20 <tobgle>	that's the way we'll have it in the milestone1 (0.1)
Mar 02 21:08:36 <grumbel>	I could live with just a large tux, but we would need some other action to replace the lack of a small tux
Mar 02 21:08:56 <virus>	grumbel, what about an angry, drunken, crazy,... tux
Mar 02 21:09:12 <paroneayea>	Ooh!  Or an enraged, firey-eyed tux...
Mar 02 21:09:17 <virus>	it would be fun to have dozends of extras that "powerup" the tux for a specific situation
Mar 02 21:09:26 <tobgle>	paroneayea: we have such a tux in CVS!
Mar 02 21:09:33 <paroneayea>	really?  Nifty
Mar 02 21:10:07 <grumbel>	http://super-tux.sourceforge.net/development/images/actions2.jpg
Mar 02 21:10:19 <grumbel>	virus: no, that wouldn't be fun
Mar 02 21:10:30 -->	wallaba (~wallaba@Toronto-HSE-ppp3911804.sympatico.ca) has joined #supertux
Mar 02 21:10:51 <virus>	grumbel, well, at least it would not be that mario like. :)
Mar 02 21:10:59 <grumbel>	having powerups that allow a lot of variing action depending on the context is good, simply having trillions of different actions alone isn't
Mar 02 21:11:08 <paroneayea>	heck... the game doesn't have to be perfectly like mario
Mar 02 21:11:17 <paroneayea>	as long as it's fun and maintains the platformer-like aspect
Mar 02 21:11:25 <virus>	paroneayea, exactly.
Mar 02 21:11:28 <paxed>	do we have a list of powerups somewhere?
Mar 02 21:11:36 <tobgle>	it's important to metion, that this meeting shouldn't be yet another , how should the gameplay look like in SuperTux XY, we want to find skilled musicians and graphic specialists.
Mar 02 21:11:45 <virus>	and if tux was able to throw fish it could be funny, too. :)
Mar 02 21:11:50 <grumbel>	paroneayea: yep, it doesn't has to be mario, but it shouldn't suck either ;)
Mar 02 21:12:12 <grumbel>	http://super-tux.sourceforge.net/development/actions.html
Mar 02 21:12:19 <grumbel>	but most of that webpage is post-milestone1
Mar 02 21:12:34 <tobgle>	paroneayea: the game won't be like mario in the end, nobody wants that, this is only a milestone1 step
Mar 02 21:12:52 <paroneayea>	good to hear :)
Mar 02 21:13:09 <paroneayea>	by the way... what kind of optimizations are being built into the engine?
Mar 02 21:13:31 <tobgle>	paroneayea: from a coder standpoint?
Mar 02 21:13:35 <paroneayea>	my friend and I have been building a from-scratch SDL engine called the "Commodore Pickle engine"
Mar 02 21:13:38 <paroneayea>	yeah
Mar 02 21:13:51 <paroneayea>	ours basically tracks everything about the sprites for you
Mar 02 21:14:04 <paroneayea>	and only updates the parts of the screen that need to be updated
Mar 02 21:14:15 <tobgle>	paroneayea: you can use it in pure SDL or with OpenGL now. (not exactly the answer on your question ;))
Mar 02 21:14:22 <paroneayea>	increasing the frame rate a bit
Mar 02 21:14:38 <tobgle>	such tweaks aren't on our "agenda"
Mar 02 21:14:48 <paroneayea>	right... but what if they're already done?
Mar 02 21:14:55 <Gislan>	are there any debian packages with supertux?
Mar 02 21:14:55 <paroneayea>	we've already finished that code.
Mar 02 21:14:56 <tobgle>	SuperTux has been tweaked here and there since 0.0.5 thought
Mar 02 21:15:01 <paroneayea>	ah
Mar 02 21:15:03 <grumbel>	todays multi ghz cpus can pretty much handle everything
Mar 02 21:15:04 <tobgle>	let's say, it has been rewritten ;)
Mar 02 21:15:25 <grumbel>	Gislan: would be relativly useless in this early stage
Mar 02 21:15:25 <paroneayea>	well, you're talking to a 600 mhz shmuck
Mar 02 21:15:51 <Gislan>	hmm....but i hate installing anything with 'make install'
Mar 02 21:15:56 <grumbel>	should still be fast enough in 640x480
Mar 02 21:15:57 <tobgle>	paroneayea: do you have 3d-acceleration? then use SuperTux with OpenGL , no frame problems left
Mar 02 21:16:05 <Gislan>	I can even build debian packages with this for you if you want
Mar 02 21:16:07 <grumbel>	Gislan: thats why you don't do 'make install'
Mar 02 21:16:26 <grumbel>	Gislan: most stuff can run from source directory these days (well, at least the good stuff ;)
Mar 02 21:16:33 <tobgle>	Gislan: you should check checkinstall ;)
Mar 02 21:16:42 <virus>	*just checking out the cvs... have only seen 0.0.5, yet*
Mar 02 21:16:59 <Gislan>	yeah, I use it sometimes, but classic debian packages are much better for me :)
Mar 02 21:17:00 <tobgle>	virus: be warned, some parts in CVS are known to not work
Mar 02 21:17:42 <Gislan>	silly question: where is supertux cvs?
Mar 02 21:18:09 <grumbel>	http://super-tux.sourceforge.net/milestone1/download.html
Mar 02 21:18:51 <Gislan>	grumbel: thx
Mar 02 21:19:11 <tobgle>	we need to find people that can make sounds for the menu for example.
Mar 02 21:19:42 <tobgle>	tile designers are equally welcome as well as people that can produce MOD/XM/IT musics
Mar 02 21:20:10 <grumbel>	ogg music is fine too 
Mar 02 21:20:26 <tobgle>	grumbel: doesn't work with the SuperTux Engine, or am I wrong?
Mar 02 21:20:31 -->	insid0r (~bobs@CPE-65-31-115-95.wi.rr.com) has joined #supertux
Mar 02 21:20:33 <tobgle>	grumbel: can SDL_mixer play oggs?
Mar 02 21:20:42 <grumbel>	I think so
Mar 02 21:20:46 <tobgle>	hmm hmm
Mar 02 21:20:49 <grumbel>	or at least it shouldn't be hard to add
Mar 02 21:21:02 <tobgle>	well, it blows up the size of SuperTux packages
Mar 02 21:21:14 <grumbel>	I don't care as long as the music is good
Mar 02 21:21:39 <tobgle>	ppl, it's your turn!
Mar 02 21:21:53 <paroneayea>	btw... insid0r, who just joined, is the guy behind the CP engine I was telling you guys about.  We have this evil scheme to integrate our engine into your game and make it faster.
Mar 02 21:22:01 <grumbel>	do we want to have a 'oberwelt'?
Mar 02 21:22:16 <insid0r>	wewt?
Mar 02 21:22:33 <paroneayea>	insid0r was not informed of this evil scheme
Mar 02 21:22:43 <insid0r>	the "we" is tentative :P
Mar 02 21:22:43 <tobgle>	grumbel: yes, I think so
Mar 02 21:22:48 -->	raiskis_ (~chatzilla@rl045112.radiolinja.net) has joined #supertux
Mar 02 21:22:49 <wolfman8k>	paroneayea: does your engine have a website?
Mar 02 21:23:26 <paroneayea>	wolfman8k: yes, but it's more insid0r's than mine... go to http://zaeden.sourceforge.net
Mar 02 21:23:29 <insid0r>	better than that. it has a game being built around it :P I haven't made a site for the engine itself. I was waiting till that project grew
Mar 02 21:23:46 <grumbel>	tobgle: ok, should be tilemap that too or make it large-bitmap based?
Mar 02 21:24:24 <--	a-rdel has quit ()
Mar 02 21:24:43 <paroneayea>	grumbel: sorry, I've got to step in and say tilemap.
Mar 02 21:24:53 <tobgle>	grumbel: It's better to have only ONE solution, which is really maintained then, you know what I mean. So a tilemap is the way to go.
Mar 02 21:25:09 <grumbel>	oky, no problem with that
Mar 02 21:25:45 <grumbel>	ok, speaking of levels, anybody around who want to design some?
Mar 02 21:26:10 <raiskis_>	Is there an leveleditor?
Mar 02 21:26:13 <tobgle>	you should know, that 0.0.6 will come along with a level editor!
Mar 02 21:26:17 <tobgle>	:)
Mar 02 21:26:25 <paroneayea>	then yes.
Mar 02 21:26:26 raiskis raiskis_ Mar 02 21:26:29 <paroneayea>	I would like to give that a try
Mar 02 21:26:30 <grumbel>	raiskis_: http://pingus.seul.org/~grumbel/tmp/windstille-0.2.1-supertux.tar.bz2
Mar 02 21:26:33 <virus>	grumbel, does supertux allow y scrolling or only x scrolling?
Mar 02 21:26:34 <raiskis_>	_Will_ come out
Mar 02 21:26:42 <tobgle>	raiskis_: you can checkout CVS. it's not ready for JoeUser yet, thought.
Mar 02 21:26:46 <grumbel>	virus: only x-scrolling for milestone1
Mar 02 21:27:03 <virus>	grumbel, allright and without paralax scrolling, right?
Mar 02 21:27:06 <tobgle>	we have actually 2 leveleditors
Mar 02 21:27:09 <grumbel>	the leveleditor above is a static binary, should work happily on every linux distro
Mar 02 21:27:19 <grumbel>	virus: paralax scrolling should be there
Mar 02 21:27:22 <raiskis_>	I'm checking out atm, painfully slowly right now
Mar 02 21:27:41 <tobgle>	call it -sourceforge-
Mar 02 21:28:01 <paroneayea>	it won't work on my zaurus then :)
Mar 02 21:28:17 <virus>	hmm... what's the basic tile size of supertux?
Mar 02 21:28:22 <grumbel>	virus: 32x32
Mar 02 21:28:23 <tobgle>	32x32
Mar 02 21:28:42 <virus>	*think* and a game screen is N x N tiles big?
Mar 02 21:28:50 <grumbel>	20x15
Mar 02 21:28:52 <tobgle>	N x 15
Mar 02 21:28:53 <paroneayea>	seems a bit large.  Maybe I've been fooling around with 16 bit emulators for too long though.
Mar 02 21:29:23 <grumbel>	http://pingus.seul.org/~grumbel/tmp/supertux-gamescreen.jpg
Mar 02 21:29:23 <raiskis_>	The leveleditor is 4MB ???
Mar 02 21:29:30 <grumbel>	thats how it should look like
Mar 02 21:29:37 raiskis raiskis_ Mar 02 21:29:50 raiskis raiskis_ Mar 02 21:29:54 <virus>	is there a way to have supertux stand "inbetween" two tiles... e.g. instead of having stairs a ramp ?
Mar 02 21:29:59 <tobgle>	raiskis_: that's grumbel's editor, checkout SuperTux CVS for a built in one
Mar 02 21:30:07 ---	msd has changed the topic to: supertux is GotM - Official IRC Meeting starts at 20:00 GMT - err today, 10 minutes l/topiceft
Mar 02 21:30:07 <grumbel>	raiskis_: it contains a bit more stuff than really needed (ie. half of windstille game)
Mar 02 21:30:16 <--	msd (~intrepid@web.speedlan.hu) has left #supertux ("Leaving")
Mar 02 21:30:20 <raiskis_>	ah, ok :)
Mar 02 21:30:22 <tobgle>	virus: such things are planned
Mar 02 21:30:35 <virus>	tobgle, M1 does only have tiles (32x32) , right?
Mar 02 21:30:39 <tobgle>	virus: 0.0.5 - 0.0.6 is largely rewriting and such
Mar 02 21:30:58 <tobgle>	virus: we could allow other sizes for background tiles in the next releases
Mar 02 21:31:16 <wolfman8k>	virus: i sort of did a small from-scratch version of "supertux" that supports ramps: http://benny.kramekweb.com/junk/supertux7.png
Mar 02 21:31:17 <tobgle>	virus: we want to split up the current level-format soon
Mar 02 21:31:21 <insid0r>	tiles and tilemaps are the easy way to go for level design
Mar 02 21:31:30 <insid0r>	but what you should do is have tux a freely positioned sprite
Mar 02 21:31:38 <insid0r>	so that he isn't constrained to the tiles and their positions.
Mar 02 21:31:38 <insid0r>	:/
Mar 02 21:31:57 <paroneayea>	yep.  See, this is why insid0r and I should be integrating our CP engine.
Mar 02 21:32:03 <tobgle>	insid0r: so it is :)
Mar 02 21:32:05 <virus>	wolfman8k, hey, you're working with FOX, right?:)
Mar 02 21:32:16 <wolfman8k>	virus: yeah :)
Mar 02 21:32:20 <insid0r>	instead of doing the oldschool 8086 game route and check collisions based solely on tile positions, you do a full collision check of sprite on sprite
Mar 02 21:33:03 <tobgle>	insid0r: aren't that high CPU costs?
Mar 02 21:33:27 <virus>	CPUs are quite cheap nowadays... (bad joke alert!)
Mar 02 21:33:42 <tobgle>	no comment
Mar 02 21:33:43 <insid0r>	not if you're smart about it. the planned collision system in my engine will have scalable precisions
Mar 02 21:34:02 <insid0r>	so you can effectively have a box around the sprite, which would make for next to no CPU usage
Mar 02 21:34:22 <insid0r>	or you could have one point calculated for every 2 pixels of the sprite... or even every pixel (the most precise detection), or anything inbetween
Mar 02 21:34:34 <tobgle>	insid0r: I guess SuperTux will stay old-school the next time, this could change when pre 0.1 development begins, but that's not the topic
Mar 02 21:34:49 <paroneayea>	alright... let me sum this up.
Mar 02 21:35:01 <tobgle>	ups
Mar 02 21:35:02 <paroneayea>	If insid0r and I successfully integrate the CP engine into the project
Mar 02 21:35:05 <wolfman8k>	i don't really think it's practical to replace the supertux "game engine" for milestone 1
Mar 02 21:35:05 <paroneayea>	and you see how awesome iti s
Mar 02 21:35:06 <paroneayea>	er
Mar 02 21:35:07 <paroneayea>	is
Mar 02 21:35:09 <tobgle>	I mean post 0.1 development ;)
Mar 02 21:35:14 <grumbel>	old school is good
Mar 02 21:35:14 <paroneayea>	will you give it a shot?
Mar 02 21:35:25 <insid0r>	old school is horrible :P tux can't be free-floating then.
Mar 02 21:35:27 <grumbel>	and boxes make a whole lot of things much easier anyway
Mar 02 21:35:36 <grumbel>	insid0r: of course he can
Mar 02 21:35:36 <tobgle>	paroneayea: giving it a shot , surely. But we don't need it.
Mar 02 21:35:46 <wolfman8k>	yeah, i think bounding box collisions for everything is the best
Mar 02 21:35:51 <tobgle>	insid0r: of course he can /me to
Mar 02 21:35:52 <tobgle>	o
Mar 02 21:35:59 <virus>	grumbel, the fakeshots look great right now. :)
Mar 02 21:36:49 <tobgle>	SuperTux really needs artists in all areas! I know/hope you are here!
Mar 02 21:37:00 <insid0r>	bounding boxes is essentially the lowest accuracy collision setting on my collision system. but you could, if you chose, make the most detailed collision system. I'm going to be making it with vectors, so you could have one point per every X pixel and compare that against any other sprite with less or more complex collision masks
Mar 02 21:37:05 <virus>	another thing of interrest... does supertux use the alpha channel of png graphics?
Mar 02 21:37:20 <grumbel>	anyway, those interested in doing levels should checkout the editor, it already pretty useable, import/export to native supertux format will follow as soon as supertux has a sane format that supports non-hardcoded tiles
Mar 02 21:37:21 <paroneayea>	well... I can help with the development of graphics, easy
Mar 02 21:37:25 <paroneayea>	but I need to know what to develop
Mar 02 21:37:47 <tobgle>	insid0r: I'll probably implement some sort of bitmap-collisions in SuperTux, this isn't planned for 0.1, but I think this is highly precise, too.
Mar 02 21:38:22 <tobgle>	virus: it uses the alpha channel :)
Mar 02 21:38:34 -->	MeLassen (6883@tannpirker.uio.no) has joined #supertux
Mar 02 21:38:38 <virus>	allright. :)
Mar 02 21:38:42 <tobgle>	paroneayea: you could start with a new theme
Mar 02 21:38:54 <tobgle>	paroneayea: and with checking out the CVS
Mar 02 21:39:13 <paroneayea>	okay... we need something that isn't wintery.  everything seems wintery in linux games, and quite frankly I'm getting sick of it.
Mar 02 21:39:16 <wolfman8k>	about themes: are they really needed?
Mar 02 21:39:22 <grumbel>	paroneayea: for a new theme I would suggest either desert or something 'green' (jungle or whatever)
Mar 02 21:39:28 <wolfman8k>	paroneayea: i think the plan is for tux to travel around the world
Mar 02 21:39:28 <virus>	tobgle, discussing with ppl who haven't actualy seen the latest dev snapshot is great, isn't it?:)
Mar 02 21:39:32 <tobgle>	wolfman8k: for 0.1 they are. for 0.0.6, no.
Mar 02 21:39:49 <tobgle>	virus: yeah ;)
Mar 02 21:39:51 <wolfman8k>	tobgle: why not just have one giant collection of tiles?
Mar 02 21:40:15 <virus>	wolfman8k, I think it would be hard to keep the collection in a sane state...
Mar 02 21:40:23 <tobgle>	wolfman8k: errm
Mar 02 21:40:34 <tobgle>	wolfman8k: themes are for jungle levels and so on
Mar 02 21:41:01 <grumbel>	wolfman8k: I think one-collection of tiles is the way to go from a programming point of view
Mar 02 21:41:02 wallaba wolfman8k Mar 02 21:41:09 <wolfman8k>	tiles could be sorted, to help level editing. but why limit each level to only use one collection of tiles?
Mar 02 21:41:17 <grumbel>	wolfman8k: the themes-thing is more a level-designers thing to keep things consistent
Mar 02 21:41:20 <virus>	tobgle, I think I'll chuck my luck with some space tiles. :)
Mar 02 21:41:37 <tobgle>	paroneayea: SuperTux is expected to make a trip around the world, go into /data/levels/default/ and open the levels file to see the countries (Bill Kendrick had the idea)
Mar 02 21:42:48 <tobgle>	wolfman8k: the way you mentioned was used in SuperTux back in the Bill K. days and I changed it for good reasons ;)
Mar 02 21:43:46 <paroneayea>	okay, will do
Mar 02 21:43:55 <virus>	wolfman8k, just think of third party levels... it would result in mixed up tiles probably.
Mar 02 21:44:21 <virus>	however a level format that "imports" one to n specific tile sets would probably ok.
Mar 02 21:44:21 <wolfman8k>	i think it would work fine with third party levels. all the tiles would be added to one giant master pool
Mar 02 21:44:40 <wolfman8k>	when the level is loaded, the game scans it and only loads the tiles that it uses
Mar 02 21:45:03 <tobgle>	wolfman8k: adding a possibility to use more than one theme at once is a post 0.1 feature
Mar 02 21:45:09 <wolfman8k>	because there are probably a lot of tiles that should be shared between different "countries"
Mar 02 21:45:14 <virus>	wolfman8k, you sound like linus actualy... a monolithic design might be good for some stuff but not for levels!
Mar 02 21:45:34 <tobgle>	wolfman8k: there are some tiles, that aren't in level-themes and generally shared, no reason to worry
Mar 02 21:45:36 <--	wallaba has quit (Read error: 104 (Connection reset by peer))
Mar 02 21:45:37 -->	wallaba_ (~wallaba@Toronto-HSE-ppp3911804.sympatico.ca) has joined #supertux
Mar 02 21:45:38 <grumbel>	there is no point in limiting the engine that way
Mar 02 21:45:49 <wolfman8k>	grumbel: do you agree with me on this issue?
Mar 02 21:45:49 <grumbel>	the engine should support any number of tiles
Mar 02 21:45:53 <grumbel>	wolfman8k: yep
Mar 02 21:45:58 <wolfman8k>	*phew* :)
Mar 02 21:46:17 <wolfman8k>	i think the level editor could have different tile sets sorted in different tabs
Mar 02 21:46:21 ---	wallaba_ is now known as wallaba
Mar 02 21:46:21 <tobgle>	the themeability will stay! DOT
Mar 02 21:46:27 <grumbel>	the *editor* might restrict the few to a subset of the tiles to make it easier to not mix them up, but thats all
Mar 02 21:46:29 <virus>	I don't think it should be _one_ big pool. It could be handled with "import tileset <blah>" statements in the levels. :)
Mar 02 21:46:35 <tobgle>	wolfman8k: themes != tilesets
Mar 02 21:47:06 <wolfman8k>	i think that each tile could be maybe some extended .png format. then you just add them all into a directory structure:
Mar 02 21:47:06 <tobgle>	wolfman8k: themes override the default LOOK of tiles, not more
Mar 02 21:47:14 <virus>	tobgle, guess I got themes - tilesets wrong, too, pls explain. :)
Mar 02 21:47:19 <wolfman8k>	tiles/jungle/vine.png tiles/misc/brick.png
Mar 02 21:47:35 <--	raiskis has quit (Connection timed out)
Mar 02 21:47:46 <wolfman8k>	tobgle: so i could take a level, and change it's theme, and then the level's appearence will change?
Mar 02 21:47:50 <wolfman8k>	hm... that could be cool
Mar 02 21:47:52 <tobgle>	wolfman8k: that's nearly the way the themes ARE handled
Mar 02 21:48:02 <grumbel>	its a rather useless feature
Mar 02 21:48:03 <tobgle>	wolfman8k: so it is NOW!!!
Mar 02 21:48:21 <grumbel>	since it wouldn't work unless all themes use *exactly* the same tiles
Mar 02 21:48:30 <grumbel>	and that would limit there freedom quite a lot
Mar 02 21:48:37 <virus>	grumbel, I like it... at least you can the level twice and think you played two different levels :P
Mar 02 21:48:38 <wolfman8k>	yeah, i think you are right grumbel
Mar 02 21:48:48 <tobgle>	grumbel: who's freedom ???
Mar 02 21:49:06 <grumbel>	my freedom as a graphic designer
Mar 02 21:49:06 <tobgle>	wolfman8k, grumbel: you are both getting it wrong :(
Mar 02 21:49:13 <tobgle>	why?
Mar 02 21:49:28 <raiskis_>	|<--	raiskis has left irc.freenode.net (Connection timed out) I have???
Mar 02 21:49:48 <wolfman8k>	raiskis_: irc does not lie :P
Mar 02 21:49:54 <grumbel>	tobgle: because I would have to make sure that all themes have the same number of tiles 
Mar 02 21:50:29 <grumbel>	tobgle: it of course doesn't matter if we just use one 'default' theme and crunch all tiles (desert, ice, etc) into it
Mar 02 21:50:41 <tobgle>	grumbel: if a tile is missing a default tile can be loaded. Btw. that's the same as KDE/IceWM etc. themes.
Mar 02 21:51:10 <maxy>	I can see one good reason for this limitation, and that's "one tile = one byte"
Mar 02 21:51:13 <grumbel>	tobgle: theming sucks, its just a lame excuse for not doing it right in the first place
Mar 02 21:51:22 <tobgle>	grumbel: you should begin to understand, that themes are about the look and not about the "tiles"
Mar 02 21:51:26 <grumbel>	maxy: make byte a short, problem solved
Mar 02 21:51:54 <tobgle>	grumbel: I didn't hear any reasonable argument for now ;)
Mar 02 21:52:35 <grumbel>	tobgle: if we just use one theme for the whole game I won't have a problem
Mar 02 21:53:02 <maxy>	grumbel: that's ugly you can't have human-readeable text level files then :) ok I don't know whether that ist the case right now
Mar 02 21:53:08 <tobgle>	grumbel: you mean, all levels should take place in antarctica?!
Mar 02 21:53:20 <paroneayea>	grumbel: wait a minute... then I think we hit the problem I was addressing earlier
Mar 02 21:53:22 <grumbel>	maxy: numbers are pretty human readable
Mar 02 21:53:38 <tobgle>	maxy: we'll have leveleditors anyway
Mar 02 21:53:52 <paroneayea>	grumbel: every single game in Linux looks like it takes place in antarctica.  It gets frustrating.
Mar 02 21:53:53 <maxy>	jep, sure.
Mar 02 21:53:57 <grumbel>	tobgle: the levels should be whereever they like to be, the default theme will contain all 'worlds'
Mar 02 21:54:06 <maxy>	would just be a geeky thing, nothing more :)
Mar 02 21:54:16 <paroneayea>	wait, grumbel... let me get this straight
Mar 02 21:54:19 <--	MeLassen has quit ("looking forward for the next version")
Mar 02 21:54:29 <paroneayea>	you are all for having multiple environments
Mar 02 21:54:33 <tobgle>	grumbel: this looks to me like ancient design, sorry
Mar 02 21:54:45 <paroneayea>	you just think that the cactuses should be allowed to be in antarctica too, yes?
Mar 02 21:55:22 paroneayea paxed Mar 02 21:55:39 <grumbel>	paroneayea: from a programming point of view *YES*, from a design point of few *NOT*
Mar 02 21:55:46 <wolfman8k>	paroneayea: i think so yes. cactuses in antarctica. that doesn't mean that the level designers *should* do that. it just means they can :)
Mar 02 21:55:51 <grumbel>	its pointless to hardcode a design-guide into code
Mar 02 21:56:16 <tobgle>	ppl can change themes, whenever they want, problem solved DOT
Mar 02 21:56:36 <tobgle>	that is the reason for the themes
Mar 02 21:56:37 <paroneayea>	no wait tobgle, it isn't
Mar 02 21:56:47 <paroneayea>	the concern I'm seeing
Mar 02 21:57:03 <tobgle>	I probably know what you mean ;)
Mar 02 21:57:11 <paroneayea>	is that the designers here want the ability to go beyond just the appearance
Mar 02 21:57:35 <paroneayea>	so that the cactus behaves like a cactus.  So that each world doesn't feel the same but just look different.
Mar 02 21:57:56 <grumbel>	exactly
Mar 02 21:58:09 <tobgle>	cactus is a good example to explain why the themes are good!
Mar 02 21:58:24 <paroneayea>	oh?
Mar 02 21:58:24 <grumbel>	if I have a cactus, every world needs a cactus like thing and thats pointless
Mar 02 21:58:31 <wolfman8k>	i think the idea is also that it might not be possible to do a one-to-one mapping of tiles from one environment to another. so you can't take a desert level with a cactus and change it to a ice level with a snow plant
Mar 02 21:58:46 <tobgle>	as long as the cactus does impact the gameplay it won't be in the themes!!!
Mar 02 21:59:09 <paroneayea>	but what if you want a mixed level?
Mar 02 21:59:24 <paroneayea>	what if I want an area of the level to have what looks like a cavern?
Mar 02 21:59:28 <paroneayea>	or look all dried up?
Mar 02 21:59:40 <grumbel>	exactly
Mar 02 21:59:58 <grumbel>	one of my levels already starts on normal ground and moves into a cave in the last parts of it
Mar 02 22:00:05 <tobgle>	I never saw such a level
Mar 02 22:00:17 <tobgle>	 / what a bad excuse
Mar 02 22:00:18 <paroneayea>	regardless, it's an ability designers want.
Mar 02 22:00:24 <paroneayea>	now hold on.
Mar 02 22:00:29 <paroneayea>	let's not get angry here
Mar 02 22:00:45 <paroneayea>	we're trying to work together, not tear each other apart :)
Mar 02 22:02:20 <tobgle>	we'll rewrite the level-format anyway, multiple themes/appeareances per level could be a design criteria
Mar 02 22:02:35 <paroneayea>	what does everyone think of that
Mar 02 22:02:39 <paroneayea>	is that acceptable?
Mar 02 22:03:13 <paroneayea>	if we can switch between themes, I think I should be okay with it.
Mar 02 22:03:44 <tobgle>	Every tile could have a "tag" for it's theme in example
Mar 02 22:03:46 <grumbel>	switching themes is a) useless b) easily implementable if all tiles are in one theme
Mar 02 22:04:10 <paroneayea>	okay... listen to this.  My friend Jay came up with an idea for the level design... (I'm chatting with him over GAIM)
Mar 02 22:04:22 <grumbel>	tobgle: this is something that should go into the editor or into a style-guide, but *NOT* into the game code
Mar 02 22:06:09 <sjbrown>	hi guys.  i'm interested in the format the content of supertux will be stored in.
Mar 02 22:06:24 <sjbrown>	particularly, if it would be usable in my engine.
Mar 02 22:06:26 <paroneayea>	to quote him: "a level = tarball  when the level loads, the tarball is temporarily unpacked  level.set is run and that basically defines the tilemaps  it's so simple  like this, level.set loads the tilemaps you wanna use  common tilemaps can be distributed with the game, custom tilemaps distributed with each level level.set can load any of the above.
Mar 02 22:06:26 <paroneayea>	then when you design your level, the tilemaps you use would be like:   tile(0,12). tile #12 out of the first tile set loaded.   etc. that way you get maximum possible space saving (by having common tiles) and maximum customizability 
Mar 02 22:06:30 <grumbel>	sjbrown: hasn't been decided, some kind of text thing most likly
Mar 02 22:06:55 paroneayea paxed Mar 02 22:07:01 <grumbel>	paroneayea: overly complicated
Mar 02 22:07:21 <grumbel>	have a simple 'int'->png-file mapping and all problems are solved
Mar 02 22:07:27 <tobgle>	paroneayea: agree with grumbel ;)
Mar 02 22:07:34 <wolfman8k>	yeah, best is to just have tile("jungle/vine.png) or tile("misc/brick.png")
Mar 02 22:08:08 <tobgle>	which, doesn't differ much from the current situation, it differs slightly _not much_
Mar 02 22:08:34 <tobgle>	you can't use multiple _appearences_ in one level, that's all
Mar 02 22:08:39 <tobgle>	and can be changed
Mar 02 22:08:48 <paroneayea>	see, that's what we're arguing on
Mar 02 22:09:07 <paroneayea>	grumbel and I want multiple appearances, while you don't think there's any reason for it.
Mar 02 22:09:53 <tobgle>	there can be reasons for it, but it doesn't seem to be a must have to me
Mar 02 22:10:00 <paroneayea>	but think about Mario Bros.... at least you'd change different segments of the level that had different tilemaps.  You'd go down the pipes and be in the underground area, then you'd come back up again.  Also, I'm wondering when that's planned ot be in supertux.
Mar 02 22:10:06 <paroneayea>	maybe that's how we can solve this problem
Mar 02 22:10:19 paroneayea paxed Mar 02 22:10:24 <paroneayea>	by allowing swithing between multiple areas, aka pipes in mario, per level
Mar 02 22:10:33 <sjbrown>	paroneayea: that's basically a level switch.
Mar 02 22:10:47 <paroneayea>	hm. :\
Mar 02 22:10:47 <grumbel>	paroneayea: sublevel support is planed
Mar 02 22:10:50 <sjbrown>	what's the diff between that and changing levels?
Mar 02 22:11:06 <--	Andre4s has quit ("Client exiting")
Mar 02 22:11:09 <sjbrown>	i guess level state is preserved.
Mar 02 22:11:13 <grumbel>	sjbrown: a sublevel is something small like a bonus-room or something like that
Mar 02 22:11:17 <paroneayea>	changing levels you'd go from level one to level two.  It would actually be counted, wouldn't it?
Mar 02 22:11:22 <paroneayea>	sublevel wouldn't count thta
Mar 02 22:11:24 <paroneayea>	er
Mar 02 22:11:24 <paroneayea>	that
Mar 02 22:11:27 <tobgle>	grumbel: sublevel support is one more reason for deprecating multiple appearences per level
Mar 02 22:11:42 <grumbel>	why that?
Mar 02 22:11:59 <grumbel>	and why the f*** do you want to hard-code a style-guide into the game code?
Mar 02 22:12:36 <paroneayea>	wait... that's why Jay's plan keeps the style-guide out of it.
Mar 02 22:12:41 <grumbel>	its not like we are programming a snes or something other oldschool which restricted the number of tiles per map in hardware
Mar 02 22:12:47 <sjbrown>	grumbel: in the pipe example, a sublevel is basically just another level, but the state of the first level is maintained.
Mar 02 22:12:54 <maxy>	maybe so a spike has always the same id, be it (metallic / ice / cactus)?
Mar 02 22:12:58 <paroneayea>	it picks which parts of the style you want in your level
Mar 02 22:13:12 <paroneayea>	whoa... we already addressed the cactus issue :)
Mar 02 22:13:14 <grumbel>	sjbrown: its not only the state, its the whole translation sequence that is totally different
Mar 02 22:13:32 <tobgle>	maxy: !
Mar 02 22:13:39 *	tobgle is tired
Mar 02 22:13:55 <sjbrown>	grumbel: i'm not sure what you mean by "translation sequence".  I'll defer to you on this one.
Mar 02 22:14:24 *	tobgle has to prepare a few things for school now
Mar 02 22:14:54 <Gislan>	what about internationalization? will supertux support other languages (intro, menu etc) ?
Mar 02 22:15:10 <grumbel>	sjbrown: transition sequence or however you call it, the whole endsequence
Mar 02 22:15:40 <grumbel>	Gislan: maybe, but thats something I would like to care about after the game is in a useable state
Mar 02 22:15:45 <tobgle>	Gislan: do you think that's needed? The most linux-games don't address this issue. For 0.1 SuperTux won't leave this common path.
Mar 02 22:16:23 <Gislan>	ah...ok
Mar 02 22:17:39 <raiskis_>	Wesnoth does. And it's nice :) But there will not be much text in super-tux, am I right?
Mar 02 22:17:46 <grumbel>	pingus does too :)
Mar 02 22:18:02 <grumbel>	and adonthell is working on it 
Mar 02 22:18:10 <tobgle>	pydance doesn't :9
Mar 02 22:18:26 <wolfman8k>	will supertux have any story or naaration at all? or only an intro and ending?
Mar 02 22:18:33 <tobgle>	come on, this is maybe even past 1.0 work
Mar 02 22:18:41 <sjbrown>	Gislan: internationalization is relatively easy to do once you've got a working product.
Mar 02 22:18:57 <sjbrown>	assuming you don't do something silly in the code to make it hard.
Mar 02 22:19:09 <tobgle>	wolfman8k: Scrolling text is the only thing I can think of for 0.1 so far.
Mar 02 22:19:09 <grumbel>	wolfman8k: most likly only intro/ending and something between the worlds
Mar 02 22:19:24 <tobgle>	wolfman8k: every level could have a little introduction so
Mar 02 22:19:27 <grumbel>	wolfman8k: and in-game 'dialog' ie. info-blocks, bonus games stuff
Mar 02 22:19:56 <wolfman8k>	yeah... ok
Mar 02 22:20:00 <Gislan>	sjbrown: sure, it's very easy if engine allows you to change font for all texts in game
Mar 02 22:20:17 <Gislan>	sjbrown: is it possible in supertux?
Mar 02 22:20:58 <sjbrown>	I assume they're using SDL_ttf, so that sounds doable.
Mar 02 22:21:05 <grumbel>	Gislan: currently that is possible
Mar 02 22:21:06 <tobgle>	we don't
Mar 02 22:22:28 <tobgle>	I invite all ppl which want to contribute graphics or sounds to use our mailing list.
Mar 02 22:22:42 <virus>	besides - who is the de facto maintainer of the project? i guess tobgle but I'm unsure right now. :)
Mar 02 22:23:05 <tobgle>	virus: I picked the project up, so that's me currently ;)
Mar 02 22:23:11 <grumbel>	tobgle keeps care of the code, I keep care of graphics and levels
Mar 02 22:23:27 <paroneayea>	so, this mailing list....
Mar 02 22:23:30 <grumbel>	nobody keeps care of the webpage, so its a bit outdated ;)
Mar 02 22:23:36 <paroneayea>	I noticed.
Mar 02 22:23:46 <virus>	grumbel, is there need for a new webpage?
Mar 02 22:23:48 <grumbel>	anybody around who would like to keep care of the webpage?
Mar 02 22:24:08 <grumbel>	virus: not right now, but if milestone1 is ready, then yes
Mar 02 22:24:49 <tobgle>	sorry guys, I have to do my homework now :(
Mar 02 22:24:58 <virus>	well, I recently put the webpage of VCOM online. http://www.vcom.org/ - If you like the look of my webpages I could create something for supertux. :)
Mar 02 22:25:03 <--	maxy has quit ("gone")
Mar 02 22:25:24 <Gislan>	maybe you should use wiki?
Mar 02 22:25:39 <Gislan>	then everyone could keep it up to date
Mar 02 22:25:48 <tobgle>	Gislan: they don't work in projects of this little size, I have experience with that ;)
Mar 02 22:26:12 <grumbel>	virus: looks good. for supertux its however more of a content problem
Mar 02 22:26:30 ---	tobgle is now known as tobgle|away
Mar 02 22:26:36 <grumbel>	virus: ie. we need somebody that takes care of the webpage and updates it with info from the mailinglist, cleanup outdated stuff, etc.
Mar 02 22:26:47 <virus>	grumbel, sure, just to give you a impressions of how my webpages are made up (100% valid XHTML + CSS)
Mar 02 22:27:28 <virus>	grumbel, how is the current webpage made up? simple HTML files or rendered dynamicaly by some script?
Mar 02 22:27:37 <Gislan>	tobgle: it doesn't have to be big page heavly loaded with info, just a simple page with download, install and screenshots section etc which can be easily edited by any developer or even user
Mar 02 22:27:55 <virus>	besides... what is the _official_ URL of supertux?:)
Mar 02 22:28:01 <grumbel>	virus: xml translated via xalan to html
Mar 02 22:28:49 <grumbel>	virus: http://super-tux.sourceforge.net/milestone1/
Mar 02 22:29:47 -->	raiskis__ (~chatzilla@rl045112.radiolinja.net) has joined #supertux
Mar 02 22:30:59 <tobgle|away>	ok, I'm doing my homework now, could you please dicuss the sounds/musics issue? we have a lack here. My personal feel is that that's nearly as important as graphics
Mar 02 22:31:09 <tobgle|away>	s/dicuss/discuss
Mar 02 22:32:34 -->	david_v (~david_v@c213-200-135-241.cm-upc.chello.se) has joined #supertux
Mar 02 22:33:06 <--	david_v (~david_v@c213-200-135-241.cm-upc.chello.se) has left #supertux ("Client exiting")
Mar 02 22:33:51 <paroneayea>	well... gee.  Sounds I'm not so experienced with myself...
Mar 02 22:35:21 <virus>	ah, supertux is C, allright.
Mar 02 22:36:01 <paroneayea>	whoa crap
Mar 02 22:36:02 <grumbel>	virus: its planed to migrate to C++ in the future
Mar 02 22:36:14 <paroneayea>	just discovered a huge problem with the collision detection :)
Mar 02 22:36:19 <paroneayea>	when your FPS is low
Mar 02 22:36:23 <paroneayea>	you just go right through the floor
Mar 02 22:36:27 <virus>	paroneayea, true. :)
Mar 02 22:36:36 <Gislan>	c++? objective supertux? sounds cool :)
Mar 02 22:37:15 <paroneayea>	any plans to fix that in any upcoming releases
Mar 02 22:37:20 <virus>	grumbel, it would make the code a lot easier in some parts. Especialy the enemies - right now called "badguys" could be extended to a "chracateristic" behaviour
Mar 02 22:37:28 <grumbel>	does anybody have a good suggestion for a 'flying' or 'jumping' enemy
Mar 02 22:37:37 <virus>	grumbel, what about the evil tomato?:)
Mar 02 22:37:51 <virus>	I guess penguins don't like tomatos. :P
Mar 02 22:37:52 <grumbel>	no vegetables please :)
Mar 02 22:38:06 <virus>	*think*
Mar 02 22:38:19 <paroneayea>	how about... mini-angry helicopters?  lol..
Mar 02 22:38:25 <Gislan>	there should be an evil freebsd demon ;)
Mar 02 22:38:34 <grumbel>	simply attaching wings to the iceblock might already be enough, but anything better is welcome
Mar 02 22:38:43 <grumbel>	Gislan: no OS related stuff either
Mar 02 22:39:13 <Gislan>	why? it's geeky and funny :P
Mar 02 22:39:23 <grumbel>	geeky stuff isn't funny
Mar 02 22:39:23 <wolfman8k>	grumbel: you are looking for something like the flying mushroom enemies in smb3?
Mar 02 22:39:39 <paroneayea>	like user friendly.  Not funny.
Mar 02 22:39:46 <paroneayea>	*dodges flames*
Mar 02 22:39:50 <grumbel>	I am thinking of the flying koopers (turtles) in smb1
Mar 02 22:40:13 <virus>	grumbel, what about an evil SGI man coming arround?:)
Mar 02 22:40:14 <paroneayea>	I have a good idea, but I'd have to draw it.  Any idea where I should send it grumbel?
Mar 02 22:40:27 <virus>	eerm
Mar 02 22:40:30 paroneayea paxed Mar 02 22:40:31 <virus>	no not SGI... *laughts*
Mar 02 22:40:41 <Gislan>	paroneayea: userfriendly is really funny....at least in the middle of the night :)
Mar 02 22:40:45 <grumbel>	paroneayea: upload it somewhere and post the url
Mar 02 22:40:48 <virus>	I ment SCO :)
Mar 02 22:41:39 <virus>	grumbel, I'd love to see "karl klammer" as enemy. *g*
Mar 02 22:41:52 <paroneayea>	grah....
Mar 02 22:41:53 <sjbrown>	grumbel: if you're going to migrate, why not just migrate to python?
Mar 02 22:42:03 <Gislan>	there should be a bad guy - pig (spam) :))
Mar 02 22:42:10 <grumbel>	sjbrown: that would require a complete rewrite
Mar 02 22:42:45 <sjbrown>	well, you might be able to make some of the C stuff act like libraries and just plug them into python.
Mar 02 22:42:49 <virus>	sjbrown, I've never used python for coding UI stuff. Do you have any experiences with PyGAME ?
Mar 02 22:42:55 <sjbrown>	but whatev.  it's your code.
Mar 02 22:43:02 <Gislan>	I've played some time with pygame
Mar 02 22:43:15 <Gislan>	very good library for python
Mar 02 22:43:17 <sjbrown>	virus: yes.  check out http://sjbrown.ezide.com/games/writing-games.html
Mar 02 22:43:52 <paroneayea>	just tried out the CVS version.  much better.
Mar 02 22:43:55 <sjbrown>	and check out http://pygame.org/gamelets/#SCROLLJB
Mar 02 22:44:08 <wolfman8k>	sjbrown: i sort of started a new c++ version of supertux:
Mar 02 22:44:08 <wolfman8k>	http://benny.kramekweb.com/junk/supertux3.png
Mar 02 22:44:10 <wolfman8k>	http://benny.kramekweb.com/junk/supertux7.png
Mar 02 22:44:27 <wolfman8k>	sjbrown: it started out with python, but i moved to c++ because python was too slow :/
Mar 02 22:44:55 <sjbrown>	yeah.  I've heard scrolljb gets down to 10 fps on 500Mhz computers.
Mar 02 22:45:24 <paroneayea>	it does.. I can vouch for that ;_;
Mar 02 22:45:50 <sjbrown>	there are some optimizations that could be made.  especially in the content.
Mar 02 22:46:14 <sjbrown>	slow computers hate full alpha surfaces.
Mar 02 22:46:27 <paroneayea>	found a bug I'm going to try to work on.... that damned jumping problem
Mar 02 22:46:32 <grumbel>	sjbrown: even fast computers hate alpha surfaces
Mar 02 22:46:36 <grumbel>	only opengl loves them ;)
Mar 02 22:47:08 <sjbrown>	true enough.
Mar 02 22:47:11 <wolfman8k>	if you do alpha surfaces in opengl through python it shouldn't be a problem
Mar 02 22:47:37 <paroneayea>	why's that?
Mar 02 22:47:37 <sjbrown>	but not all computers have hardware OpenGL.
Mar 02 22:48:44 <wolfman8k>	i think it's safe to assume that all relevant gaming computers will have at least half-decent opengl support
Mar 02 22:49:15 <paroneayea>	not true.  A lot of computer users flock to 2d games because they don't have good opengl support.
Mar 02 22:49:29 <sjbrown>	it's totally up to the developer as to what to target.
Mar 02 22:49:34 <paroneayea>	I used to be one of them.  Any idea how much time I spent playing Kobo Deluxe back then?  Jeebus.
Mar 02 22:49:44 <sjbrown>	personally, i'd like my games to work well on laptops.
Mar 02 22:53:09 <grumbel>	anybody around who would be willing to maintain a win32 port of supertux?
Mar 02 22:53:12 <paroneayea>	: \  Am I right in that this game doesn't have actual sprite support?  that's what it's looking like while I'm browsing the code...
Mar 02 22:53:31 paroneayea paxed Mar 02 22:53:40 <grumbel>	paroneayea: depends on what you expect from sprite support
Mar 02 22:54:13 <paroneayea>	I mean _actual_ sprite support, where the engine handles the coordinates and calculates that seperately.  Where it doesn't get messy in the main code.
Mar 02 22:55:58 <paroneayea>	it would be nice if all of that was handled in a simple render() function at the end of the game loop
Mar 02 22:56:40 -->	basse_ (~basse@cs78204018.pp.htv.fi) has joined #supertux
Mar 02 22:57:11 <paroneayea>	that, at least to me, is the ideal way of handling sprites.  Also, is layer integration handled in the sprite data?  It doesn't look so...
Mar 02 22:57:20 <paroneayea>	er, not layer integration
Mar 02 22:57:23 <paroneayea>	layer information
Mar 02 22:58:02 <--	raiskis_ has quit (Connection timed out)
Mar 02 22:58:13 <grumbel>	currently it traverses all the objects in game_draw()
Mar 02 22:58:19 <Gislan>	another silly question: why there's no configure/autoconf/automake/etc ?
Mar 02 22:58:37 <grumbel>	because nobody has written it yet
Mar 02 23:00:00 <Gislan>	ah... :)
Mar 02 23:00:23 <Gislan>	thought that there are some problems with that...
Mar 02 23:01:02 <tobgle|away>	another reason for it was, that it isn't needed atm
Mar 02 23:01:08 <tobgle|away>	s/was/is
Mar 02 23:01:30 <grumbel>	the current makefiles really suck, since they don't even get the dependence tracking right
Mar 02 23:01:59 <Gislan>	but imho you should start thinking about things like that....I hope you'll need beta testers soon 
Mar 02 23:02:07 <--	raiskis__ has quit (Read error: 110 (Connection timed out))
Mar 02 23:02:47 -->	psi_ (~psi@D39cb.d.pppool.de) has joined #supertux
Mar 02 23:03:38 <grumbel>	Gislan: will take a while will the game gets beta-tester ready
Mar 02 23:03:52 <grumbel>	first we need a bit more fixed up gameplay and levels of course
Mar 02 23:04:12 <sjbrown>	hmm.  i just checked out cvs.
Mar 02 23:04:20 <grumbel>	those who want to help are again, invited to try the level editor and do some levels with it: http://super-tux.sourceforge.net/milestone1/download.html
Mar 02 23:04:25 <sjbrown>	is the code a lot different that kendricks?
Mar 02 23:04:34 <sjbrown>	it seems to have a more buggy feel.
Mar 02 23:04:41 <grumbel>	sjbrown: its completly restructured
Mar 02 23:04:56 <grumbel>	from a gameplay point of view its currently more buggy, yep
Mar 02 23:05:01 <sjbrown>	ah.
Mar 02 23:05:19 <Gislan>	grumbel: I'll try to make some new levels tomorrow, but I'm not very good in such things :)
Mar 02 23:05:55 <paroneayea>	grumbel: when are these newer graphics from the level editor going to make it into the game?
Mar 02 23:06:10 <grumbel>	paroneayea: 0.0.7 release
Mar 02 23:06:18 <paroneayea>	ah, k
Mar 02 23:06:21 <grumbel>	they need a new level format first
Mar 02 23:06:38 <grumbel>	and especially we need to get rid of hardcoded tiles first
Mar 02 23:06:41 <paroneayea>	new level format?  ARGUE!!!111@
Mar 02 23:07:00 *	wolfman8k is starting to get tired
Mar 02 23:07:00 <paroneayea>	sorry.  Thought that was almost funny
Mar 02 23:08:23 *	paroneayea thinks he should get to studying.
Mar 02 23:08:26 <paroneayea>	later.
Mar 02 23:08:49 <paroneayea>	grumbel... I'll try to get back to you on that graphic when I finish it. I might have free time later tonight
Mar 02 23:09:56 <virus>	grumbel, have you ever tried SCONS ?
Mar 02 23:10:01 <virus>	http://www.scons.org/
Mar 02 23:10:17 <virus>	I'm using this alternative to the GNU auto-xxx stuff.
Mar 02 23:10:41 <wolfman8k>	scons is the good
Mar 02 23:11:11 <--	paroneayea has quit ("Leaving")
Mar 02 23:11:15 <grumbel>	virus: havn't tried it, only browsed the manual a bit
Mar 02 23:11:54 <grumbel>	currently a simple makefile however should be enough for supertux
Mar 02 23:11:56 <virus>	It's quite nice and almost anything is done magicaly without having to write kilometres of makefiles. :)
Mar 02 23:12:11 <wolfman8k>	everyone should use scons instead of make imho :)
Mar 02 23:12:39 <wolfman8k>	and while i'm dreaming, subversion should be used instead of cvs :D
Mar 02 23:12:51 <wolfman8k>	and python should be used a lot more :)
Mar 02 23:12:57 <virus>	eerm, why is supertux using a make target for every single object?
Mar 02 23:13:10 <wolfman8k>	and people should use css to do layouts in web pages instead of html tables >:o
Mar 02 23:13:34 <grumbel>	virus: because the makefile sucks ;)
Mar 02 23:13:39 <virus>	the ".c.o" target helps!
Mar 02 23:13:48 <grumbel>	wolfman8k: how does one do good layout in css?
Mar 02 23:13:56 <virus>	.c.o:
Mar 02 23:14:07 <virus>	[tab]$(CC) -c $<
Mar 02 23:14:12 <virus>	and you're fine. :)
Mar 02 23:14:23 <grumbel>	I know
Mar 02 23:14:25 <grumbel>	send patches
Mar 02 23:15:47 <wolfman8k>	grumbel: using css positioning and stuff. i'm not really an expert. i just copy code :) the only problem is that ie sucks donkey balls when it comes to css :(
Mar 02 23:17:10 <virus>	wolfman8k, valid CSS is mostly displayed correct in IE (5.5- is horrible, but 6.0+ can does at least obey the basic rules)
Mar 02 23:17:12 <grumbel>	wolfman8k: I have tried a bit with the positioning stuff of css, but either it got *way* more complicated than simple tables or it simply didn't work at all in all browsers
Mar 02 23:17:33 <virus>	however IE just fucked the whole CSS box model, but M$ does that with every standard...
Mar 02 23:17:42 <grumbel>	the worst thing is that if css breaks it mostly renders the webpage near unusable
Mar 02 23:17:57 <virus>	I sometimes got to laught when thinking of M$ even fucking up the SMB proctocol which is the very backbone of all windows domains
Mar 02 23:18:04 <grumbel>	tables down do that
Mar 02 23:18:33 <grumbel>	s/down/don't/
Mar 02 23:19:04 <virus>	grumbel, a good strict html file including a nice CSS is usualy displayed with grace by IE... even the older ones
Mar 02 23:19:10 <virus>	grumbel, do you know CSSZenGarden?
Mar 02 23:19:31 <virus>	http://www.csszengarden.com/ - it's worth a look. :)
Mar 02 23:19:48 -->	jeorb (~andy@64.246.32.74) has joined #supertux
Mar 02 23:20:31 <jeorb>	hi
Mar 02 23:21:34 -->	paroneayea (~paroneaye@brt-mer231-234.brt-mer.depaul.edu) has joined #supertux
Mar 02 23:21:35 <paroneayea>	hey
Mar 02 23:21:40 <paroneayea>	I finished the flying graphic
Mar 02 23:21:44 <paroneayea>	or, the concept art
Mar 02 23:22:16 <virus>	gn8 everybody. After finishing my UDP wrapper (works actualy) I got to sleep. :)
Mar 02 23:22:34 <paroneayea>	oh right... this is an XCF file... gotta convert it to something you guys can see
Mar 02 23:23:25 <paroneayea>	okay, lookit:  www.lingocomic.com/gfx/goodies/wingling.png
Mar 02 23:23:40 <paroneayea>	if you think that looks half decent, I'll color it in
Mar 02 23:24:00 <virus>	paroneayea, looks nice. :)
Mar 02 23:24:15 <Gislan>	yeah, I like it
Mar 02 23:25:44 <grumbel>	looks good, might however not fit into the arctic theme
Mar 02 23:25:45 <paroneayea>	you think so?  I've got a good idea for the color scheme...
Mar 02 23:25:48 <paroneayea>	true
Mar 02 23:26:09 <paroneayea>	I'll go color it anyway.
Mar 02 23:26:16 <paroneayea>	heck, I don't feel like studying :)
Mar 02 23:26:19 <grumbel>	should fit good into a lava/wasteland one
Mar 02 23:26:49 <Gislan>	but if you add some ice icicles on the wings, it could be used in arctic them too :))
Mar 02 23:27:07 <paroneayea>	I could create a more arctic variation if you like
Mar 02 23:27:12 <paroneayea>	something that looks less devilish
Mar 02 23:27:21 <paroneayea>	more cute, even
Mar 02 23:28:13 <grumbel>	Gislan: yep, but I probally prefer a iceblock with wings there 
Mar 02 23:28:59 <Gislan>	grumbel: maybe you're right ;)
Mar 02 23:29:15 <--	ian__ has quit ("Leaving")
Mar 02 23:30:37 <paroneayea>	gah!  I spent that whole time coloring on the same layer as my outline :(
Mar 02 23:32:35 <--	virus has quit ("umount /dev/brain")
Mar 02 23:33:08 <--	psi_ has quit ("leaving")
Mar 02 23:33:13 <paxed>	if you walk underneath the winged iceblock, it falls ;)
Mar 02 23:35:05 <paroneayea>	so this thing's turning out to be quite purple as I'm coloring it...
Mar 02 23:35:47 <Gislan>	question about code: is there any #define DEBUG var or something like this which tells whole program whether to display basic debug info (such as "player killed") or not?
Mar 02 23:38:39 ---	tobgle|away is now known as tobgle
Mar 02 23:38:47 <paroneayea>	care to see my progress on the coloring job? :  www.lingocomic.com/gfx/goodies/wingling_color.png
Mar 02 23:38:50 <tobgle>	Gislan: yes, DEBUG_MSG("A message");
Mar 02 23:39:05 <tobgle>	paroneayea: hey, cool
Mar 02 23:39:18 <paroneayea>	tobgle: thanks
Mar 02 23:39:52 <Gislan>	yeah, it's really cool
Mar 02 23:40:07 <paroneayea>	I'm thinking that the wings should be green.... hm.  That might not match.
Mar 02 23:40:26 <paxed>	and red tail-tip?
Mar 02 23:40:39 <paroneayea>	paxed: good idea
Mar 02 23:40:52 <tobgle>	grumbel: it should be the freedom of a level-designer to use a certain enemy/object in any level with any design/theme/appereance, don't you think so? Or do you only think that we don't need more than antarctica(or a new version of it) atm?
Mar 02 23:41:50 <paroneayea>	tobgle: I'll throw in my two cents: it should definetly be the freedom of the level designer.  It's awesome in the hacked super mario bros 3 when you encounter the angry sun enemy in the ice world.
Mar 02 23:42:40 <paroneayea>	does anyone want the XCF file of this image when I'm done with it?
Mar 02 23:42:53 <grumbel>	tobgle: its should be of course up to the level designer, but the normal levels shouldn't mix styles like wild
Mar 02 23:43:48 <grumbel>	there is nothing worse then a level that simply uses all the tiles at the same time without a good reason
Mar 02 23:44:25 <grumbel>	on the other side one can build pretty damn interesting levels when mixing styles, but one has to do that with care
Mar 02 23:44:47 <Old_Belge>	Are there problems with collision detection?
Mar 02 23:44:54 <tobgle>	grumbel: I know what you want to say, but creating a new enemy shouldn't depend on existing styles(etc.) per se IMHO
Mar 02 23:44:55 <grumbel>	Old_Belge: yep
Mar 02 23:45:21 <Old_Belge>	Any idea in which source files the problem occurs?
Mar 02 23:45:26 <tobgle>	Old_Belge: little problems :) not that we can't fix them or so, it's a lack of time ;(
Mar 02 23:45:32 <tobgle>	Old_Belge: player.c
Mar 02 23:45:35 <grumbel>	tobgle: yep, sure it shouldn't depend on the current style, we can collect everything we get for the past milestone1 time
Mar 02 23:45:50 <paroneayea>	question: any other types of characters you need developed besides flying ones?
Mar 02 23:46:05 <tobgle>	grumbel: why not for the milestone1 time? It won't be antarctica only grumbel!
Mar 02 23:46:20 <grumbel>	 when it comes to release time I like to strip out (ie. remove from the levels) stuff that doesn't fit in
Mar 02 23:46:32 <tobgle>	paroneayea: I don't know the correct word, but some kind of end-enemy/final-opponent ;)
Mar 02 23:46:39 <grumbel>	tobgle: it won't be antarctica only as soon as we get a good looking other tileset
Mar 02 23:47:25 <tobgle>	paroneayea: I spider would be cool, too.!
Mar 02 23:48:02 <grumbel>	paroneayea: maybe some final boss enemy might be usefull
Mar 02 23:48:20 <tobgle>	grumbel: isn't that what I just sayed? ;)
Mar 02 23:48:45 <grumbel>	looks like I skiped that line ;)
Mar 02 23:49:04 <grumbel>	end-boss should probally simply be a snowman
Mar 02 23:49:29 <tobgle>	an angry ice-bear for me ;)
Mar 02 23:49:31 <paroneayea>	hm.... snowman...
Mar 02 23:49:33 <paroneayea>	ice-bear
Mar 02 23:49:46 <grumbel>	or that, something that fits the theme
Mar 02 23:50:05 <Gislan>	main boss definitly should be Yeti :)
Mar 02 23:50:12 <tobgle>	naaah
Mar 02 23:50:40 <tobgle>	Gislan: Yeti lives in the highest mountains not in the antarctica ;)
Mar 02 23:51:27 <paroneayea>	hm.  I think I'll develop a few bosses
Mar 02 23:51:34 <paroneayea>	you guys can pick and choose
Mar 02 23:51:38 <tobgle>	yep
Mar 02 23:51:47 <paroneayea>	some non-ice ones too
Mar 02 23:51:55 <tobgle>	even better
Mar 02 23:55:58 <paroneayea>	hm... I dunno about this green wing thing.  Wanna check it out?
Mar 02 23:56:05 <Gislan>	sure
Mar 02 23:56:15 <paroneayea>	okay, it's up
Mar 02 23:56:24 <paroneayea>	www.lingocomic.com/gfx/goodies/wingling_color.png
Mar 02 23:56:53 <Gislan>	looks good enough for me
Mar 02 23:57:09 <Gislan>	not for the arctic theme, but jungle theme maybe....
Mar 02 23:57:19 <paroneayea>	okay
Mar 02 23:57:35 <Gislan>	of course you may change colour of wings to dark red and put it in dungeon theme :)
Mar 02 23:57:45 <paroneayea>	I was also thinking of making a monster that walked and spat things out of it's mouth
Mar 02 23:59:16 -->	zratchet (~chatzilla@user-0vvdas1.cable.mindspring.com) has joined #supertux
Mar 02 23:59:19 <Gislan>	now you need to make animation of this flying monster with green wings :)
Mar 02 23:59:21 <tobgle>	hi zratchet!
Mar 02 23:59:51 <zratchet>	tobgle: hi... quite a few people today
Mar 02 23:59:56 <zratchet>	GotM?
Mar 03 00:00:02 <tobgle>	I guess so ;)
Mar 03 00:00:42 <zratchet>	tobgle: GotM = game of the month or what?
Mar 03 00:01:03 <tobgle>	zratchet: yep, www.happypenguin.org
Mar 03 00:01:22 <paroneayea>	who's this?
Mar 03 00:01:43 <tobgle>	paroneayea: a SuperTux on Mac user :)
Mar 03 00:01:47 <paroneayea>	ahhh
Mar 03 00:10:09 <Gislan>	got to go now
Mar 03 00:10:10 <Gislan>	bye
Mar 03 00:10:19 <paroneayea>	later Gislan
Mar 03 00:10:24 <--	Gislan has quit ("Leaving")
Mar 03 00:15:15 <paroneayea>	hm...
Mar 03 00:15:20 <paroneayea>	made another concept art....
Mar 03 00:15:23 <paroneayea>	not sure this one is so good.
Mar 03 00:16:10 <paroneayea>	www.lingocomic.com/gfx/goodies/theking.png
Mar 03 00:16:28 <paroneayea>	It would make more sense if it were colored.
Mar 03 00:16:44 <--	wolfman8k has quit ("Leaving")
Mar 03 00:18:10 <tobgle>	paroneayea: nice! that guy shocks me ;)
Mar 03 00:18:21 <paroneayea>	you think so?
Mar 03 00:18:22 <tobgle>	paroneayea: can you try your luck on a GNU? ;)
Mar 03 00:18:39 <paroneayea>	sure... I was actually considering developing one for the FSF
Mar 03 00:18:39 <tobgle>	paroneayea: not as enemy, as friend of Tux ;)
Mar 03 00:18:43 <paroneayea>	right
Mar 03 00:18:50 <grumbel>	no GNU, please
Mar 03 00:18:56 <zratchet>	paroneayea: I have some ideas on a GNU
Mar 03 00:19:03 <zratchet>	grumbel: why not?
Mar 03 00:19:12 <paroneayea>	uhoh... I sense a flamewar *hides*
Mar 03 00:19:25 <grumbel>	zratchet: a fat tux riding on a fat gnu is not something I would like to see
Mar 03 00:19:33 <grumbel>	fat mario on yoshi already looked bad enough
Mar 03 00:20:04 *	tobgle votes for a little young GNU
Mar 03 00:20:06 <tobgle>	baby
Mar 03 00:20:11 <grumbel>	and I want to strip this whole free-software thing out of the game as much as possible
Mar 03 00:20:21 <tobgle>	grumbel: I'm with you
Mar 03 00:20:21 <paroneayea>	grumbel has a point there
Mar 03 00:20:46 <zratchet>	well, use a yak then... more tux-environment-like anyway
Mar 03 00:20:51 <zratchet>	or a seal
Mar 03 00:20:52 <grumbel>	having a baby-gnu or having a gnu in a cutscene (say as king of some lang or whatever) is ok
Mar 03 00:21:00 <tobgle>	grumbel: but this one is a exception. Kids for example won't see the political things behind anyway and a GNU is still an animal.
Mar 03 00:21:09 <tobgle>	grumbel: thanks ;))
Mar 03 00:21:35 <grumbel>	it simply shouldn't look like the gnu is only in there for the complete lack of any inspration
Mar 03 00:21:35 <zratchet>	would be fun to have some other (ant)arctic animals...
Mar 03 00:21:46 <zratchet>	and/or other animals in different themes
Mar 03 00:21:50 <zratchet>	ok
Mar 03 00:21:51 <zratchet>	 i c
Mar 03 00:22:23 <paroneayea>	agreed.  Anyway, I have an easier time coming up with deranged looking creatures, like the wingling thing
Mar 03 00:23:37 <zratchet>	if not a gnu...
Mar 03 00:24:03 <paroneayea>	it should be something that's good beyond just the arctic
Mar 03 00:24:09 <zratchet>	yes
Mar 03 00:24:15 -->	kittyhawk (~mike@65-37-54-105.nrp6.roc.ny.frontiernet.net) has joined #supertux
Mar 03 00:24:22 <paroneayea>	holy crap!
Mar 03 00:24:27 <zratchet>	maybe not an animal in that case...
Mar 03 00:24:31 <paroneayea>	is that kittyhawk from montrose academy?
Mar 03 00:24:35 <zratchet>	a mecha ;)
Mar 03 00:24:35 <kittyhawk>	no, sorry
Mar 03 00:24:44 <paroneayea>	damn you! *curses sky*
Mar 03 00:24:48 <kittyhawk>	apologies.
Mar 03 00:24:51 <paroneayea>	it's ok
Mar 03 00:25:02 <--	zratchet (~chatzilla@user-0vvdas1.cable.mindspring.com) has left #supertux
Mar 03 00:25:09 -->	zratchet (~chatzilla@user-0vvdas1.cable.mindspring.com) has joined #supertux
Mar 03 00:26:40 <zratchet>	what I'd like to see is a character that:
Mar 03 00:26:41 <zratchet>	can use horns or something to get rascals or dig thru walls...
Mar 03 00:26:43 <zratchet>	can be ridden and used to stampede rascals
Mar 03 00:26:45 <zratchet>	can stampede without riding and boomerang to Tux and let him get back on
Mar 03 00:26:47 <zratchet>	can bounce Tux off his back for higher jumps
Mar 03 00:27:01 <zratchet>	maybe a robot? I don't know ;)
Mar 03 00:27:38 ---	ChanServ removes channel operator status from tobgle
Mar 03 00:27:40 <kittyhawk>	I think a tux-sliding-on-belly move would be more appropriate :)
Mar 03 00:27:52 <kittyhawk>	of course, it would be different than what you propose.
Mar 03 00:27:55 <zratchet>	for which of those abilities?
Mar 03 00:28:19 <kittyhawk>	I guess it would replace the killing rascals with horn ability.
Mar 03 00:29:18 <grumbel>	zratchet: donkeykong contry had such stuff, never really liked it from a gameplay point of view
Mar 03 00:29:38 <zratchet>	hm...
Mar 03 00:29:40 <zratchet>	ok
Mar 03 00:29:51 <zratchet>	just ideas... ;)
Mar 03 00:30:06 <grumbel>	I am searching more for things that can be used in multiple ways 
Mar 03 00:30:19 <grumbel>	say an iceblock, you can jump on him to disable him
Mar 03 00:30:27 <grumbel>	grab him, throw it at other enemies
Mar 03 00:30:38 <grumbel>	use to to trigger unreachable bonus blocks
Mar 03 00:30:45 <paroneayea>	well, for that walking thing that spits things out I was working on (you haven't seen it yet)
Mar 03 00:30:49 <grumbel>	and suchs
Mar 03 00:31:00 <paroneayea>	you could use it to fire globs at enemies while it is unconcious
Mar 03 00:35:15 <paroneayea>	anyway.. I have class.  If any of you want to contact me at any time, shoot me an email at creat0r@lingocomic.com  <- notice the zero in creat0r
Mar 03 00:37:35 ---	zratchet is now known as zratchet_away
Mar 03 00:37:41 <--	paroneayea has quit ("Leaving")
Mar 03 00:43:27 <--	kornl has quit ("Leaving")
Mar 03 00:45:42 <--	tobgle has quit (Read error: 104 (Connection reset by peer))
Mar 03 00:47:33 <--	zratchet_away (~chatzilla@user-0vvdas1.cable.mindspring.com) has left #supertux
**** ENDING LOGGING AT Wed Mar  3 00:55:12 2004
</pre>