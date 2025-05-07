6000 wörter

# 1 Einleitung (5-10% -> 300-600)

## &nbsp;&nbsp;&nbsp; 1.1 Motivation

Dieses Kapitel beschreibt wieso wir uns mit dem Thema beschäftigen. Es umreißt den größeren Rahmen der Arbeit (sprich warum ist das Thema allgemein relevant und warum es sinnvoll ist sich damit zu beschäftigen)

## &nbsp;&nbsp;&nbsp; 1.2 Problemstellung

Dieses Kapitel beschreibt die konrekte Problemstellung für das vorliegende Projekt der HVV.

## &nbsp;&nbsp;&nbsp; 1.3 Zielstellung

Dieses Kapitel deutet das Ziel der Arbeit an auf Basis der Problemstellung und der Motivation.
Was wollen wir technisch und wissenschaftlich sowie methodisch erreichen
Was wollen wir NICHT erreichen

## &nbsp;&nbsp;&nbsp; 1.4 Aufbau und Methodik der Arbeit

Dieses Kapitel hat 2 Funktionen.
Erstens soll die Methodik der vorloegenden Arbeit dargelegt und auf das konkrete Projekt angewendet, beschrieben werden.
Zweitens soll es die Struktur der Arbeit, sprich die Glierung, kurz als Text erläutern, sodass ein roter Faden erkennbar ist.
Die Gliederung soll dabei bereits die Methodik referenzieren und die einzelnen Shcritte der Methodik mit den Gliederungspunkten mappen, sodass der Leser versteht, wann welcher Schritt umgesetzt wird.

# 2 Theoretischer Hindergrund und Forschungsstand (22% -> 1320)

## &nbsp;&nbsp;&nbsp; 2.1 Large Language Models

Fließender Übergang zu LLM, welche NLP/NLU-Methoden verwenden, jedoch generativer Art sind. Beleuchtung des Trainings und der unterschiedlichen Modelle und Größen von LLM sowie Darstellung der aktuellen Produkt-Landschaft. Ggf. kurzer Fokus auf Benchmarks, falls sinnvoll.

- Verwendung für NER, entity extraction

## &nbsp;&nbsp;&nbsp; 2.2 Retrieval-Augmented Generation

Funktionsweise und Relevanz von RAGs darstellen sowie auf aktuelle Paper und deren (erfolgreiche) Anwendung eingehen. Aufzeigen der Fähigkeiten und des Nutzens von RAGs im Kontext unserer Problemstellung (ebenfalls darstellung von Limitationen). Beleuchtung von unterschiedlichen Varianten

## &nbsp;&nbsp;&nbsp; 2.3 Prompt Engineering

# 3 Praktische Anwendung (1350)

## &nbsp;&nbsp;&nbsp; 3.1 Struktur und Konzept der technischen Umsetzung

In diesem Kapitel soll die Struktur der technischen Lösung auf HIgh Level dargelegt werden.
Die einzelnen Bausteine sollen in deren Funktionsweise beschrieben werden.
Es soll ein Gesamtbild entstehen, sodass man erkennen kann, wo kommen die Daten her, wie werden sie verarbeitet, was entsteht E2E.

- use case classifier
- UC1 einfache Routenabfrage Zustandsdiagramm

## &nbsp;&nbsp;&nbsp; 3.2 Data Acquistion und Data Understanding

In diesem Kapitel sollen die verwendeten Daten und dessen Struktur dargelegt werden. Dies kann dabei sowohl die Input Queries als auch die API Daten umfassen.

- Routen/Orte sind ständig im Wandel -> dynamisch
- LLM muss mit aktuellen Daten als Kontext arbeiten
  - per API/RAG-Schnittstellen
- abwägung möglicher Datenquellen
  - openstreetmap
  - geofox api
  - rag

## &nbsp;&nbsp;&nbsp; 3.3 Modeling

In diesem Kapitel sollen die einzelnen Bausteile der technsichen Lösung erläutert werden im Detail.
Anschließend sollen verschiedene Implementierungsansätze abgewogen werden, die während der Implementierung erwogen wurden: verschiedene LLMs, qdrant, geofox api.
Zuletzt soll die technische Lösung evalusiert werden. Die Testing Schritte sollen dabei technisch in deren Implementierung dargelegt sowie deren Ergebnisse interpretiert werden.

-

### &nbsp;&nbsp;&nbsp; 3.3.1 Verarbeitung der Input-Queries

- extraktion von parametern
  - prompt engineering
  - Abwägung verschiedeneder Large Language Modelle
- Behandlung von Probelmen
  - nutzer vergisst Start anzugeben

### &nbsp;&nbsp;&nbsp; 3.3.2 Formulierung und Implementierung der Datenabfrage

- passende verwendung von API/RAG
- Abwägung verschiedeneder embedding Modelle

### &nbsp;&nbsp;&nbsp; 3.3.3 Antwortgenerierung

- Kombination aus Query und API/RAG antworten als LLM Query
  - prompt engineering
  - einhaltung eines passenden schreibstils (HVV konform)
- behandlung von problemen
  - von nutzer angegebene Startpunkt existiert nicht

### &nbsp;&nbsp;&nbsp; 3.4 UI/UX Design

# 4 Evaluation der technischen Lösung (1350)

## &nbsp;&nbsp;&nbsp; 4.1 Konzept

getestet wird:

- extraktion von parametern
- embedding suche
- antwort mit angemessenem Stil

## &nbsp;&nbsp;&nbsp; 4.2 Ergebnisse

## &nbsp;&nbsp;&nbsp; 4.3 Identifizierte Limitationen

In diesem Kapitel soll die technische Lösung hinsichtlich der Problemstellung kritisch bewertet werden. Wird das Problem gelöst? Ist die Problemlösung angemessen? Welche Lösungen haben sich als ideal herausgestellt und warum?

# 5 Consulting der HVV (ca. 18% -> 1080)

## &nbsp;&nbsp;&nbsp; 5.1 Aktuelle Situation

## &nbsp;&nbsp;&nbsp; 5.2 Zieldefinition

## &nbsp;&nbsp;&nbsp; 5.3 Lösungskonzeption

## &nbsp;&nbsp;&nbsp; 5.4 Zeit- und Kostenplanung

## &nbsp;&nbsp;&nbsp; 5.4 Zusammenfassung der Optionen

In diesem Kapitel soll der Consulting Teil der Arbeit formuliert werden. Wie ist die aktuelle Situation bei der HVV und warum soll hier überhaupt etwas angepasst oder entwickelt werden? Wie ist das Ziel zu definieren und wann/womit wird es erreicht (Metriken)? Wie kann eine konkrete Lösung aussehen und gibt es hier eine günstigere/schlankere und eine umfassendere/kostenintensivere Lösung? Wie sieht eine Zeit- und Kostenplanung konkret für die Lösung/en aus (Vollintegration mit Backend und Frontend)? Abschließend eine Zusammenfassung der Keyfacts sowie der potenziellen Optionen zur Zielerreichung.

# 6 Zusammenfassung und Ausblick (5-10% -> 300-600)

## &nbsp;&nbsp;&nbsp; 6.1 Zusammenfassung

## &nbsp;&nbsp;&nbsp; 6.2 Ausblick

Zuletzt soll die technische Implementierung zusammengefasst werden. Was hat funktioniert, was nicht. Referenz auf die Methodik, den theoretischen Hintgerund/aktueller Forschungsstand sowie die Zielstellung und Problemstellung der Arbeit ist sinvoll.
Im Ausblick sollen die möglichen nächsten Schritte dargelegt werden. Was kann als nächstes folgen, was sollte man noch evaluieren, testen, implementieren, welche themen aus dem aktuellen forschungsstand sollen noch aufgegriffen werden.
