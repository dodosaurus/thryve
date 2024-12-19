# If it was better EV, would it be like?

## 19-12-2024

Ak by nasa appka mala byt len lepsi Endurance Vault, ktore veci by mali byt lepsie a ine?

1. mobile friendly - mozno aj mobile only, ale najdu sa ludia ktori by to mozno chceli pouzivat ako web appku, napr. ja :) je to ale velka vec, kedze pouzivatelia Stravy su vacsinou len mobile usri = companion app musi byt hlavne ako mobile app, bez debaty.
2. krajsie karty a baliky - aj ked sme sa na arte dost narobili, karty a baliky by mali velmi zaujat - je to core mechanika hry, je to v konecnom dosledku ta blyskajuca sa odmena za namahu. Obe by mali byt v podstate 3D objekty ktore sa daju natacat, otacat; balik by mal mat svoju hrubku. V dalsom bode rozpravam o rozsireni mechaniky tierovania - a aj karty teda tym ze by boli silver/golden/platinum verzie, by mali mat pekne grafiky v tychto verziach. Karty by mali mat broders a nejaky "pill" ak su vyssej rarity, nech to nie je len shadow a odtien karty.
3. viac prekopana kolekcia, viacero vrstiev kariet - karty by mali mat viac viditelnych properties s ktorymi budeme pracovat v meta game mechanikach
  - cyklisti by mali mat viditelne timy (asi aj maju uz)
  - krajiny povodu pretekov
  - tiers - cize nie len rarities ale aj silver/golden/platinum karty
4. meta mechaniky, resp. ako vyrobit viac engagementu usra
  - achievements - otvor 1,3,5,10,25,50 balikov, vsetkych s jedneho timu, the greatest classics riders (last year), last year grand tour winners, my maaan victor, vsetky preteky z danej krajiny, monumenty, grand tours
  - leaderboards - pocas season viest card power statistiku
  - tiers - silver/golden/platinum karty sa budu dat najst aj v baliku, ale nie tak casto; budu sa dat vyrobit - cize 3 karty z nizsieho tieru budu sa dat prekonvertovat na vyssi - ako matrioska, neviem ale ci to nebude az prilis ak sa chce clovek dostat do platinum verzie (mozno tou spravime tak ze sa nebude dat otvorit v balikoch, max. gold); je to podobne ako v Teamfight Tactics, kde 3kove verzie champov su v nedohladne ale tym ze pridame sposoby ako otvarat karty user bude mat vela kariet
  - baliky by sa mohli dat otvarat aj automaticky ked prejde nejaky cas - cize kazdy den by mohol pribudnut jeden balik, aby user mal co robit, cize by tam bol aj casovy counter ako v Pokemon TCG
5. design celkovo musi byt lepsie spraveny a naplanovany - pouzit Figmu?
6. lepsi auth. flow - mali by sme si usra ulozit aj pod nasim token v nasej appke - hoci cez Google/Apple SSO, az potom pytat pripojenie Stravy
7. performance by mal byt dobry na priemernom zariadeni dnesnej doby
8. efektivne fetchovanie aktivit - mozno by sme ani nemuseli fetchovat aktivity, ako skor len celkove cislo nejake zo statistik. Treba hlavne ale fetchovania nalepit len na komponenty ktore to potrebuju, nerobit cakanie na vlak a vsetko komponenty musi cakat aj user na loading indikatore.

### Konkretne zdroje

- na panning mechanizmus pre balik aj karty mozme pouzit https://www.youtube.com/watch?v=msErROjFY08&t=31s React Native Filament
