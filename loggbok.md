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

## Sprint 3 – vecka 42

### Vad jag arbetade med

Denna vecka fokuserade på att bygga en gateway mellan mikrotjänsterna och frontend. Då uppgiften var stor valde vi att jobba tillsammans. Mitt huvudansvar för veckan var att se till att depployment på Render skedde. 

Utöver att lägga upp gateway på Render och koppla den till våra mikrotjänster, fick jag även skriva om gateway för att den ska hantera en cookie.

### Eventuella problem och hur jag löste dem

När vi testade våran gateway på Render fick vi ett 401 fel när vi jobbade mot product-mikrotjänsten trots att vi var inloggade.

### Samarbete och agilt arbete

Jag valdes ut till Scrum Master och ansvarade för att skapa korten i Trello och dela ut arbetet. På måndag morgon överförde jag uppgifterna i product backlog till våran trello tavla och försökte bryta ned uppgiften efter bästa förmåga till checklistor.

På måndag hade vi, som vanligt, vår Sprint Planing kl. 10. Under mötet gick vi igenom tavlan och veckans uppgifter. Efter att ha förstått upgifterna gjorde vi en Scrum Poker med Fibonnacci-nummer, som motsvarar de nummer som läraren har gett oss, och delade upp uppgiften. Då veckans uppgifter var stora valde vi att jobba tillsammans med kodning, informationsinhämntning, tolking av teori och bidrag med kod. Utifrån detta beskrev vi våra sprintmål.

Varja dag hade vi våra daily scrum klockan 10:00, förutom på tisdagar och torsdagar, då mötet flyttades till efter lektionen. Under daily scrum gick vi igenom vad som skulle göras. Då vi jobbade gemensamt denna vecka behövdes ingen större informationsspriding och daily scrum förvandlades till den kanal vi arbetade tillsammans i.

## Sprint 4 – vecka 43

### Vad jag arbetade med

- Vilka items i backloggen arbetade du med?
- Vad blev färdigt, vad blev inte färdigt?

### Eventuella problem och hur jag löste dem

- Lite om ev problem och lösningar på dem

### Samarbete och agilt arbete

- Beskriv tex sprintplanering, daily scrums, annat samarbete kortfattat

## Sprint 5 – vecka 44

### Vad jag arbetade med

- Vilka items i backloggen arbetade du med?
- Vad blev färdigt, vad blev inte färdigt?

### Eventuella problem och hur jag löste dem

- Lite om ev problem och lösningar på dem

### Samarbete och agilt arbete

- Beskriv tex sprintplanering, daily scrums, annat samarbete kortfattat

## Sprint 6 – vecka 45

### Vad jag arbetade med

- Vilka items i backloggen arbetade du med?
- Vad blev färdigt, vad blev inte färdigt?

### Eventuella problem och hur jag löste dem

- Lite om ev problem och lösningar på dem

### Samarbete och agilt arbete

- Beskriv tex sprintplanering, daily scrums, annat samarbete kortfattat
