# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Alors, avant qu'on commence, comment aimerais-*tu* lires ?

`publish("show_options_bottom")`

# intro-start-2

n3: Maintenant, commençons notre histoire...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: CECI EST UN HUMAIN

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: ET CA C'EST L'ANXIÉTE DE CET HUMAIN

n: _TU_ EST L'ANXIÉTE

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nan. Non, nan, j'écoute pas. Je suis sur mon téléphone.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: TON TRAVAIL EST DE LE PROTÉGER *DANGER*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Haa! Tu te défiles de ta vie en allant sur Twitter ! Encore !

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Ouais Je me demande pourquoi je me pose pas à écouter mes pensés plus souvent.

`hong({eyes:"neutral"});`

n: VITE, AVERTIE LES DU *DANGER!*

```
bb({eyes:"look"});
```

[Oh non, regarde cette nouvelle est horrible!](#act1d_news)

[Oh non, c'est un tweet qui parle de *nous* là ?](#act1d_subtweet)

[Ho, un GIF d'un chat qui boit du lait](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Heh moui c'est mignon, Je--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: LES CHATS DIGERES PAS LE LAIT ET ON EST HORRIBLE D'AIMER CETTE CRUAUTÉ SUR UN ANIMAL

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



