# 1 Motivation und Zielstellung
	
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
  
# 2 Theoretischer Hindergrund und Forschungsstand
  ## &nbsp;&nbsp;&nbsp; 2.1 Natural Language Processing 
  Einleitung des theoretischen Grundlangen anhand "der Basics" und Erläuterung, was unter NLP zu verstehen ist, wie sich NLP von NLU abgrenzt und warum NLP/NLU zur Lösung unserer Problemstellung notwendig ist. Hier wird ebenfalls auf die Verarbeitung (bspw. Tokenisierung eingegangen)
  ## &nbsp;&nbsp;&nbsp; 2.2 Large Language Models
  Fließender Übergang zu LLM, welche NLP/NLU-Methoden verwenden, jedoch generativer Art sind. Beleuchtung des Trainings und der unterschiedlichen Modelle und Größen von LLM sowie Darstellung der aktuellen Produkt-Landschaft. Ggf. kurzer Fokus auf Benchmarks, falls sinnvoll.
  ## &nbsp;&nbsp;&nbsp; 2.3 Retrieval-Augmented Generation
  Funktionsweise und Relevanz von RAGs darstellen sowie auf aktuelle Paper und deren (erfolgreiche) Anwendung eingehen. Aufzeigen der Fähigkeiten und des Nutzens von RAGs im Kontext unserer Problemstellung (ebenfalls darstellung von Limitationen). Beleuchtung von unterschiedlichen Varianten
  ## &nbsp;&nbsp;&nbsp; OPTIONAL: *2.4 Graph-Datenbanken* alternativ *2.4 API*
  *Darstellung von NoSQL-Datenbanken und/oder Graph-Datenbanken zur Speicherung und Nutzung von Daten mit Relationen. Ebenfalls Beleuchtung von Kombinationen von Graph-Datenbanken, RAGs und LLMs mit vorhandenen Lösungen* 
  
  alternativ 
  
  *Darstellung und Erläuterung von APIs inkl. aktueller Standards sowie Vor- und Nachteile*

# 3 Praktische Anwendung

  ## &nbsp;&nbsp;&nbsp; 3.1 Struktur und Konzept der technischen Umsetzung

  In diesem Kapitel soll die Struktur der technischen Lösung auf HIgh Level dargelegt werden.
  Die einzelnen Bausteine sollen in deren Funktionsweise beschrieben werden.
  Es soll ein Gesamtbild entstehen, sodass man erkennen kann, wo kommen die Daten her, wie werden sie verarbeitet, was entsteht E2E.

  ## &nbsp;&nbsp;&nbsp; 3.2 Data Acquistion und Data Understanding

  In diesem Kapitel sollen die verwendeten Daten und dessen Struktur dargelegt werden. Dies kann dabei sowohl die Input Queries als auch die API Daten umfassen.

  ## &nbsp;&nbsp;&nbsp; 3.3 Modeling

  In diesem Kapitel sollen die einzelnen Bausteile der technsichen Lösung erläutert werden im Detail.
  Anschließend sollen verschiedene Implementierungsansätze abgewogen werden, die während der Implementierung erwogen wurden: verschiedene LLMs, Neo4J, qdrant, geofox api.
  Zuletzt soll die technische Lösung evalusiert werden. Die Testing Schritte sollen dabei technisch in deren Implementierung dargelegt sowie deren Ergebnisse interpretiert werden.
  
  ### &nbsp;&nbsp;&nbsp; 3.3.1 Vektorisierung der Input-Queries
  ### &nbsp;&nbsp;&nbsp; 3.3.2 Formulierung und Implementierung der Datenabfrage
  ### &nbsp;&nbsp;&nbsp; 3.3.3 Kontextualisierung des Input Queries
  ### &nbsp;&nbsp;&nbsp; 3.3.4 Visualisierung der Benutzerinteraktionen
  ### &nbsp;&nbsp;&nbsp; 3.3.5 Abwägung verschiedeneder Large Language Modelle
  ### &nbsp;&nbsp;&nbsp; 3.3.6 Abwägung der Datenquellen
  ### &nbsp;&nbsp;&nbsp; 3.3.6 Evaluation der technischen Lösung
  
# 4 Evaluation der technischen Lösung
  ## &nbsp;&nbsp;&nbsp; 4.1 Kritische Bewertung
  ## &nbsp;&nbsp;&nbsp; 4.2 Identifizierte Limitationen
 In diesem Kapitel soll die technische Lösung hinsichtlich der Problemstellung kritisch bewertet werden. Wird das Problem gelöst? Ist die Problemlösung angemessen? Welche Lösungen haben sich als ideal herausgestellt und warum?

# 5 Consulting der HVV
  ## &nbsp;&nbsp;&nbsp; 5.1 Aktuelle Situation
  ## &nbsp;&nbsp;&nbsp; 5.2 Zieldefinition
  ## &nbsp;&nbsp;&nbsp; 5.3 Lösungskonzeption
  ## &nbsp;&nbsp;&nbsp; 5.4 Zeit- und Kostenplanung
  ## &nbsp;&nbsp;&nbsp; 5.4 Zusammenfassung der Optionen
 In diesem Kapitel soll der Consulting Teil der Arbeit formuliert werden. Wie ist die aktuelle Situation bei der HVV und warum soll hier überhaupt etwas angepasst oder entwickelt werden? Wie ist das Ziel zu definieren und wann/womit wird es erreicht (Metriken)? Wie kann eine konkrete Lösung aussehen und gibt es hier eine günstigere/schlankere und eine umfassendere/kostenintensivere Lösung? Wie sieht eine Zeit- und Kostenplanung konkret für die Lösung/en aus (Vollintegration mit Backend und Frontend)? Abschließend eine Zusammenfassung der Keyfacts sowie der potenziellen Optionen zur Zielerreichung.

# 6 Zusammenfassung und Ausblick
  ## &nbsp;&nbsp;&nbsp; 6.1 Zusammenfassung
  ## &nbsp;&nbsp;&nbsp; 6.2 Ausblick

 Zuletzt soll die technische Implementierung zusammengefasst werden. Was hat funktioniert, was nicht. Referenz auf die Methodik, den theoretischen Hintgerund/aktueller Forschungsstand sowie die Zielstellung und Problemstellung der Arbeit ist sinvoll.
 Im Ausblick sollen die möglichen nächsten Schritte dargelegt werden. Was kann als nächstes folgen, was sollte man noch evaluieren, testen, implementieren, welche themen aus dem aktuellen forschungsstand sollen noch aufgegriffen werden.
