# Back to card game idea

## 15-12-2024

### What is too much engagement for athletes using our app
Nasa appka ma byt companion app. Farming hry, alebo Pokemon TCG, ktory som skusal nedavno, dava hracovi do ruk nejaky core gameplay loop, na ktory sa ma naviazat. My mame ale (mozno) tu vyhodu, ze core "activity" by mala byt realna fyzicka aktivita. Chceme ju vylepsit, posilnit, nejakou komplementarnou hrou. Cize to ze sportovec ide behat, bajkovat, na turu, cvicit je ten hlavny bod - ten gameplay loop.

Nemusime sa teda snazit vymyslat hory doly aktivity. Nerad by som aj videl aplikaciu presytenu cervenymi bodkami a pop-upmi ze rob toto user, rob hento. Ma to byt kludna aplikacia. Ma dat akurat dostatok aktivit, aby tam clovek prisiel po tom co si zasportuje a potesil sa, ze okrem endorfinov, lepsej kondicie a zdravotneho stavu, dostane este nieco.

Je teda farming hra dobry napad?

Z tohoto pohladu je to mozno overhead. A zbierat karticky je mozno prijemnejsie, nie take narocne. Musime brat na zretel cielovu skupinu - sportovcov, ktori nie vsetci su hraci hier. Zlozitejsie herne mechanizmy (vyskumy, rozne dependency na postup a podobne) by mozno bolo pre nich moc a nepouzivali by to.

### Enhanced card collecting loop
Cize ak by sme sa vratili k core z Endrance Vault. EV je dobry koncept ale chyba mu viac farieb, designu, zaujimavejsi gameplay loop, krajsie karticky, nejake meta kolekcie (world tour timy), achievementy (!).

Ako to vylepsit? Mohli by sme mat viacero mechanizmov ako ziskat balicek. Nie len aktivitou - ale to by stale bolo hlavne.

1. ziskavam balicky cvicenim

2. ziskavam balicky achievementmy
  - otvoril si jeden balicek, 5, 10, 20
  - otvoril si 3 preteky
  - otvoril si cyklistov z 3 roznych timov
  - z prvej desiatky
Achievemnty by davali nejaky bonus, za ktory by si clovek vedel znovu otvorit balik.

3. ziskavam konkretne karty "reroll-om" cize ak mam viac kopii viacerych kariet, viem vziat 3 a za vymenu dostanem jednu random s vyssou raritou

4. viem si zvolit KONKRETNU common kartu aku chcem pustenim 6 inych kariet

X. kazda karta by mala viacero "flairov" - obycajne, bronze, silver, gold, platinum
Ziskavali by sa kombinaciou 3 kariet nizsej rarity.
V balickoch stale budu len obyc karty, ale mozme pridat nejaky speci balik/eventy.

### Tech stack?
Tu uz Godot nie je taky jasny. Na fyzike tu az tak nezalezi. Takze React Native.

Co moze byt ale tazke:
- vytvorit pekny leskly 3D model baliku kariet
- vytvorit peknu obrubu, lesknucu sa vyssich flairov kariet (silver, gold, platinum obruba)
- animacie (vo videach spominaju problem s rozlicnymi platformami)

### The theme
Tema cestnej cyklistiky je fajn, ale nie znama vseobecnemu publiku, ktore je na Strave. Atleti ktori robia ine sporty - hlavne zeny, v tomto nebudu vidiet temu, ktora im inklinuje.

Napady na ine tematiky pre karty:
1. prirode a kulturne pamiatky sveta - je to troska nesportova tema, ale znama sirokemu publiku, len ci by bola az tak engaging a nie je prilis nudne. Vela hier a appiek pracuje s touto temou.
2. sportove eventy z roznych sportov - toto je akoby sub-skupina prveho napadu, pre sportovcov. Mozme zahrnut maratony, ultra behy, cyklisticke eventy na ceste alebo na horach. Budeme cestovat po svete kartickami, ale na udalosti, ktore by mohli byt velkej skupine usrov inklinujuce.