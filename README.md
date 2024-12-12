Mappeinnlevering 4
Emne 7 Software Design
TID: 2024-12-06 til 2024-12-11 12:00
Hjelpemidler: Alle
Vedlegg: «Emne 7 Mappe 4 2024.zip»
Innlevering: Zip fil av hele applikasjonen.
Oppgavebeskrivelse
I denne oppgaven skal du videreutvikle Todo-applikasjonen ved å implementere et repositorylag, arbeide med relasjoner mellom tabeller og modeller, og legge til avansert service-logikk. 
Målet er å gjøre applikasjonen mer strukturert og funksjonell, samtidig som du får erfaring 
med datamodellering og god arkitektur.
Oppgavene
1. Repository Pattern
• Lag et repository-lag for datatilgang, og sørg for at all kommunikasjon med databasen 
skjer gjennom dette laget.
• Opprett et interface for repositoryet, og implementer det med nødvendige metoder for 
å håndtere CRUD-operasjoner for Todo-oppgaver.
• Registrer repositoryet i Dependency Injection-containeren, slik at det kan brukes av 
TodoService.
• Oppdater TodoService slik at den kun kommuniserer med repositoryet og ikke direkte 
med databasen.
2. Relasjoner mellom tabeller
• Opprett en ny modell for kategorier, og legg til en relasjon mellom Todo-oppgaver og 
kategorier:
o En Todo kan tilhøre én kategori.
o En kategori kan ha flere Todo-oppgaver.
• Oppdater datamodellene og databasen for å støtte denne relasjonen, inkludert 
nødvendige migrasjoner.
• Lag en ny controller for kategorier med CRUD-funksjonalitet.
• Oppdater Todo-applikasjonen slik at oppgaver kan kobles til kategorier ved 
opprettelse eller oppdatering.
• Legg til støtte for å filtrere Todo-oppgaver basert på kategori.
3. Avansert service-logikk
• Utvid TodoService med ny funksjonalitet som lar deg:
o Hente alle oppgaver tilhørende en spesifikk kategori.
o Finne antall Todo-oppgaver per kategori.
o Hente alle fullførte Todo-oppgaver, inkludert informasjon om hvilken kategori 
de tilhører.
• Sørg for at logikken for disse funksjonene håndteres i TodoService og ikke i 
controlleren.
