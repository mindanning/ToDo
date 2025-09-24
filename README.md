# ToDo
En enkel To-Do applikasjon i SwiftUI. Appen gir brukeren mulighet til å lage, vise, redigere og slette oppgaver.

# struct Oppgave
Dette er oppskriften på en oppgave.
Hver oppgave får et unikt id-nummer (UUID).
Den har tittel, beskrivelse, frist (dato) og status (Ikke startet, Pågår, Fullført).

# enum Status
Dette er listen over de tre mulige statusene:
 - Ikke startet
 - Pågår
 - Fullført
Her er det også lagt til:
Et ikon som passer til status (klokke, timeglass, hake).
En farge (oransje, blå, grønn) som gjør status mer tydelig.

# InnholdsView
Dette er hovedsiden i appen.
Viser en liste med alle oppgavene.

# OppgaveDetaljVisning
Dette er siden som åpnes når du trykker på en oppgave i listen.
Her kan brukeren endre:
 - Tittel
 - Beskrivelse
 - Frist (dato)
 - Status
Skjermen er bygget opp som et skjema (Form).

// Midlertidige variabler som lagrer det brukeren skriver inn i skjemaet
 @State private var tittel: String = ""
    @State private var beskrivelse: String = ""
    @State private var frist: Date = .now
    @State private var status: Status = .ikkeStartet
