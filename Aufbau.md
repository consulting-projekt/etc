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
  
# 2 Theoretischer Hindergrund von Retrieval Augmented Generations

  ## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2.1 Funktionalität von RAGs
  ## &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2.2 Vorteile von RAGs

  Das Kapitel des theoretischen Hintergrunds hat 2 Funktionen.
  Konrket soll die FUnktionsweise und die Relevanz von RAGs dargelegt werden als Theorieblock.
  Im 2. Teil jedes Kapitels sollen aktuelle Papers von RAGs und deren Anwendung referenziert werden.
  Damit soll aufgezeigt werden, wie andere bereits diese Problemstellung mittels RAG gelöst haben und welche Vorteile sie aufgezeigt haben (sowie auch Limitationen)

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
  
# 4 Evaluation und Consulting zur technischen Lösung
  ## &nbsp;&nbsp;&nbsp; 4.1 Implementierte Vorteile
  ## &nbsp;&nbsp;&nbsp; 4.2 Aufwandsschätzungen
  ## &nbsp;&nbsp;&nbsp; 4.3 Limitationen

 In diesem Kapitel soll der Consulting Teil der Arbeit formuliert werden. Welcher Vorteil bietet die technische Lösung dem Kunden und welche Aufwände sind dabei verbunden. 
 Welches Problem des Kunden wird dabei für HVV gelöst. Aber auch: welche Limitationen liegen vor.

# 5 Zusammenfassung und Ausblick
  ## &nbsp;&nbsp;&nbsp; 5.1 Zusammenfassung
  ## &nbsp;&nbsp;&nbsp; 5.2 Ausblick

 Zuletzt soll die technische Implementierung zusammengefasst werden. Was hat funktioniert, was nicht. Referenz auf die Methodik, den theoretischen Hintgerund/aktueller Forschungsstand sowie die Zielstellung und Problemstellung der Arbeit ist sinvoll.
 Im Ausblick sollen die möglichen nächsten Schritte dargelegt werden. Was kann als nächstes folgen, was sollte man noch evaluieren, testen, implementieren, welche themen aus dem aktuellen forschungsstand sollen noch aufgegriffen werden.
