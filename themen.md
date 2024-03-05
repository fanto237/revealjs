# Bereich 1: Architektur


## 1. Beurteilung von Datenbank-Replikationen im Rahmen eines Fail Overs Szenario

`Ansprechpartner: Paul Ziemann`

Zur Erhöhung der Datenverfügbarkeit und Datensicherung ist die Replikation von Datenbanken ein
gängiges Mittel. Bei der Verbesserung der Ausfallsicherheit eines Portales ist die Einrichtung einer unabhängigen Failover-Instanz mit eigener Datenbank ein Teilaspekt. Die Synchronisierung der Live- und Failover-Datenbanken muss hierbei zuverlässig funktionieren. Um dies sicherzustellen, sollen verschiedene Möglichkeiten der Datenbank-Replikation (täglicher Dump und Restore, Replikation mit Slony, pgpool oder weiteren Tools, Replikation auf Datenträgerebene, …) verglichen und bewertet werden. Der Vergleich soll unter anderem hinsichtlich Einrichtungs-/Konfigurationsaufwand, Ausfallsicherheit, Performance und Eignung erfolgen. Abschließend soll ein Vorschlag für eine Umsetzung basierend auf dem Vergleich erfolgen

# Bereich 2: Cloud

## 2. Kubernetes Architektur
`Ansprechpartner: Andreas Hartmann`

Im Rahmen der Arbeit sind die von Kubernetes adressierten Konzepte zum Betrieb und Deployment von verteilten Systemen darzustellen und deren Nutzung prototpisch anzuwenden. Siehe hierzu auch https://leanpub.com/k8spatterns.

Technologien:
- Kubernetes
- Spring Cloud

# Bereich 3: Continous Delivery

## 3. Ablösung einer bestehenden Provisionierungslösung durch Ansible

`Ansprechpartner: Jens Kostka`

Im Zeitalter von dynamisch skalierenden Infrastrukturen sind sich auf Knopfdruck konfigurierende Server eine unabdingbare Voraussetzung. Dies wurde bereits durch das Provisionierungstool „Chef" (https://learn.chef.io/#/) für eine Cloud-basierenden Lösung der zentralen Continuous-Integration–Umgebung der adesso AG realisiert.  Im Rahmen einer Abschlussarbeit soll die veraltete Lösung durch neue Anforderungen erweitert und zu Ansible, einem neueren (besseren) Provisionierungstool, hin migriert werden.

Technologien:
- Jenkins
- Docker
- Unix (CentOS)
- Ansible
- Chef


## 4. Umgang mit Datenbank in einem Continuous Delivery Umfeld

`Ansprechpartner: Sebastian Laag`

**Themeneinführung:**
Mit Continuous Delivery (CD) strebt man an, Anwendungen möglichst schnell und automatisiert in Produktion zu bringen. Techniken wie das automatisierte Testen, Continuous Integration und Continuous Deployment ermöglichen einen schnellen Entwicklungsprozess. Dieser ermöglicht einen ständigen, zuverlässigen und wiederholbaren Auslieferungsprozess, sodass Erweiterungen und Fehlerbehebungen einer Anwendung mit minimalem Risiko und minimalem manuellen Overhead an den Kunden ausgeliefert werden können. Im Rahmen dieser Arbeit soll untersucht werden, wie man in diesem Kontext mit Datenbank umgeht. Dazu zählen Punkte wie die automatisierte Installation der Datenbanken mit Werkzeugen wie Chef und die Änderungen von Datenbank-Schemata mit Rails Migrations, Liquibase, Flyway oder anderen Werkzeugen. Liquibase und Flyway sind dabei interessant, weil sie aus dem Java-Umfeld kommen. Darüber hinaus kann man Datenbank-Imports und -Exports nutzen. Mögliches Beispiel kann der adesso Profiler sein.
Warum spannend:
Continuous Delivery verspricht den Entwicklungsprozess zu beschleunigen, sodass der Kunde schnellstmöglich den aktuellen Entwicklungsstand eines Projektes nutzen kann. Dabei sind vor allem die zügige Auslieferung von Bugfixes und Erweiterungen interessant. Da in der Praxis häufig die Datenbank als problematisch angesehen wird, soll dies untersucht werden. Hier ist vor allem der Umgang mit Versionierung und Refactorings im Rahmen von Datenbankänderungen spannend.
Herausforderung:
- Wie können Datenbankänderungen im Rahmen von CD verarbeitet werden
- Welche Produkte im Java-Umfeld können eingesetzt werden, um Datenbankänderungen in die Produktion einzuspielen
- Wie können Datenbanken automatisiert und zuverlässig installiert bzw. aktualisiert werden
Weitere Möglichkeiten:
- Nutzung der Erkenntnisse zur Verwendung in adesso Projekten zur Verbesserung der Softwarequalität und Beschleunigung der Auslieferung an den Kunden
Literatureinstieg:
- Jez Humble & David Farley. Continuous delivery: reliable software releases through build, test, and deployment automation. ISBN 978-0-321-60191-9.
- http://www.opscode.com/chef/
- http://guides.rubyonrails.org/migrations.html
- http://www.liquibase.org/
- http://code.google.com/p/flyway/

Technologien:
- Chef
- Rails Migrations
- Liquibase
- Flyway

# Internet of things
## 5. Entwurf und Implementierung einer IoT Software Architektur auf Basis der Bosch IoT Cloud


`Ansprechpartner: nicht angegeben`

Die Bosch IoT Cloud stellt für die speziellen Anforderungen von IoT-Entwicklern verschiedene Cloud-Services zur Verfügung. Es sollen IoT-Projekte und IoT-Szenarien architektonisch entworfen und realisiert werden, die die Schichten IaaS (Infrastruktur as a Service), Paas (Platform as a Service) und SaaS (Software as a Service) der Bosch IoT Cloud nutzen. Basierend auf unterschiedlichen IoT Devices, Cloud Services, IoT Protokollen und Ausgabegeräten können verschiedene Implementierung je nach Schwerpunkt des Studiums durchgeführt werden. Ein Vergleich der Bosch IoT Cloud mit anderen verfügbaren Cloud Anbietern soll ebenfalls im Rahmen der Master Arbeit erfolgen.

Technologien:
- Bosch IoT Cloud
- Micro Services
- API Design
- Cloud Protokolle
- Cloud Technologien
- Performance
- IT Sicherheit u. Datenschutz
- IAM
- Big Data
- UX
- Mobile Divices
- Smart Home
- Automated Driving/Connected Cars
