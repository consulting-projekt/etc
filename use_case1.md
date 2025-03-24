## Vertiefung von Use Case 1: Einfache Routenabfrage mit semantischer Suche

### Technische Implementierung

#### Architekturansatz: LLM mit Graph-RAG

1. **Datenvorbereitung**:
   - HVV-Liniennetz als Graphdatenbank modellieren
   - Knoten: Haltestellen, POIs (Points of Interest)
   - Kanten: Verbindungen zwischen Haltestellen mit Fahrtzeiten
   - Semantische Anreicherung: Tagging von Haltestellen mit Eigenschaften wie "Innenstadt", "Touristenattraktion", etc.

2. **Kernkomponenten**:
   - **Frontend**: Chat-Interface für Nutzereingaben
   - **NLU-Modul**: Extraktion von Absichten und Entitäten aus Nutzereingaben
   - **Graph-RAG-System**: Verknüpfung zwischen semantischen Konzepten und konkreten Haltestellen
   - **Routing-Engine**: Berechnung von optimalen Verbindungen
   - **Antwortgenerator**: Nutzerfreundliche Formulierung der Ergebnisse

3. **Prozessablauf**:
   - Nutzer stellt Anfrage (z.B. "Wann kommt der nächste Bus in die Innenstadt?")
   - LLM extrahiert Absicht (Fahrplanabfrage) und Entitäten (Ziel: "Innenstadt")
   - Graph-RAG identifiziert relevante Haltestellen, die mit "Innenstadt" assoziiert sind
   - Routing-Engine berechnet Verbindungen zum identifizierten Ziel
   - LLM generiert natürlichsprachliche Antwort mit den gefundenen Verbindungen

### Datengrundlage und synthetische Daten

1. **Echte Daten**:
   - GTFS-Feeds des HVV (falls verfügbar)
   - OpenStreetMap-Daten für Hamburg
   - POI-Datenbanken (z.B. über Google Places API, OpenStreetMap)

2. **Synthetische Daten**:
   - Generierung eines vereinfachten Liniennetzes basierend auf öffentlich zugänglichen Karten
   - Künstliche Fahrplandaten mit realistischen Taktzeiten
   - Synthetisches Mapping von semantischen Konzepten zu Gebieten:
     ```json
     {
       "Innenstadt": ["Rathaus", "Jungfernstieg", "Mönckebergstraße", "Hauptbahnhof"],
       "Hafen": ["Landungsbrücken", "Baumwall", "HafenCity Universität"],
       "Seenähe": ["Alster", "Außenalster", "Planten un Blomen"]
     }
     ```