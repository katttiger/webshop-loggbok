# Sprintloggbok

## Nuvarande staus

- Vi återuppväckte våra mikrotjänster på render och lade till CORS-konfiguration för order-, product- och authservice.
- Vi skapade webshoppens frontend.
- Webshoppen har login-funktionalitet.
- Kundvagn har skapats.
- Produkter hämtas från databasen och visas på en sida.
- Produkterna kan filtreras på kategori och namn.
- Varje produkt har en egen sida.
- Order kan läggas och betalning simuleras via Stripe.
- Frontend har en tydlig styling.
- Adminstratörer kan lägga till nya produkter.
- Webshoppen kan kontrollera användarens behörigheter så att vanliga användare inte kan komma åt administratörens sidor.
- En 404-sida finns och visas om en felaktig url anges.
- För att kunna komma åt hemsidan måste man vara inloggad. Om man försöker komma åt hemsidan utan att vara inloggad kommer man att omdirigeras till login-sidan.
- Användaren kan loggas ut.
- Användarens information sparas i sessionstorage, där information hämtas från en JWT som innehåller information om användaren och dennes rättigheter.

- Sätta upp ramar för det agila arbetet
- Alla har fått vara scrum master en gång (vi byter av efter varje sprint)

---

## Sprint 3 – vecka 42

### Vad jag arbetade med

Denna vecka fokuserade på att bygga en gateway mellan mikrotjänsterna och frontend. Då uppgiften upplevdes vara stor valde vi att jobba tillsammans denna sprint.

Vi kunde dock dela upp oss när det kom till att skapa repository, skapa docker image och att skapa instansen på Render. Jag fick ta hand om det sistnämnda samt skriva om gateway så att användarhantering sker med hjälp av en cookie.

### Eventuella problem och hur jag löste dem

Vi har lyckats registrera våra tjänster på Render, men funderar fortfarande på hur det ska gå att koppla ihop det ordentligt. Då vi fortfarande har frågor och fokuserar på funktionalitet väljer vi att skjuta upp denna fråga till senare.

### Samarbete och agilt arbete

Jag valdes ut till Scrum Master och ansvarade för att skapa korten i Trello och dela ut arbetet. På måndag morgon överförde jag uppgifterna i product backlog till våran trello tavla och försökte bryta ned uppgiften efter bästa förmåga till checklistor.

På måndag hade vi, som vanligt, vår Sprint Planing kl. 10. Under mötet gick vi igenom tavlan och veckans uppgifter. Efter att ha förstått upgifterna gjorde vi en Scrum Poker med Fibonnacci-nummer, som motsvarar de nummer som läraren har gett oss, och delade upp uppgiften. Då veckans uppgifter var stora valde vi att jobba tillsammans med kodning, informationsinhämntning, tolking av teori och bidrag med kod. Utifrån detta beskrev vi våra sprintmål.

Varja dag hade vi våra daily scrum klockan 10:00, förutom på tisdagar och torsdagar, då mötet flyttades till efter lektionen. Under daily scrum gick vi igenom vad som skulle göras. Då vi jobbade gemensamt denna vecka behövdes ingen större informationsspriding och daily scrum förvandlades till den kanal vi arbetade tillsammans i.

---

## Sprint 4 – vecka 43

### Vad jag arbetade med

Veckans fokus låg på tester och att se till att användaren är inloggad även när sidan laddas om.

Under måndagen fokuserade två av oss på den sistnämnda uppgiften och vi lyckades skapa den endpoint som behövdes och förbereda frontend för konverteringen. Dessvärre kom vi inte ända in i mål och behövde lyssna på föreläsningen på tisdagen för att kunna färdigställa uppgiften, nu med hjälp av Jakob. Efter detta är användaren fortsatt inloggad även om sidan laddas om och utloggningen tar bort dennes information.

På onsdagen låg fokus på tester och där var teorin det mest krävande, men vi hjälptes åt och kunde få till de tester som beskrivits i backlogg. Utöver att undersöka hur tester kunde integreras i applikationen skulle vi även sätta upp en testmiljö och skriva tester med mockat data. För detta ändamål använde vi MSW och mockade en server, användare och produkter för att kontrollera att tjänste-lagret i frontend fungerade och att fel hanterades på ett bra sätt.

När vi var klara med det fortsatte vi med att jobba med driftsättning av frontend på Render. Den stora utmaningen var att koppla ihop frontend med gateway.

### Eventuella problem och hur jag löste dem

Vi stötte tidigt på patrull vad gällde adminsidorna. När vi uppdaterade till att använda en cookie för inloggning slutade våran admin-naviation att fungera. Resultatet är att admin inte kan nå admin-sidorna och loggas ut. Detta problem försökte vi lösa samtidigt som vi jobbade på metoden för att hämta informaiton om användaren från cookie. Vi misstänker att felet ligger i hur applikationen hanterar omdirigeringen av användaren, vilket innebär att datorn inte läsa av användaren eller att personen loggas ut när sidan renderas om. Vi valde att avsluta våra egna experiment och lyssna på vad läraren hade för tips. Tack vare dem löste vi problemet och kunde gå vidare.


På torsdagen bytte vi fokus till deoplyment på Render. Det som ställde till det för oss var att vi på vissa ställen i applikationen hade glömt att byta URL, så vissa services pekade på den lokala porten och inte på instansen på Render. Vi lyckades lösa detta med hjälp av läraren och AI, som båda påpekade att URL:er och cookie stökade till det. 

Vidare misslyckades några av våra mockade tester när vi försökte köra igenom det på GitHub. Vi tänkte först att det var metoderna som spökade men kunde inte komma på vad det var då testet hade gått igenom föregående dag. Vi valde därmed att kontrollera våra miljövariabler i GitHub och på Render, vilket löste ut det hela.


### Samarbete och agilt arbete

Sprintplaneringen skedde på måndagen. Under mötet flyttade vi över uppgifter från product backlog till våran Trello-tavla och använde Scrum poker för att avgöra vilka kort vi skulle ha i våran sprintplanering. Vi satte upp våra sprintmål och fokus den här veckan låg på datahantering i cookie och att sätta upp tester. Våran ambition var att alla skulle jobba med ett tekniskt kort var och att när man blev klar så skulle man jobba med undersökningarna då de inte påverkade något annat i backlogg.


---

## Sprint 5 – vecka 44

### Vad jag arbetade med

- Vilka items i backloggen arbetade du med?
- Vad blev färdigt, vad blev inte färdigt?

### Eventuella problem och hur jag löste dem

- Lite om ev problem och lösningar på dem

### Samarbete och agilt arbete

- Beskriv tex sprintplanering, daily scrums, annat samarbete kortfattat

---

## Sprint 6 – vecka 45

### Vad jag arbetade med

- Vilka items i backloggen arbetade du med?
- Vad blev färdigt, vad blev inte färdigt?

### Eventuella problem och hur jag löste dem

- Lite om ev problem och lösningar på dem

### Samarbete och agilt arbete

- Beskriv tex sprintplanering, daily scrums, annat samarbete kortfattat
