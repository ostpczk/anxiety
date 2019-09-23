# act1

```
SceneSetup.act1();
```

(...300)

n: A TO JEST CZŁOWIEKA LĘK

n: _TY_ JESTEŚ LĘKIEM

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Hej! Znowu ty i ja?

`hong({eyes:"0_neutral"})`

n: TWOIM ZADANIEM JEST BRONIĆ SWOJEGO CZŁOWIEKA PRZED *NIEBEZPIECZEŃSTWEM*

`bb({eyes:"look", mouth:"small_lock"})`

n: WŁAŚCIWIE, ODTWARZANIE PONOWNIE TEJ GRY STANOWI DLA NIEGO *ZAGROŻENIE* 

n: SZYBKO! OSTRZEŻ GO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Człowieku! Słuchaj, jesteśmy w zagrożeniu! Gracz...

[...będzie nas ponownie maltretować!](#act1_replay_torture)

[...nie odnajdzie alternatywnego zakończenia!](#act1_replay_alternate)

[...doświadczy dysonans ludonarracyjny!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Sprawi, że zwiniemy się w kulkę i popadniemy w płacz!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Sprawi, że roztrzaśniemy telefon za sprawą ataku paniki!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Sprawi, że *NIE* uderzymy organizatora imprezy!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Zmusi nas do uderzenia sympatycznego organizatora imprezy!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Przynajmniej może nie spadniemy z budynku tym ra--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: SKŁONI NAS DO ZESKOCZENIA Z DACHU.
{{/if}}

`bb({body:"fear"});`

b: WSZYSTKIE TE OKROPNE RZECZY NAM SIĘ STANĄ A POTEM --

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Sure, the story as a *whole* is the same, but each chapter has two possible endings, plus all the branching dialogue opti--

`bb({body:"fear"});`

b: The player will be disappointed, close this browser tab, delete our software, and then we'll--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: A lewd-what now?

`bb({eyes:"normal"});`

b: The story arc was about how you can *CHOOSE* to build a healthy collaboration with your fear,

`bb({eyes:"normal_right"});`

b: But replaying the game will give the same story, implying your *CHOICES* don't matter,

`bb({eyes:"narrow_eyebrow"});`

b: Thus showing a contradiction between the game's message and mechanics,

`bb({eyes:"fear"});`

b: Thus unraveling the fabric of this narrative universe,

`bb({body:"fear"});`

b: And then we'll--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: DIEEEEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Okay let's get back into character.

```
Game.clearText();
```

n4: (LET _YOUR_ ANXIETY BLAH BLAH BLAH MOST SIMILAR TO WHAT _YOUR_ FEAR BLAH BLAH YOU KNOW THE DRILL)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Och tak, mój wilk powrócił. Cudoooooownie.

`hong({eyes:"0_neutral"})`

n: TWOIM ZADANIEM JEST BRONIĆ SWOJEGO CZŁOWIEKA PRZED *NIEBEZPIECZEŃSTWEM*

`bb({eyes:"look", mouth:"small_lock"})`

n: WŁAŚCIWIE, TA KANAPKA STANOWI DLA NIEGO *ZAGROŻENIE* W TEJ CHWILI

n: SZYBKO, OSTRZEŻ GO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Człowieku! Słuchaj, jesteśmy w zagrożeniu! Niebezpieczeństwem jest...

`bb({body:"squeeze"})`

n4: (POZWÓL _SWOIM_ LĘKOM WEJŚĆ W ŻYCIE! WYBIERZ CO _CIEBIE_ NIEPOKOIŁOBY NAJBARDZIEJ)

(#act1_normal_choice)

# act1_normal_choice

[Jemy samotnie lunch! Znowu!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Nie jesteśmy produktywni podczas jedzenia!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Ten chleb pszenny jest dla nas niezdrowy!!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Don't you know loneliness is associated with premature death as much as smoking 15 cigarettes a day?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Um, thanks for citing your sources but--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Which means if we don't hang out with someone *right now* we're gonna-

`bb({body:"panic"})`

b: DIEEEEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: YOU USED *FEAR OF BEING UNLOVED*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Whip out your laptop and do some work right now!

`hong({eyes:"0_annoyed"})`

h: Um, I'd rather not get crumbs in my keyboa--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: If we're not contributing to the body of society then we're a society-parasite!

b: The society-body will go to the society-doctor for medication to kill their society-parasites then we'll--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: DIEEEEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: YOU USED *FEAR OF BEING A BAD PERSON*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Have those studies been replicat--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Processed wheat will spike our blood sugar so they'll have to amputate all our limbs and then we'll-

`bb({body:"panic"})`

b: DIEEEEEEEEEEEEEEEEEEE

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: YOU USED *FEAR OF BEING HARMED*

(#act1b)

# act1b

n: IT'S SUPER EFFECTIVE

`bb({mouth:"smile", eyes:"smile"});`

b: See, human? I am your loyal guard-wolf!

`bb({body:"pride_talk"});`

b: Trust your gut! Your feelings are always valid!

`bb({body:"pride"});`

n: GET YOUR HUMAN'S ENERGY BAR TO ZERO

n: TO PROTECT THEIR PHYSICAL + SOCIAL + MORAL NEEDS, YOU CAN USE:

n: FEAR OF *BEING HARMED* #harm#

n: FEAR OF *BEING UNLOVED* #alone#

n: AND FEAR OF *BEING A BAD PERSON* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (PRO-TIP: PLAY THE CHOICES THAT PERSONALLY HIT YOUR DEEPEST, DARKEST FEARS!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: you know what maybe it's time to check my phone.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTECT YOUR HUMAN

n: FROM THE WORLD. FROM OTHER PEOPLE. FROM THEMSELF.

n: GOOD LUCK

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ROUND ONE: *FIGHT!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. Facebook feed says there's a party happening this weekend.

`bb({eyes:"uncertain"});`

b: Doesn't that weirdo throw a party *every* weekend?

`bb({eyes:"uncertain_right"});`

b: What inner void are they trying to fill? They must be deeply messed up inside!

`hong({eyes:"surprise"});`

h: Also, I got an invite?

`bb({eyes:"fear", mouth:"normal"});`

b: Well then!

[Say yes, or we'll die from loneliness!](#act1c_loner)

[Say no, it's full of poisonous drugs!](#act1c_drugs)

[Ignore it, we just make parties sad.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Fifteen cigarettes a day, human! Fifteen!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Then no one will show up at our funeral, they'll dump our ashes into the ocean, we get eaten by a whale,
{{/if}}

{{if !_.fifteencigs}}
b: and we become WHALE POOP!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: So yeah we should go to that party!
{{/if}}

{{if _.parasite}}
b: Just bring the laptop so we can do work, and not be a society-parasite.
{{/if}}

{{if _.whitebread}}
b: Just as long as they don't serve WHITE BREAD
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: GOD. If it'll make you shut up, fine.

h: I'll say yes.

{{if _.whalepoop}}
b: Whale poop, human! Whale poop!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: or even worse... WHITE BREAD
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: We'll overdose on so much meth and white bread they won't be able to fit our fat corpse into the cremation furnace!
{{/if}}

{{if !_.whitebread}}
b: We'll overdose on so many drugs the undertaker will wonder how our body was *already* pre-embalmed!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Besides, can't party, we need to do work or we're a terrible society-parasite!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: GOD. If it'll make you shut up, fine.

h: I'll say no.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: All we ever do is cry in a corner about how loneliness is as deadly as 15 cigarettes a day.
{{/if}}

{{if _.parasite}}
b: All we ever do at parties is worry about how we should be productive instead.
{{/if}}

{{if _.whitebread}}
b: All we ever do is worry about how the unhealthy food options are going to kill us.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: gee i wonder why.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: So if we go we'll make them feel bad, but if we reject their invite we'll also make them feel bad!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ALL WE DO IS MAKE PEOPLE FEEL BAD, SO WE SHOULD FEEL BAD

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. If it'll make you shut up, fine.

h: I'll ignore the invite.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Anyway. Facebook's too much. I need something calmer, less anxiety-producing.

`hong({eyes:"neutral"});`

h: What's new on Twitter?

`bb({eyes:"look"});`

[Oh no, look at that horrible news story!](#act1d_news)

[Oh no, is that tweet secretly about *us?*](#act1d_subtweet)

[Hey, a GIF of a cat drinking milk](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: God, it feels like the world's burning, isn't it?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: It feels like it's all ending, like everything's dying and we're doomed and there's nothing we can do about it.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Let's retweet that story!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Okay I'll retweet it just please be quiet!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Screw it, let's look at Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: It's a subtweet! A sneaky, sneaky subtweet!

`hong({eyes:"annoyed"});`

h: It's probably not?

`bb({eyes:"narrow", mouth:"small"});`

b: but what if they're all talking behind our back

h: They're n--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: IN FRONT OF OUR BACK

`hong({eyes:"sad", mouth:"sad"});`

h: I d--

`bb({eyes:"narrow", mouth:"small"});`

b: but *what if*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *what if*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, gonna try Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh ya that's cute, just retweeted it, I thi--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: CATS CAN'T DIGEST MILK AND WE'RE TERRIBLE PEOPLE FOR ENJOYING ANIMAL ABUSE

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, gonna try Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, photos from yesterday night. So *that's* what those weekly parties are like.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, looks way too crowded for my anxiety.

h: Maybe I shouldn't have said yes to the invite?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Change our answer? Like a jerk?!](#act1e_yes_dontchange)

[Change our answer! It's too crowded!](#act1e_yes_changetono)

{{if _.subtweet}}
[Yeah they were totally subtweeting us.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Wait we retweeted without fact-checking.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[You know, you've got really bad posture?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: They were counting on us to come and now we're betraying their trust? Do you wanna die alone?!

{{if _.fifteencigs}}
b: FIFTEEN. CIGARETTES.
{{/if}}

{{if _.whalepoop}}
b: WHALE. POOP.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll keep it as yes!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Don't you know about human stampedes?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: In 2003 a Rhode Island nightclub had a fire and the panic made people jam the exits so 100 people burned to death-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: DO YOU WANT THAT TO HAPPEN TO US-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: SAY NO SAY NO SAY NO SAY NO SAY NO SAY NO SAY NO SAY NO SAY N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll change my answer to no! God!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... that looks really fun.

h: Maybe I shouldn't have said no to the invite?

`bb({mouth:"normal", eyes:"normal"});`

[Change our answer? Like a jerk?!](#act1e_no_dontchange)

[Change our answer! Don't die alone!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Yeah they were totally subtweeting us.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Wait we retweeted without fact-checking.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[You know, you've got really bad posture?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Everybody was counting on us!

b: ...to leave them alone and let them have a nice party without a horrible disgusting {{if _.whitebread}}white-bread-munching{{/if}} creep like u--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll keep it as no!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chronic loneliness increases our cortisol levels as well as risk for cardiovascular disease and stroke!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: FIFTEEN. CIGARETTES.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Shut up shut up I'll change my answer to yes! God!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: All our problematic tweets have come back to roost!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: We're gonna get called out and cancelled and dragged with a rope on horseback down the information superhighway!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Why are you like this?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: We're spreading disinformation! We're destroying trust in a free press!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: We're the reason fascism will arise from the rubble of democracy!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Why are you like this?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Do you want to have a pretzel for a spine?! Stop hunching over your screen!

```
bb({body:"meta"});
```

b: That means you too.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Why are you like this?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... that looks really fun.

h: Maybe I shouldn't have ignored the invite?

`bb({mouth:"normal", eyes:"normal"});`

[Keep ignoring, we're still party poopers.](#act1e_ignore_continue)

[Actually, say yes.](#act1e_ignore_changetoyes)

[Actually, say no.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: It's kinda rude to keep ignoring them though, no?

`bb({eyes:"normal_right"});`

b: Well other people always ignore *us*, so

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: so let's just call it even.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: You're... letting me have fun?

b: Well, I mean, loneliness *can* kill us.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: It's too crowded. Crowds are dangerous.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Whatever. New Tinder notification.

`bb({eyes:"uncertain"})`

b: What, that hookup app?

`hong({eyes:"annoyed"})`

h: It's not a hookup app, it's just a way to meet new peopl--

`bb({eyes:"narrow"})`

b: It's a hookup app.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, I got a match! They look cute!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Please don't ruin this for m--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: DANGER DANGER DANGER DANGER DANGER DANGER

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Jesteśmy *wykorzystywani* przez innych.](#act1f_used_by_others)

[*Wykorzystujemy* innych.](#act1f_using_others)

[DOPASOWALI CIĘ Z SERYJNYM ZABÓJCĄ](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Random hookups may be able to fill the hole down there,

b: but they can never fill the hole...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: in *here*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: The point is WE'RE GOING TO DIE ALONE

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Myślisz że części intymne innych są jak Pokémony które musimy schwytać?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (pokemon - piosenka przewodnia)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ ^Zdzirą^ być naprawdę chcę-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Jak nigdy dotąd nikt-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Brać za ^chuj^a lub ^cyce^-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ Łydki, łydki, łydki!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ ZBOCZE-MON! CZY JUŻ WSZY-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chodzi o to, że jesteśmy manipulacyjni i zdemoralizowani.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: They'll trap you in a well and force-feed you white bread to fatten you up so they can wear your skin like a suit!
{{/if}}

{{if _.parasite}}
b: They'll bludgeon you with a pomodoro timer and say "YOU SHOULDA BEEN MORE PRODUCTIVE YOU PARASITE"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: They'll tear your flesh to gory confetti, turn your entrails into streamers, and mix your blood into a punch bowl! 
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: How's THAT for a party invite?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: Mam dość tej gry.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"samotność nas uśmierci"... {{/if}}
{{if _.parasite}}"jesteśmy pasożytem społecznym"... {{/if}}
{{if _.whitebread}}"nie jedz tego, to nas zabije"... {{/if}}
{{if _.subtweet}}"obgadują nas za naszymi plecami"... {{/if}}
{{if _.badnews}}"świat płonie"... {{/if}}
{{if _.hookuphole}}"umrzemy samotnie"... {{/if}}
{{if _.serialkiller}}"ta osoba jest seryjną zabójcą"... {{/if}}
{{if _.catmilk}}"koty nie mogą trawić mleka"... {{/if}}
{{if _.pokemon}} ^debilna^ parodia piosenki... {{/if}}

h: ja tylko chcę żyć.

h: ja tylko chcę wolności od tego... cierpienia.

`bb({eyes:"look_sad"});`

b: Hej... człowiek...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Będzie dobrze.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Jako twój lojalny wilk stróż, zawsze mam na oku wszystkie czychające niebezpieczeństwa i będę czynić co tylko w mojej mocy, aby cię chronić.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Obiecuję.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ostatnia aplikacja. Instagram. Co my tu mamy?

`hong({eyes:"sad"});`

h: ... więcej zdjęć z imprez.

`hong({mouth:"sad"});`

h: Wszyscy tu wyglądają na szczęśliwych. Wolni od zmartwięń. Wolni od zgrozy.

`hong({mouth:"anger"});`

h: Boże, czemu ja nie mogę być jak oni? Czemu nie mogę być po prostu *normalnym człowiekiem?*

`bb({eyes:"normal_right"});`

b: A już mówiąc o imprezach, w sprawie zaproszenia na ten weekend, oto moja OSTATECZNA decyzja:

`bb({eyes:"normal"});`

[Powinniśmy iść.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Powinniśmy je odrzucić.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Powin--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^PIERDOL^.*

`hong({body:"2_you"});`

h: SIĘ.

(...500)

b: c

(...1500)

`bb({eyes:"wat_2"});`

b: co?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: IDĘ na tą imprezę,

{{if _.act1g=="go"}}
h: NIE dlatego że ty chcesz, ale dlatego że *JA* chcę.
{{/if}}

{{if _.act1g=="dont"}}
h: Dokładnie DLATEGO że ty nie chcesz.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: NIE sprawujesz nade mną kontrolę.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Teraz wybacz, ale daj mi dokończyć tą kanapkę w ciszy i spokoju ^kurwa^.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AAAAA ZGINIEMY](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AAAAA WSZYSCY NAS NIENAWIDZĄ](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AAAAA JESTEŚMY OKROPNYMI LUDŹMI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AAAAA ZGINIEMY AAAAAAAAAAAAAA

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AAAAA WSZYSCY NAS NIENAWIDZĄ AAAAAAAAAAAAAA

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AAAAA JESTEŚMY OKROPNYMI LUDŹMI AAAAAAAAAAAAAA

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: GRATULACJE

(...500)

n: SUKCESOWNIE OBRONIONO POTRZEBY FIZYCZNE + SOCJALNE + MORALNE SWOJEGO CZŁOWIEKA

n: ALEŻ, PATRZ JAK BARDZO JEST WDZIĘCZNY!

(...500)

n: TERAZ ŻE PASEK ENERGII OSIĄGNĄŁ ZERO, SPRAWUJESZ BEZPOŚREDNIĄ KONTROLĘ NAD DZIAŁANIAMI CZŁOWIEKA

`bb({mouth:"smile", eyes:"normal"});`

n: WYBIERZ RUCH KOŃCOWY

`bb({mouth:"small_lock", eyes:"fear"});`

n: *DOKOŃCZ GO*

[{WALKA: Ukaraj telefon komórkowy, źródło stresu!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{UCIECZKA: Skul się w kłębek i włzaw się!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Twoja komórka daje ci ataku paniki!

`bb({eyes:"anger"})`

b: Zuckerberg i firma uprowadzają twoje zdrowie psychiczne dla inwestycji VC!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Daj swojej komórce nauczkę! Obróć ją w proch! Rozbij ją na miazgę!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNISZCZYĆ ZNI--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Cały świat jest przepełniony zgrozą!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Bądź jak pancernk! Stul się w kulkę w celu samoobrony!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: SKUL SIĘ I PŁACZ SKUL SIĘ I PŁACZ SKUL SIĘ I PŁACZ SKUL SIĘ I PŁACZ SKUL SIĘ I PŁACZ SKUL SIĘ I PŁA-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`
