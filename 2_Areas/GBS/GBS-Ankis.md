#gbs
1.1. Was sind Rechensysteme?
;; 
Rechensysteme sind offene, dynamische, technische Systeme. 


1.2. Was sind die Fähigkeiten des Rechensystems? 
;;
Speicherung und Verarbeitung von 
Information sowie der Fähigkeit zur Kommunikation. 


1.3. Wie ist ein Offenes System aufgebaut? 
;; 
Ein Offenes System besteht aus Komponenten. Verbindungen zwischen Komponenten beschreiben Abhängigkeiten.
Es besizt Schnittstellen zur externen Einwirkung auf das System. 


1.4. Was ist die Aufgabe von Schnitstellen und wie sind die aufgebaut?
;; 
Schnittstellen ermöglichen verschiedene Sichten auf ein System.
- Von außen: **Black-Box-Sicht**.
- Von innen: **White-Box-Sicht**. 

1.5. Was zeigen Black bzw. White Box Sichten?
;;
- **Black-Box-Sicht:** Zusammenfassungen von Komponenten und Abgrenzungen liefern Einheiten, für die Black-Box-Sichten möglich sind.
- **White-Box-Sicht:** Rekursive Aufteilung in Komponenten bzw. Sub-Komponenten liefern verfeinerte White-Box-Sichten.

1.6. Erklär was ist ein dynamisches System und wie ist die aufgebaut?
;;
- Eine Reihe von Eigenschaften beschreiben den **Zustand des Systems** - zu einem Betrachtungszeitpunkt. Diese Eigenschaften verändern sich über die Zeit.
- Eigenschaftsänderungen sind **Zustandsänderungen**.
- Eine Folge von Zuständen bzw. Zustandsänderungen beschreibt das **Systemverhalten.**
- Diese Fähigkeit zur Zustandsänderung erhält ein Rechensystem durch **aktive**(z.B. CPU) und **passive** Komponenten (z.B. Arbeitsspeicher).
- Aktive Komponenten führen Aktionen aus, die Zustandsveränderungen bewirken und passiven Komponenten sind Hilfsmittel für diese Aktionen.

1.7. Wie ist ein Rechensystem realisiert? 
;;
Ein Rechensystem ist mit hardware und softwaretechnischen Mittel realisiert.

1.8 .Was ist ein Betriebssystem?
;;
- Das Betriebssystem ist selbst ein **Programm**, das die Ausführung von System oder Anwendungsprogrammen **steuert** und **überwacht** und für die Anwendungsprogramme eine **Schnitstelle** zu den Hardware Komponenten bereitstellt.
- Schnittstellen sind z.B. Operationen wie `read` und `write` für den Zugriff auf gespeicherte Daten.


1.9. Was sind die Aufgaben eines Betriebssystems? 
;;
- Abstraktion und Management von Ressourcen.

1.10. Was ist Abstraktion bezüglich BS, geben sie ein Beispiel dafür?
;;
- Vereinfachung, Bereitstellung von abstrakten Konzepten und gemeinsamen Schnittstellen, z.B. Dateien.
- • Lösung: Betriebssystem definiert einheitliche Operationen (Schnittstelle), z.B. read, write.
- Programmierer nutzt diese Operationen
- Betriebssystem setzt diese auf die Geräte-spezifischen Befehle um 
	- unter Verwendung eines gerätespezifischen Treibers, der die Details des Geräts versteht

1.11. Was bedeutet Management von Ressourcen bezüglich BS, geben sie ein Beispiel dafür?
;;
- Steuern und Kontrollieren der Programmausführung 
- Beispiel:  Kontrolle der CPU-Nutzung: welches Programm darf wie lange ohne Unterbrechung die CPU nutzen 
- Strategische Entscheidungen 
- Priorisierung: Wer hat Vorrang? Fairness?
- Agil, adaptiv: Wie geht man mit spontanen Anforderungen um? 
- Operative Entscheidungen 
- Einem Programm die CPU zu einem bestimmten Zeitpunkt zuweisen bzw. wegnehmen


1.12. Was sind die Faktoren für die Entwicklung von BS?
;;
**1.Fortschritte der Hardwaretechnologie**, ein gutes Preis-Leistungs-Verhältnis wi z.b große Festplattenspeicher zu geringen Preisen.
- Anforderungen an das Betriebssystem: u.a. 
- Schnelle Zugriffe auf gespeicherte Daten ermöglichen, 
- Unterstützung von Parallelverarbeitung: viele Programme gleichzeitig im Speicher
**2.Übergang von rein numerischer Berechnung zur allgemeinen Informationsverarbeitung.**
- Interaktive Verarbeitung, Graphische Datenverarbeitung, Multimedia 
- Anforderungen an das Betriebssystem: u.a. 
- Grafischer Nutzeroberflächen: Nutzung auch durch Nicht-Spezialisten 
- Realzeit-Unterstützung, z.B. bei Verarbeitung von Videos
**3. Neue Anwendungsbereiche und Digitalisierung**
- • Auslagerung von Diensten und Datenspeicherung an externe Anbieter (im Gegensatz zum eigenständigen Betrieb)
- Auslagerung des Rechenzentrums bzw. der Server 
- Vernetzung von physischen mit digitalen Komponenten 
- z.B. Energie-Bereich, Auto 
- Einbetten von IT in Objekte des täglichen Lebens 
- z.B. Internet of Things (IoT), z.B. smart Home 
- Anforderungen an das Betriebssystem: u.a. 
- Cloud-Computing, Virtualisierung und Containerisierung (Docker etc.) 
- Eingebettete Betriebssysteme: u.a. ohne Nutzerschnittstellen

1.13. Was sind die Betriebsarten?
;;
- Stapelverarbeitung (batch processing)
- Transaktionsbetrieb (transaction system)
- Dialogbetrieb (time sharing)
- Echtzeitbetrieb (real time system)

1.14. Erklär die Betriebsarten.
;;
- Stapelverarbeitung: 
	- Das Programm wird vor dem Start komplett definiert und geschlossen ausgeführt. 
	- Nutzer-Interaktion ist nicht vorgesehen
- Transaktionsbetrieb (transaction system):
	- Auch bekannt aus dem Bereich der Datenbanken 
	- ACID-Kriterien (Atomarität, Konsistenz, Isolation, Dauerhaftigkeit)
- Dialogbetrieb (time sharing) 
	- Interaktion zwischen dem Nutzer und dem Betriebssystem 
	- Erfordert (G)UIs
- Echtzeitbetrieb (real time system) 
	- Harte Echtzeit (hard deadlines) – Reaktionszeit darf nicht überschritten werden 
	- Weiche Echtzeit (soft deadlines) – Gewisse Toleranzen sind erlaubt.
	- Einsatzbeispiele: Robotik (hart), Multimedia-Anwendungen (weich)

1.15. Was sind die Zweck und ziele von BS?
;;
**Zweck:** General Purpose vs Special Purpose
**Ziele:** Hohe Auslastung, Kurze Antwortzeiten, Geringer Energieverbrauch.

1.16. Was sind die Typen von Betriebssystemen?
- Server-Betriebssysteme wie SuperMUC, MPI oder dedizierte BS für Datenzentren.
- Server- und Desktop-Betriebssysteme wie Linux, Windows, MacOS.
- Mobile BS wie Android und iOS.
- Eingebettete Betriebssysteme wie QNX, L4(embedded), PikeOS, TinyOS, RTOS, RIOT. Die einfach Echtzeit-fähig sind.

1.17. Wie sind die Ressourcen klassifiziert?
;;
- **Anzahl der Nutzungen** 
	- Einmal benutzbar
	- Wiederholt benutzbar
- **Parallelität**
	- Parallel benutzbar (uneingeschränkt) z.b (Dateisystem) 
	- Exklusiv benutzbar (Drucker)
	- Beschränkt parallel benutzbar
- **Dauerhaftigkeit** 
	- Unterbrechbar (CPU, Speicher) 
	- Ununterbrechbar (DVD-ROM)
- **Zentrale Ressourcen**
	- Prozessoren (CPUs, Rechnerkerne) 
	- Arbeitsspeicher
- **Periphere Ressourcen**
	- Kommunikationseinheiten 
	- Speichereinheiten
	
1.18. Was ist ein Prozess?
;;
- Ein Prozess ist ein Programm in Ausführung.

1.19. Unterschied zwischen Prozess und Programm
;;
- Programm ist eine passive Einheit, Prozess eine aktive Einheit
- Ein Programm kann in mehreren Prozessen (Instanzen des Programms) ausgeführt werden: z.B. zwei Instanzen von Microsoft Word 
- Ein System besteht aus einer Menge von Prozessen

1.20. Was braucht ein Prozess?
;;
- Ressourcen um seine Aufgabe zu erfüllen.

1.21. Was ist die Beziehung zwischen CPU und Prozess?
;;
- Konzeptuell besitzt jeder Prozess seine eigene CPU 
- In Realität muss sich der Prozess die CPU mit den anderen Prozessen teilen: dies ist die Prozessorverwaltungsaufgabe des Betriebssystems

1.22. Was besitzt jeder Prozess?
;;
- Jeder Prozess besitzt einen eigenen Prozessadressraum.
1.23. Was ist ein virtueller Adressraum?
;;
- Virtueller Adressraum ist eine Abstraktion des physischen Speichers 
- Enthält Programmcode und Daten

1.24. Wie sind diese Adressräume in Hardware?
;;
- Adressräume verschiedener Prozesse sind von der Hardware gegeneinander abgeschottet

1.25. Wie s


