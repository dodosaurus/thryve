# Brainstorm about tech stacks

## 14-12-2024

### Initial thoughts
To v akom tech stacku sa bude robit appka ovplyvni komplexnost a v konecom dosledku cas, za ktory sa vyroby prva funkcna verzia produktu.

### Rozbor - React Native
PROS:
- Typescript
- skoro ako Next JS
- sme full vo component frameworku, v ktorom som ako doma a teda cisto v IDE v ktorom rad robim (Cursor, VS Code)
- vieme viac vyuzivat AI
- integracia modulov ako autorizacia cez Stravu bude lahsia, lebo bude podobna ako v EV
- je to aplikacny vyvoj prakticky, ktory mi je blizky; len budeme tu appku musiet zrobit ako hru

CONS:
- stale tam budu mobilne specifika ktore sa budem musiet naucit a im pochopit
- sme obmedzeny tym ze nie sme v game engine - animacie, tilesety, fyzika; ma predpripravene objekty (nodes) pre postavy, fyzikalne objekty v 2D priestore
- mozno bude niektore veci problematickejsie vyvinut, kedze IDE bude cisto code editor; nie je to ako v Unity/Godote

### Rozbor - Godot
PROS:
- herny engine, prisposbeny na vyvoj hry v pixel grafike (fyzika, animacie, tileset nastroje a pod.) - je to big deal

CONS:
- GDScript, ktory neovladam
- IDE ktore neovladam
- vyvojove prostredie Godot ktore neovladam
(= learning overhead velky asi)
- absencia AI autocompletion a pomocnych agentov


Ten cas, ktory budem potrebovat na Godot bude dost velky. Trebalo by viacero projektov podla YT spravit. LEbo len robenim projektov sa clovek uci kodit hlavne.

S Reactom (aj ked toto je React Native) som uz robil viac krat a mam aj celko mkomplikovane projekty uz za sebou, ako aj Endurance Vault. V reale MVP bude hotovy skor v React Native.