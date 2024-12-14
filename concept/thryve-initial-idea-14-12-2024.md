# Initial idea

## 14-12-2024

### General premises

Dalsi krok dopredu od EV.

"Boost your fitness and your pharmacy will thryve."

- mobile only (Android + iOS), cize blizsi sirsej populacii
- hra, ktora bude zahrnat aj nejaky iny gameplay loop ako cire nakupovanie hernych predmetov za zarobene peniaze cvicenim
- mala by vytvorit cyklus "grindovania", tak ako v RPGckach; hrac musi mat pocit ze na tom zalezi, a do toho bude zakompovany zakladny kamen, co bude jeho fyzicka aktivita
- predmety ktore nakupi sa budu dat pouzivat, a sposob vyuztia by mal hraca posuvat vyssie v leveli, k nejakym milestonom = malo by ho to tahat viac sportovat

### Minimal viable product
Spravit jednoduchu hru, na zaciatok, kde si user bude kupovat truhlicky so semienkami liecivych rastlin. Bude ich nasledne sadit do svojej zarhadky. Semienka bude kupovat za mince,ktore si zarobi aktivitou na Strave. Cim viac bude sportovat tym sa bude posuvat aj jeho research tree a bude moct v truhlicakch najst viac druhov semienok. Rastlinka ked narastie (kazda bude mat nejaky polcas, kedy sa bude dat zozbierat) sa bude dat predat - najprv ako susena v lekarni, ktoru ako herna postava bude hrac tiez vlastnit. Peniazky ktore utrzi bude vediet minut na vybavenie zahradky a lekarne. Na zaciatok to budu len nejake dekorativne veci.

Na zaciatok to bude bez avatara. Sadenie by malo prebiehat automaticky a v nejakom 2D top-down gride sa rastlinka zasadi automaticky na svoje miesto. Bude mat na zaciatok 3 staty, ako bude rast.

Mozme spravit aj to, ze za s-coins sa budu nakupovat aj ine veci do zahradky (vsetko co suvisi s pestovanim).

### What is the finishline/endgame, user can aspire to?

Zveladovanie lekarne a zahradky, za trzby z urody. User mozno zo zaciatku neriesi kde to skonci. Ale aj trochu ano.

Seasons:
Cely rok budujeme zahradu, lekaren, predavame, zveladujeme lekaren. Postup by bol spraveny tak, ze kupovat veci nebude take lahke. Mozno tym znizime engage usra - ale pocita sa s tym ze samotna aktivita v Strave je hlavnym bodom zaujumu. Nasa hra ma byt len ako **companion game**. To, ze rastliny budu rast pomaly, profit nebude prichadzat tak rychlo, snad neprideme o usrov. Aj fitness nepride zo dna na den. Aj nasa hra by mala tak fungovat.

Na konci season by mal mat user decentnu zahradu s liecivym rastlinkami, lekaren vynovenu, s roznymi pristrojmi, s obstojnym profitom z predaja na ucte. To sa sfoti a prepocita sa "thryve score". Lekaren sa ulozi do "siene slavy". User si ju bude vediet pozriet spatne, v read mode a spomenut si na svoj uspech. V momente vsak nastane wipe, a bude musiet zacat s novou zahradou. Tento wipe by sa mohol diat v zime.

### Currencies 

Hra bude zahrnat 2 rozne menove systemy, pricom budu spolupracovat.
Zaklad je, aby kazdy uzivatel musel aspon troska cvicit. Ked nebude, ta hra bude prenho onicom.

1. s-coins
2. euro

1. s-coins bude mena, ktora bude predstavovat core value hry. Bude sa zarabat fyzickou aktivitou nahranou na Stravu. Mal by som to odstupnovat po 20 minut/40 minut/hodina. Tieto tri tiery poksytnu rozne mnoztsvo s-coinov. Za kazde mnozstvo - uz aj za 20 minut. Sa budu dat kupit nejake semienka (truhlicka), bude ale obsahovat menej semiacok.

S-coins mozme postupne pretavit aj do mikrotransakcii, ktore by mohli eventualne vyrabat nejake revenue. Ak by ale uzivatel necvicil, bude musiet platit, lebo hra bude fungovat tak, ze ak s-coins uzivatel nema, nevypestuje nic. Cize mohlo by to sluzit mozno, ako dokupenie zopar s-coinov, ked sa user chce boostnut a podobne. Ked zakomponujeme multiplayer element, musime tento koncept este premysliet, aby neboli diskriminovani ti ktori skutocne cvicia.

Semienka sa, este raz, NEMOZU dat kupit inak.

2. eura - po vypestovani rastlinky, ta sa spracuje bud na suseny (sypany) caj, alebo v buducnosti na ine liekove formy a tie bude hrac predavat vo svojej malej lekarni. Tym ze mu tam budu chodit ludia a kupovat produkty zarobi eura. Bude to mena, ktora bude sluzit na nakup vybavy do zahrady a lekarne. Vybava bude mat hlavne utilitny vyznam. V zahrade bude rozsirovat mnozstvo rastlin ktore sa daju z daneho druhu vypestovat, znizovat cas vypestovania (sklenik), nejake hnojenie. V lekarni bude sluzit na nakupenie vybavu na prirpavu liekovych foriem - susicka, sackovac na sackovane caje, tabletkovac, mlyncek, laboratorium na pripravu extraktov, sirupov a pod.

Eura by sa mohli dat minut aj na dekoracne ucely. Bud zahrady, lekarne, alebo avatara ktory bude uzivatel ovladat.

Poznamky:
Cize s-coins budu nepriamo produkovat eura, kedze ak nebudu rastliny nebudu ani eura. Este vysi vo vzduchu research a postup po roznych rastlinkach. Aj to ze ake liekove formy mozme z danej rastlinky vyrabat bude asi zavisiet ako dlho s rastlinkou uzivatel pracoval a kolko jej predal. Kazda jedna by mala mat osobitny research postup. Zakompovanie eur do researchu treba este premysliet.

### Auth

1. vrstva bude login k nam do appky, bud cez:
- username/heslo/**krajina** (pre leaderboard zoradovacky)
- cez Google ucet
- cez Apple ucet

Dalo by sa to spravit len cez Stravu, ale takto sa staneme velmi zavislmi na ich platforme. Takto troska spomalime onboarding proces, ale v buducnosti mozme pridat ine sportove krmitka - Google Fit napr., Garmin Connect a pod.

2. po vytvoreni uctu bude user promptnuty pripojit Stravu (zaciatok); tokeny zo Stravy si ulozime do DB pod hlavny ucet, ktory uz bude z prveho stepu

V mobile asi auth. bude fungovat inak. Ked sa user uz prihlasi, asi ho tak lahko neodhlasime. Resp. jedine ked odinstaluje appku alebo sam sa bude chciet odhlasit. Jedine co budeme musiet handlovat, je Strava session, ktora bude expirovat.

### Offline vs. online state

Bude to inak ako ked som robil webove aplikacie. Na zaciatok nechceme implementovat multiplayer, no chceme aby user, ked sa logne inde, mal ulozeny postup v hre. Potrebujeme niekde ukladat aj login informacie. Chceme vsak, aby appka fungovala aj inde - aby si hrac vedel pozriet svoju zahradku a ak ma menu (s-coins ci eura, to je jedno), vedel nakupovat veci. Rastlinky by mali rast aj v offline a mali by sa dat zbierat a posielat do lekarne. 

VYZVA:
Synchronizacia medzi offline postupom a online ulozenym postupom.

1. User samozrejme nevie dostat s-coins z aktivity ked sa nepripoji na net - aktivity musime nejak nenarocne ukladat aj online (uvodny koncept je ze len cas aktivity, trvanie teda) aj offline
2. Postup v hre nejak ukladat aj online treba. Treba mysliet aj na casy ked user dlho bude offline - napoji sa zrazu, bude mat 10 aktivit, v zahradke nic, lebo vsetko uz odpredal. Postupil v hre a tento postup bude treba aj ulozit inde.

Specialne casy:
- user sa logne inde a na inom zariadeni uz spravil offline postup, ktory nebol zosynchronizovany - moze vzniknut konflikt

Vynutit fungovanie len online???? Mozno. Tym, ze sme zavisli od Stravy, je to mozno legitimne. Ludia su teraz aj tak furt pripojeni na net.

### Avatar - yes or no

PROS:
Avatar uzivatelovi asi dava pocit, ze tam ma postavu do ktorej sa dokaze "prevtelit", dokaze si ju customizovat, spravit svoju. 

Ak by sme raz zaviedli multiplayer - avatary by boli prijemne spestrenie. Kedze by sme mali in-game postavy, ktore by predstavovali nasich hracov. Neboli by to len taki neviditelni administratori.

Je to asi fajn aj z toho pohladu, ze clovek vidi ze niekto vykonava tu pracu v zahrade a lekarni. Ze nie je to len samo objavovanie sa cinnosti a len tukanie prstov, ale ze tam niekto beha a to robi.

CONS:
Technicky narocnejsie, hlavne pri mobilnej hre ako bdue postavicka ovladana? Asi joystick na display nechceme. Kedze je to strategicka, budovatelska mini strategia - avatar by mohol len behat podla toho co sa user rozhodne robit. Mohol by mat nejake funny idle animacie, ze si sadne oddychne, pozera na zapad Slnka a tak.

Poznamky:
Mohol by to byt lekarnik v bielom, no v bezeckych botaskach, v turistickych botach, bajk by bol oprety o plot zahradky :) Podla toho aku aktivitu by uzivatel najcastejsie robil.