# World of Warcraft

my WoW Addons and Settings Export

See my [Addon-List](https://github.com/svenflender/wow/blob/main/Addon.md)

## Addons 

### Baganator - Categories

Bag Addon - [Baganator](https://www.curseforge.com/wow/addons/baganator)

Last Change: 24.09.2024
```json
{"categories":[{"source":"23","name":"Gegenstandsaufwertung","search":"#Gegenstandsaufwertung|Tapferkeitsstein|Vorbotenwappen|Wachsklumpen"},{"source":"11","name":"Dunkelmond-Jahrmarkt","search":"Dunkelmond-Jahrmarkt|Dunkelmond-Spielpreis|Dunkelmond-Ticket"},{"source":"12","name":"Items","search":"!war within&!Dunkelmond&!Goblingleiter"},{"source":"13","name":"Seelengebunden","search":"seelengebunden&#rüstung&#ausrüstung&>400"},{"source":"17","name":"Beim Anlegen gebunden","search":"!seelengebunden&#rüstung&#ausrüstung&>400"},{"source":"27","name":"Schlüsselstein","search":"Schlüsselstein&Seelengebunden&Mythische"},{"source":"8","name":"Wappenröcke","search":"Wappenrock"},{"source":"14","name":"Kampfhaustiere","search":"#kamphaustier|#Haustier"},{"source":"15","name":"Kochen","search":"fleisch|fisch|kochkunst|Portioniertes Steak"},{"source":"25","name":"Beim Anlegen gebunden","search":"!seelengebunden&(einhändig|zweihändig|wurfwaffe|schildhand|nebenhand|köcher)&>400"},{"source":"4","name":"Optionales Handwerksmaterial","search":"optionale reagenzien|Funke der Omen"},{"source":"1","name":"Monfest","search":"Mondfest"},{"source":"5","name":"Ingenieurskunst","search":"teile"},{"source":"3","name":"Juwelierskunst","search":"juwelierskunst&!Rüstung&!Anlegen"},{"source":"2","name":"Verzauberkunst","search":"verzauberkunst"},{"source":"19","name":"Kürschnerei","search":"leder&!Rüstung&!Anlegen"},{"source":"18","name":"Fertigungsreagenzien","search":"fertigungsreagenzien|#reagenz"},{"source":"7","name":"Bergbau","search":"metalle steine"},{"source":"6","name":"Inschriftenkunde","search":"inschriftenkunde"},{"source":"9","name":"Schneiderei","search":"stoffe|faden|#handwerksmaterial&Band|Schneiderei"},{"source":"24","name":"Seelengebunden","search":"seelengebunden&(einhändig|zweihändig|wurfwaffe|schildhand|nebenhand|köcher)&>400"},{"source":"16","name":"Kräuterkunde","search":"kräuter"},{"source":"26","name":"Steinmetzkunst","search":"gewichtsstein|schleifstein"},{"source":"20","name":"Berufswissen","search":"wissen&studieren"},{"source":"21","name":"Truhen und Beutel","search":"Truhe|Geldbeutel|Vorratspaket|Schließkassette|Kapital des Wesirs"},{"source":"22","name":"Braufest","search":"Braufest"},{"source":"10","name":"Kampfkuriosität","search":"Kuriosität"}],"version":1,"order":["27","21","default_hearthstone","default_potion","default_food","default_consumable","10","----","_Berufe","5","2","9","19","16","7","3","6","15","4","18","default_tradegoods","default_reagent","default_gem","default_recipe","20","__end","----","_Rüstung","17","13","8","default_profession","default_auto_equipment_sets","default_armor","__end","_Waffen","24","25","26","__end","----","default_container","default_questitem","default_key","default_miscellaneous","23","14","default_battlepet","default_toy","default_other","default_junk","default_special_empty","----","_Feiertag","11","1","22","__end","----","_Alte Erweiterungen","12","__end"],"modifications":[{"showGroupPrefix":true,"source":"23","priority":0},{"showGroupPrefix":true,"source":"22","priority":3},{"showGroupPrefix":true,"source":"21","priority":3},{"showGroupPrefix":true,"source":"20","priority":3},{"showGroupPrefix":true,"source":"26","priority":3},{"showGroupPrefix":true,"source":"27","priority":3},{"source":"8","priority":3},{"source":"9","priority":0},{"source":"default_tradegoods","priority":-1},{"source":"default_hearthstone","priority":3},{"showGroupPrefix":true,"source":"25","priority":0},{"items":[221763,213611],"source":"18","priority":0},{"items":[228414,228956],"source":"5","priority":0},{"source":"15","priority":0},{"source":"default_battlepet","priority":3},{"items":[116406],"source":"default_food"},{"items":[21100],"source":"1","priority":0},{"showGroupPrefix":true,"source":"default_key","priority":-1},{"items":[211806],"source":"3","priority":0},{"source":"2","priority":0},{"items":[222649,224807],"source":"19","priority":0},{"source":"4","priority":0},{"items":[222553],"source":"7","priority":0},{"source":"6","priority":0},{"source":"14","priority":3},{"showGroupPrefix":true,"source":"24","priority":0},{"source":"16","priority":0},{"source":"17","priority":3},{"showGroupPrefix":true,"source":"13","priority":3},{"showGroupPrefix":true,"source":"12","group":"expansion","priority":2},{"items":[92794,72018],"source":"11","priority":0},{"source":"10","priority":0}],"hidden":[]}
```

## Macros

### Priest - Mount and Angelic Feather

Change the mount and spellnames to your used ones

```
/cast [nocombat,swimming]Dunkelwasserrochen;[nocombat,outdoors,flyable]Leuchtender Sternensucher;[nocombat,outdoors]Erneuerter Protodrache;[nocombat,outdoors,noflyable]Schecke;[nocombat,nostance,@player][combat,@player]Engelsfeder;[@player]Engelsfeder
```

### Focus Macro with Icon

Change the Icon ID to your favorite one

**Icons:**  
0 No Icon  
1	Star  
2	Circle  
3	Diamond  
4	Triangle  
5	Moon  
6	Square  
7	Cross (X)  
8	Skull  

**Usage:**
1. Select Target
2. Klick Macro
3. Kill Mob

Delete Focus: Shift + Klick Marco

```
/focus [exists][]
/run if GetRaidTargetIndex("focus") then SetRaidTarget("focus",0) end
/clearfocus [mod:shift, exists]
/run if not GetRaidTargetIndex("focus") then SetRaidTarget("focus",3) end
```

### Focus/Mouseover/Target Interrupt

Change the spellname to your used one

```
#showtooltip Zurechtweisung
/cast [@focus,exists][@mouseover,exists][@target] Zurechtweisung
```

## Weak Auras

### Fishing - Wiederverwendbarer übergroßer Schwimmer

Displays an icon that shows the remaining duration of the ![reusable oversized bobber](https://wow.zamimg.com/images/wow/icons/large/achievement_profession_fishing_outlandangler.jpg) [reusable oversized bobber](https://www.wowhead.com/de/item=202207/wiederverwendbarer-%C3%BCbergro%C3%9Fer-schwimmer) and casts the fishing rod when clicked.

> [!WARNING]
> This Weak Aura uses [Secure Frames](https://github.com/WeakAuras/WeakAuras2/wiki/protected-frames)

```
!WA:2!fw1tVTrru844iHyRq0gAsAdvOvb1qsPK2K(NuQuLQxh7Mao2H1o02dG9S7o27qwpZYmZ68hqO2CQhr(ax4MpuXb4I)cakFcgzvXhGEGpa5la8MzTtBdiHpSEE)zM379B(9EtMIt2EYGjdE2c9i(mAvwc3hFPXgGsKHmELyjHrfZ(N9ejEJe(jh5(XyxcnorYte41Wc)WUTtIKKicfhYdWnrG04RSdEFhjEpP7UKazywVimTLmCkhkQn2PgyOlS9sgLHQjCBXzjX90gttJmh6ZIIqXcCO6mz7d(MFKmNY2eZBbgEB32iFot9oQP6grAtK1GKZHYO4UMZtl6jiTJJW9djbyxmdsqEdhb5a8u9rbFtIqId2eT34VsGqhNVFLMnfy563VXtg7jJngyL6dqYwmcv6LVq5AfCh4ZyrbSDPv3LeJBC0iXcbqM5OXZghk5KwTWCXhmpF4YNRbTYqv2OlkHJ01RywVB8PRENvw1f3bdh)6yuKm8LaOBK3IJBs2ZT6wfkv6qrmokAJaH1jMRM0em3VE(CvRvVATCU1CsOePxCeAFm31ealaF1rBLEbypWFnSWxVqPTkUDPUj0HPM18Ql)C1eQBOwsDn1IQROUUAz1NyP(y1vvZ3qTIL6JMn(8FEegqsUnG8HyQTdorIv3uDl1TTIphYxs6GRLEGBYcW)6yhdqgMtrrFjaeah6NFzmN1IJfI0l6RCPXgVRah10aUkBihfijKTsCOM55IBPzE3DA1edarpK)o67wAWZoF8KAcwDrica(hLELLj(IgLMpnz82iWHHluZ09eBZDzr8zFTTdSlg)ZYKjt2xMQDug5KB7AvIFpJsOXGbNdX)HAoTtoq840ar2dhyu(0bPuLhpmDoYyxtTin3hQootcvMM)7uUs5cQj4qrP9PNXrFtAKf(1DyfqLXNTiNCG9xKGcaubzxR2Bu4JI0aJUDbg(d5O4dF4WfPjqhIGaTGngwZVgDo(CBuUCb36ovQvRYMUB8G1Rn4Kqxf6tU4Wk6rVrC0wn8OkBxR0gLl8xdAfX2Tih)TjyQ)(BnX1xALBLwDAdhP)SM(wfUmZEOwsV7bEjsjJwPdMd81EA1PJeMQVE9OsRRwi)jqZrqp0dgPj045jjN5Kdj(7qbgwwZgR6JIWzD0ldnkkbtQeNZenhZaHqVqmPvO8PormuqN(ejUnuiqFDWSxy8F)xogcy9xtzONeosQCAxZKpREA7(S2EizORFesiMwrTCGUvF9c17R)gFwWRCdNYyg6eEAveAypUHVRbh1hUscjOFK3QRSXDEmPYQD6IOK2gi82UcjIllEegjWvLCdO9wq37mdcgIY11tQ5cmmjkqCO2pZHoJtBeHwuTVXB1bQVt99Qz8AsOer4Pv3NqtBDGZZIV3WPI)Xx9c1yWpUUDh6nVTApl1py5ahHC(UbS6(qbXA3Wl9)9Y81KM2uM0wpeQoM2zP0RDBjmbXYg(fXG7iBU99ELlP4GX6P329SZZXqxuromDBH5CmAN7Q2ZLhsMe45Lrk4GUQy)eooNjttnuddpiaBFUfTTTW0alRtfG7wflZffzApelS4)YSEKeCJXlY45JaQMyH5kHBktp91G3a05YR0SD8Cl(Fgcjm5feHsqFvP3Kz(o49)J7PUDv7LVXY3C1BUOZbmw7m9BQHdGlaZiY2tY87KoW9cz(T(Zrc8YrBHJOXtAEkn9TkycTlaenCrrXHOSQZS(936D)7FeUApoTN3GWMxrRM3TqHYEazQjP10QPMwzn4A(iH0UjWBi0wCcvhqm0aCsJA85h9QOEG3AebcMbfe2ttjjgQJ1HJ8OXX7GXX509msxnHlCsH3TwA5vxA5j78Ih9pd
```
### Wago.io Links

- [Tamas The War Within Helper](https://wago.io/TamasTheWarWithinHelper)
- [Myu's Knowledge Points Tracker](https://wago.io/L7lpDrqUO/10)
- [Luxthos WeakAuras](https://www.luxthos.com/)

## Details

Profile

```
T37AZroYvIH(BXH)G0iRUnsaK4rhE)qXMf7MUjl2ll2tVZgt0GOQcSkiIcOmaQMdBpIHES279gATLT3iU3B4RTLJWYr4V4i0Q3EKwPpm)b6(FKpNt(apkufk2BpRVwxnpizHczMN88(CYtM5RyV6IxnEvE2vXjr4FM96O8WKKGPjrH5bPr3uMLpFryr5Ro4vJNgUQCDEuqEuyc(YlWFdpVyvusYu5lTmUy6SWYq8VdxNt)oknkF(T4FnlCz48i4VkF148SBcUkCwuqCk0BJyVAm8hJmF1iJhAIF)QKWBJYdMfvggNueCtC6SSBWXTyAiaTydkUgAY4HjV(fh)QXtaiUm6Zqq8vJhF9TjXPry)GZhrFveecG)88S1RE1KxnEDruqX08SKe8t5rRYYldWjva00RlepCjGsOz8YGRYZwgKgUmsmptJxUEzGgJLTCsyzqz8se0mGj9RJsHpNho96OCeSJsdNKend72RYGVAAwswUyMJ)Nj9tl6N24pbqhNcaefpFrj8eh5dQ3qJhYK4mrJPFBJ)2c7aAGkweIyUXJoB0q1JIFJemPpEv4uaNDuE8BU7Y)01HZYbc4DxEbIRxaujahDZSPWlc4QGvVEjof66lwHiMRYrmKQPLXLje(QOe70xn(KZEjsQME9S8SvTNkoQ5IJAY4iNn2Ue(idqMeguHuSmG5WnXZkxanLBOrAAgHdfSp3D54O8O04YBbM8vLXzPfbkiTK4gfK)YSGBwK9QXiZyrzy60OIGIO5lbAzrGC4rrbs(yDkXljEuzwwsz8kCMl)ZGLHFwq4K4K4Y4OIxnYtWJ2AoB6RM04FzP)lfpq9oBvuzb(2JdNmjp61XH4eHEaW2olsW)3bJLXd9zUsCAvpJubCcKotdngCBzdO)Ys)xerWti2cniAgmk5GynslMf)64IS89HHgWJRlcMmVI(CCAzuoY)9PJF(Wto5GZo7zF6yuHYKSSRFWZbTfpae0bcXcyeaP1OO0GvzfYHHB4(qxAOEGf34HCfppYtMTwJLfZP2ZFjodiZLRlakJglyjXbwsmGLE(pIdt4ro4pCF14xMLNmBm08iG9cWhrvdpGjcYjw0M0b32artrC3M07YW85ksEmmNeYTah2lfV7tPFvQXp5rjalXRJWEzL6PaTQmtOUeLidxceWsseE9eKEeCdO)Av4kGyEGa8Xrrk5s6iaDBldtNvqYkv0WMmYEYzONeP5jrAMkKIqjZWpBvEurXnHGG4KSCKaSB(gsMw(MAUMdsIFZBcZNbkPKIDv49DZbsZpHcXAZw4lz6rr(aqDlqdIxIiJLrLlYMrirjQo7QRkIkBXGvrjwLfNsWDzz2Yg4mymKCVhX5Eg2CtlptdptlB7xD1deYFh5zzA6WnnT98y(owg43qCJh564AZSSzUUwChMVf(nCC6De3W0XG5AZ9nmTSC9f9wPKZPcdsGaYeDoPyWK55Yb9YKOURhZe(Wf1)Wb1ETsjtKctPqKO5AW6AdTswGIzuarzAmUaTgwSGm9Uc8raS(UkcuEEKRPb3L757AB67y4ykMtJrnaldZVwOvRImfcwEPXq0(aWum0XVokHmuanmD9YO8yWlHGIBlkJwc)A5KSKc0Jequym51HySrTTqlMffwUiqj6vScgvemf(CuSt3uQStqctttINEnAgjBvukYITHlvtxaFmkDUWSOY2IqSeqSfORoRq7fOOh6prq5TRIiDaOJvuhLUEfynAE2AsqUcesZaFxMiDvAIW3N40GmqhJCUiKHj7wXPZdaE143acbaUAE4kKhgWfxfUoPe5wdtwTieNPCH3sazeukiSzaMfZHPwaGRkeQoiQlqTtNc02u4)jJdrP3c6Tb1qa(POa0NxiSzuGEdbkFZJkNUq4BfI)r9Wtu046(N1IQd8xwsx4IsUsQdbvQbyIzGMHaY3WAJeA8wzXoyYAqUmLGKLGlE53ga(cak2TPzb8IXiBtseYuDqB2dP7gGbNQExGDf(wwiCXlFAuq4uqDm40b5xOYdPPjHargLkbFlwcKO6wbhmB2zPfFQ0TLpng9xU4tPMePF9A(MSEfPpvkAH0V2C)epRYNNo8IUSdjQWptjrjrYOhW4CyMy2HYrbGs8viN(SBbNIJNQCfw7GloFq(nH2VgQ(lRXzhaSGZJtHyjqwCL4YvjHZfkHfgtNCl68EAiOmaOuBk5aQan0EXHgvleZ72sFOag28gI2OCKq2g)RAc3IamEz2lV7snjs0P5XcDijjXZke8iAXgbZiQc13MHaLg3bsuW0Vqmvqevt4tksRbp4XHlxjnY8aVAUXykmP9agPHxfmsJGqazwqvd8PWjbrlNenRvqi4ZPOzaND)mL9mKb626FOa0sO5VHMvI8VzRbT6IObRIQdgORbNZazM8BlxanJehj5xLiRzTWpQXzmIzkCSGKelxaCjlYsMrmFGO3maTeqHtbVQLPsrdXdkcqdhjaQqLblIJsMviEakMPn4o(PVy0fdpVPf7hIw4uoDZvESq25E5GZp)4Z267lFxM4Lh)0bNoyunN65kUiBWeVdA6S7r50bpzy)nR5G98HxShJKLRAKOgD45V44dR8W1Lz4tVb1wBGp1gm825WD6zJEMUH6HZYXVEtEOEEzjCt4WHdU4PpB0Xp5PDcSBRzdhn80pzR0OwZPZp7jVOc7vdby2CoU5C6fJE2iiq0nNvBd998ZpE44l2ZXAdQ8ZhCYGdpE0wNxTXcdaTkO(9ToEgGJsEU2EDdSaR7jN94NTNu7nG2dhcK8MslkYTkYOTb4pf9lCFh3wq9lg9KZp7fp)5Nm4tQnW9tAg(XN9SAnGBy5lgeQzBNPE8U0g0CmOWWrFK2iUBL9Fqho8NyAM02ybfJtYZcNHzgd8tQMMxTPRkV9cUokcCljQOecYphCEyjr)pOsngysPd1yp0Xvf3LkAv7UuF9qxv8zoQefzB1bR5d9v5GHRqfUwBOOYM1kypFYm0GZhoAqWNaHXRLTQhfMI)QBcTkXdQ0oy3wRftZgPsmHDB1tngmU)20d56QP3kaJMJJhEYrvXZ6BWuPMXYKXvPKs88wAF0Pzr9w2SnnlOGF1m0ZTlvrA3pKq2gAFAgyRgT)KZhoCulSjRoUSHQvGIXyU1ZlYdHPLtvCYT1HWv8pCvN66VnLfokAjZVX7cEguqcoGtrJg(IloFWjDXM0HqTcRWDD08h(ETngA1Ifsk6w5Pi6Xa4VvHi7XcFUMNhUAr8uuuBrwPiRwGxTRsIUQKYYn4ONWVN2Ejxc(Topkx5PmVYlBrqgrZIl7kgp01zOjcpwjx3cP0gk)ZNNHj8Xe9MnCwm5EKJHeoW4jtfHyEd5Bx2mrQDOqKj1gLKBt0NfXnYAgLQYDzoLEdvGlQelPYeLnVkVQGThSlaNN32BZaUd1BBXO3oln5wmGhmlRZ7mKprmyecIYlf5Dp4TyefAKiwoW15LugIsVkEooIxjuMkYFa1T)ZwJyJzrLrtjTYuw7bVxrI0uWl1Pli3dHiJH4DYllKFyrucqSw1aYwI(TonygeLyKONWqFQi7HtNsXdwkJjcHA1xw0GsVcE(0GLzeRtJaaejobIYTyt3)LXhQxyKTgwIWMaobR5G7ihZAwnz(ClwhgpBzSFeZgSGOfYBB08HQx2r82Gdavg35TCgODxJ5JFF8EgEr2o8rS97AUdFdA(UWCZRsPK(TD3YKZKxn7uUAX6ggS33WiG3LVl)FB)6oo3dVLHoFx0UnF7Aydltp2MyKnBI)UGhTtsEYx3zRu8nExUR7UCYRnTPgZDhast31gX9y7GpDJU2EhVCRE20HVdm(gVSZUy)24TRqiAWWB7V9ozT3Gn0XFB82B(UUg7cqA)61E7TR2PnJfZWC7i9MsBUSTc5TWjmdRTtCA1PMBLrTf7bZWEhi62kCCT2fQRvxx7L7GNEd2uR9pOiaQ57aqAPoZHTNXbb6dC2HSsBICLSsFr8oQMm4MIvT44Q7oJOvGJbbYvfeSTdobr1NWTOBmqmAF2Ro6bCpicwBMLjUQgEM4sTydF1nV6ihFpFFhdB4N(MmFCXhW1qyXRoY3WWf8j2WYIZ4CtdX3GoucbJjhaZhAyyWSC4GQyxiYeCWaFNGiFzgUMGwloZdxodASeRw9cXVl1lMs1cqkZCk43tC68cADpSceROe6ggM00YKiCrKXgMksFD6A1R0CXOgxGEmkxQ35b5WufN7(mtdlUJVJNdcyoWqUgxT1Al9fLVF0Ft0dKGSRK5vKsQMizSY0NVZvAtMnFYBUaQat6nn31BsrGPUYfq3LckWm7olox6Nh6we5Eg6uFys880GLRb3ScQHbrVPccUjSGwngX60xCtm69j61f6SzbU(i1MFOV1Lla)3NVqTEee0SXxMJlMYKAKKDvYba0rRac52gq6KbvmEvY65XIagUP1CJiSIHMqZhGy5dqK8bio(a0d(deRf94IvyEPPfmsIYOawKtvr6zZ1vTbYxOCav5qVUKAclbuhqFfEHRyiKSdKJ5hurAvCyi)18TYFvntQwqjqodB0KT2iDjIOrRuz(C3LhKeMETKruToQgEo2mpBdWeQlA0L6cCDu3Y3yT1VrTGZcUFKZifbaTAMAzXjofJNLiJVomznH)niLK77lATVVO9((I899fD23x0DFFrV99f933xKzS3V5EtBy7nXHT3uh2EtEy7l9PSLYMQv0TMW02R2bz11fNEvMUsS6k(Amc59tZm9QIHvyGvkktjA4e0obvUDYOxfRFuHOwOeRQSOyyW)IsSc(hYIJqiWH9Z5Q(rUoNh0Q7REmnJUkK0wQ1kDv8NHzLP7sGQgQrOT8IUHPOYBIIsRbub3wB1WKkJcQkDQGA5NLmhSja3Sqz6UwK0lyQKECeAe7tp68J)Z)tVii4HxCXryUpQMVKIz9609awnyB66caTUbDvbAYVM0Qn(FowrbSV9dV7s6VS(20Vm)2nltqqxnMkJeIGUE1kWrb6ZVAmvPwfF6GPXZoiNwKC47JYFcwMwp8utSI9UP6TP6L6th(N98bJgF8zJmm)0dp7SdhC44p9XzjZcZZd)0hF2jho48ZhCYzp(fJF4st14vVsee9znPiXd0Vct1OQxPSYGcoh2J6eQQcjRVKPByI)GW8dixNU7stfhZjbT4yobxD(0IK4sbAVw9lAwJWTFsIOD3AvU34n5gmustKucvmUT8GyIUSGapsUgxaymrujH32QMUCBw1A4VvgiVhE11O4fQR34866nAPFQdgC6XZZdVv4TYevNiiqnyS1F3eQ(Bb49FsBbeCwxPXOTq9UKypIBBydrs4bXtyz76Xf1Ruz7(B7DIMrHOqPRxorwbnBQeCFuEifSRVqrAeqxI73D5xxkN)n1c(FuxC3hLeQvn3v3JZYfaJCcXmxJr4O84O0zfhHvy7N(IJFG8ZNexu(GNw1afx3MJ8HFT4PLRx2Pg33p5eikli(HWRW0hR9JDJoFJjVuRcJsASYWjXjUTkaKQjjT5svvgUJASwZVuhddnduHnLQHCzA8PKFhSQqM97kACr0QqO7a2eznElyi6uUGQwKP5zb6LRu4eVPiD7vjMV2ZPIG5uA1jsaky8ujgywube5kmYQQApb0eJf(XfBwPZByfwPwvsg25lxkdbKCxsoAYGBW61pQZiNn1roBPF7sm2HjKtkG(MqDzmkdMMILKC9hDZcNgKJbhOCvqSmq6iKKrgu3crvPLQJnQE1lcyZMcKyb48T11kpUwhIsdsHv2SOzR)QuXeP4d2N6VUrIcEatSMEwvKJ2krRgSMFkyYCX6Gup3bkS4ykFgGLXXHVwu1riBm0fJpC4fdo(KXbJVyWfVy8bdop45N8INC8OGhtR1OelV9x75h(8X6vzd74D)MszRh3pEbFT)StXk8vA88icVpyk4ytewDK3D5Zbka(HP3kEJbykh0R124YBtesl0N0opGF6tovu6W7CMnE4toD4OlUhWSCXMUqvCO7hy3ywkNdSpmZHhlxW47dsFFbyNgaS5gamWuEHsn5UG(sPi9EqjkBSNosRVtoSWphLgTu(PYwQJAMtjvYkvkwBkeA6kXo1xGCRnvNzRvNzGj1QAVOeeuKgU6PuWHn1SxTDz01Y7rooMUE(g2CMVl4cdtwR1GBvtW8DGHRDWg6hRYkyJOsJtftsCTERGKQDjGQgxf0cvoKuOgTd7clm1ClR5wmPHN(6IBMs)6rpG7y6B7WzU22U2UCk7TEuwyD5((EMWpnb30yEugF9bJQIcZ)IZE(jdpQvzWQteRoY5kqu6QYh8movkdwVg6Ep84tGP)4wjaoygQbwkZ5i3wmIjwTnFvnR2cZCtANPWMSVTzedsIxgx2018wuwThlKb1PRZbBALDM8vH)yyjqrSPOr(oYfk(ersmul3orCGpaEufolQUnHsD67AmlwLvepnm7)TBfceKxInSPNgGqxevfjmv6Lv50LK6avxIQfry6vYGx5futSt1waQ5GupSBr9DCKTpeXJpZZL56dtzcpztQzvBSKnkfl5I3uBNkr7mbDuWh5zyYnm98yUE2GankAyJ72rQ(7vvfUw6Bx2tATNY2wObA391v2Ny)Fv3RuQcwItL7x0de416D(Xp(SrJ)0Jh9Xbabioj4cCZuSSvQPnnDDbokdqteZXQ2w8zlFJ12(grviQwSH6Bk0A(GThQoWWt6CHsAVqgTYfWMfMw1McKGn52iMQTjAX4oqxp(ftxeTueffwsqHfvi1MBTIDTgkQQ0ruDpvvpeTPyMKNDTCdI1CZBQAfH00rEornWyPLxvBLZIMS(QRaGCD(kmgtXNkItEn696vuqSj3EvmcHZcZVolpe3hpIDcnydfZCiq(ZsifXJVncdisVRNbSbXWPkPDspQGeQQqOaSeHwgv(EVJHfzrPgxCp7ayWwzZQEQrDQgUCfsqPx1sU1EHOnlljEMDVhFRm0wFhBRksmun3TOXd06XNjs9ANBk4nyILLavL)p6uPz1irQBpwBTPlt9grlgfQFDyIOkc7ChcJ7AQKSjHhkYN24WcABErLtyq1MEwptrdoslvIayZKB6hznPrEjfVCPWLpAR9IoGHwoOTRovNARa)IdeA3NjAHImjtRx1oxwVPypYXZ3HHjMcSv5ABk1qJ6CEGl320YaCbH54cMTS1gSI(Sv(gLr0MnbyqtawqP3abx84ZoqeShjYGCUi)oWcmd3xzlbvKIywhzByiNNObDGoUovWjxkpKacWDg2CCtEKGLVhWfI(fmQrRW(tSbwWCJkHb52iHCNG2yDQOrb)MsX9Xw8mMUYgX85l7EA3GO2MocepvfFfyvv6YSD8DnC8XGYjxuca0qqEi8Qq8hcOxUH5Uo6wWKA6ErPfEQSEEae0(S4POFwIzVupq1(Fub948LkXpuAycOm4AubISvLHtiVwOAdxEogqFdIWavyfOqP6yjqCwmGBOVy01zLbwUn4UHJNRNd4Wcx4Mmy0EckfjgfLuKJBJhxzQSP1ad9orGR3M41fpb3gkIQGJ4Ik51A9oTrl7B))k8BGAvvhkDgXJbHZ4A75WSD99TCKZlQ3BMaWMl9Cl0KS3CXD4aJ5BXHF65AwV3QJtPTn(EUFJBHi02TXA)T13vpJy0g)UB8xRwjHDoZG5cov6AZmCymfSVXWJWUOozK8XuPtOIkUgii1u7l2vZcrR(FDXrWWkCrnHrD2E0cBBzlWKeT3Vp5lw)VSjXmMJz9R)x2s6YDD2FYTQ(mi5QvW1nfti6kkjzuSDYTbInfsxK6AKi0R3fYdBLEGDxrjAVF0uMh)9JOUNKiUXxvKitvDtPJu)E40FEqH8uHztDqkMlWipEA1epDtLdGoudBFW(PJJRPHXovouF59AP5QoJXgJfLau9iAagY52mFxgeKOjBtL2n1jR25oQ9GI6StrS2uBmLrZuDAYqRERAnqRW3BBrYWTrVSi)0LThnUT5Vv6R8n94aI0YYZYNPdJSAG06RD7sgPMw0nqI7bgUkWtFtBuFPRLbe1LsRzhcSKO1KgOXvHZMHR2bUvk2a7wLEKoaIAm2B8D3Fv0MgFvRJ()VJcGg6O30phBxBFpFMLb31YMzVjxvxoe4UfzG3pDWHtkYYL726oBWKk0e)9bTIMocF989P)1VFXE822gYabc3lEcMZ(Xf1gCwVI8UFpm0tyNP5XL3dNdUpMbnTyVhYncDr7nF9I4DG8Bd4)DrIrTgBBHsvUDvn6dQO92)b)))FkC6a5j3PCES6z)cmvGl(ViQr1jFZSak1bj0B7qPYsScnnE71fr5pMweerzvjEAcUO)txGjAcd9wyt20Y00QE6dwNgl2XBXHjvfEGihx5rtfBWWAZorHal3UA6OPtIVkkqH1PnUws0RPLUserURcmXdZNvHL5yMiWJGKS8s1seVze3Q5bfsUoWAz0TRYYsQfsUPlddjxT0byS(4P2rrqZZ0gzISR2xGvrJ388TRrowu4hezjs55I48z4jyt5TKUEy0OO)tZkJuGoHzeskke3KW0IOu4bvjHeEewAeYPkWlvFHYKhegrrPY9OW2ZDqn3UmLjCR95fxLJw6Z0n8eJJclIKKBp01i74etYxHte6mZOAsqdxVGi2WAJtg1jYZ)Nu05hATBPdPa4zavmhW5mfpgU6UVP2yUkpof(B8Kkr9kYSVPFhr5WUiAk4Zk0FaVJ8WfHYgIQcmjou9(LxCE7qFpI68RTZ5b)QDT8m9nmSWtDkdC1xq)iv7y(JS9T88C98mDm44s)aFVLB1oL)iOTowqSaEy0aggU437j3H84PWfU6QqZXfEKwSilF9o4(ipUhOcWYWXXZY1ZKl)667sDSI45qy8EauWSCPvdbhF5wIgaFhlaQn42ogg22(YfQsTHTpYXW3ZXaxnlWJwdMH87RVrTpYLX4ywo4qSfgM0ua9tsUF1hXGb339H4gdsUf8XE1322Gz77cUwXvafT77pcMSU(gw2gqelwY1oJP2H8Kt2Moa6cysnHMRs6OSaVvWeMjhKQyy5H7eaMg1ub3JSzw0(csJpDbuneeHTNh4UNPEYQPvoqp5ZSDSm8C8mOO2SCL8Xj4PidWMak0MjwrGjRNhOY9l4gue51xd(FHCrjkq16quQCZmssRacQprMSwvQ2R)mW7DpQ05tYan8fymjmxBlmFwEqWF22MYfd76y0KavFd53gSau2KLFRAFjOZmXwAnbEYJvmQkNlWJM0BfvSgacwnbbhthi6mWdAhgW)ZvR4Peem2giGKqGLdOfgw(o2IdYnrMNDGN5bFh8yac91G1i5(W7iBoWezbIt(UyyH8AnTtGrU9jO1yZ3JdYYga)Sb30GAQRyn28WSC7GmEwalkx10kKHFnKXw6icb5B2abbGd0LmaGT8CTmjviU7bccijmpUn8llFq6cLDD4cqTZESoOYAaQD2reOs7tWA0sxFUVfiq7cI6wIuK6U3StD36EyNm9SBac2EWeY3G5a6BzEmJMSt9bcD36(4OnAXrdQ8nGPHdZ0g1UC)eQ6U19bc8w8mUq3WbFNTbZkw(TKRn7be6U1vcqQxde7aoEChvb619m2pi1UfYYYXee0852UE(EEE3tKvNTUpqWL3ujOHbZLBHwsTTLvwHD)GWrEW8heiW6jaaaXXJPC925Oseu1iyx2vTQyBGa7EGRd9wBa9GKytzoWjaBCpTbM8ayryI2BVrGD36(K5C4TK5CnmXAzXgm0ZBRcNTdv4ObtWlfhqzTqAJZLYHD1JBGaDXvzYKBHhpPCBVEuKPLvmAa9UgwMU(wgGJsgGPdV7NSIThi)dCFo((iu4SfzLUhKDJNzEon1TbycOXGTwdxthzgeVhK6oBDpGGpVL4kWU77zaUmcmI87Tg(oBDVom42YHbKxXJXbho9ymRMCB9rV8C5GxCmxWoJbyM3Al0lWHyWsoNzXmbMtx7nPxSoOxUnHuxtpi4zqhk45iO0HjllW9ez1DR7JLX1PjYYdiHUCqDUl6F)9KLP7w3hlJttBrGMrWtdtmvP4IAWVFGq3TUpwMwcoq7SGzGj4sNHfEYn0GLXQxSaWcyyB6aacZuOn3DtwMUhKkFhRiRoGDbiIilh8muE)0e42uPp41ge2fmsoGzgp290V9UBDFGGnRPYitpqHNdQcgpXY8UNkJ6S19A4UPMBi6phtlWznW2PjOq4(rwDXLUgSpB4cwFXJzNUjRDpiBqw5U(mgOxX0cRrtXcOX7351M4uiSeBOd8GNdX(szdyF8erbPD26EXP2T0Ucyzph02Jjetp7(HtHiVC4iYccheCks7orlCA3dYg4uhG70Ydiaq0hqSkM7JsyONDAXNAcJIRLdeRNfE(7CVMqGBzG6xiMEg4SNBL0ABxH7Cq2CcHMEzmSslnqtl7zaZn1N66AIRJiQcHZKyL93eC3TUx(uElN2bmIngSgmxSC23GSocDhgS(Ayb(CcXE6u7qOh0X66dgqnbeoZGTf8C3dCDO3SdeOxde4iWvXhIAZ2tuM(97tbj3U5W48qdiUiX)4Z3)HRv76L9OLfFgy7XhpAK8HW2982t2JJGWE9XqzaVtT4czsULGLHZCDaRvUGEfxoT7g4gDqB6CG71z8wwQbFZmTDz2qeuM(M(3lN7g5BQpbJAkf3zVUteROeOLzuM2KH6Bia1dXBMNW4u649tvJWJmXvf(vJh)YJV4Xpn45dgn8KGJo(8XxeC2ZhoA4HyRgCXfNF8bV4IHbJhEYWhFrWfV4IZo)4bNqzXtTBHoE0rNP)gtrTrC6Wtp78pj4fJh8KHbdoz45xqnz4OhFgL1YGdoF4GND4zVCuWJF6GZVa)YtXTl1zNEWayCo(0H4JgFb8ANcV(rdhCXloF44GNF2ZFXZP(6QOOz4kxlxfe6zV84rqFgG58n4fJWFjG0Jhp4GtggC2ikNYIzBJ(xUpNieW5VyutyvnrRMJWxF0zNdtn1JON8ItobE3tgc4lbGGp9SNFXXNnASedxHB3E3VDKl9n0j2OOKlLf36eK3zIypSpYg)H(gzPuJtOJx2Gth8SJh9eQFwNsN()k(bW89zF8WZhCYjho4IbbVCW5JO3CeWfogPhba3WaaV2ayKBoRGW00S14HZlYG(0JhdVYNiMX1Xq4r5EAHM3BAzEI8UHqCqLR5yN0f(5aa2oBuJXVAj0evf8wx4mDv6UXThLAv5AuqXttIwhis9ToL3Bnj3BSyquX3lobJJ(mArg9XzpdjnJzw0pnPFs4qqE5a5D7LSg3Bu571QzGgpVAfXA8y5new1EUTRVDB9PQX6UUXPy)wgXTvWN12FfnEF9w9BmPctwP7ITgSRa)vFq1tKgpU3oPR51EaPngK77mtom3Vj4wPV1Uhz2wrMl2iy0fXwXTP051R4QhjO2(bwCtZr3efxLiwUy5ksRRJNj7OA0P9tvTYhV7vOgcscpN)KBhITwqCGzu)Qltl)QBtlFzD55BrRzBv9Et1yGWYw9vXM1X2)aAT6iNwDeCR61n2heho8ObV4evNQoYnKBgKg1q5NKT(UlhKhD3LLlGFCaGe(hqv6X68q1vzxRkGFV0sSeOkrAwg9(ODI(BIkB(y5EA4Mfriy9KxC8jhUbrdPwZudFz7TkqnqO5E8Stk))S1rcNmK7yrQClOdQz51jJUMjODl2I4s5OHNdeaNf6lKyhZaWuRA4q7pejwnEu4IRdxU6kkoNo3mz3KLplWOrUPPnF14baSHB)rC7ub0P055XxDv0w7OxgfUcGVdaO2WTEGpK79JFXY5Gw)05p6Ul)6dZX9bgiI(rD2BdiAZTbJxF1vziUtDOKH9M3g924PlsIIxU7(6X45feUnZEEwCbaMgMQdWmQt9WieWo(T)NE7p7T)TV9xa))F77(bV9)XDx(U)pE7p5DFhyConoppl)UlpgjfBmAyrWiUk5cokggNJsa(2dYskvN)z444BB7khN)FE339TFX7((V93)2FdnA)63(lU7Y3(tHFdJlmAyLOHxRo7AGEAwcmZIZbJQND15G48nG4S8uuJUV68DSe4R3()lmi)839dHb6N8UFimP(UV779UVd8SFZB)j3RPwEgW)s)eNBcSO6OHL3bHgyE(YF5QRGp3n9r0TdYNcodeCk4V5PuPQFR6OBJ4K5E4AbsZJ)ZV9N82F1B)5Wpbufmh(RGr5gqm4Ul)hY6gWjMCAZ0qvMMOmaKMBAbUhrxvw7cqpnCE80GJqJgr54RRpp4WE0zZEmce1)OTl8TgRwOJqDcitZ4vXavxFWXrZDmBgcr53(VfOy)oGT5392Vayv(ziJZ7(lGb5jjHXegWSBmGsg4fRMNhol60SSurt0h8CKyQTTAG()c4c)PcgL3(3ad3Vf(jYMa(CbEtcQ5294CkQQ6K4xdMtpiB5e9HwhH0TCD9QgLFfkR9U)LWO9lE33dgHjjzzl3fd4iHu8tfwRViB90f6J6ojVcJ7lgG)nV77b8jFbc6V7)tKBbNk7eYFzyEECwEWyYk(twJQIfEZQOgmBM9EsnyVpudLOlZ11XWBhZdufr2kWa2h9EnJuYSUBWYEs4Rd3TU0ZxCBwcUxW(4SeqUntKZ)kcGTPrVcRw7NWQPrTUvCdsSZU1Cp7wTrsh4FvAKHo9V5D)ae9(U)sTIY)veh63biW)A8ZF9PHRHiC6Eyew7VkkjikjAjDcJml61ybut(gq5rtzjWZWuiTDs0KO0IvRtVUm6bdaJ5HRbLM7qey8cWzG0aHYIta7OVsSDu1ZiURZ9zg1Ju9EmPuc3MmlxpXy)5xWSCmDSypIzJ)Nb8VI)cEIj9JpV8UlFCwE(6vLrZU7sSuNtKxZU48bOmI8gZ19UnEj4P6DURhZz39(zHxdoHNx(1kU7YNKcDpooNl2ZCI2loqQvdGPTHs50pcKX(PW))ZLY3)839xbwpXN8Rq(oa9HkefUXi4ggHzJuMQBLuSPLRJNuy4Fhqe(xJYVOtfcfEiza6Lbzdv9aAPJ6bp9KgmIl1N9FhCw4xdq0VauiliD1APJHJy2OeeT9XJHKEg6tdJtV7YlOImVnmyPK9WDgKCs8Fbf7WwciOFd1p)A0dmkGQpss4W6zGAptphGOy26COlqqnzSuIlCUXUbHNV42cT7s1bcLCHPRNPPubY)nae(9qN8DrfRKvUVaWqcs6fnjPyfpr9JMh3XZ33RcV(Djp4(jW05xO8Bu2N)8399rFhB3NoC8AQI6tEfS5P0c9xJWbyrKqoV938U)k0sC7(W2bVBRO(qZ86Iv8Mu6W2XY30E3chFmeHzuYDxMDfi7DDSQqxLOpBA3kmYsZj7674izN(3Jw(qWs7KWVe9K8D)LKM4lAltiJgWRAYAPSqVzpjqHcn7FxPU9w9OjtCiUB5x1JmrvJm(T)hboIVpOAdiUW)Jm9s)Dbso5R7B))g69Fdif)lGN8f4B1Eem5245zV4oEuncmgtocy7)9yFa91Vf(nmwpaEaQQ4xcDjo0FpcD8d3a0zmFFQEqhzRLnWkrWx5rXpq6x(VJcg43d)1VMyWe(z83upuH2yfUNhfdNTzfwXG7Qyu)vV77aHZ8trwDjo)x3Up4wEgcMkBRAqNNCE)xdtPVp5o4xiGaIr97IIoae(fB2FGWJPjj8yBxV)C14raM(HV9NlDY8Nl8NskpVTzhVEpXuZoiqQ39DrmgHLWiD(bD1h(cCVtnXohPy3)vOL)gekW5fmp)B3KRaRVzQ9vYemBv7)redWpJOo)ukKrsTc0tFHKV7Nc)nOsyd4YLHvxa1XvIig(MCTogzGB)oP27F97(xaG4Mcgo(EUgKuRDLKbZWLv510xiO8Oegmp)EKwySJ)zV93rb6(liETVxhkcT9X6SLIz2O(0N)HB6Zz10q4zPLNfAce6jeHKau7VZMIxMmdSq7PUQsiG5iraGwr8Ku1B3AfpjC2T3D5ldVDAoevg64WPRlIfkDPMtDV2zlS61e8ZNepDb0(zryt(YFCE5T5r5fI0taU5NwPp01rK7bTqbwoi(QPlkE9tGjiigGmIv2Tr8NmteppSOacyqk2IfLU4EOHRdYYNld8)IOLRscZXjYhhLJNpeiAR2dHqUb7MLk3)aPdMNJGqRKtSS5gsx6hF96KRbZe0bN3m8qaTlQGVjtCN7OqtOPjbvyaEQTGhWnGpUXumhTC6CWSzzBUDQPtYKqQT4XSXvLI7DhLRo4ryKadEqEuAkUBzah9clIYJIba0(5F0EnkI9F7NozTOM6Vc6R3GxMYr52p8BTAonMA3RmTTnf44HOlSac8(psrYw2Cm0xRrwyHTk8Ng4IUjm)nldjUSVooy3MTgW(49r9(nMrtWtGzYdBCqusBUGRscP4dswxIKf5DH7ErtWa2Njp5tOU1uJFWQZtk5bwu5(8ECi5OBZdV(AKP8Iq8eYb9vpu4qInUPkC9ACNGH78dtNkhEWJjSDpaqetLrxTobJ1ilFPu6X0qOZqFNWydQFTC1Xzyz6y2xqmXuKfJJYxbXhD3LhpllrkUJTUXLtJTHNN0vcaS9mTm6ZrTd)wH5RxN(nbzU4eqSv4YwPsFIjDZAwDvEHhzamw9WKmC39amOybQ1I6vmvVdXdi6IS7U8BSkpB63OkEjHNC6lokBdWzmB5izAXbV2939inuebz86LWKb3184ONUbjUsUgCyYwtIbxX97bx9eq1GyM8I8I40iuRhEMzjDAg7aAe0sXgU(ovilBlREWvhppnkBnDEnNDdDg9iqpatKRqRN(cQIGENVcGE9vuLLlO7NvFe887Jvn9BTohzwFmiNNG7t0ADVNFJlRkqTQTTQ795(U(9y88GCCb6QXjDbiMfjOVI234EOcKGn4vPlWZ1IB1JOq00S8qHUwCqOKSl5pPMt9VD9(37dF)ZR1)(gANl4229PIJ078GH4QrJ65oiltY8lAm17o1jUCT0ferMrpSMtJiTX40iSCrrAyEuv4CIRxf3kDC4JKGUj(jEp02WuqRwCKu9Zf3exqQO)g5rLG9sHwclxhdA)opY1RsjHYo5NFbOK2YVVCc1iW0OWCYDd6uQSHwcxFnzaCdtRVg8uXYV3SoLwIlBhjhiolUGzKsqgBpTSgg1Pe(1T040dYAqsYdUiRmAznzHtdl0bIiS4OV2ab7yoY1fcSvAXzg9zY55XRqgOHlXvWfMfIt8EWXa0ZQoCh4ST6cI8SclFD8SGja2EX65Gr9WPxFZcWAPYLeVAM1vXDb4cFohcuz3GkEovMofxzfG15XjH3aq53iml6Bi93KXXTUeogwvUwvzxbR8mFEpj67JdVoSyX3uIPfPJkAwnogYWLNDndxgoFGmCjBpna10mWSuYUoCdhREMaNI3GRGbaGmEfOJqK)3rIws9CL1DhpFVpmw3rTCRlI2WaVxLwcta5PjeoGwIEuseLKL)1YHFwOjgRfOjrZPUVY8oMwVp42x8QCrhCUt1)Cthm509O)hVbGNeJB2Ea(pjlJeGfWVO906sAutyGRyuDSXDzDpkEcldNMCBXsKyJNJUiF0bk8VPypv6xxTGT7he1clHyNUxQfsIrLcHZbx8XZxaLEaFtDOjGblR66eD7b3cQYLk1pmgmyeIa6JxKjzoarsbUTMsaFh(FNu00s)IVDD8Q3he863arSFdv(ZSn9PlRDGzSAO4A0eol96ttWG1ZxNFBnE8NNJxegA0KNqHGFnfcCh7Vkgb36wNC(GGUWIA4EXgcb3kUNQOJacnxyLZfMCpnxiPP3OpnuHtr9ELz6Qo6w8qIPYuH4wJZVMiUoT6GPpFBEp6BFC(A07fsvY0WC8S8LCnIXXt4brfiyu3dYAjT3Z1OhvGNVE5KeYJOZxp5wPllmiiqzpZQcZ0XZu3ZM4kc0NUpuAhpTHrhtxobLtlwjdoGAFZBsxW4GLH1hexiXtpKBA7bz11RRnMfpwL)aUo8ECWB0TlxhHSGViLUU8fUqk5WP238U2fCHegxnlUNHDpC4NUUmKG9tdNVmC5YSYf6bGAEZBfxC3ZR5IW1xOVvUuvqouqi5HtlfbTPxFcvPS4unbSD51zKm7bfjsAfHxwfHjvagM5lLKBQ9IrWTA1xr9O6121OVWrgEBKAXLYEDOiNsKxg(sgjTqmZ1Uwp7JhwW9ObdVz8JWa1i4hyRMNek7FQ5IbOkabxdR6zkYTp0)ZOurrMO0rGmuHCm8f2tyvvsKhUNsvKxmn095u2rRZJP0iCoOT7kr5evLeBHBymDDfryiVp8yiDvgHlTUTwBbMfKEudncvhVme1vmCofEgOUwNjeUVqBuvTfz6BQdWbdhTVCEDsu4v1SqniDAmfKgAYfdXrf8GJf3wENCwjl77zPJwdCWe0n1No1jyo)XnXr9zcOP30wuyKmwTIqapae1gd5(94Y3PqyGs5aW51Y4ROSTRxLABHygRsqM7R1QcVGrFCsVy5eWF7IRxNGCRsDfQU3qXjvjfJB(7gvObVpxwNJAEEAgQqsLZrMcSvYW(MalAfuB2NXMNdX4eLqR8)JZdNi6xUHNTyLXzm)6CoSpaCo6mHykOO6klc8FYx7IgZYM3xqoNE7xBwiLL6K4ILHPQLLgy7e9mRgSZRLizx7EWkVmg1dmjmNYcUiAhvEKDTfQn1vqKLNTHHDvApWZYOD39pnBjGZtP8QhlOPPQ12K5k0PzwLCoa8nQRsOpvA0QLi03GB5JKem)z61SxSYKmZAoHBxvRq4neuFU(Cm4CpezwXuIEoSOiI2wmcB6atPe7xfdUTLj)d1eGlxumMUAHSXdUdf(33e31I9eFs8YOhCXcicFQEKWanfjXx0yrV7wZKIvTCoXbpW6b9a(wjy8F(AuV8HrtdVvRL0uSxkzME1yonRY8nUaA9g)MOiTusswmjj1Vs3iZrbZm8o2UVafgVk(AkjCIdPVBI01)farwsn7wg1az7Q8fB2lhZJZcNVor4O2tIsJkcXvmRIL0t0)v1PehxIFLLdWnX(sZhe208WLc3eEnWwIobQCz2YuuYcmlZAWVJ5hg9bMEsNqSQeyHGtuojGNkBS(wTbm5)coM)PHZjT8hlfOCarFroZywv2v9841DX0QVLZaVdhPY1ffOsNlKSk1UyA5lXp1ST67X1(573RxiVmoDwXu05vW4DzZvJH7j8brxGuw(UwUFf4fOvT4KXQM6dUgnDLtHOmTgh4V9z9OW)L6fAis6j4tJKYVIMl6FTTwlqpH5hAFp0frf292(Fq6EuFLixCm7glgM3hUS0BAAknORlPkCiCyFixiazCC2w1tCS1xfJG2UlNoSnQLyaEpCrdMphVoqXn9gU9NsVww0gJKTw0)6qD5CpTDfoEWnW7D9EYNKPkDMH5IRbfDb3ieY01SLTTVT2TeoOWZWTh31gFlUl9Ie7JPC0qWK8VuiKjAUyaCRgatDoD5(U4T0wpb6IlM0kv3p(6W8z3kZ5TO5IbqB41gpSovdGNVVLLzFdambIJMdoVnlcxv4Xk5azZfdGwmMBAXQJIaoQEqruNJuaycGM0YJLLG(iz7f7XcTKmqz0zBaFdZ(SKno(6VgEETE3L4DAvwbsQhKxlGuHUcDjGbijFJQG4augVhK0tIUk)l)XF5pkEoojEAwA88j5k2ipL1sDHHHoeQxhl88hJ740N5Y1LaNZpE915RNlX(uZeDC12OXIRDCJ4W6J8EAeOLBwiwSyxqx1VvmNsslVMWRLEPofSVo9kC9My8wmUaxpJfGhUH53uJ7xc98QnbKzv2KrkRHFFjun(l)r3eLF9BIwpxkelRPaz7fJGwaMB4Qx7nGPf0w0NF5zjXHPLs2ZNc2Xcr)wKLpieQPVCsOfHbx38Qpjy8EnexGlgJe8)ZJsafQPYHWbp7zeEQuvWzCdFNQGJWdruZ(clfVz5wfEn4MsuSCv)fnu01(10)0q2YOx9p5l)YF80fLaNFkHIEgi(wrIL6FCQeE9T0bE9budQUGYaMutTcohdgEVG1Zmyw81Dzaq2yr3xj5INVrAvdoWN6rg4l)pmbKaaupEt3bK3WfP5qSmFD8c1aR1d1Ugq2zIHZQMUol7pC668WdGxAe0c12oEg8VcK5QQ5mUHJ)xjYCvvDgN7xz0XI5BW97BzOUszrlxysBz(Azg0nW7PuXauZUSp3UbBB)(vaQRXT1GKV9I8W0ASTYbWRUIBwdbV92SzbTiAyPdvxWtkxuzx2LR9TJBthaB9matxGxW9OQiIo8gQSzRYtSOqyyvvCghVGy)GrNfDGyiy118v38gRVkQEOqiqmBcZxol)l)TvyjMTCoywnaqCYnuEB3xuotxuS6QO4RukWFz48kPbMOUQy6YodpNvTQcd3G37iqlnsKgnD460RJsurItTxmcvMPD91QOiyWX9EWk9A0DVRkJKoc46aMeeEz7YR5JNUgvj1K9vvvNhIB4Er5Ph)z4PbZ6Lvkzf72hMBLB2wv5jw4kspKz0V3LGeW1fRsOntunVyKK4k7ZmpN6wGy(9vdlPzldtIqD3RNqcblJRrH9LmP1eLzMn9IXS36VzwOI((AuXXVD61YDIiMilf(VswMzORIxmp69naplArY1zRUssIZwTkNoHpK1WRyJ0Z8mQztGX(7SrUnmR5vxoUkmnFmFj9ma)5RVbf0KtGZqYqzKsFk1EXiuzNgiY1CH3N1x6Caf2LGKMCeeEmvmvVMdYyeQktm8oyN1WYCpkS)Y)IY3iLbEkEpDKuupmhzHuZQktmUPzdvrM95k2ZYUolDs(A4pFnwLbdYdFWZcRncm55ex1ua3lG1gH(cZzaDqovc21KOjsRA1iqX5qxTmQl(KVvgwTnj1UCukL3Lf56lxw5zmL4IPfxy4IwxiW3SiUaVVUhJxngWRhL8QXJh8j4vzQ6A0pvCzixwR7wHhSkB0xvDWWtocp8vWf0lsCs5qx)mZcV9vJbgw5fnEqkEXFeoNULSNotDYWS5fcS6AvvDLilV6rexXi4LQdElqRoFVWdnR40Oc8cObpRBwVmvCcmHhno6dDMzrxb8GXVo6b4TOaDrOlFG4kCq9TYRPj8UwTK2K8n)A8Yic9Zumj1NWyT7EckXduoXFPhkXbot7btCl(ihUwVIEaRFjXQo5IMOWSZAJQA9r9P5Lx1LXeEhdItGLrbY79o115dEzlfRpBKK3N5fIRgFX9JDx3Z5nV7UUkorEl4ooUmAjo7iWfVRGZUrCP)0fwhFb55Tu3O9DrjrwN8SBMnvuwWnPIL1UzLsYOB)N4uIJnqF2rHNjpHjj0DSH(ugAE0skJ0fbmmvOtOBSMPxhSqiwk2CrvVU68EHoiQe0O2dJcWH3AAq0RPRGC5L8lmfKpGifQJ7QzR6UNwUkzDHGzuDWKvgkeufxAiY79zyEVcVCMND4rKADBrLlrh3K6VJoQSADGmcK5lK3qo0Gwqhbi453wK4Qq2d9BcyRcV6Q4ptCYgMVw0MrMMCdfoNEcEnJy45Yy45Hn3NUQmSLk6OtiPQ2zJNwUlJL9K4yCeltS3BW2QjuBAIxGZDb1W3YBc1uTYzzIP0f3f)UDd1y78bhl2aQ5cO289cz7xb2uvW6txYvcWUbu7ZBd1ECoa3U2owyd92cuJvKPfFtO2su6CwVpqTztCTLRH1wW10f5EdoexdWsQdEtk5t1ska1wBc1q78T3exlVmSYbBwnp1Y0xIoOaJu(hNlM2)Jn8)hBAF3LMMpYY8r2SpFW0Y4xd6mel07JU7sMLf7HwEchi6ObpjQ8XceeOZ840RY(6Fegq260zFZQ(ajpipyhT)uuVXy5LQ2zPdXf2heJZPL78ZV7YP5Qv9HwuaPskChdkdMbD4L(kQ4m1REaGLFiDQv2XykVR2bnzflccVcvKrQVediOWiz9mKCZ7S1qpNsaeb6NhHM6WtXhS3gGD2GKKdYkkIkoeuC(quITZjorsouOI6iOlkwendrEamiuMs3V7eqE3L)jW0kFnDabEF7mznPE3L3G17bwSkcwUhIN5vB0zw(F(Fc(pyfIG95)iGAk7pakW)HUaGA3mMNGssyHhNefMUELMq(qbJFhTbXthsLoMKCFDeW6LaotL8i6ZM0pp(nza30SyGcbwC)YFuKy9wOsChNqFoTM(ZuH(C0x(JNHo1ZAZJB6(iUvpaQzNTzpb0dru8ZYcNNaw0k3oG1wwG59i7(WG2D2M9eWGroDEKemE2x(ltJNVlexBoFd)hzB0d850zB2t47SCX2W(z5XF2x71XV56TdBTLamCEKT9NlpzGF(jd(KHNhCYWbF8qQlWZzvuVamzr5P7hi0543wOXG9ilVp)S0hVGo41MhDA2SiSetk)6FKWgwhVUeCp9tU4Ph)4dFXONm8SrbJVyW5xqWsrujQ0R4r7qxGqtr41rkp3WJ(X0a8S)S57SD1D1FlAea1EyL9b(uR1VU1rJAa6im9oxb(7PhUWBPZbs0jU55HRwGBue4DyIoH0RaArfx4GL3UkQ23kdKs4LhARQvVtDQ8GKSEFRHXWKBWBj0y84zfvZ1Q94zvP80eggD6lTnOVH(HIRqWs8gax(OUyd0F7XZWxwKIaJoP0dXsQbEPxE25NCisIVyiD(vFEnY9QWBtYcNXEKcliFG5JKGL8ZwpcZQPjBZbY0xpqp(Pdo5KHahvWPND4qXOqNzx1Be7r28hzA3xJSA3iZhXn2kVUPDNV(FKx))nIx)q0i7OOjyECPS)CrCEkwZCtJj)QAW3lQTsEBQoWo6UDMeNoF9)itYFyZK42jv)RaLJEBoqmV(0Z53QrwShXDFFDr3YOJEJ3VB1wSnBhBVD98I8OzFTSxhk8dDNei6iPR5qHBlX92zsQJZxFL257EhU22rmnEe35dGpBnHKEbJ22Ny2pYI)3)GrBfMyMX)FbGrBfXch2)7DWOTMbd3hzyTvZhwED86M)rZh)HT5dR2kOnWck9V35vTBQzhuI5IsU7mUyBwNTzFZ8r6CSkFonmjdpZa2dDT2MThpq7Y2DhZ2QZx)pkp9h0Yt22Ds1)W7oMnFZbYOp3XWRasdOrCQrmo6dNT1M5M23Z)Hmp1vmMfDOw2vd3RCuJjJhp8k7Qd(koj1(DpOVxEFQw(z1QvgepdJ5cxVNPzHtx0EjXJsa2WiX1yuGErMPUGE)GuCrKNOV3IwGhga4oEp4QSC8s)iVu2g5Amix0nACDnQTo6Y1hP54td0I4sXTQgTSQxfNxq3QfJfxLjI7GKQUHKTYXZ4Qz17SdAVM840idxlsfQaVkIsVkEUETBwMnlJwxJI1tccllP6wosSmpz5XGmtzyY40Wv0QdtVd9kzbiy3Xf)dtEX)GxIeeudmc06HQ6K4Itel3mE1OGpJWCXGEQvrP0dfCm0YBbGxebEnbnbrACAw(sX9EZTurEG3Jqh9aUNfwS(w4DoniAylw3RX38QJCaPfF8S92333K5RUCRx8QJ8nWcUZXWYIZ4YRVBoTE7zjzYbW8HGegZYHBYDXnXjoy2CdlxqSX10eR0rCn240ybraz8k6SUYqTYuIfa8EHW3kUBsfgBsD047ff69dHF0dCSnWJlgFxpBFdpp1LT(NHx0QUCtGk44JLqS4UD0IibECtBlClbG77kxB7ksGnqACS4Chhtxhhd3ojb0nffRbc2ScbB9hyiyxl80NYHzd8D(UIRhBjcg478C4yLc5Y8m8QqWU4giMBjUWPT82abB5JOylpx77pcglLLuPzFycTwR9sRPTuS6S4svJ7PO66(QxskBRSvQxCr66rsRs78bhFyd9GKAsqZzF6aPkMAwqEwsuH6sFQspUwlEHOWjefsH(kyAmP9F8HKoxHHRHHOJOhNodSfpBnEAi9CQnQ2EgOdNUOXOp9SOBLRDTALUpBY3kAAjE41fgNIfyjR2cCxnW1F5XRNCbobXodPpBcuds0WbUHzXt)kaD0zNmIASC00Kw5fvOaAE1)Z)
```

