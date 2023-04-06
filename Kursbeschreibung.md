# Concurrency Oriented Programming (von Daniel Kirch)

Wir schreiben das Jahr 1986. Joe Armstrong und sein Team bei der Firma Ericsson stehen vor der schwierigen Herausforderung, eine geeignete Programmiersprache für die Entwicklung von Telefonvermittlungsservern zu finden. Die hohen Anforderungen an diese Server beinhalten unter anderem:

- Parallelität: sie müssen in der Lage sein, eine große Anzahl Anfragen gleichzeitig zu bearbeiten
- Echtzeit: Anfragen müssen innerhalb weniger Sekunden bearbeitet werden
- hohe Verfügbarkeit: Server müssen über mehrere Jahre in Betrieb bleiben mit minimalen Ausfallzeiten
- Fehlertoleranz: sie müssen sowohl mit Softwarefehlern als auch Hardware-Ausfällen umgehen können
- Hot Swapping: Wartung und Systemupdates werden ohne Unterbrechung des Betriebs durchgeführt

Bald schon kommen Armstrong und seine Kollegen zur Erkenntnis, dass keine der damals existierenden Programmiersprachen gut geeignet ist diese Anforderungen zu erfüllen und die Idee für Erlang (kurz für Ericsson language) ist geboren. Doch auch eine neue Sprache allein ist nicht ausreichend und deshalb ist Erlang selbst untrennbar verbunden mit der Laufzeitumgebung ErlangVM und einer Sammlung von Werkzeugen und Bibliotheken namens OTP (kurz für Open Telecom Platform).

Das Paradigma von Erlang/OTP ist Concurrency Oriented Programming ("Alles ist ein Prozess."), das bedeutet:

- das Starten und Beenden von Prozessen ist einfach und kostengünstig
- Prozesse sind strikt isoliert und können nur durch asynchrone Nachrichten kommunizieren
- die Behandlung von Fehlern erfolgt nicht lokal

Die Einführung von Erlang/OTP ist sehr erfolgreich und 1998 erreicht das Erlang-basierte System AXD301 eine Verfügbarkeit von 99,9999999% bei einem Test der British Telecom (etwa 3-4 Neunen besser als andere Systeme zu der Zeit). Kurz darauf wird das bis dahin proprietäre Erlang open source, aber bleibt dennoch lange Zeit eine Nischentechnologie.

Es dauert viele Jahre, bis im Jahr 2011 José Valim die Grundideen von Erlang wieder aufgreift und auf moderne Webserver anwendet, die inzwischen sehr ähnlichen Anforderungen genügen müssen. Das Ergebnis ist die Sprache Elixir und das Phoenix Framework, die sehr eng mit Erlang verwandt sind und ebenfalls die ErlangVM als Laufzeitumgebung nutzen. Aufgrund einfacher Erlernbarkeit, hoher Zuverlässigkeit und guter Skalierbarkeit erfreuen sich Elixir und Phoenix heute einer stetig wachsenden Community.

In diesem Kurs wollen wir uns gemeinsam mit der Sprache Elixir und den Konzepten von Concurrency Oriented Programming auseinandersetzen. Dazu gehört neben einigen theoretischen Inhalten natürlich auch eine gehörige Portion Praxis in Form von Programmieren. Es ist der kurzfristigen Planung und nicht zuletzt der Faulheit des Kursleiters geschuldet, dass er nicht schaffen wird alle Inhalte ausführlich vorzubereiten, d.h. es wäre schön, wenn du auch ein gewisses Maß an Eigenmotivation (z.B. Ideen für Programmierprojekte) mitbringst. Voraussetzungen für den Kurs sind etwas praktische Erfahrung im Programmieren (C/C++, Java, Python o.ä.) und grundlegende Kenntnisse von Programmierparadigmen (imperativ, objektorientiert, funktional usw.).

Daniel Kirch programmiert seit über 4 Jahren beruflich mit Elixir und liebt diese Sprache nicht zuletzt wegen ihrer einfachen Syntax.
