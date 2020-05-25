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

h: Hej... Znowu ty i ja?

`hong({eyes:"0_neutral"})`

n: TWOIM ZADANIEM JEST BRONIĆ SWOJEGO CZŁOWIEKA PRZED *NIEBEZPIECZEŃSTWEM*

`bb({eyes:"look", mouth:"small_lock"})`

n: PRAWDĘ MÓWIĄC, PONOWNE GRANIE W TĘ GRĘ STANOWI DLA NIEGO *ZAGROŻENIE* W TEJ CHWILI

n: SZYBKO, OSTRZEŻ GO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Człowieku! Słuchaj, jesteśmy w niebezpieczeństwie! Gracz...

[...będzie nas ponownie maltretować!](#act1_replay_torture)

[...nie odnajdzie alternatywnego zakończenia!](#act1_replay_alternate)

[...doświadczy dysonansu ludonarracyjnego!](#act1_replay_dissonance)

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
b: Sprawi, że rozbijemy telefon wskutek ataku paniki!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Sprawi, że *NIE* uderzymy organizatora imprezy!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Zmusi nas do uderzenia Życzliwego Antyzłoczyńcy, organizatora imprezy!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Może przynajmniej tym razem nie spadniemy z budyn--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: SKŁONI NAS DO ZESKOCZENIA Z DACHU.
{{/if}}

`bb({body:"fear"});`

b: WSZYSTKIE TE OKROPNE RZECZY NAM SIĘ PRZYDARZĄ, A POTEM--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Jasne, przygoda jako *całość* jest taka sama, lecz każdy akt ma dwa możliwe zakończenia, plus liczne rozgałęzione opcje dialo--

`bb({body:"fear"});`

b: Gracz będzie rozczarowany, zamknie przeglądarkę, usunie oprogramowanie, a wtedy--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Dyso- co?

`bb({eyes:"normal"});`

b: Cała ta fabuła jest o *WYBORACH* budujących zdrową relację z lękiem,

`bb({eyes:"normal_right"});`

b: Ale ponowne przejście gry doprowadzi tak czy inaczej do tej samej historii, co implikuje że twoje *WYBORY* nie mają znaczenia,

`bb({eyes:"narrow_eyebrow"});`

b: Co daje sprzeczność pomiędzy przesłaniem a mechaniką gry,

`bb({eyes:"fear"});`

b: I ujawnia strukturę tego narracyjnego wszechświata,

`bb({body:"fear"});`

b: Skutkiem czego--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: ZGINIEEEEEEEEEEEEEEMY

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

h: Dobra, wróćmy teraz do naszych ról.

```
Game.clearText();
```

n4: (POZWÓL _SWOIM_ LĘKOM BLA BLA BLA CO _CIEBIE_ NIEPOKOIŁOBY BLA BLA WIESZ CO ROBIĆ)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: O pięknie, mój wilk powrócił. Cudoooooownie.

`hong({eyes:"0_neutral"})`

n: TWOIM ZADANIEM JEST BRONIĆ SWOJEGO CZŁOWIEKA PRZED *NIEBEZPIECZEŃSTWEM*

`bb({eyes:"look", mouth:"small_lock"})`

n: PRAWDĘ MÓWIĄC, TA KANAPKA STANOWI DLA NIEGO *ZAGROŻENIE* W TEJ CHWILI

n: SZYBKO, OSTRZEŻ GO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Człowieku! Słuchaj, jesteśmy w niebezpieczeństwie! Grozi nam to, że...

`bb({body:"squeeze"})`

n4: (POZWÓL _SWOIM_ LĘKOM WEJŚĆ W ŻYCIE! WYBIERZ CO _CIEBIE_ NIEPOKOIŁOBY NAJBARDZIEJ)

(#act1_normal_choice)

# act1_normal_choice

[Jemy samotnie lunch! Znowu!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Nie jesteśmy produktywni podczas jedzenia!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Ten chleb pszenny jest dla nas niezdrowy!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Nie wiesz, że samotność wpływa na ryzyko przedwczesnej śmierci niczym wypalanie 15 papierosów dziennie?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Em, dzięki że podajesz źródła, ale--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Co oznacza, że jeśli nie będziemy spędzać czasu z kimś *w tej chwili*, to-

`bb({body:"panic"})`

b: ZGINIEEEEEEEEEEEEEEMY

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: UŻYTO *LĘKU PRZED SAMOTNOŚCIĄ*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Wyjmij laptopa i zacznij pracować teraz!

`hong({eyes:"0_annoyed"})`

h: Em, wolę nie mieć klawiatury pełnej okru--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Jeżeli nie wnosimy swojego wkładu w ciało społeczne, to jesteśmy pasożytem społecznym!

b: Ciało społeczne pójdzie do doktora społecznego, który przypisze mu lek przeciw społecznym pasożytom, i wtedy-- 

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ZGINIEEEEEEEEEEEEEEMY

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: UŻYTO *LĘKU PRZED BYCIEM ZŁĄ OSOBĄ*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Czy te badania zostały powtórzone na--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Przetworzona pszenica podniesie poziom cukru w naszej krwi, więc będą musieli amputować nam wszystkie kończyny, a potem-

`bb({body:"panic"})`

b: ZGINIEEEEEEEEEEEEEEMY

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: UŻYTO *LĘKU PRZED ZROBIENIEM SOBIE KRZYWDY*

(#act1b)

# act1b

n: TO BYŁO SUPER EFEKTYWNE

`bb({mouth:"smile", eyes:"smile"});`

b: Widzisz, człowieku? Jestem twoim lojalnym wilkiem stróżem!

`bb({body:"pride_talk"});`

b: Ufaj swym instynktom! Twoje uczucia zawsze są prawidłowe!

`bb({body:"pride"});`

n: OBNIŻ PASEK MOCY TWOJEGO CZŁOWIEKA DO ZERA

n: DO OBRONY JEGO POTRZEB FIZYCZNYCH + SOCJALNYCH + MORALNYCH, MOŻESZ UŻYĆ:

n: LĘKU PRZED *KRZYWDĄ* #harm#

n: LĘKU PRZED *SAMOTNOŚCIĄ* #alone#

n: I LĘKU PRZED *BYCIEM ZŁĄ OSOBĄ* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (MAŁA RADA: WYBIERAJ TE OPCJE, KTÓRE SĄ TWOIMI NAJWIĘKSZYMI, NAJGŁĘBSZYMI OBAWAMI!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: wiesz co, czas sprawdzić mój telefon.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: OBROŃ SWOJEGO CZŁOWIEKA

n: PRZED ŚWIATEM. PRZED INNYMI LUDŹMI. PRZED SAMYM SOBĄ.

n: POWODZENIA

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: RUNDA 1: *WALCZ!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Zobaczmy, na Facebooku jest post o imprezie w ten weekend.

`bb({eyes:"uncertain"});`

b: Czy to dziwadło przypadkiem nie urządza imprez w *każdy* weekend?

`bb({eyes:"uncertain_right"});`

b: Jaką wewnętrzną pustkę stara się wypełnić? Musi mieć naprawdę narąbane w głowie!

`hong({eyes:"surprise"});`

h: I do tego mam na nią zaproszenie?

`bb({eyes:"fear", mouth:"normal"});`

b: No to...!

[Przyjmij, inaczej zginiemy z samotności!](#act1c_loner)

[Odrzuć, imprezy są pełne prochów!](#act1c_drugs)

[Zignoruj je, i tak psujemy atmosferę.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Piętnaście papierosów dziennie, człowieku! Piętnaście!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Nikt nie zjawi się na naszym pogrzebie, wysypią nasz popiół do oceanu, zjedzą nas wieloryby,
{{/if}}

{{if !_.fifteencigs}}
b: i staniemy się WIELORYBIĄ KUPĄ!
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
b: Czyli tak, idziemy na tę imprezę!
{{/if}}

{{if _.parasite}}
b: Tylko nie zapomnij laptopa, żebyśmy mogli pracować i nie być pasożytem społecznym.
{{/if}}

{{if _.whitebread}}
b: Oby tylko nie serwowali CHLEBA PSZENNEGO
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: BOŻE. Jeżeli to cię w końcu uciszy, zgoda.

h: Przyjmę zaproszenie.

{{if _.whalepoop}}
b: Kupa wieloryba, człowieku! Kupa!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: albo jeszcze gorzej... BIAŁEGO CHLEBA
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Przedawkujemy metamfetaminę i chleb pszenny, a jak będą nas kremować, to nie będą w stanie wpakować naszego tłustego cielska do pieca!!
{{/if}}

{{if !_.whitebread}}
b: Przedawkujemy narkotyki tak mocno, że grabarz będzie się dziwić, jakim cudem nasze ciało *już* zostało zabalsamowane!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Zresztą, nie możemy imprezować, trzeba pracować, bo inaczej jesteśmy pasożytami społecznymi!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: BOŻE. Jeżeli to cię w końcu uciszy, zgoda.

h: Powiem, że nie idę.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Jedyne co robimy na imprezach, to siedzimy w kącie i płaczemy nad tym, że samotność jest równoważna paleniu piętnastu papierosów dziennie.
{{/if}}

{{if _.parasite}}
b: Jedyne co robimy na imprezach, to zamartwiamy się tym, jak bardzo jesteśmy nieproduktywni.
{{/if}}

{{if _.whitebread}}
b: Jedyne co robimy na imprezach, to zamartwiamy się tym, jak niezdrowa dieta może nas zabić.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: rany ciekawe czemu.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Więc jeśli pójdziemy to ich zasmucimy, ale nie idąc również ich zasmucimy!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: PRZEZ NAS LUDZIE SĄ TYLKO SMUTNI, WIĘC POWINNIŚMY SIĘ TYLKO SMUCIĆ

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ech. Jeżeli to cię w końcu uciszy, zgoda.

h: Zignoruję zaproszenie.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Zresztą, Facebook mnie przerasta. Potrzebuję czegoś spokojniejszego, mniej niepokojącego.

`hong({eyes:"neutral"});`

h: Ciekawe co słychać na Twitterze?

`bb({eyes:"look"});`

[O nie, spójrz na tę okropną historię we wiadomościach!](#act1d_news)

[O nie, czy ten tweet jest tak naprawdę *o nas?*](#act1d_subtweet)

[Hej spójrz, kotek pije mleko](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Boże, wydawać się mogło, że cały świat płonie, co nie?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Jakby wszytko dobiegało końca, wszystko ginęło, jesteśmy straceni i nic nie możemy na to poradzić.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Udostępnijmy tę historię!

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

h: Okej, zrobię to, ale bądź już cicho!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Olać to, sprawdźmy Snapa.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: Obgadują nas! Podstępnie nas obgadują!

`hong({eyes:"annoyed"});`

h: Chyba raczej nie?

`bb({eyes:"narrow", mouth:"small"});`

b: a jeśli wszyscy gadają za naszymi plecami

h: Co ty, nie--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: PRZED NASZYMI PLECAMI

`hong({eyes:"sad", mouth:"sad"});`

h: Wątp--

`bb({eyes:"narrow", mouth:"small"});`

b: ale *co jeśli*

h: Z--

`bb({eyes:"narrow_eyebrow"});`

b: *co jeśli*

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

h: okeeeej, może Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Ano! Ale słitaśne, udostępnię to, pewnie--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: KOTY NIE POTRAFIĄ TRAWIĆ MLEKA I JESTEŚMY OKROPNYMI LUDŹMI CIESZĄC SIĘ NA WIDOK ZNĘCANYCH ZWIERZĄT

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

h: okeeeej, może Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Oho, fotki z wczorajszej nocy. A więc to *tak* wyglądają te cotygodniowe imprezy.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Aj, wygląda tłoczno. Trochę się cykam.

h: Może jednak nie trzeba było przyjmować tego zaproszenia?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Zmienić odpowiedź? Jak jakiś matoł?!](#act1e_yes_dontchange)

[Zmień odpowiedź! Tam jest za dużo ludu!](#act1e_yes_changetono)

{{if _.subtweet}}
[O tak, obgadują nas na sto procent.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Czekaj, udostępniliśmy coś bez zweryfikowania faktów.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[[Wiesz, że masz naprawdę złą posturę?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Liczyli na to, że przybędziemy, a teraz chcesz zdradzić ich zaufanie? Chcesz umrzeć samotnie?!

{{if _.fifteencigs}}
b: PIĘTNAŚCIE. PAPIEROSÓW.
{{/if}}

{{if _.whalepoop}}
b: KUPA. WIELORYBA.
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

h: Zamknij się, zamknij pysk, decyzja to nadal tak!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: A co jeśli będzie masowa panika?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: W 2003 roku w klubie nocnym w Rhode Island wybuchł pożar i masowa panika spowodowała zablokowanie wyjść, przez co 100 ludzi spłonęło żywcem-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: CZY CHCESZ ABY NAM TO SIĘ PRZYDARZYŁO-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: NIE IDŹ NIE IDŹ NIE IDŹ NIE IDŹ NIE IDŹ NIE I-


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

h: Zamknij się, zamknij pysk, zmieniam zdanie na nie! Boże!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... wygląda na to że się naprawdę dobrze bawią.

h: Może trzeba było jednak przyjąć zaproszenie?

`bb({mouth:"normal", eyes:"normal"});`

[Zmienić odpowiedź? Jak jakiś matoł?!](#act1e_no_dontchange)

[Zmień odpowiedź! Nie chcemy zginąć sami!](#act1e_no_changetoyes)

{{if _.subtweet}}
[O tak, obgadują nas na sto procent.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Czekaj, udostępniliśmy coś bez zweryfikowania faktów.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Wiesz, że masz naprawdę złą posturę?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Wszyscy liczyli na nas!

b: ...abyśmy ich zostawili w spokoju i pozwolili się dobrze bawić bez okropnego, obrzydliwego{{if _.whitebread}}, pszenicożernego {{/if}} dziwaka takiego jak m--


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

h: Zamknij się, zamknij pysk, nadal nie idę!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Przewlekła samotność podnosi nasz poziom kortyzolu, a także ryzyko chorób układu krążenia i zawału! 

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: PIĘTNAŚCIE. PAPIEROSÓW.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Zamknij się, zamknij się, zmieniam decyzję na tak! Boże!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Wszystkie nasze problematyczne tweety obracają się przeciwko nam!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Zostaniemy wytknięci, odrzuceni i odwleczeni konno po infostradzie! 

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

h: Czemu musisz być takim...?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Rozpowszechniamy dezinformację! Niszczymy zaufanie do wolnej prasy!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: To przez takich jak my faszyzm wyłoni się z gruzów demokracji!

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

h: Czemu musisz być takim...?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chcesz mieć precel z kręgosłupa?! Przestań garbić się przed tym ekranem!

```
bb({body:"meta"});
```

b: Hej, ty również.

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

h: Czemu musisz być takim...?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... wygląda na to że się naprawdę dobrze bawią.

h: Może nie trzeba było ignorować zaproszenia?

`bb({mouth:"normal", eyes:"normal"});`

[Ignoruj ich dalej, i tak psujemy zabawę.](#act1e_ignore_continue)

[Wiesz co, przyjmij.](#act1e_ignore_changetoyes)

[Wiesz co, odrzuć.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: To trochę nieuprzejme wszystkich ciągle ignorować, co nie?

`bb({eyes:"normal_right"});`

b: Znaczy się, inni ciągle ignorują *nas*, więc

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: więc jesteśmy kwita.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Czyli... pozwalasz mi na zabawę?

b: No spójrz, samotność *może* nas zabić.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Tam jest zbyt tłoczno. Tłumy są niebezpieczne.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Mniejsza z tym. Mam powiadomienie na Tinderze.

`bb({eyes:"uncertain"})`

b: Co, na tej apce do podrywania?

`hong({eyes:"annoyed"})`

h: To nie apka do podrywania, tylko sposób poznawania nowych lu--

`bb({eyes:"narrow"})`

b: Apka do podrywania.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oho, dopasowanie! Ale słodko wygląda!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Błagam tylko mi tego nie popsu--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: UWAGA UWAGA UWAGA UWAGA

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Inni nas *wykorzystują*.](#act1f_used_by_others)

[*Wykorzystujemy* innych.](#act1f_using_others)

[DOPASOWALI CIĘ Z SERYJNYM ZABÓJCĄ](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Przygodne podrywy być może wypełnią pustkę jaką masz tam na dole,

b: Ale nigdy nie wypełnią pustki...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *tu*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Chodzi mi o to, że UMRZEMY SAMOTNIE

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

b: ♫ ^Kurwiszczem^ być naprawdę chcę-

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

b: ♫ Cyc, ^dupę^, uda pieść-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ ^Fiut^, ^jajca^ i łydki!-

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

b: Chodzi mi o to, że jesteśmy manipulacyjni i zdemoralizowani.

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
b: Wepchnie cię do studni i utuczy pszenicą, aby następnie cię obedrzeć ze skóry i nosić ją jak garnitur!
{{/if}}

{{if _.parasite}}
b: Zatłucze cię na miazgę minutnikiem kuchennym, ostatnie co usłyszysz to "TRZEBA BYŁO PRACOWAĆ PASOŻYCIE"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Rozszarpie twe ciało niczym krwawe konfetti, przerobi twe bebechy na serpentyny, naleje krew do wazy na poncz! 

{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Co powiesz na TAKIE zaproszenie?!
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

h: Mam dosyć tej gry.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"samotność nas uśmierci"... {{/if}}
{{if _.parasite}}"jesteśmy pasożytem społecznym"... {{/if}}
{{if _.whitebread}}"nie jedz tego, to nas zabije"... {{/if}}
{{if _.subtweet}}"obgadują nas za naszymi plecami"... {{/if}}
{{if _.badnews}}"świat płonie"... {{/if}}
{{if _.hookuphole}}"umrzemy samotnie"... {{/if}}
{{if _.serialkiller}}"ta osoba jest seryjnym zabójcą"... {{/if}}
{{if _.catmilk}}"koty nie potrafią trawić mleka"... {{/if}}
{{if _.pokemon}} ^debilna^ parodia piosenki... {{/if}}

h: ja tylko chcę żyć.

h: ja tylko chcę wolności od tego... cierpienia.

`bb({eyes:"look_sad"});`

b: Hej... człowieku...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Będzie dobrze.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Jako twój lojalny wilk stróż zawsze mam na oku wszystkie czyhające niebezpieczeństwa, i będę czynić co tylko w mojej mocy, aby cię chronić.

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

h: Wszyscy tu wyglądają na szczęśliwych. Wolni od zmartwień. Wolni od lęku.

`hong({mouth:"anger"});`

h: Boże, czemu ja nie mogę być jak oni? Czemu nie mogę być po prostu *normalnym człowiekiem?*

`bb({eyes:"normal_right"});`

b: Skoro mówimy o imprezach, w sprawie zaproszenia na ten weekend, oto moja OSTATECZNA decyzja:

`bb({eyes:"normal"});`

[Powinniśmy iść.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Powinniśmy nie iść.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

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

h: IDĘ na tę imprezę,

{{if _.act1g=="go"}}
h: NIE dlatego że ty chcesz, ale dlatego że *JA* chcę.
{{/if}}

{{if _.act1g=="dont"}}
h: Dokładnie DLATEGO, że ty nie chcesz.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: NIE sprawujesz nade mną kontroli.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: A teraz daj mi dokończyć tę pyszną kanapkę w ^pierdolonej^ ciszy i spokoju.

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

n: UDAŁO CI SIĘ OCHRONIĆ POTRZEBY FIZYCZNE + SPOŁECZNE + MORALNE SWOJEGO CZŁOWIEKA

n: SPÓJRZ TYLKO JAK BARDZO JEST CI WDZIĘCZNY!

(...500)

n: JAKO ŻE PASEK MOCY OSIĄGNĄŁ ZERO, SPRAWUJESZ BEZPOŚREDNIĄ KONTROLĘ NAD DZIAŁANIAMI CZŁOWIEKA

`bb({mouth:"smile", eyes:"normal"});`

n: WYBIERZ RUCH KOŃCOWY

`bb({mouth:"small_lock", eyes:"fear"});`

n: *WYKOŃCZ GO*

[{WALKA: Ukarz telefon komórkowy, źródło stresu!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{UCIECZKA: Skul się w kłębek i rycz!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Twoja komórka przyprawiła cię o atak paniki!

`bb({eyes:"anger"})`

b: Zuckerberg i spółka dewastuje twoje zdrowie psychiczne, by zbić kokosy na inwestycjach venture capital!

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

b: ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZCZ JĄ ZNISZ--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Cały świat jest pełen zagrożeń!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Bądź jak pancernik! Stul się w kulkę w celu samoobrony!

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
