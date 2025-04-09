### vcielky  present:

# Facebook Clone
## (ako mobilná verzia)

## Obsah
- [Úvod](#úvod)
- [Slovný rozbor a analýza úlohy](#slovný-rozbor-a-analýza-úlohy)
- [Odôvodnenie zvolených technológií](#odôvodnenie-zvolených-technológií)
- [Diagram použitých služieb](#diagram-použitých-služieb)
- [Príspevok členov tímu](#príspevok-členov-tímu)
    - [Natália Tomková](#natália-tomková)
    - [Jozef Gočík](#jozef-gočík)
    - [Patrik Štefančík](#patrik-štefančík)
    - [František Vaľko](#františek-vaľko)
- [Dokumentácia k používaniu aplikácie](#dokumentácia-k-používaniu-aplikácie)
    - [Setup](#setup)
    - [Spustenie](#spustenie)
    - [Vstupy](#vstupy)
    - [Výstupy](#výstupy)

## Úvod
Táto dokumentácia poskytuje komplexný prehľad o našom projekte, vrátane analýzy úlohy, použitých technológií a postupov pre inštaláciu a použitie aplikácie. Navrhovaná aplikácia má za cieľ poskytnúť užívateľom prostredie podobné sociálnej sieti Facebook, s dôrazom na jednoduchú a intuitívnu použiteľnosť.
## Slovný rozbor a analýza úlohy
Naša aplikácia umožňuje užívateľom vykonávať viacero kľúčových funkcií, vrátane sledovania a vyhľadávania iných používateľov, pridávania nových príspevkov a vyjadrovania svojho súhlasu s príspevkami pomocou funkcie "like". Tieto funkcie tvoria základ interakcie v sociálnom prostredí aplikácie a sú dôležité pre vytvorenie užívateľskej skúsenosti, ktorá pripomína populárnu sociálnu sieť Facebook.
## Odôvodnenie zvolených technológií
Pri vývoji našej aplikácie sme sa rozhodli využiť kombináciu rôznych cloudových služieb, ktoré nám poskytujú potrebnú funkcionalitu a výkon. Konkrétne sme sa spojili s týmito službami:

Firebase: Používame Firebase na autentifikáciu používateľov, ukladanie informácií o používateľoch a ukladanie fotografií. Jeho jednoduchá integrácia a množstvo nástrojov pre autentifikáciu a ukladanie dát nám umožňujú rýchlo vytvoriť backend pre našu aplikáciu.
MongoDB Realm: Pre ukladanie dát o príspevkoch a aktivitách sme sa obrátili na MongoDB Realm. Jeho flexibilita a možnosť rýchleho vývoja nám umožňujú efektívne spravovať a manipulovať s dátami, čo je kritické pre správne fungovanie našej sociálnej aplikácie.
Amplify AWS: Na zasielanie push notifikácií sme zvolili službu Amplify AWS. Jeho spoľahlivosť a jednoduché použitie nám umožňujú efektívne komunikovať s našimi užívateľmi a upozorniť ich na dôležité udalosti v aplikácii.
Pre vývoj front-endu sme sa rozhodli použiť Flutter pre jeho schopnosť vytvárať multi-platformové mobilné aplikácie s jednotným kódom.

## Diagram použitých služieb
Využili sme 3 cloudové služby. 1. Firebase - autentifikácia používateľov, ukladanie informácií o používateľoch a ukladanie fortografií. 2. MongoDB Realm - ukladanie dát o príspevkoch a aktivitách. 3. Amplify AWS - posielanie push notifikácií.
![Diagram](https://private-user-images.githubusercontent.com/166152352/328986921-08a58b6e-df8d-4d53-8903-d0b9ee9dea41.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDQyMTA4ODEsIm5iZiI6MTc0NDIxMDU4MSwicGF0aCI6Ii8xNjYxNTIzNTIvMzI4OTg2OTIxLTA4YTU4YjZlLWRmOGQtNGQ1My04OTAzLWQwYjllZTlkZWE0MS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjUwNDA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI1MDQwOVQxNDU2MjFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT05ZGM5MWZkZDFlZDVjYTY1YTlhMzA3NGRjMjAyZDI2NWJmM2VhNTZiNmI3NWViYzc2YmVkN2RhM2IzNmRkNjgzJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCJ9.ohkQ4NTgcLbrZefYlp5fe3H_ntZ1uRkIinnHg-Y9fss)


## Príspevok členov tímu

### Natália Tomková
Pracovala som na integrácii AWS - Amplify a Push notifikácií, ako aj na vývoji frontendu pre sign_in, sign_up a feed obrazovky.
### Jozef Gočík
Firebase -> setup, autentifikácia - vytvorenie triedy AuthMethods, ukladanie foografií - vytvorenie triedy StorageMethods, prepojenie s MongoDB Realm, navrhnutie User modelu + UserService triedy. MongoDB Realm -> setup, vytvorenie RealmService triedy, navrhnutie Post modelu + PostService triedy, navrhnutie Activity modelu + ActivityService triedy.
### Patrik Štefančík
V tomto projekte som sa venoval vývoju frontendu pre settings a add_edit_post a ich funkcionalite.
### František Vaľko
Pracoval som prevažne na UI vo flutteri -> konkrétne na bottom_navigation_bar, search_screen a activity_screen + výpomoc pri integrácií AWS

## Dokumentácia k používaniu aplikácie
### Setup
1. Stiahnite si zdrojový kód z repozitára.
2. Nainštalujte Flutter SDK podľa inštrukcií na oficiálnej stránke.
3. Nainštalujte všetky závislosti pomocou príkazu flutter pub get.
### Spustenie
1. Pre spustenie aplikácie stiahnite [aplikáciu Facebook Clone](https://drive.google.com/file/d/1gHkrbrlE-PxvIStfG1uXtThvB4CBbO7e/view) a nainštalujte ju na vaše zariadenie.
2. Po inštalácii aplikácie ju spustite a prihláste sa pomocou svojich prihlasovacích údajov.
3. Po úspešnom prihlásení budete môcť používať všetky funkcie aplikácie.
(alternatívne spustenie):
4. Stiahnite si zdrojový kód z repozitára.
5. Otvorte projekt vo vašom obľúbenom vývojovom prostredí.
6. Pripojte svoje zariadenie alebo spustite emulátor.
### Vstupy
1. Prihlasovacie údaje (username,e-mail,heslo) pre prístup k aplikácii.
2. Obsah príspevkov, a iných interakcií.
### Výstupy
1. Zobrazenie domovskej obrazovky so správami a príspevkami.
2. Možnosť pridávať nové príspevky.
3. Notifikácie o nových správach a interakciách pomocou AWS. 
 
