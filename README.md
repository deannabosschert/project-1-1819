# Project 1 @cmda-minor-web · 2018-2019

## Zoek in de de collectie van de OBA

### Inspiratie

Mijn concept is gebaseerd op het idee van Charlotte (Project Interaction 2019, CMD Amsterdam):
"Voor de kinderafdeling, de jongste lezers helpen vinden door ze visueel te laten zoeken met dezelfde categorieën als
Bv griezel plaatje aanklikken (en daarna een ander plaatje?)  om tot boekkeuze te komen (en dan de weg krijgen naar de boekenkast)."

Binnen de site van de KinderOBA miste ik inderdaad het casual browsen binnen de algemene genres; er kan alleen gezocht worden via de search bar of via al uitgelichte genres of thema's. Aangezien kinderen vaak nog aan het ontdekken zijn van welke soort schrijvers ze houden of van welk thema, lijkt dit mij toch een best belangrijk missend onderdeel.

### Mijn concept

Kinderen kunnen een boek vinden door middel van filteren via genres op basis van visuele weergaves van de verschillende genres ipv tekstueel.
Over het algemeen zoeken kids hun boeken voornamelijk uit op basis van omslag en wat voor associatie ze hebben bij een bepaald onderwerp, dus waarom dan ook geen mogelijkheid tot casual browsen binnen een genre op basis van een visuele representatie van het genre?

Denk hierbij aan:
Griezelboeken - Spookje
Detective - Vergrootglas
Avontuur - Kompas
Dieren- Pootafdruk
Geschiedenis - Romeinse zuilen
Humor - Smiley
Oorlog/verzet - Vlag en prikkeldraad
Psychologie - Brein
Spanning - Pistool
Sport - Voetbal, tennisracket, basketbal
Sprookjes/Mythologie - Toverhoed
Vriendschap/liefde - Drie personen, hartjes

Misschien uit te breiden met een soort moodboards bij de iconen (onder een dropdown oid?) waardoor een kind een wat bredere indruk op kan doen van het genre.

### Wat gaat er gebeuren?

1. Overview op de homepage laadt alleen de 12 iconen
2. Wanneer op één van de iconen wordt geklikt en de user naar de pagina van het desbetreffende genre wordt gelinkt, wordt de API pas aangeroepen --> route naar genreDetailpagina.
3. Filteren op: book - dutch - ageYouth - [genre of topic dat aangeklikt is] - sorteren op [title] - &count=25
4. Op de genreDetailpagina worden vervolgens de boeken geladen, wanneer er op een van deze geklikt wordt, word je doorverwezen naar de detailpagina van het desbetreffende boek; nieuwe API call waarin het volgende wordt opgevraagd: titel, auteur, omslagfoto [...]

Genres:

- detective
- humor
- oorlog-en-verzet
- psychologisch-verhaal
- romantisch-verhaal
- sprookjes

Topic:

- Geschiedenis
- Cultuurgeschiedenis
- Vriendschap
- Verliefdheid
- Wereldoorlog I
- Wereldoorlog II
- Sprookjesfiguren
- Magie
- Liefde

Language:

- dut

Sorteren:

- sort=title

Resultaten:

- &count=25

### Idee 2

Situatie: je wil graag een boek lenen bij de OBA Oosterdokskade, maar deze is vaak al uitgeleend. Je hebt geen zin om geld te betalen voor een reservering en zet het boek maar gewoon in je 'favorieten' voor later. Het boek is nog wel beschikbaar bij andere vestigingen maar aangezien zij niet op je route liggen vind je het niet waard om er speciaal voor te gaan kijken, zeker aangezien je al vaak onderweg bent en anders heel specifiek naar de locaties van andere vestigingen te kijken.

Idee: afgekeken van de app Swarm; je krijgt een melding zodra je GPS opmerkt dat je in de buurt van een OBA-vestiging bent waar een boek van je verlanglijst beschikbaar is.
