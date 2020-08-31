# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Zdrówko!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);i
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah*, kopie tak, jak trzeba.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Wiesz...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: A dokładniej, kopie moje lewe oraz prawe ciało migdałowate.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Przypominasz mi mnie z czasów mojej młodości. Kiedy jeszcze dręczył mnie zwierz w mojej głowie.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Tak się cieszę, że mogę ci przekazać to, co wtedy było mi potrzebne, i pomóc ci zabić tę bestię tak, jak ja swoją.

```
publish("act3",["roofhunter",2]);
```

r: Hej, szybkie pytanko: prawda czy wyz--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: WYZWANIE!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Dobra.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Widzisz ten błękitny basen tam na dole?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Taa? Sześć pięter niżej?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Wskocz do niego.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Chwila, co?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: Zwierz zaczął wyć, co?

```
publish("act3",["roofhunter",23]);
```

r: *O nieeee, to niebezpieczne, nie rób tegooo.*

```
publish("act3",["roofhunter",22]);
```

r: Ale właśnie dlatego potrzebujemy doznań na granicy śmierci! Życie to są chwile! Carpe diem! Wciągaj kokę z ^dupy^ ^kurewki^, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Pokaż tej bestii, że kładziemy tłustego *^chuj^a* na jego ^pierdole^nie! Wskakuj.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: No, ale czasami, eee... strach ma jakiś powód...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Przepraszam, czy mam do czynienia z kolejną ofiarą szarlatanów klepiących bzdury, że złe uczucia są niby *dobre?*

```
publish("act3",["roofhunter",17]);
```

r: ^Dupki^, którzy rządzą tym światem, zostawiają *nam* lęk i depresję,

```
publish("act3",["roofhunter",18]);
```

r: A potem wygłaszają TED Talki, gdzie mówią, że musimy "zaakceptować" bycie ^ruchanym^ w ^dupę^, oraz "pogodzić się" z tym demonem-sadystą w naszych głowach!

```
publish("act3",["roofhunter",6]);
```

r: Ja wiem, że *ty* dobrze wiesz, że to zwierzę *krzywdzi* takich jak my. *Torturuje* takich jak my.

```
publish("act3",["roofhunter",19]);
```

r: Nie jest naszym przyjacielem, lecz dziką bestią, którą należy albo *uśpić*,

```
publish("act3",["roofhunter",20]);
```

r: albo *przedziurawić jej łeb*.

```
publish("act3",["roofhunter",27]);
```

r: Inaczej ona wygra.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: A właśnie że nie.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Nie pozwolę jej wygrać.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: I to mi się podoba! Wierzę w ciebie! Dajesz czadu! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: nie nie nie nie nie

n: TEN ROZDZIAŁ MA DWA MOŻLIWE ZAKOŃCZENIA. JEDNO Z NICH JEST *BARDZO, BARDZO ZŁE.*

b: NIE NIE NIE NIE NIE NIE NIE NIE NIE NIE NIE

n: WYBIERZ MĄDRZE. OBROŃ SWOJEGO CZŁOWIEKA

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: POWODZENIA

```
Game.clearText();
bb({ eyes:"start" });
```

[Człowieku, ty tu możesz UMRZEĆ!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[To jest nierozważne i niebezpieczne!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Te chore zwyrole nie są twoimi przyjaciółmi!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: Cz--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Wiesz, twoje sztuczki nie robią już na mnie wrażenia... próbowałeś tego już pierdyliard razy.

h: Jesteś wilkiem, który wołał "wilk!".

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Tego też już próbowałeś.

b: człowieku, proszę...

`hong({ eyes:"look_right" });`

h: O, ja bardzo *przepraszam*, że Big Pharmie nie podoba się moje samoleczenie.

h: Spójrz ^ciul^u, *wszyscy* mamy sposoby na zamknięcie ci ryja.

`hong({ body:"look_up", eyes:"look_up" });`

h: Niektórzy rzucają się w wir pracy.

`hong({ body:"look_down", eyes:"look_down" });`

h: Niektórzy rzucają się w seks, prochy i scrollowanie Facebooka.

`hong({ body:"normal", eyes:"look_right" });`

h: Niektórzy rzucają się w innych ludzi.

`hong({ eyes:"angry" });`

h: Ja rzucę się do tego basenu.

[Po pijanemu? Ten basen jest SZEŚĆ PIĘTER NIŻEJ](#act3_bad_1_harm)

[Kurczę, to tak mi dziękujesz?](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Ok, przyznaję się. Namieszałem.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Nawet jeśli wpadniesz do wody, to napięcie powierzchniowe roztrzaska ci żebra i dostaniesz *co najmniej* wstrząsu mózgu!

h: Ech.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Był taki Rusek na YouTubie, co skoczył i przeżył.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: Ja- przepraszam bardzo, *dziękujesz?*

`bb({ eyes:"angry" });`

b: Właśnie po to *istnieję!* Ponieważ ludziom nie można ufać, że się sami ochronią!

b: Całe życie próbowałem ci uratować skórę, a teraz po pros--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: hehe.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: No ja ^pierdolę^, to bardzo *^kurwa^* mało powiedziane!

`hong({ body:"yell_2" });`

h: Tak, zgniły, ^zasra^ny, krwią zalany śmieciu! Nie dość że namieszałeś, to ^kurwa^ niemiłosiernie z^jeba^łeś!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Coś jeszcze, Kapitanie Oczywisty?

[Ale mszczenie się na mnie to nie ta droga!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ale tym razem *naprawdę* mam rację!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Zraniłem cię.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Musisz mieć zdrowy stosunek do swoich emocji, a nie topić je w--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Tak więc proszę, odłóż butelkę i--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: proszę... nie...

h: Twój pasek energii zdaje się być niemiłosiernie pusty, wilku.

h: Radzę ci dobrać twoje następne słowa bardzo ostrożnie.

`bb({ eyes:"normal" });`

[Dobra. kończę z ochranianiem ciebie.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Cały czas miałem rację.](#act3_bad_2_right)

[Przepraszam.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Tak więc dawaj, skacz. Patrz, jak bardzo się tym przejmę.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: No dobra. Do dna.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: NIE CHWILA CZEKAJ TO BYŁA ODWRÓCONA PSYCHOLOGIA LICZYŁEM NA TO ŻE ZROBISZ NA *ODWRÓT* TO CO PO--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: Wystawiasz się na *niebezpieczeństwo*. Twoi rzekomi koledzy cię *wykorzystują*. A *ty* wykorzystujesz swoich rzekomych kolegów.

`bb({ eyes:"sad" });`

b: Tak więc proszę cię, człowieku... dlaczego mi nie wierzysz?!

h: Bo ty nigdy *mi* nie wierzyłeś.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Inne wilki strażnicze mają ludzi, którzy naprawdę poświęcają czas, by je wytrenować, by *nauczyć* się współpracy.

b: A nie gardzą swoimi wilkami dlatego, że próbują ich chronić! Tak więc dlaczego nie mo--

`bb({ eyes:"normal" });`

h: Błędna odpowiedź, ^chuj^u.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"Jedyną rzeczą, której powinniśmy się bać, jest strach."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Nie smuć się, raduj się!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Wszyscy mędrcy naszych czasów są zgodni: negatywne emocje są *złe!*

`hong({ eyes:"less_angry" });`

h: No pffft! Właśnie dlatego nazywają się *negatywne!*

b: człowieku... proszę...

`hong({ eyes:"normal" });`

h: Pamiętasz moje słowa? “Po prostu pragnę wolności od tego cierpienia.”

h: Moje życzenie się spełniło. Nie czuję już bólu, strachu, ani lęku...

h: Nic już nie czuję.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Tak obsesyjnie dbałem o to, by nikt cię nie skrzywdził, że nie zauważyłem, że to *ja* cię raniłem.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: BRAWO, ^KURWA^.

`hong({ body:"yell_1" });`

h: JA ^PIERDOLĘ^. Tyle czasu potrzebowałeś, by to w końcu zrozumieć?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Mogłeś oszczędzić nam tylu kłopotów, kudłaty tępaku. Czemu tego wcześniej nie zrozumiałeś?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...*przepraszasz.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: *Za co* przepraszasz?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Przepraszam, że nie byłem dobrym obrońcą.](#act3_good_3_protector)

[Przepraszam, że cię nie szanowałem.](#act3_good_3_respect)

[Przepraszam.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Przepraszam, że mam okropnego człowieka!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Przepraszam, że cię nie szanowąłem.](#act3_good_3_respect)

[Przepraszam, że cię zraniłem.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: Moim zadaniem jest ostrzegać cię przed *prawdziwym* niebezpieczeństwem, ale ja warczyłem tylko na auta i listonosza.

`bb({eyes:"sorry_up"});`

b: Warczyłem na cienie. Tyle warczyłem.

`bb({eyes:"sorry"});`

b: *Każdy* chciałby po tym wszystkim założyć mi kaganiec.

`bb({eyes:"sorry_down"});`

b: Przepraszam.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Miałem być *twoim* lojalnym psem-stróżem, ale ja zachowywałem się, jakbyś to *ty* miał się *mnie* słuchać.

`bb({eyes:"sorry_up"});`

b: Jest różnica pomiędzy obrońcą a strażnikiem więziennym, a ja przekroczyłem granicę.

`bb({eyes:"sorry_down"});`

b: Przepraszam.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Tak obsesyjnie dbałem o to, by nikt cię nie skrzywdził, że nie zauważyłem, że to *ja* cię raniłem.

`bb({eyes:"sorry_up"});`

b: Byłem złym psem.

`bb({eyes:"sorry_down"});`

b: Przepraszam.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: No cóż, to tak czy inaczej był głupi pomysł.

h: Moim zamiarem było tylko cię poturbować, i, no cóż, jesteś poturbowany.

h: Powiedzmy, że w tej rundzie mamy remis, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Ok.

h: Ok.

n: *REMIS*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: No chyba sobie jaja robisz. Po tym wszystkim, co ten zwierz ci narobił, tak się po prostu *poddajesz?*

r: Co się dzieje? *Boisz* się?

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Tak.

h2: Boję się.

`publish('hong-next')`

h2: I mam do tego prawo!

`publish('hong-next')`

h2: Nie ma w tym nic złego, że się boję.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Czy to był dźwięk zamykania drzwi?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: nie...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: nie nie nie

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NIE!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
