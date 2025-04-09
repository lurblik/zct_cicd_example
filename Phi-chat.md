<h1 align=center> ⊱Phi-Chat⊰ </h1>

<h3>Súhrn: </h3>

&emsp;&emsp;V tomto projekte sme sa snažili vytvoriť implementáciu chatbota pomocou "Gemini API", nasadenú v cloude. Tento projekt je kontajnerizovaná streamlit aplikácia využivajúca veľký jazykový model "Gemini Pro" pomocou "Gemini API" a "Azure Cosmos DB" databázu s "Mongo DB" na ukládanie histórie chatu aplikácie. 

<hr>

<h3>Zvolené technológie: </h3>

- 📖 Knižnica Streamlit - pre zjednodušenie tvorby použivateľského rozhrania
- 👁️ Veľké jazykové modely - na ziskávanie odpovedí pre chatbota
- 💾 Azure cosmos db - NoSQL_db, mongo_db, poskytovaná Microsoft Azure na ukládanie chatu použivateľa 
- ⛅ Aplikácia je hostovaná cloudovým poskytovateľom Microsoft AZURE
- 🐳 Docker - na kontajnerizáciu našej aplikácie
- 🐍 Python 3.9-slim

<hr>

<h3>Diagram použitých služieb: </h3>
<br>

![[Pasted image 20250409165252.png]]
<br>

Použivateľ do aplikácie zadá otázku a otázka sa pošle veľkému jazykovému modelu ktorý vygeneruje odpoveď, a pošle ju späť na stránku kde ju použivateľ uvidí. V momente keď použivateľ zadá otázku tak sa uloží do databázy. 
<hr>

<h3>Rozdelenie práce: </h3>

- 🙍‍♀️ S. Čorbová - cloud + databáza
- 🙍‍♂️ M. Grus - dokumentácia + kontajnerizácia aplikácie
- 🙍‍♀️ I. Soláriková - front-end aplikácie
- 🙍‍♂️ M. Košarič - integrácia veľkého jazykového modelu do aplikácie pomocou Gemini API

<hr>

<h3>Návod na používanie aplikácie: </h3>

- Otvoríme si ľubovoľný internetový prehliadač. 
- Vložíme tento link <code>https://phichat.azurewebsites.net/</code> do vyhľadavacieho okienka.
- Tlačidlom ENTER potvrdíme vyhľadavanie danej adressy. 
- Na obrazovke sa otvorí pracovné prostredie nášho chatbota "Phichat" ktorému môžeme začať pokládat otázky.
- Po krátkom čakaní dostaneme odpoveď na zadanú otázku.
- Pri ukončovaní práce s chatbotom môžeme vymazat historiu pokial nechceme aby si konverzáciu pamätal a následne zatvoríme kartu v prehliadači. 

<hr>
