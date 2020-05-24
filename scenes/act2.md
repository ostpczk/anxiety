# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: A *widzieliście* tę "wiadomość" że gdzieś tam, coś tam złego się wydarzyło?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: h-hej...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Jak ja nie znoszę takich newsów. Czysta sensacja i clickbait.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: f... fajna impreza...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Niby prawda, ale ludzie to piszą, bo jest na to popyt. *Prawdziwym* problemem są ludzie, którzy klikają w ten chłam.

```
publish("act2",["dee",3]);
```

s: Co za chory ^pojeb^ udostępnia takie smutne wiadomości, i zasmuca wszystkich swoich przyjaciół?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: No! Masakra.

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: A *widzieliście* ten "artykuł", co wszędzie wisi na mediach społecznościowych?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: h-hej...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Jasne! Fejk nius widoczny na kilometr. Jak można w to wierzyć, i do tego taki chłam udostępniać?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: f... fajna impreza...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: No cholerka, ziomek. Tak boli sprawdzenie w Google czy to w ogóle prawda?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: No! Masakra.

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Tak więc powtarzam, Kompleks Memiczno-Przemysłowy wykorzystuje koty.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: h-hej...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Rozwiń tę tezę.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: f... fajna impreza...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: No zobacz, wczoraj ktoś zretweetował GIF kota pijącego mleko.

```
publish("act2",["dee",3]);
```

s: Przecież one nie trawią tego ^szajsu^! Co za człowiek udostępnia *znęcanie się nad zwierzętami*?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: No! Masakra.

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: No więc się odpowiedzi nie doczekałem!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: h-hej...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Pomimo tego, że mieliście dopasowanie na Tinderze?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: f... fajna impreza...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: No dokładnie! Co, boi się że ja niby *seryjny zabójca* jestem czy co? Paranoja.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: No! Masakra.

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: No dokładnie! Myśli, że przygodnym seksem nie da się wypełnić pustki w sercu?

s: Nie można być taką cnotką niewydymką! Otwórz umysł, rozłóż nogi!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: No! Masakra.

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: No dokładnie! Wyglądem w ogóle nie zwala z nóg, ale i tak byłoby branie!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Złap je wszystkie!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: RUNDA 2: *WALCZ!*

[O nie, oni wszyscy nas nienawidzą!](#act2a_social)

[*Wlepiasz wzrok* w tego rudzielca?](#act2a_perv)

[Hej, porozmawiajmy o sensie życia.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Psujemy nastrój tej imprezy będąc takim smutasem!

`bb({eyes:"shock", body:"two_up"})`

b: Zabijamy pozytywne wibracje! Popełniamy morderstwo wibracji z premedytacją!

`bb({eyes:"normal", body:"normal"})`

b: Człowieku, musimy stąd iść *teraz*, zanim--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Jest o wiele bardziej seksi od nas, więc jeśli tylko na niego *spojrzymy*, to znaczy, że--

`bb({eyes:"shock", body:"two_up"})`

b: JESTEŚMY CREEPAMI

`bb({body:"normal"})`

b: Jesteśmy odrażającymi, złymi do szpiku kości, niedobrymi, obleśnymi, okropnymi zbok--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Jeśli by tak na to wszystko spojrzeć, to co prawdziwie sensownego możemy zrobić? 

`bb({body:"normal", eyes:"sad"})`

b: Wnieść coś do dziedzictwa ludzkości? Wszystkie wielkie dzieła obracają się w gruz niczym Ozymandias. Miłość? Śmierć ostatecznie wszystkich rozłączy.

`bb({eyes:"sad_r"})`

b: A ile tej śmierci jest! *My* zginiemy. *Nasi bliscy* zginą.

`bb({eyes:"shock", body:"two_up"})`

b: Kurdebele, druga zasada termodynamiki oznacza, że nawet nasz *wszechświat* zginie!

`bb({eyes:"suspect", body:"normal"})`

b: I pewnie powiesz, "dzięki śmierci możemy docenić wartość życia"? Równie dobrze możesz powiedzieć, że niewolnictwo jest dobre, bo sprawia, że doceniamy wolność!

`bb({body:"one_up"})`

b: Co jeszcze, "sens życia trzeba znaleźć samemu"? Tak postępują sekciarze, szury i foliarze!

`bb({eyes:"shock", body:"two_up"})`

b: Życie nie ma znaczenia, śmierć nie ma znaczenia, nawet *znaczenie* nie ma znaczenia! Co dusza śmiertelna ma--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Eee... człowieku, słyszysz mnie?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *WDECH*

`bb({mouth:"small_talk"})`

b: MUSZĘ CIĘ OSTRZEC PRZED...

[Tym samym zagrożeniem, ale *bardziej*!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[*Innym* zagrożeniem społecznym!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[*Innym* zagrożeniem moralnym!](#act2b_different_moral)
{{/if}}

[Ignorujesz zagrożenie! To niebezpieczne!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: EMOCJE SĄ ZARAŹLIWE! JEŻELI STĄD NIE PÓJDZIESZ, TO ZARAZISZ WSZYSTKICH SWOJĄ CHOROBĄ PSYCHICZNĄ!

b: Spowodujesz zabójczą epidemię ZESPOŁU SMUTASA

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Musimy stąd zwiewać i poddać się permanentnej kwarantannie w małym pokoju z Netflixem i jedzeniem na telefon!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "kwarantannie";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NIE BĄDŹ CREEPEM. TO JEST NIEZGODNE Z PRAWEM!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Ustawa o creepach, art. 74e ust. 1: Osoba fizyczna, która wpatruje się w: 1) te umięśnione ramiona, 2) tę pupcię jak marzenie - będzie zwana dalej

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "WIELKIM, OBLEŚNYM, PASKUDNYM ZBOCZEŃCEM".

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "prawie karnym";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: I wiesz co, nawet jeśli uda ci się znaleźć szlachetny cel w życiu, *nadal* możesz wszystko spartaczyć!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel marzył o pokoju na świecie oraz wzajemnym porozumieniu między kulturami. Z tego powodu chciał uczynić podróż łatwiejszą.

`bb({eyes:"normal_r"})`

b: Potrzebował zatem taniej metody budowy tuneli dla pociągów. Dlatego wynalazł nowy materiał zwany "dynamitem"...

`bb({body:"one_up", eyes:"normal"})`

b: Który został wykorzystany w I wojnie światowej by ZABIĆ MILIONY LUDZI

`bb({body:"two_up", eyes:"shock"})`

b: OTO EFEKT MOTYLA, CZŁOWIEKU! ILU LUDZI WŁAŚNIE ZABIJASZ PRZEZ PRZYPADEK W TEJ CHWILI

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "I wojnie światowej";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Prawdę mówiąc, wiesz co jest gorsze od bycia nielubianym przez nikogo? Bycie lubianym przez *każdego*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Innymi słowy, stanie się jednym z *tych* imprezowiczów, stale szukających doznań.

`bb({body:"normal", mouth:"small"})`

b: Płytkie życie z płytkimi kolegami, znającymi tylko płytkiego ciebie!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Człowieku, musimy uciekać od tych hedonistycznych zombi zanim zamienią nas w jednego z nich!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombi";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Ludzie giną z głodu i padają ofiarą ludobójstw *w tej chwili*, a my nic, tylko imprezujemy!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Pewien mądry człowiek raz powiedział, "aby zło zatriumfowało, wystarczy, by dobry człowiek niczego nie robił."

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: A MY NIC NIE ROBIMY.

`bb({mouth:"small"})`

b: CHODZĄC NA IMPREZY, POMAGAMY *HITLEROWI*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitlerze";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Myślisz że nic ci nie grozi, gdy wyjmiesz baterie z czujnika czadu?

`bb({eyes:"suspect_r"})`

b: Nawet nie poczujesz trucizny! Tylko napadnie cię senność a potem--

`bb({body:"scream_c_1"})`

b: ZGINIEEEEEEEEEEEEESZ

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "tlenku węgla";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Nareszcie, człowieku, chyba znowu mnie słyszysz!

`bb({eyes:"closed", body:"point"})`

b: OSTRZEGAM CIĘ PRZED...

{{if _.a2_first_choice=="louder"}}
[Tym samym zagrożeniem, ale *jeszcze bardziej*!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[Tym samym zagrożeniem, ale *bardziej*!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[*Innym* zagrożeniem społecznym!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[*Innym* zagrożeniem moralnym!](#act2c_different_moral)
{{/if}}

[Czy masz pewność co pijesz?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: Właściwie, Netflix i jedzenie na telefon nie jest dostateczną kwarantanną! Zarazimy dostawcę!

`bb({body:"one_up", mouth:"small"})`

b: Musimy wyjechać na Syberię, gdzie będą nam dostarczać jedzenie dronem!

`bb({body:"two_up", mouth:"normal"})`

b: A potem będą musieli wysterylizować drona, by zabić wszystkie nasze ZARAZKI SMUTASKI

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "kwarantannie";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: 2. WIELKI, OBLEŚNY, PASKUDNY ZBOCZENIEC podlega karze 72-godzinnego pobytu w jednej z tych średniowiecznych maszyn do publicznego upokarzania.

b: 3. Przepisu ust. 2 nie stosuje się, w przypadku gdy takie coś go *kręci*,

`bb({body:"scream_a_1"})`

b: ponieważ jest WIELKIM, OBLEŚNYM, PASKUDNYM ZBOCZEŃCEM

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "prawie karnym";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFEKT MOTYLA! Używasz niebiodegradowalnego kubka z plastiku?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BACH, TOKSYNY Z WYSYPISKA PRZECIEKNĄ I ZABIJĄ DZIECKO

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Pocisz się i serce wali ci jak młot?

`bb({body:"scream_a_1"})`

b: BACH, PRZEZ CIEBIE NASZ SYSTEM OPIEKI ZDROWOTNEJ ZBANKRUTUJE I MILIONY LUDZI ZGINĄ

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "efekcie motyla";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Te hedonistyczne zombi zmierzą w twoim kierunku, zawodząc:

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: LAAAAAJKI. LAAAAAAAAAAJKI.

`bb({body:"scream_a_1"})`

b: Następnie cię CHAPNĄ i zamienią w DURNEGO DRESA i/lub KOŁTUŃSKĄ KARYNĘ!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombi";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: NAZIŚCI MARSZUJĄ WŁAŚNIE KROKIEM DEFILADOWYM PO ULICACH

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: I mówią, *jak dobrze, że ci 'dobrzy ludzie' się obijają, skupieni na takich bzdurach jak 'relaks' czy 'dbanie o siebie'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Teraz wszystko pójdzie po naszej myśli; jak dodamy gazu, to nie zabraknie nam czasu!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitlerze";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Tak się zastanawiam, czy w tym budynku w ogóle *jest* czujnik czadu?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: A co, jeśli my wszyscy wdychamy tlenek węgla *W TYM MOMENCIE?*

`bb({body:"scream_a_1"})`

b: NAWET NIE ZOBACZYMY JAK ŚMIERĆ NADCHODZI. PO PROSTU PRZESTANIEMY ISTNIEĆ NA WIEKI WIEKÓW--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "tlenku węgla";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: A co, jeśli po prostu jesteśmy *u podstaw naszej osobowości niezdolni* do bycia kochanym, albo kochania innych?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Co jeśli coś wewnątrz nas nieodwracalnie pękło dawno temu? Albo nigdy nie było w nas obecne?

`bb({body:"scream_a_1"})`

b: AAA JESTEŚMY ZEPSUCI! TACY ZEPSUCI TACY ZEPSUCI TACY ZEPSU--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: A co, jeśli po prostu jesteśmy *zepsuci do szpiku kości?*

`bb({body:"one_up", eyes:"sad"})`

b: Inni mają w naturze czynienie dobra, ale my czynimy "dobro" tylko z poczucia winy bądź wstydu, jeżeli w ogóle.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: Co jeśli w naszej naturze jest zadawanie ludziom krzywdy? Co jeśli nie możemy być niczym **innym* jak kulą u nogi naszych najbliższych?

`bb({body:"scream_a_1"})`

b: AAA JESTEŚMY ZEPSUCI! TACY ZEPSUCI TACY ZEPSUCI TACY ZEPSU--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Nie jestem irracjonalny. *Istnieją* ludzie, którzy dodają narkotyki do alkoholu. To jest prawdziwa rzecz, która faktycznie się zdarza.

`bb({eyes:"suspect"})`

b: Człowieku, czy nie boli cię głowa? Czy nie wiotczeją ci kończyny? Mam wrażenie że umieramy.

`bb({body:"scream_a_1"})`

b: AAA UMIERAMY! UMIERAMY UMIERAMY UMIERA--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "drinkach";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: K^UUUCHWA^!

h: JA P^IERDOL^Ę C^HUJ^ W D^UPĘ^ *K^UURRRWA^ MAĆ*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Hura, człowieku! Jak ja się cieszę że znowu mnie słyszysz!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Dlaczego nie odpowiadasz?

`hong({body:"facepalm"})`

h: Do ^diabła^, ty skończony debilu.

`hong({body:"facepalm_2"})`

h: Znasz tę indiańską opowiastkę?

h: "W tobie mieszkają dwa wilki, nadzieja i rozpacz, który zwycięży? Ten, którego karmisz."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Moim celem było cię *zagłodzić*, ty sadystyczny ^dupku^!

`hong({body:"smile", mouth:"smile"})`

h: Walić to, spróbuję afirmacji.

h: *Ludzie mnie kochają. Jestem osobą dobrą. Mądrą. Piękną. Wyjątkową.*

`bb({eyes:"suspect"});`

[Rany julek, ależ z ciebie narcyz!](#act2d_narcissist)

[Wiesz że afirmacje *nie działają?*](#act2d_disproven)

[omygy nie przypisuj randomowych historyjek kulturom rdzennym](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Prawdę mówiąc, osobom o niskim poczuciu własnej wartości tylko *pogarszają* sprawę!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Było takie badanie – randomizowane kontrolowane badanie kliniczne; eksperymentator nie wiedział, kto był w jakiej grupie.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Wynik: osoby z niskim poczuciem własnej wartości, proszone o powtarzanie afirmacji czują się *gorzej* niż gdyby nic nie mówiły!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Sprawdź w Google Scholar, człowieku,

`bb({body:"scream_b_1"})`

b: A POTEM PRZESTAŃ ROZPROWADZAĆ ANTYNAUKOWE FAKE NEWSY

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: *Musisz* pokornie uświadomić sobie własne wady, by stać się lepszym człowiekiem!

`bb({body:"two_up", eyes:"suspect"})`

b: Zapleśniałego pokoju nie uratujesz odświeżaczem powietrza! Wypierając się swoich wad tylko sobie szkodzisz.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Na szczęście ja, twój lojalny wilk-stróż, mogę ci ujawnić twoje wady. W chwili obecnej, jest nimi-

`bb({body:"scream_b_1"})`

b: WSZYSTKO. WSZYSTKO JEST ŹLE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Indianie to *prawdziwi ludzie*, a nie jakieś "szlachetne dzikusy", którymi możesz się podeprzeć, by twoje porady niczym z ciasteczka szczęścia brzmiały nieco bardziej *egzotycznie*.

`bb({eyes:"suspect_r"})`

b: Degradujesz indywidualne osoby oraz bogate kultury do roli pocztówki! To jest "życzliwy rasizm"!

`bb({body:"scream_b_1"})`

b: SKOŃCZ Z TYM RASIZMEM TY SKOŚNOOKI PATAFIANIE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^CHUJDUPAKURWA^.

`hong({body:"yell", mouth:"yell"})`

h: Wiesz co? Jesteś *irracjonalny*.

h: Wszyscy wiedza, że emocje są irracjonalne! W szczególności strach!

`hong({body:"facepalm_2"})`

h: Jesteś bezużyteczną pozostałością ewolucyjną, jak wyrostek robaczkowy lub zęby mądrości!

`hong({body:"yell", mouth:"yell"})`

h: ^Kurwa^, cała ta metafora z wilkami jest do bani! Jesteś jedynie kapką neurochemikaliów w mojej głowie.

`hong({body:"cross", mouth:"cross"})`

h: Dlaczego mam słuchać bezwartościowego, irracjonalnego, nieistniejącego ^zasrań^ca takiego jak ty?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Jeżu, człowieku! To bardzo krzywdzące słowa.](#act2e_hurtful)

[Jestem uczuciem. Uczucia są prawidłowe.](#act2e_valid)

[Człowieku, ty *też* "jesteś jedynie kapką chemikaliów."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Jestem *częścią* ciebie, dobrze o tym wiesz. Mówiąc takie rzeczy, ranisz *siebie*.

`bb({body:"scream_a_1"})`

b: Dlaczego się bijesz, człowieku? PRZESTAŃ SIĘ BIĆ.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Twoje najgłębsze motywacje to dopamina, twoja najpromienniejsza radość to serotonina.

`bb({body:"one_up"});`

b: Twoje wspomnienia to wagi synaptyczne, twój rozum to sygnały elektryczne podatne na zakłócenia.

`bb({eyes:"normal", body:"normal"});`

b: Więc jeśli twierdzisz, że *ja* jestem irracjonalny, bo jestem "jedynie kapką chemikaliów"... to co dopiero *ty*!

`bb({body:"two_up", eyes:"shock"});`

b: A jeśli *oboje* jesteśmy irracjonalni, to znaczy że *nigdy* nie uda nam się odkryć, jak być spełnionym i szczęśliwym!

`bb({body:"scream_a_1"})`

b: AAA JESTEŚMY ZEPSUCI! TACY ZEPSUCI TACY ZEPSUCI TACY ZEPSU--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Poczekaj... "oni" mówią, że uczucia są prawidłowe, że zawsze należy akceptować swoje emocje.

`bb({eyes:"suspect_r"});`

b: Ale "oni" twierdzą też, że emocje są irracjonalne, że nie można im ufać.

`bb({eyes:"angry"});`

b: O nie, "oni" cały ten czas nas okłamywali!

`bb({body:"scream_a_1"})`

b: "ONI" KARMIĄ NAS SPRZECZNYMI TREŚCIAMI, BY UZALEZNIĆ NAS OD PRZEMYSŁU COACHINGOWEGO

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Nie wytrzymam. Boże, to tak boli, ja *nie zniosę* tego.

h: Nie umiem cię udobruchać. Nie umiem cię ignorować. Nie umiem z tobą walczyć. 

`bb({eyes:"suspect"});`

h: Nieważne co robię, nie mogę się ciebie pozby--

`bb({body:"cry_1"});`

b: No bo może ty NIE MASZ SIĘ MNIE *POZBYĆ*.

`bb({body:"cry_2"});`

b: Jak myślisz, jak *ja* się czuję, człowieku?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Z całych sił staram się być twoim wiernym psem stróżem, ale ty widzisz we mnie Wielkiego Złego Wilka!

b: Więc próbuję jeszcze *bardziej* ostrzec cię przed niebezpieczeństwem! *Większymi* zagrożeniami! *Innymi* zagrożeniami!

`bb({eyes:"cry_2"})`

b: Ale nieważne, jak bardzo staram się ciebie obronić, ty *wciąż* myślisz, że jestem twoim wrogiem!

`bb({body:"cry_5"});`

b: Co robię nie tak?!

`bb({body:"cry_2"});`

b: *Wiem*, jestem beznadziejny w tym, co robię. Ale *próbuję*, człowieku!

`bb({body:"cry_3"});`

b: ...Naprawdę próbuję.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Nie musisz słuchać moich ostrzeżeń, albo się ze mną zgadzać, albo nawet mnie *lubić*.

`bb({eyes:"cry_r_2"});`

b: Jedyne czego chcę... to odrobiny cierpliwości.

`bb({eyes:"cry_r_3"});`

b: Proszę cię, pobądź ze mną jeszcze chwilkę, nie odwracaj się ode mnie i--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Hejka.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Wyglądasz, jakby twoje myśli rozkładały cię na łopatki.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Aż tak bardzo to widać?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: No, było słychać jak drzesz się na swoją bluzę i gadasz coś o {{_.a2_hoodie_callback}}.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: o jeżu, jestem w totalnej rozsypce.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Hej. Wyluzuj, jesteś w dobrym gronie. Lęk dopada każdego z nas.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Kurde, dosłownie wczoraj opowiadali mi, jak komuś na kampusie puściły nerwy i rozbił telefon!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Kurde, dosłownie wczoraj opowiadali mi, że widzieli kogoś zwiniętego w kulkę jak pancernik, jak płakał przy ludziach!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Słuchaj: znam z autopsji to, o czym mówisz, tego zwierza w głowie.

```
publish("act2",["party_hunter",8]);
```

r: Tak jak my *wszyscy*. Właśnie dlatego robię te imprezki co weekend - by zapomnieć o naszych troskach, zapomnieć o tej bestii.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ale mój lęk...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Głowa do góry. Zwierzę ci się, moje życie było dawniej takie jak twoje. Aż w końcu ja i znajomi poznaliśmy sposób na wyciszenie tego dołującego głosu na zawsze...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: Domowej roboty. Kopie nieco mocniej niż... jakby to powiedzieć, cokolwiek co można dostać legalnie.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Dajesz, do dna!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[O mój Boże.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[To nie jest dobry sposób radzenia sobie z problemami.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Nie przyjmuj drinków od nieznajomych.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: N--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, jaki wykwintny bukiet!

h: Bogaty aromat "wyłącz swój umysł," z delikatną nutą "nigdy w życiu nie poczujesz nic więcej"!

b: To jest złe, człowieku. To jest naprawdę, naprawdę złe.

[W ten sposób zaczyna się uzależnienie.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[*Wiedziałem*, że gospodarz jest porządnie popaprany!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Do tej flaszki mogli ci wsypać prochy!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: W ten--

(#act2h)

# act2h_opt2

b: Do tej flaszki mogli--

(#act2h)

# act2h_opt3

b: *Wiedziałem*, że--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Wyborne, i do tego tańsze od terapii!

b: CZŁOWIEKU BŁAGAM CIĘ PRZESTAŃ

h: Hehehe!

h: I co mi teraz zrobisz, ^kutafonie^?

b: Tak mi przykro, człowieku.

b: Będę musiał użyć mojego ATAKU SPECJALNEGO

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Co ty  ^odpierdala^sz?

h: Będziesz dalej kłapać tym *pyskiem*, by--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: CO TO DO DIASKA BYŁO

b: Wybacz mi. Musiałem ci pokazać konsekwencje.

{{if _.SPECIAL_ATTACK=="harm"}}
h: MÓJ WŁASNY *TRUP* STANĄŁ MI PRZED *OCZAMI*. OBLAZŁO MNIE DOZNANIE BYCIA *MARTWYM*.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: *WSZYSCY* PATRZYLI SIĘ NA MNIE Z *OBRZYDZENIEM*. BYŁO *SŁYCHAĆ WSZYSTKO*, CO MÓWILI.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: W MOICH *USZACH* ROZLEGŁ SIĘ *TRZASK* PĘKAJĄCYCH *ŻEBER*. W MOICH *USTACH SMAK KRWI* W POWIETRZU.
{{/if}}

b: Wybacz, człowieku.

n: *WYKOŃCZ GO*

[{WALKA: Sprzedaj gospodarzowi cios w nos.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{UCIECZKA: Spadamy stąd.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Ten rudzielec-psychol cię wykorzystywał.

b: Próbował cię zdemoralizować, spaczyć do takiego samego stopnia!

`bb({ body:"yell_angry_1" });`

b: Zdziel psychola w pysk! Wal bez litości!

`bb({ body:"final_1" });`

b: UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDERZ UDE--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: *Wiedziałem*, że wszyscy ci imprezowicze to porąbani ludzie. Wszyscy uśmierzają swój ból paskudnymi rzeczami!

`bb({ body:"yell_1" });`

b: I próbują cię podpuścić; liczą na to, że zrobisz to samo! Oni cię demoralizują! Musimy stąd zwiewać!

`bb({ body:"final_1" });`

b: ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWAĆ ZWIEWA--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Wszystko ok?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-ty...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: ty *perwersie*.

r: Podoba mi się to. Przyjdź na imprezę za tydzień, złotko.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok, cześć, ciao, adios, au revoir

r: Może dzisiaj twój zwierz wygrał, ale wróć, a uwarzę dla ciebie coś jeszcze mocniejszego!

h2: sayōnara, auf Wiedersehen, zài jiàn, szalom

r: Ty i ja, razem pokażemy tej bestii, kto tu rządzi!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok sorry muszę spadać

`publish("act2",["party_hunter",16]);`

r: Cholera. Zwierz dzisiaj wygrał?

`publish("act2",["party_hunter",15]);`

h2: nie, nie, ja, eee, idę przebiec maraton. szybko jak błyskawica.

`publish("act2",["party_hunter",19]);`

r: Przyjdź na imprezę za tydzień, skarbie. Uwarzę dla ciebie coś jeszcze mocniejszego.

h2: ok dzięx muszę biec biec biec biec biec

r: Ty i ja, razem pokażemy tej bestii, kto tu rządzi!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Człowieku! Wszystko okej?!

```
publish("act2", ["act2_end","next"]);
```

b: Jejuniu, było *blisko.* Mogliśmy naprawdę--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Idę na imprezę za tydzień.

h: Gdy następnym razem się spotkamy, to ja cię nie tylko *pokonam*...

h: Ja cię ^kurwa^ *zabiję*.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)