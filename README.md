## Outlook CalDav Synchronizer ##

Outlook-Plugin, welches Ereignisse, Aufgaben und Kontakte zwischen Outlook und Google, SOGo, Horde oder einem anderen CalDAV- oder CardDAV-Server synchronisiert. Unterstützte Outlook-Versionen sind 2019, 2016, 2013, 2010 und 2007.

### Projekt-Homepage ###
[http://caldavsynchronizer.org](http://caldavsynchronizer.org)

### Lizenz ###
[Affero GNU Public License](https://www.gnu.org/licenses/agpl-3.0.html)

### Autoren ###

- [Gerhard Zehetbauer](https://sourceforge.net/u/nertsch/profile/)
- [Alexander Nimmervoll](https://sourceforge.net/u/nimm/profile/)

Dieses Projekt wurde 2015 zunächst als Masterarbeit an der [Technischen Universität Wien](http://www.technikum-wien.at) im Studiengang Software Engineering gestartet und wird jetzt von Generalize-IT Solutions OG, FN 466962i, 1210 Wien, Österreich betrieben.

Outlook CalDav Synchronizer ist eine freie und Open-Source-Software (FOSS). Sie können das Projekt jedoch unterstützen, indem Sie bei Sourceforge oder direkt bei PayPal spenden.

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=PWA2N6P5WRSJJ&lc=US).

### Zusammenarbeit mit Nextcloud ###

Neue Zusammenarbeit mit Nextcloud, siehe [https://nextcloud.com/blog/nextcloud-offers-caldav-synchronizer-for-outlook-users/](https://nextcloud.com/blog/nextcloud-offers-caldav-synchronizer-for-outlook-users/).

Für eine mögliche Unternehmensunterstützung (Enterprise-Kunden) kontaktieren Sie uns bitte [hier](https://caldavsynchronizer.org/enterprise/contact/)!

### Empfohlener Android DAV-Client ###

Wir arbeiten eng zusammen und testen die Interopabilität mit DAVx⁵ für Android. Siehe [https://www.davx5.com](https://www.davx5.com), wir können es wirklich weiterempfehlen! Zusammen mit DAVx⁵ haben wir jetzt experimentelle Unterstützung für die Farbgebung nach Ereignissen eingebaut, indem die Farbe der Outlook-Kategorie dem Attribut COLOR des Ereignisses zugeordnet wird.

### Getestete CalDAV-Server ###

- Baïkal
- Cozy Cloud
- cPanel
- Cyrus Imap 2.5
- DAViCal
- EGroupware
- FastMail
- Fruux
- GMX
- Google Calendar
- Group-Office
- Horde Kronolith
- iCloud
- Kolab
- Landmarks
- Mac OS X Server
- mail.ru
- mailbox.org
- Nextcloud
- One.com
- Open-Xchange
- Owncloud
- Posteo
- Radicale
- SabreDAV
- SmarterMail
- SOGo
- Synology DSM
- Tine 2.0
- Yahoo
- Yandex
- Zimbra 8.5
- Zoho Calendar

### Features ###

- Open Source AGPL, das einzige kostenlose Outlook CalDav-Plugin
- Zwei-Wege-Synchronisation
- Unterstützung für Lokalisierung
- SSL / TLS-Unterstützung, Unterstützung für selbstsignierte Zertifikate und Authentifizierung von Clientzertifikaten
- Manuelle Proxy-Konfigurationsunterstützung für NTLM oder Basic-Auth-Proxys
- Automatische Erkennung von Kalendern und Adressbüchern
- Konfigurierbarer Synchronisationsbereich
- Synchronisieren Sie mehrere Kalender pro Profil
- Synchronisieren Sie Erinnerungen, Kategorien, Wiederholungen mit Ausnahmen, Wichtigkeit, Transparenz
- Synchronisieren Sie Organizer und Teilnehmer und den eigenen Antwortstatus
- Task-Unterstützung
- Google native Kontakte-API-Unterstützung mit Zuordnung von Google-Kontaktgruppen zu Outlook-Kategorien.
- Unterstützung für Google-Tasklisten (Synchronisierung über Google Task Api mit Outlook-Aufgabenordnern)
- CardDAV-Unterstützung zum Synchronisieren von Kontakten
- Ordnen Sie Outlook-Verteilungslisten Kontaktgruppen im SOGo VLIST-, KIND: GROUP- oder iCloud-Gruppenformat zu
- Zeitgesteuerte Synchronisation
- Änderungsgesteuerte Synchronisation
- Manuell ausgelöste Synchronisation
- Unterstützung für die Synchronisierung der WebDAV-Sammlung (RFC 6578)
- Kategoriefilterung (CalDAV-Kalender / -Tasks mit Outlook-Kategorien synchronisieren)
- Ordnen Sie die CalDAV-Serverfarben den Outlook-Kategorienfarben zu
- Zeigt Berichte über die letzten Synchronisierungsläufe und den Status an
- Taskleistensymbol mit Benachrichtigungen
- Massenerstellung mehrerer Profile
- Verwenden Sie die Servereinstellungen aus dem Outlook IMAP / POP3-Kontoprofil
- Ordnen Sie die Windows- den Standard-IANA / Olson-Zeitzonen zu
- Konfigurierbare Zuordnung von benutzerdefinierten Eigenschaften von Outlook
- Erstellen Sie DAV-Serverkalender / Adressbücher mit MKCOL
- Zuordnen von Outlook-formatierten RTF-Objekten zu HTML-Beschreibungen über das Attribut X-ALT-DESC
- Unterstützung für RFC7986-Farbverarbeitung für Ereignisse, Zuordnung der Farbe der Outlook-Kategorie zum Attribut COLOR

### Verwendete Bibliotheken ###

-  [DDay.iCal](http://www.ddaysoftware.com/Pages/Projects/DDay.iCal/)
-  [Apache log4net](https://logging.apache.org/log4net/)
-  [Thought.vCard](http://nugetmusthaves.com/Package/Thought.vCards)
-  [NodaTime](http://nodatime.org/)
-  [ColorMine](https://www.nuget.org/packages/ColorMine/)

### Installationsanweisungen ###

**WARNUNG**: Ab Release 3.0.0 ist .NET Framework 4.6.1 die Mindestanforderung.

Laden Sie die `OutlookCalDavSynchronizer-<Version>.zip`-Datei herunter, entpacken Sie sie in ein beliebiges Verzeichnis und starten Sie die Datei setup.exe. Sie können den Standardinstallationspfad ändern, aber Sie müssen ein Verzeichnis auf dem `C:\` -Laufwerk verwenden. Wenn sich das Installationsprogramm über die fehlenden Visual Studio 2010-Tools für Office Runtime beschwert, installieren Sie es manuell über [Microsoft Download-Link](https://www.microsoft.com/en-us/download/details.aspx?id=56961).
Sie sollten auch manuell auf die neuesten Visual Studio 2010 Tools für Office Runtime (Version 10.0.60828) aktualisieren, wenn Sie eine ältere Version installiert haben, da einige COMExceptions behoben wurden.

Ab Version 2.9.0 ist das Standardinstallationsverzeichnis `ProgramFilesDir\CalDavSynchronizer\` und das Installationsprogramm speichert das Verzeichnis für die nächsten Updates. Die Installationsoption für die Installation von Jeder anstelle des aktuellen Benutzers funktioniert jetzt für Outlook 2010 und höher, wenn Sie das Add-In für alle Benutzer auf dem aktuellen Computer installieren möchten. Für Outlook 2007 können Sie das Add-In nur für den aktuellen Benutzer installieren.

Es wird empfohlen, auf das neueste .NET-Framework zu aktualisieren. Die minimal erforderliche Version ist .NET 4.6.1, die unter Windows XP nicht unterstützt wird. Wenn Sie Outlook CalDav Synchronizer für Windows XP benötigen, können Sie von [hier](https://sourceforge.net/projects/outlookcaldavsynchronizerxp/) einen Backport auf .Net 4.0 herunterladen, danke, [Salvatore Isaja](https://sourceforge.net/u/salvois/profile/) für die großartige Arbeit!

### Änderungsprotokoll ###

#### 3.5.0 ####
- Erschienen am 26.02.2019
- Neue Features
	- Hinzufügen des Profiltyps für EGroupware.
	- Hinzufügen des Profiltyps für FastMail.
	- Mapping der formatierten Beschreibung aus dem Google Kalender.
	- Ausführen des Serverzugriffs für die Kontaktsynchronisierung im Hintergrund.
	- Entfernen der allgemeinen Option "Ungültige Einstellungen korrigieren".
- Fehlerbehebungen
	- Verbesserung der GetOwner und überprüfen der Organiser-Eigenschaft, wenn die Besitzereigenschaft nicht gefunden wurde (Workaround für OpenX-change).
	- Verbessertes SOGo-Profil und Hinzufügen von VLIST-Verteilerlisten zu den Standardprofileinstellungen.
	- Verbesserte Massenprofilerstellung und Einstellung des korrekten Synchronisationsmodus sowie Aktualisierung der E-Mail- und Planungseinstellungen des Servers.
	- Für RECURRENCE-ID wurde derselbe Werttyp und die gleiche Tzid wie für DTSTART verwendet, um mit RFC 5545 kompatibel zu sein.
	- Die Erzeugung von originalOutlookDatesWithExceptions wurde korrigiert. Verwendet immer die Zielzeitzone.

#### 3.4.0 ####
- Erschienen am 13.01.2019
- Neue Features
	- Unterstützung für Kalender-Proxy für automatische Erkennung (Kalender-Proxy-Lesezugriff, Kalender-Proxy-Schreibzugriff), Feature-Request 103 hinzugefügt.
	- Zugriffsrechte in der Auswahlauswahl für die automatische Erkennung anzeigen.
	- Option hinzugefügt, um den Organiser für die Serveridentität festzulegen.
	- Erkennung der Server-E-Mail-Adresse wurde hinzugefügt und als Standard für freigegebene schreibbare Kalender festgelegt.
	- Verbesserte Tooltips in SelectResourceForm und Anzeige von Ressourcen-URI und Farbwerten als Tooltip.
	- Swisscom-Profileinrichtung wurde aktualisiert.
	- Konfigurationsoption für die Kontaktzuordnung hinzugefügt, um Jubiläumsdaten zu Kontakten zuzuordnen. Unterstützt die Eigenschaften ANNIVERSARY, X-ANNIVERSARY und X-MS-ANNIVERSARY und schreibt ANNIVERSARY.
	- Option hinzugefügt, um Aufgabenerinnerungen als absoluten DATE-TIME-Wert zuzuordnen, was für IOS erforderlich ist, Feature-Request 105.
	- Brasilianisches Portugiesisch-Übersetzungen hinzugefügt. Danke an Flávio Zarur Lucarelli!
- Fehlerbehebungen
	- Leere PHOTO-Eigenschaften in vCards ignorieren.
	- Wenn in QueryOutlookFolderByGetTableStrategy keine Langzeit-Wert verfügbar ist, greife auf die kurzfristige ENTRYID zurück, um ArgumentException in row.BinaryToString() zu vermeiden.
	- Fehler beim Löschen von Entitäten protokollieren.
	- Fehler in GetCurrentUserPrincipalUrl behoben. Wählt nur den Href-Knoten aus.
	- Fehler in den Aufgabenerinnerungen relativ zum DUE-Datum behoben.
	- Fehler in der Benutzeroberfläche und Übersetzungen behoben.

#### 3.3.0 ####
- Erschienen am 09.12.2018
- Neue Features
	- Open-Xchange-Profiltyp hinzugefügt.
	- ICloud Calendar-Profiltyp hinzugefügt.
- Fehlerbehebungen
	- Ignorieren von Alarmen, bei denen sich ACTION von DISPLAY unterscheidet, um E-Mail-Alarme nicht als Outlook-Erinnerungen zu synchronisieren, Ticket # 978.
	- Erzwingen, dass der Organiser der Ausnahme mit dem Ereignisorganisator identisch ist, um SameOrganizerForAllComponentsException zu vermeiden. Github-Issues 240 und 244.
	- Using-Block in try/catch verschoben, um Fehler mit SaveAndReload von leeren AppointmentItems zu vermeiden.
	- Verbesserte Deserialisierung von SOGo-VLISTs.
	- Begrenzung der CalDav-Ressourcen auf 255 Zeichen.

#### 3.2.1 ####
- Erschienen am 11.09.2018
- Fehlerbehebungen
	- Setzen des Default BusyStatus auf Free für AllDay-Ereignisse, ohne dass TRANSP gesetzt ist, Ticket #951.
	- Setzen des Vergleichs von WebResourceName auf Case-Sensitiv, vermeiden von Problemen mit DavMail-URIs.
	- Fehler in Unit Tests behoben.
	- Verbesserte Integrationstests.
	- Überprüfung der Internetverbindung asynchron, um das Blockieren bei DNS-Problemen zu vermeiden, Ticket #968.

#### 3.2.0 ####
- Erschienen am 17.05.2018
- Neue Features
	- Französische und italienische Übersetzungen hinzugefügt.
	- NuGet-Pakete wurden aktualisiert.
- Fehlerbehebungen
	- Doppelte Kategorien wurden entfernt (Ticket #881).
	- Nicht nur COMExceptions in OutlookUtility-Funktionen abfangen, siehe Issue 229.
	- Tippfehler in deutscher Übersetzung behoben.

#### 3.1.1 ####
- Erschienen am 02.05.2018
- Fehlerbehebungen
	- E-Mail aus Empfänger CN entfernt. Sollte Teilnehmer mit Name (E-Mail) <E-Mail> vermeiden.
	- Escapen des Backslashes, DDay.iCal workaround. Ticket #810, Issue 226.

#### 3.1.0 ####
- Erschienen am 25.03.2018
- Neue Features
	- Zuordnung von tentative zu TRANSP: OPAQUE statt TRANSPARENT, Feature-Request 94.
	- Ereigniszuordnungskonfiguration hinzugefügt, um öffentliche Outlook-Ereignisse der Standardsichtbarkeit statt der öffentlichen zuzuordnen, Feature-Request 98. Festlegen dieser Option als Standard für Google-Profile.
- Fehlerbehebungen
	- Korrektur der Übersetzung für die OL2007-Symbolleiste, Ticket #821.
	- Einige russische und deutsche Übersetzungen wurden aktualisiert.
	- Fehler in Integrationstests behoben.
	- Die Auswahl von Berichten in der Listenansicht wurde korrigiert.
	- Fehler beim Parsen von Berichtsnamen für große Sequenznummern behoben.
	- Ticket 842: Alle Seiten des Google Task Service lesen.
	- Wiederholen ohne Sync-Token, wenn Sync-Token ungültig ist.
	- Die Zuordnung der Wochentags-Wiederholungsregel mit FREQ=DAILY;BYDAY=MO,TU,WE,TH,FR wurde korrigiert, Ticket #847.

#### 3.0.0 ####
- Erschienen am 10.02.2018
- **WARNUNG**: Diese Version ist ein bedeutendes Upgrade und erfordert .NET Framework 4.6.1 als Mindestanforderung. Das automatische Upgrade funktioniert nicht, wenn Sie nur noch .NET Framework 4.5 installiert haben. Installieren und aktualisieren Sie in diesem Fall manuell!

- Neue Features
	- Upgrade auf .NET Framework 4.6.1.
	- Lokalisierungsunterstützung hinzugefügt.
	- Deutsche und russische Übersetzungen hinzugefügt (Weitere folgen und Hilfe erwünscht, kontaktiere uns!)
	- Allgemeine Option zum Umschalten der Sprache der Benutzeroberfläche hinzugefügt (zum Neustart von Outlook ist ein Effekt erforderlich).
	- UI-Neugestaltung für allgemeine Optionen mit WPF TabControl.
	- Verbesserte Erreichbarkeit durch Hinzufügen von Schlüsselwörtern zum Menüband.
	- Profiltyp für Swisscom hinzugefügt.
	- Google API und andere NuGet-Pakete wurden aktualisiert.
	- Sortierung von Synchronisierungsberichten.
- Fehlerbehebungen
	- Viele Tippfehler behoben.
	- Einige Inkonsistenzen der Benutzeroberfläche und der Inhalt, der an Bildschirmprobleme angepasst wurde, wurden behoben.
	- Verbesserte Log-Protokollierung.
	- Verbesserter Profilstatus.
	- Verbesserte Integrationstests.

#### 2.27.0 ####
- Erschienen am 23.12.2017
- Neue Features
	- Kolab-Profil hinzugefügt, Dank an Achim Leitner.
	- Verbessertes Standardverhalten von Schaltflächen.
	- Zuordnung von Outlook OfficeLocation zum ExtendedAddress-Attribut hinzugefügt.
	- Refactoring und Restrukturierung von Profiltypen.
- Fehlerbehebungen
	- Entfernung des Escapings in vCardStandardReader, um Probleme mit einigen Servern zu vermeiden, die vCard NOTES falsch enkodieren, siehe Ticket #741.
	- "Google Maps Organizer und Teilnehmer" ist nun standardmäßig für Google deaktiviert.
	- Zwischenspeichern der Synchronisierungslaufergebnisse, damit ViewModelTransientProfileStatuses beim Öffnen nicht leer ist, siehe Issue 217.
	- Die Behandlung der vCard-ORG-Eigenschaft für die Zuordnung von Organisation und Abteilung zu Outlook-Firmennamen und Abteilungseigenschaften wurde korrigiert.
	- Ausnahme beim Rekonstruieren eines Hauptereignisses behoben, Ticket #777.
	- Verbesserte Log-Protokollierung.
	- Fehler in Integrationstests behoben.

#### 2.26.0 ####
- Erschienen am 15.11.2017
- Neue Features
	- Neues Logo und Anwendungssymbol, Dank an Michael C. Krieter!
	- Unterstützung für absolute Alarme und Alarme in Bezug auf das Ende hinzugefügt und Outlook-Erinnerungen zugeordnet, wenn der Alarm vor dem Beginn des Termins ist (andere werden in Outlook nicht unterstützt), Feature-Request 82.
- Fehlerbehebungen
	- Verbesserte Farb- und ShortcutKey-Zuordnung.
	- Deaktivierung von IsCategoryFilterSticky standardmäßig auch für Ereignisse.
	- Verbesserte Profiltrennung.
	- Erstellt Outlook-Elemente mit dem Standard-ItemType des Ordners, wenn includeCustomMessageClasses aktiviert ist, Feature-Request 80.
	- Fehler in Integrationstests behoben.
	- Festlegen von PercentCompleted, nachdem der Taskstatus in TaskMapper festgelegt wurde, um zu verhindern, dass der Wert verloren geht, wenn der Status nicht in Bearbeitung ist.
	
#### 2.25.0 ####
- Erschienen am 07.10.2017
- Neue Features
	- Optionale WebDAV-Auflistungssynchronisierung (RFC 6578) für Kalender- und Adressbuchauflistungen wurde hinzugefügt. Dies beschleunigt die Erkennung von Serveränderungen erheblich, schließt jedoch die Verwendung des Zeitbereichsfilters aus.
	- EventColor-Category-Zuordnung verbessert. Vorhandene Kategorien werden verwendet, wenn die Farbe übereinstimmt.
- Fehlerbehebungen
	- Verwenden eines offiziellen Zertifikats für die Click-Once-Codesignierung.
	- Verhindern von InvalidCastExceptions in QueryOutlookFolderByGetTableStrategy.
	- Das Statusfenster nicht alive halten, wenn es nicht sichtbar ist.
	- IsCategoryFilterSticky ist standardmäßig deaktiviert und fügt Warnungen hinzu, wenn der Kategoriefilter falsch verwendet wird.
	- Kategorien nicht automatisch wechseln, wenn sich der Kategoriefilter ändert.
	- Nicht nur COMExceptions abfangen, wenn auf Besprechungseinladungen geantwortet wird, Ticket #721.

#### 2.24.0 ####
- Erschienen am 12.09.2017
- Neue Features
	- Unterstützung für RFC7986-Farbbehandlung für Ereignisse hinzugefügt, Zuordnung der Farbe der Outlook-Kategorie zum Attribut COLOR, Feature-Request #76.
	- Profiltyp für mail.de hinzugefügt.
	- Profiltyp für iCloud-Kontakte hinzugefügt.
	- Unterstützung für das Zuordnen von Verteilerlisten zu iCloud-Kontaktgruppen wurde hinzugefügt.
	- Anmeldeinformationen und Proxy aus dem Profil für Weblclient zum Herunterladen von Foto-URLs verwendet, Korrektur der Synchronisierung von Kontaktfotos für iCloud und andere, Feature-Request #71.
	- Allgemeine Option hinzugefügt, um a) Alle Entitätensynchronisierungsberichte zu protokollieren und b) Entitätsnamen in Entitätssynchronisationsberichte aufzunehmen.
-  Fehlerbehebungen
	-  ArgumentNullException in Nodatime-Zeitzonenumwandlungen vermeiden, Ticket #674, #677.
	-  Ignorieren redundanter Entitäten in GetTransformedEntities.
	-  Ungültiger DTSTART in VTIMEZONE behoben, Issue #210.
	-  Einige Code-Bereinigung und Refactoring.

#### 2.23.0 ####
- Erschienen am 13.08.2017
- Neue Features
	- ProfileType für SmarterMail hinzugefügt.
	- REV-Eigenschaft für Vcards aktualisiert, Issue #204.
	- Aktualisierte NuGet-Pakete für Google API auf 1.28.0 und NodaTime auf 2.2.0.
- Fehlerbehebungen
	- Vermeiden von IndexOutOfRangeException beim Analysieren von IMAddress, Ticket #652.

#### 2.22.2 ####
- Erschienen am 12.07.2017
- Fehlerbehebungen
	- Outlook-TimeZone-Ids case-insensitive gemacht, ArgumentException verhindert, Tickets #640, #649.
	- Restliche Entitäten gelöscht, wenn die Erstellung in Outlook fehlschlägt.
	- Vermeiden von InvalidOperationException in vCardStandardReader für unbekannte IM ServiceTypes, Ticket #645.
	- Die chunked-Synchronisierung ist standardmäßig aktiviert.
	
#### 2.22.1 ####
- Erschienen am 22.06.2017
- Fehlerbehebungen
	- InitialMatching für GoogleContacts und GoogleTasks behoben, wenn mehr neue OutlookItems als ChunkSize vorhanden sind. InvalidOperationException vermieden (Kann nicht auf ein gelöschtes Objekt zugreifen!), Ticket #632.
	- Behoben: # 611CALDAV hängt Outlook, #613 CalDav blockiert Outlook, DoEvents-Aufruf in Synchronisierungsfortschrittsleiste entfernt.

#### 2.22.0 ####
- Erschienen am 21.06.2017
- Neue Features
	- Kontaktzuordnungskonfiguration hinzugefügt, um das Standard-IM-Protokoll beim Schreiben von IM-Adressen (Ticket #543) zu wählen.
	- Kontaktzuordnungskonfiguration hinzugefügt, um IM-Adressen als IMPP-Attribut anstelle von X-PROTOCOL zu schreiben, z. X-AIM, Ticket #543.
	- SIP IMServiceType hinzugefügt und X-SIP in vCardStandardReader unterstützt.
	- Synchronisationsprofil für web.de hinzugefügt.
	- Verbessertes EntityMatching für sehr große Kalender (> 5000 Einträge) durch Verwendung von EventServerEntityMatchData anstelle von iCalendar zum Abgleichen.
- Fehlerbehebungen
	- Fehler bei der Google Oauth2-Authentifizierung "Zugriff verweigert" unter Windows7 / 8.1 ohne Administratorrechte behoben.
	- Verbesserte Log-Protokollierung. 

#### 2.21.0 ####
- Erschienen am 30.05.2017
- Neue Features
	- NodaTime wurde auf Version 2 aktualisiert, um die Zeitzonenberechnungen zu verbessern.
	- NuGet-Pakete für Google APIs aktualisiert.
- Fehlerbehebungen
	- Standardmäßig keine Chunk-Synchronisierung aktiviert.

#### 2.20.0 ####
- Erschienen am 29.05.2017
- Neue Features
	- Volle Unterstützung für Chunked-Synchronisation.
- Fehlerbehebungen
	- Vermeiden Sie eine NullReferenceException, wenn TYPE in der Eigenschaft X-SOCIALPROFILE in vCardStandardReader leer ist, Ticket #599.
	- Mapping von Outlook EmailAddress1 konfigurierbar gemacht (wenn es HOME oder WORK zugeordnet werden soll), Ticket 193.
	- Das Lesen des vcard KEY-Attributs wurde korrigiert, wenn das Encoding nicht explizit auf base64 festgelegt ist, Issue 195.

#### 2.19.2 ####
- Erschienen am 13.05.2017
- Fehlerbehebungen
	- Berücksichtigung der Chunk-Größe auch für Google Contact API-Leseaufrufe, Ticket #586.
	- Umstellung der Zuordnung von E-Mail-Adressen und Zuordnung von HOME zu email1 und WORK zu email2, um konsistenter zu sein, Ticket 193.
	- Login-Hinweis für die Google-Autorisierung bereitgestellt.
	- Größere Synchronisationsintervalle hinzugefügt, Feature-Request 70.
	- Das Layout für die OK- und Abbrechen-Schaltfläche in GeneralOptionsForm wurde korrigiert.
	- Verbesserte Integrationstests.

#### 2.19.1 ####
- Erschienen am 18.04.2017
- Fehlerbehebungen
	- Problem behoben, dass die Symbolleiste in Outlook 2007 nicht zugreifbar war, behoben. Ticket #570.
	- Verbesserte Integrationstests.

#### 2.19.0 ####
- Erschienen am 16.04.2017
- Neue Features
	- Abbrechen und Verschieben der Synchronisierung, wenn der Server HTTP 429 meldet.
	- Bricht die Synchronisierung bei netzwerkbezogenen Ausnahmen ab und betrachtet sie als Warnung, wenn sie die ersten 2 mal auftreten. Dies sollte helfen, Fehler beim Starten des Laptops nach dem Ruhezustand zu vermeiden oder wenn VPN noch nicht bereit ist. Issues #104, #181.
	- Blockieret nicht den Outlook-Start mit der Komponenteninitialisierung. Vermeidet das Problem, dass Outlook das Add-In nach einem langsamen Start deaktiviert.
	- Refactoring von Integrationstests.
- Fehlerbehebungen
	- Problem mit MapDistListMembers2To1 für Mitglieder behoben, die nicht aus dem Adressbuch aufgelöst wurden.
	- Die Zuordnung der E-Mail-Adresse für Google Home-Adressen zu Outlook Email1Adresse, wurde behoben. Ticket 561.
	
#### 2.18.0 ####
- Erschienen am 26.03.2017
- Neue Features
	- Zuordnung von Verteilerlisten zu Kontaktgruppen mit KIND: group hinzugefügt.
	- Profiltyp für Easy Project / Easy Redmine mit speziellem Einrichtungsassistenten hinzugefügt.
	- Profiltyp für Mailbox.org hinzugefügt.
	- Profilauswahl auf WPF umgestellt.
- Fehlerbehebungen
	- MessageBox mit Warnung vor vertraulichen Daten in der Protokolldatei hinzugefügt, bevor das Protokoll angezeigt wird.
	- Konfigurationsoption für die Aufgabenzuordnung hinzugefügt, um Outlook-Start und Fälligkeitsdatum von Aufgaben als Floating ohne Zeitzoneninformationen zuzuordnen, um Probleme mit Aufgaben über Zeitzonen hinweg zu vermeiden, Ticket #530.
	- NuGet-Pakete wurden aktualisiert.

#### 2.17.0 ####
- Erschienen am 26.02.2017
- Neue Features
	- Eine allgemeine Option wurde hinzugefügt, um die Synchronisierungsfortschrittsleiste anzuzeigen / auszublenden und den Schwellenwert für die Anzeige konfigurierbar zu machen.
	- App.config-Einstellung für SoftwareOnly WPF-Rendering hinzugefügt, um Probleme mit Grafikkartentreibern und Hardwarebeschleunigung zu vermeiden. Ticket #480.
- Fehlerbehebungen
	- Vermeiden von System.Collections.Generic.KeyNotFoundException für die Google-Kontakt-API. Das Paging beim Abrufen von Google-Gruppen beachten. Ticket #511.
	- Geführte Weiterleitung auch für 303 in WebDavClient, Ticket #516.

#### 2.16.0 ####
- Erschienen am 14.02.2017
- Neue Features
	- Es wurde eine Warnung hinzugefügt, wenn der Einweg-Synchronisationsmodus zum Löschen des vorhandenen nicht leeren Outlook-Ordners oder zur Replizierung eines leeren Ordners auf dem Server führen würde.
	- Möglichkeit hinzugefügt, die Chunked-Ausführung auch für Google-Kontakte zu verwenden.
	- Option zum Deaktivieren des Sticky-Kategoriefilters hinzugefügt.
	- Zuordnung von ROLE zu Outlook Profession für Kontakte hinzugefügt. Kategoriefilter-Ticket #505.sticky.
- Fehlerbehebungen
	- Besserer Umgang mit SOGo VLIST-Mitgliedern als Empfänger, damit der zugrunde liegende Kontakt verwendet wird.
	- Nimmt an, dass ein HTTP-404 nur ein leeres Adressbuch bezeichnet , wenn die Adressbuchressource vorhanden ist.

#### 2.15.1 ####
- Erschienen am 31.01.2017
- Fehlerbehebungen
	- Ausnahmebedingung in QueryAppointmentFolder wurde vermieden, wenn nicht auf GlobalAppointmentID zugegriffen werden kann oder null ist, Ticket #491.
	- Die Fenstergröße des GeneralOptions-Fensters wurde vergrößert und die Bildlaufleiste hinzugefügt. Dadurch werden Probleme bei Geräten mit niedriger Auflösung vermieden.

#### 2.15.0 ####
- Erschienen am 29.01.2017
- Neue Features
	- Große Leistungsverbesserungen beim Zugriff auf Outlook-Ordnerdaten, wenn sich nichts geändert hat. Das Abrufen aller Elemente vermeiden. Eine allgemeine Option hinzugefügt, um die Ordnerabfrageoption zu konfigurieren.
	- Viele Verbesserungen der Benutzeroberfläche, ein Link zum Anzeigen / Ausblenden erweiterter Einstellungen und allgemeine Option zum Festlegen der Standardeinstellungen wurde hinzugefügt.
	- Allgemeine Optionen neu geordnet / gruppiert.
	- Viele Verbesserungen des vCard-Readers, Unterstützung für verschiedene X-Eigenschaften für IMs, Ticket #463.
	- Nicht erkannte Eigenschaften in vCard OtherProperties gespeichert.
- Fehlerbehebungen
	- Try/catch um DateTimeZoneNotFoundException, Ticket # 484.
	- Das doppelte Hinzufügen der E-Mail-Adresse wurde vermieden.
	- FormatException in vCardStandardReader abfangen und Warnungen von vcard-Deserialisierung protokollieren.
	- Warnen, wenn RRULE COUNT=0 ist, und COM-Ausnahmen vermeiden, wenn ungültige Werte für RecurrencePattern Occurrences oder PatternEndDate festgelegt werden.
	- Don't set RRULE COUNT if Occurrences is an invalid number.
	- NullReferenceException vermieden, wenn eine SOGo-VLIST eine Mitgliedskarte ohne FN hat. Leere Mitglieder vermieden.
	- Catchen einer möglichen COMException, wenn auf eine Besprechungseinladung geantwortet wird.
	- Problemumgehung für das Lesen falsch codierter Vcard-PHOTO-Attribute aus globalen SOGo-Adressbüchern, die aus LDAP / AD-Avatar-Bildern zugeordnet werden.
	
#### 2.14.1 ####
- Erschienen am 17.01.2017
- Fehlerbehebungen
	- Das Installationsprogramm wurde aktualisiert, um die Abhängigkeit von Thought.vCards zu beheben.

#### 2.14.0 ####
- Erschienen am 16.01.2017
- Neue Features
	- Anfängliche Unterstützung für das Synchronisieren von Kontaktgruppen / Verteilerlisten (unterstützt nur das SOGos-eigene VLIST-Format).
	- Eigene Version von Thought.vCards von [https://github.com/aluxnimm/Thought.vCards](https://github.com/aluxnimm/Thought.vCards) anstelle von NuGet-Paket verwenden und vCardImprovedWriter entfernt.
	- VCardWriter verbessert und Unterstützung für verschiedene IM-Servicetypen hinzugefügt, Ticket #463.
	- Unterstützung für ADR-Postfach und erweiterte Adresse hinzugefügt, Festure-Request 17.
- Fehlerbehebungen
	- Entfaltete Zeilen vor der weiteren Verarbeitung in vCardStandardReader behebt Probleme mit langen Untereigenschaften wie X-ABCROP-RECTANGLE.
	- Setzt die wiederkehrende Aufgabe DTSTART auf PatternStartDate, um zu vermeiden, dass DTSTART fehlt. Ticket 465.
	- ProgressWindow auf Wpf umgestellt, um DPI-Probleme zu vermeiden.
	- Projekt-URLs im Über-Dialog aktualisiert.

#### 2.13.0 ####
- Erschienen am 03.01.2017
- Upgrade-Anweisungen
	- Outlook und Google sowie einige andere CalDAV-Server berechnen die Schnittmenge mit dem Zeitbereich für wiederkehrende Ereignisse unterschiedlich, was zu doppelten oder gelöschten Ereignissen führen kann. Es wird daher empfohlen, einen Zeitbereich auszuwählen, der größer ist als das größte Intervall Ihrer wiederkehrenden Ereignisse (z. B. 1 Jahr für Geburtstage). Der Standard-Zeitbereich für neue Profile wird von 180 Tagen auf 365 Tage in der Zukunft geändert. Für vorhandene Synchronisierungsprofile müssen Sie sie manuell ändern, wenn sie betroffen sind!
- Neue Features
	- Zuordnungskonfigurationsoption hinzugefügt, um auch Termine / Aufgaben ohne Kategorie in den Kategorienfilter aufzunehmen.
- Fehlerbehebungen
	- Set time-range default timespan to 365 days in the future and add tooltip and warning for time-range filter, ticket #450.
	- Zeitzonenprobleme bei Google-Tasks behoben, Ticket #452.
	- Kein X-ALT-DESC hinzufügen, wenn body leer ist.

#### 2.12.1 ####
- Neue Features
	- Aktualisieren von Google API NuGet-Paketen auf Version 1.20.0.
- Fehlerbehebungen
	- Verhindert NullReferenceExceptions, die durch nicht initialisierten ComponentContainer aufgrund von Ladefehlern verursacht werden.
	- Verbesserte html <-> rtf-Zuordnung für Termine.
	- Synchronisierung des Starts und des Fälligkeitsdatums der Aufgabe vom Server zu Outlook, Ticket #446.
	- Absoluter Taskalarm hinzugefügt, wenn Start- und Fälligkeitsdatum nicht festgelegt sind, Ticket #445.

#### 2.12.0 ####
- Neue Features
	- Allgemeine Option zum Aktivieren der TLS-Authentifizierung für Clientzertifikate hinzugefügt, Feature-Request 55.
	- Zugeordnete Outlook-formatierte RTFBody-HTML-Beschreibung über das Attribut X-ALT-DESC.
- Fehlerbehebungen
	- Verwenden von Kleinbuchstaben für mailto im Organisator und in den Teilnehmer-URLs, um Probleme mit einigen Clients zu vermeiden, Ticket #426.

#### 2.11.0 ####
- Neue Features
	- Möglichkeit hinzugefügt, DAV-Serverkalender / -Adressbücher hinzuzufügen.
	- Verbesserte Berechtigungsprüfung beim Verbindungstest.
	- Zuordnung des SCHEDULE-STATUS zum Flag Outlook FINVITED, das anzeigt, ob die Einladungs-E-Mail gesendet wurde. Issue 162.
	- PostBuildEvent wurde hinzugefügt, um Installationsdateien zu signieren, um eine Warnung wegen eines nicht vertrauenswürdigen Herstellers während der Installation zu vermeiden.
	- Aktualisierung der Google API NuGet-Pakete auf Version 1.19.0.
- Fehlerbehebungen
	- Legen Sie User GlobalAppointmentID als Standard für SOGo-Profile fest, um doppelte Termine zu vermeiden, wenn Outlook Einladungen sendet.
	- Die Zuordnung des vtodo-Status NEEDS-ACTION zu Outlook olTaskNotStarted wurde korrigiert. Ticket #418.
	- Rückfall in die lokale Zeitzone, wenn FindSystemTimeZoneById eine Ausnahme auslöst, Ticket #421.
	- Protokollierung für Alarme behoben und Warnung für mehrere Alarme aus dem Synchronisierungsbericht entfernt.
	- Keine Einladungen von der Serveridentität löschen.

#### 2.10.0 ####
- Neue Features
	- Profiltyp für NextCloud hinzugefügt.
	- Allgemeine Option zum Aktivieren von useUnsafeHeaderParsing hinzugefügt, die für Yahoo und cPanel Horde erforderlich ist.
	- Verbessertes Autodiscovery.
- Fehlerbehebungen
	- Das Installationsprogramm für die 64-Bit-Installation von Office für die AllUsers-Bereitstellung wurde korrigiert und der Registrierungsschlüssel wird in den richtigen HKLM-Speicherort kopiert. Ticket 410.
	- Bildlaufleiste hinzugefügt, um die Inhaltskontrolle von Profilen zu synchronisieren. Issue 176.
	- Die automatische Erkennung von iCloud CardDav wurde korrigiert. Ticket 414.
	- Trigger-Synchronisierung auch beim Start von Outlook, wenn TriggerSyncAfterSendReceive in den allgemeinen Optionen aktiviert ist. Ticket 415.
	- COMException abfangen, wenn Outlook-Element in Synchronisierungsberichten nicht gefunden wird.

#### 2.9.1 ####
- Hotfix
	- Das Erinnerungsmapping für gerade anstehende Erinnerungen wurde korrigiert. Regression wurde in 2.9.0 eingeführt. Ticket #406.
- Neue Features
	- CheckForNewVersions, StoreAppDatainRoamingFolder und IncludeCustomMessageClasses als app.config-Schlüssel hinzugefügt. Dies ist nützlich für die Bereitstellung von All Users, um die Standardeinstellungen zu ändern.
- Fehlerbehebungen
	- Verbesserte CustomPropertyMapping-Überprüfung und überprüft, ob Eigenschaften leer sind, um Nullreferenzausnahmen zu vermeiden.
	- Aktualisierte Google Api-Nuget-Pakete.

#### 2.9.0 ####
- Neue Features
	- Profil Import / Export hinzugefügt.
	- Installer wurde verbessert, Hersteller von DefaultLocation entfernt und InstallDir in der Registrierung für Updates gespeichert.
	- Passive Installation für Updates verwendet.
	- Symbolleistenschaltflächen hinzugefügt, um alle Knoten in Synchronisationsprofilen zu erweitern und zu reduzieren.
	- Allgemeine Option hinzugefügt, um standardmäßig alle Knoten in Synchronisationsprofilen zu erweitern.	
- Fehlerbehebungen
	- COMException abgefangen, wenn auf SyncObjects nicht zugegriffen werden kann, Github-Issue 175.
	- Das Installationsprogramm für die Bereitstellung aller Benutzer wurde korrigiert.
	- Korrigierte Map nur anstehende Erinnerungen für wiederkehrende Termine, Ticket #398.

#### 2.8.2 ####
- Fehlerbehebungen
	- Die Erstellung neuer Profile für Kalender- und Aufgabenprofile wurde korrigiert und die customPropertyMapping-Konfiguration ordnungsgemäß initialisiert.
	- Die Initialisierung von UserDefinedCustomPropertyMappings wurde korrigiert, um Nullreferenzausnahmen zu vermeiden.
	- Formatierung von errorMessage bei der Profilvalidierung korrigiert.

#### 2.8.1 ####
- Fehlerbehebungen
	- Vermeidet Nullreferenz Ausnahmen, wenn Optionen nach dem Upgrade auf 2.8.0 nicht gespeichert werden. Issue 174.

#### 2.8.0 ####
- Neue Features
	- Konfigurierbare benutzerdefinierte Eigenschaftszuordnung für Termine und Aufgaben.
	- Aktualisierte NuGet-Pakete für Google API und NUnit.

#### 2.7.0 ####
- Neue Features
	- Zuordnen von UID zu GlobalAppointmentID für neue Besprechungen, um Doppelereignisse von E-Mail-Einladungen zu vermeiden (nur in Outlook 2013+ möglich).
	- Option hinzugefügt, um CalDAV- / CardDAV-Synchronisierung in Abschnitten mit konfigurierbarer Abschnittsgröße durchzuführen, um OutOfMemoryEceptions zu vermeiden. Ticket 390.
	- Schaltfläche hinzugefügt, die das Profildatenverzeichnis zum Debuggen öffnet.
- Fehlerbehebungen
	- Vermeidet die ArgumentNullException, wenn Termine keine GlobalAppointmentID und Protokollwarnung haben, Ticket #389.
	- Profilsymbol in Optionen aktualisiert, wenn sich der OutlookFolderType des Profils ändert.
	- Fix für ToolBarButtons in Optionen.

#### 2.6.1 ####
- **WARNUNG**: Diese Version ändert die interne Cache-Struktur. Beim Downgrade auf eine ältere Version wird der Cache gelöscht und eine neue Anfangssynchronisierung durchgeführt!
- Fehlerbehebungen
	- Cache-Konvertierung für Aufgaben behoben.
	- Stellen Sie den Synchronisierungskontext bei jedem Klicken der Schaltfläche sicher.

#### 2.6.0 ####
- **WARNUNG**: Diese Version ändert die interne Cache-Struktur. Beim Downgrade auf eine ältere Version wird der Cache gelöscht und eine neue Anfangssynchronisierung durchgeführt!
- Neue Features
	- Bessere Unterstützung für Besprechungseinladungen.
	- Verbesserter doppelter Ereignisreiniger.
	- Aktualisierte Google Apis-Nuget-Pakete auf 1.16.0.
	- GlobalAppointmentId in RelationCache eingefügt.
- Fehlerbehebungen
	- Akzeptierte Besprechungseinladungen wurden aktualisiert, anstatt sie zu löschen und neu zu erstellen, um falsche Stornierungsmails vom CalDAV-Server zu vermeiden.
	- OverflowException für ungültige Geburtstage in Kontakten abfangen, Ticket #386.
	- DuplicateEventCleaner: Ausnahme abfangen, wenn kein Termin mehr vorhanden ist.
	- Vermeiden Sie eine Nullreferenz-Ausnahme und fügen Sie keine Serverressource hinzu, wenn diese keine gültigen VEVENT- oder VTODO-Probleme enthält. Issue 167.
	- Es wird geprüft, ob die Caldav-Ressource nicht leer ist, um ArgumentOutOfRangeExceptions zu vermeiden.

#### 2.5.1 ####
- Neue Features
	- Kontotyp für Cosy Cloud hinzugefügt und UseIanaTz als Standard festgelegt.
- Fehlerbehebungen
	- Setzen Sie BusyStatus auf "Tentativ" für Besprechungseinladungen ohne Antwort.
	- Die 307-Weiterleitungen in WebDavRequests eingeführt, Autodiscovery für Telstra BigPond korrigiert.
	- Stellen Sie sicher, dass die erkannten Ressourcenuris mit einem Schrägstrich enden.
	- Linebreak-Probleme für Open-Xchange-Vcards behoben, Ticket #290.
	- TYPE=WORK wurde der ersten Outlook-E-Mail-Adresse und TYPE=HOME für die zweite für CardDAV-Profile und Mapping der Arbeits-E-Mail zur ersten Outlook-E-Mail-Adresse und der Home-E-Mail für die CardDAV- und Google-Kontaktprofile hinzugefügt.
	- Standard-Zuordnung von Mobilfunk-, Arbeits- und Privattelefonnummern hinzugefügt, wenn diese beim Synchronisieren mit dem CardDAV-Server PhoneTypes fehlen, um den Verlust von Telefonnummern zu vermeiden.
	- Erhaltene Besprechungen von der sofortigen Synchronisierung ausgeschlossen, um Probleme mit verdoppelten Ereignissen zu vermeiden.

#### 2.5.0 ####
- Neue Features
	- Zuordnungskonfiguration hinzugefügt, um IANA-Zeitzonen anstelle von Windows-Zeitzonen zu verwenden.
	- Add-In-Start und EntityMapper asynchron gemacht.
	- ProgressBar hinzugefügt und neue Version async heruntergeladen. Github-Issue 156.
- Fehlerbehebungen
	- SCHEDULE-AGENT = CLIENT wurde auch für die Teilnehmer hinzugefügt, Ticket #354.
	- Leeres PARTSTAT vermieden und standardmäßig auf NEEDS-ACTION gesetzt.
	- Die KeepOutlookFileAs-Option (Standardeinstellung true) für Kontakte wurde hinzugefügt, um das Überschreiben vorhandener FileAs mit dem FN-Attribut zu vermeiden.
	- Setzen des Outlook-Kontakt FullName auf FN als Fallback, wenn N in vcard fehlt.
	- Setzen des Status der Outlook-Aufgabe auf Abgeschlossen, wenn das vollständige Datum vorhanden ist und percentComplete den Wert 100 hat, auch wenn der VTODO-Status fehlt. Github-Issue 154.
	- Korrigierter Mapping-Organizer, wenn CN und E-Mail identisch sind, Github-Issue 157.
	- DDay.ICal-UTC-Aufrufe wurden vermieden und stattdessen NodaTime für die Konvertierung verwendet, Github-Issue 159.

#### 2.4.0 ####
- Neue Features
	- Das Kontokennwort wurde auch für die Massenprofilerstellung hinzugefügt. Außerdem können die Servereinstellungen (DAV-URL, E-Mail, Benutzername) vom Outlook-IMAP / Pop3-Konto abgerufen werden.
	- Mapping für Aufgabenalarme mit absoluten Datums- / Zeitauslösern hinzugefügt.
	- Kategoriefilter auch für Aufgaben hinzugefügt, Feature 48.
	- Das Kontaktfoto wird heruntergeladen, wenn es von der URL bereitgestellt wird, und korrigiert das Photo-Mapping für GMX, Ticket #358.
- Fehlerbehebungen
	- Der Pfad des SOGo-Kontoprofils wurde in /SOGo/dav/ geändert.
	- Die Zuordnung von PostalAddress Country in der Google Contacts API wurde korrigiert.
	- Die Zuordnung von PostalCode für Google Contacts wurde korrigiert. Ticket #352.
	- Aktualisierte NuGet-Pakete für verwendete externe Bibliotheken.
	- Protokollierte Warnung und Vermeidung einer COM-Ausnahme für wiederkehrende Ereignisse und Aufgaben, wenn RRULE BYMONTH ungültig ist, Ticket #334.
	- Verwendet den richtigen Anforderungs-URI in Berichten, wenn der Server-URI eine andere Codierung als der Ressourcen-URI aufweist. Github-Issue 152.

#### 2.3.1 ####
- Fehlerbehebungen
	- Problem beim Positionieren und Speichern der OL2007-Symbolleiste behoben, Ticket #351.
	- Verwendet nur Start, Ende und Betreff für DuplicateEventCleaner, Ticket #330.

#### 2.3.0 ####
- Neue Features
	- Outlook 2007 toolBar-Position und Sichtbarkeit in Registry gespeichert, Github-Issue 102.
	- Doppelte Ereignisbereinigung in der Konfiguration der Ereigniszuordnung implementiert.
	- CalDavConnectTimeout als allgemeine Option hinzugefügt. Feature 46.
- Fehlerbehebungen
	- Befehlsleiste für OL2007 behoben. Ticket #339.
	- Einige Korrekturen für Wiederholungsausnahmen, wenn die Zeitzone des Termins von der lokalen Outlook-Zeitzone abweicht.
	- Das Einstellen des Organisatornamens in Outlook von CommonName und Email wurde korrigiert.
	- Allgemeine Option zum Anzeigen von Berichten zu Warnungen und / oder Fehlern auch für Systray-Benachrichtigungen. Github-Issue 143.
	- Ordnen Sie auch Standardereignisse privaten zu, wenn die Zuordnungsoption aktiviert ist. Ticket #329.
	- Stiehlt den Fokus nicht, wenn ProgressForm angezeigt wird (#328 Window steal focus, wenn die Synchronisierung gestartet wird).
	- Validierung für die Eingabe in GeneralOptionsForm hinzugefügt.

#### 2.2.0 ####
- Neue Features
	- Allgemeine Option hinzugefügt, um die Synchronisierung auszulösen, nachdem Outlook Senden / Empfangen abgeschlossen ist. Github-Issue 141.
	- Konfigurationsparameter für die Ereigniszuordnung hinzugefügt, um die Markierung CLASS: PUBLIC to Outlook Private zuzuordnen. Feature-Request 45.
	- Implementierung von DNS SRV- und TXT-Suchvorgängen für die automatische Erkennung von E-Mail-Adressen.
- Fehlerbehebungen
	- Die automatische Erkennung wurde behoben, wenn der Server mehrere Hrefs mit calendar-home-set zurückgibt. Github-Issue 139.

#### 2.1.3 ####
- Neue Features
	- Event Mapping-Konfiguration hinzugefügt, um Outlook GlobalAppointmentID für das UID-Attribut zu verwenden. Ticket #318.
- Fehlerbehebungen
	- Keine Warnung protokollieren, wenn DTEND nicht für alltägliche Ereignisse eingestellt ist. Ticket #316.
	- Präfixzusammenfassung von Ereignissen und nicht nur Besprechungen mit dem Status "Abgebrochen", da Android dies anstelle von Exatdaten für Wiederholungsausnahmen verwendet, Ticket #307.

#### 2.1.2 ####
- Neue Features
	- ProfileType für SOGo hinzugefügt.
- Fehlerbehebungen
	- Das Erkennen von gelöschten Terminen aus Ordnern in lokalen PST-Datendateien wurde behoben, wenn der Kategoriefilter verwendet wurde. Ticket #297.

#### 2.1.1 ####
- Neue Features
	- ProfileType für Orientierungspunkte hinzugefügt.
- Fehlerbehebungen
	- Vermeiden von Synchronisationsschleifen und löschen neuer Ereignisse, wenn sie eine Einladung von der Serveridentität darstellen.
	- Die Zuordnung von Ereignissen von TRANSP zu Outlook BusyStatus wurde korrigiert auf X-MICROSOFT-CDO-BUSYSTATUS.
	- Behoben: Autodiscovery bei leerem URL-Textfeld.

#### 2.1.0 ####
- Neue Features
	- Massenprofilerstellung implementiert, um mehrere Profile gleichzeitig hinzuzufügen und den Ordner für jede erkannte Serverressource (Kalender, Adressbuch und Aufgabe) auszuwählen.
	- Abfragen unterstützter Kalender-Komponentensätze und Filtern von VEVENT- und VTODO-Ressourcen für die automatische Erkennung.
- Fehlerbehebungen
	- Funktionalität hinzugefügt, um mit mehreren Gruppen mit demselben Namen für die Google Contacts API umgehen zu können.
	- Die alte CalendarUrl wurde wiederhergestellt, wenn bei der Google AutoErmittlung ein Fehler aufgetreten ist oder der Vorgang abgebrochen wurde.
	- Der default ResponseStatus-Standardwert ist NEEDS-ACTION in MapParticipation1To2, um eine Ausnahme zu vermeiden.

#### 2.0.2 ####
- Neue Features
	- Verbesserte Ereigniszuordnung von TRANSP und STATUS zu Outlook BusyStatus. (Contribution von Florian Saller).
	- Verbessertes Autodiscovery.
	- ProfileType für Sarenet hinzugefügt.
- Fehlerbehebungen
	- Ungültige-XML-Fehler in EntityRelationDataAccess werden ignoriert, sofern keine neue Version gespeichert wurde.
	- Alle Google-Kontakte wurden mit einer einzigen Anforderung abgerufen, um 503 Fehler zu vermeiden.
	- Nur Kontakte aus der Default Group aus der Google Contacts API abfragen.
	- Keinen Fehler melden, wenn das Löschen oder Aktualisieren aufgrund von Parallelitätseffekten fehlschlägt.
	- Greifen Sie auf AddressEntry nur zu, wenn der Empfänger aufgelöst werden kann und mögliche COMExceptions abgefangen werden.

#### 2.0.1 ####
- Neue Features
	- Anfängliche Unterstützung für mail.ru.
	- Option hinzugefügt, um das Outlook-Foto in der Kontaktzuordnungskonfiguration zu halten.
- Fehlerbehebungen
	- COMException abgefangen, wenn in Outlook kein Ticket eingestellt werden kann, Ticket #276.
	- Die aktuelle Mapping-Konfiguration bleibt erhalten, wenn kein Ordner ausgewählt ist.
	- Eigene Identitätsbehandlung in der Ereigniszuordnung (insbesondere für Exchange-Konten) behoben.
	- Mögliche Nullreferenzausnahme in CardDavDataAccess.GetEntities behoben.
	- Es wird geprüft, ob der Schlüssel vorhanden ist, bevor er zu targetExceptionDatesByDate in MapRecurrence1To2 hinzugefügt wird. Ticket #270.
	- Überspringen von directoryresource, wenn von der Kalenderabfrage zurückgegeben, da mail.ru selbst mit einem etag das Verzeichnis selbst zurückgibt.
	- Andere Kontrollkästchen in den Zeitplaneinstellungen wurden deaktiviert, wenn die Option "Map-Teilnehmer" deaktiviert ist.
	- X-ABCROP-RECTANGLE aus den Vcard-Fotoattributen entfernt, da der Deserializer den base64-Wert nicht parsen kann. Ticket #274.
	- Schaltfläche "Jetzt synchronisieren" während Synchronisierungsläufen deaktiviert.

#### 2.0.0 ####
- Neue Features
	- Unterstützung für die Google Contacts API zur Synchronisierung von Outlook-Kontaktordnern mit Google-Kontakten wurde hinzugefügt. Dies verbessert die Zuordnung und die Leistung, da die Google CardDAV-API einige Probleme aufweist (erste offizielle Veröffentlichung, Beta).
	- Unterstützung für Google-Kontaktgruppen, die mit Outlook-Kategorien synchronisiert werden.
	- Synchronisieren von Kontaktfotos, Webseiten, Notizen, Empfindlichkeit, Hobbies für Google-Kontakte.
	- Mapping für Jubiläum, Beziehungen (Ehepartner, Kind usw.) und IMs für Google-Kontakte hinzugefügt. (Beitrag von Florian Saller [https://sourceforge.net/u/floriwan/profile/](https://sourceforge.net/u/floriwan/profile/), vielen Dank!)
	- Benutzeroberfläche für Einstellungen für ältere Synchronisationsprofileinstellungen entfernt.
- Fehlerbehebungen
	- TYPE = JPEG wurde zu vcard-Fotoattributen hinzugefügt und Ausnahmen in MapPhoto2To1 erfasst.
	- COM-Exception beim Abrufen von Elementen aus Outlook abgefangen (Ticket #263 Fehler beim Löschen von Kontakten mit Änderungen synchronisieren sofort nach Aktivierung der Änderungen).
	- Mögliche Nullreferenzausnahme in CardDavDataAccess behoben.
	- Das Kontrollkästchen "ForceBasicAuthentication" in der WPF-Benutzeroberfläche wurde behoben.
	- Feste und vereinfachte Verbindungstests.
	- Das Kontaktfoto in Outlook wird gelöscht, wenn es auf dem CardDav-Server gelöscht wurde.

#### 1.24.0 ####
- Neue Features
	- Allgemeine Option hinzugefügt, um ungültige Zeichen in der Serverantwort zu ignorieren.
	- Neuanordnung der Synchronisationsprofile in der WPF-Benutzeroberfläche implementiert
- Fehlerbehebungen
	- Problem mit VALARM-Trigger-Behandlung behoben, wenn die Dauer null ist, Ticket #253.
	- Anzeigeprobleme für Berichte #259 behoben.
	- Fehlendes Kontrollkästchen in WPF EventMappingConfigurationView hinzugefügt (Filter negieren und alle Termine außer dieser Kategorie synchronisieren).
	- TimeRangeView für alle Ordnertypen mit Ausnahme von Terminen und Aufgaben ausblenden.
	- Proxy-Einstellungen in der neuen WPF-Benutzeroberfläche korrigiert.
	- Deaktivieren der ConflictResolution für die OneWay-Synchronisierung in der WPF-Benutzeroberfläche.

#### 1.23.0 ####
- Neue Features
	- Erste Implementierung eines kompletten Redesigns der GUI für Synchronisationsprofile mithilfe des WPF-Frameworks.
	- Allgemeine Option zum Wechseln zwischen moderner WPF- und Standard-WinForms-Benutzeroberfläche.
	- Verbessertes Update-Handling und Herunterladen vom README nach der Installation einer neuen Version.
- Fehlerbehebungen
	- Ungültige BYMONTHDAY-Werte in Wiederholungsregeln ignoriert, COMException abfangen und als Warnung protokollieren.
	- HasTime als abgeschlossen von vtodo setzen, um zu vermeiden, dass VALUE = DATE für GMT-Zeitzone RFC-kompatibel ist, Ticket #247.
	- Verbesserte Ausnahmebehandlung.
	- Sicherstellen, dass SynchronizationContext VOR dem Aufruf von async-Methoden alle Aufrufe von async-Methoden mit einem try-catch umfasst. Ticket #248.
	- Versuch, das Masterereignis zu rekonstruieren und Ausnahmen ordnungsgemäß mit Outlook zu synchronisieren, wenn die Serverressource nur aus Wiederholungsausnahmen besteht.

#### 1.22.0 ####
- Neue Features
	- Option hinzugefügt, um die Zuordnung von wiederkehrenden Aufgaben in TaskMappingConfiguration zu aktivieren / deaktivieren, um Probleme mit Servern zu vermeiden, die keine wiederkehrenden Aufgaben unterstützen.
	- In der Kontaktzuordnungskonfiguration wurde eine Option hinzugefügt, um die Formatierung von Telefonnummern beim Synchronisieren vom Server mit Outlook zu korrigieren, sodass Outlook die Länder- und Ortsvorwahl erkennen kann, Feature-Request 34.
	- Verwenden der E-Mail-Adresse für vcard FN, wenn Datei, Name und Unternehmensattribute von Outlook-Kontakten leer sind.
- Fehlerbehebungen
	- Die VTIMETONE DTSTART-Generierung für Zeitzonen mit jährlichen Floating DST-Regeln wie Jerusalem bei der Synchronisierung mit Google wurde behoben. Ticket #244. (Workaround für einen Fehler in der Bibliothek DDay.iCal)
	- Keine Filterkategorie zu Outlook-Kategorien hinzufügen, wenn der Negate-Filter aktiviert ist, Ticket #245.

#### 1.21.0 ####
- Neue Features
	- Durch die Implementierung einer Option in Netzwerk- und Proxy-Optionen zum Erzwingen der Basisauthentifizierung, die für einige Server erforderlich ist, auf denen die Aushandlung oder die Digest-Authentifizierung nicht ordnungsgemäß funktionieren, werden Verbindungsprobleme mit OS X-Servern behoben.
	- Allgemeine Option zum Aktivieren / Deaktivieren des Taskleistensymbols hinzugefügt.
	- Verbesserte Debug-Protokollierung.
- Fehlerbehebungen
	- Verwendet NullOutlookAccountPasswordProvider, wenn der Name des Outlook-Profils null ist, Ticket #239.
	- Proxy-Unterstützung in Google Tasklibrary- und Oauth-Anfragen behoben, Ticket #234.
	- Zeilenumbrüche in Vcard-Notizen und Straßenadressen wurden korrigiert, um \r zu vermeiden.

#### 1.20.3 ####
- Fehlerbehebungen
	- Outlook-Absturz beim Öffnen von Synchronisationsprofilen für Outlook 2007 (Ticket #230, #231) behoben.

#### 1.20.0 ####
- Neue Features
	- Die neue Implementierung der Teilsynchronisierung, die unmittelbar nach dem Erstellen, Ändern oder Löschen eines Elements in Outlook (mit einer Verzögerung von 10 Sekunden) ausgelöst wird, funktioniert jetzt auch für Kontakte und Aufgaben.
	- Option hinzugefügt, um das IMAP / Pop3-Kennwort aus dem mit dem Ordner verknüpften Outlook-Konto zu verwenden. Das Kennwort wird aus dem Windows-Registrierungseintrag des Outlook-Profils abgerufen.
	- Kontrollkästchen hinzugefügt, um alle Outlook-Termine mit Ausnahme einer definierten Kategorie (negiert den Kategoriefilter) in EventMappingConfiguration zu synchronisieren. Feature-Request 30.
	- Verwenden der ComboBox mit allen verfügbaren Outlook-Kategorien anstelle von TextBox, um den Kategoriefilter auszuwählen.
	- Kontotypen für Fruux, Posteo, Yandex und GMX mit vordefinierten DAV-URLs hinzugefügt und Logos zum Kontoauswahldialog hinzugefügt.
- Fehlerbehebungen
	- Bekannte URIs nach RFC behoben, sie enthalten keinen abschließenden Schrägstrich, behebt die automatische Erkennung von fruux.
	- ArgumentNullException für GoogleTasks vermeiden, wenn die Jobliste leer ist, Ticket #229.
	- Durch das Löschen von Kontaktattributen in Outlook, wenn Attribute auf dem Server entfernt werden, werden einige Probleme bei der Aktualisierung der Zuordnung von Server zu Outlook für CardDAV behoben.

#### 1.19.0 ####
- Neue Features
	- System-Statussymbol mit Benachrichtigungen zu Synchronisierungsläufen mit Fehlern und Warnungen sowie Kontextmenü hinzugefügt.
	- Synchronisationsstatus mit Informationen über die letzte Synchronisationslaufzeit und den Status hinzugefügt, auf die über Statussymbol oder das Menüband zugegriffen werden kann.
	- TaskMappingConfiguration hinzugefügt mit der Möglichkeit, Erinnerung, Priorität und Körperzuordnung umzuschalten.
- Fehlerbehebungen
	- COMException beim Zugriff auf IsInstantSearchEnabled des Outlook-Speichers abgefangen, Ticket #223.
	- Behobener Fehler beim Öffnen älterer Profile ohne Proxy-Optionen, Ticket #224.

#### 1.18.0 ####
- Neue Features
	- Deaktiviert den Präfixfilter für benutzerdefinierte Nachrichtenklassen standardmäßig und macht ihn als allgemeine Option konfigurierbar, da der Windows-Suchdienst benötigt wurde und nicht in allen Setups verfügbar sind.
	- Manuelle Schaltfläche "Nach Updates suchen" in der Info-Box hinzugefügt.
- Fehlerbehebungen
	- Bei Verwendung des Präfixfilters wurde eine korrekte Prüfung auf IsInstantSearchEnabled für den Store hinzugefügt.
	- Nicht verwendete allgemeine Option DisplayAllProfilesAsGeneric wurde entfernt.
	- Nicht benötigte enableTaskSynchronization in app.config entfernt.
	- Zuordnungsfehler in Warnungen für die Protokollierung geändert.

#### 1.17.0 ####
- Neue Features
	- Verbesserte formatierte Ansicht für Synchronisierungsberichte mit der Möglichkeit, Outlook- und Server-Entitäten anzuzeigen, die Zuordnungswarnungen oder -fehler verursachen.
	- Verbesserte Benutzeroberfläche. Erweiterte Optionen in Netzwerk- und Proxy-Optionen umbenannt und Schaltfläche in Servereinstellungen verschoben. Schaltfläche "Zuordnungskonfiguration" aus erweiterten Formularen in Hauptprofil-Konfigurationsformular verschoben.
	- Verwenden des Präfixvergleichs in Outlook-Repositorys, um auch benutzerdefinierte Nachrichtenklassen zu filtern.
- Fehlerbehebungen
	- Testeinstellungen behoben und Outlook-Aufgabenordner nicht für Google-Kalender, sondern nur für eine Google-Jobliste zugelassen.
	- Die BackColor aller UI-Formulare und Textfelder wurde in SystemColors.Window geändert.
	- Problem mit der Wortänderung im Änderungsprotokoll des Update-Fensters behoben und die Größe des Fensters wurde geändert. Feature-Request 24.
	- Leeres Passwort verwendet, wenn das Entschlüsseln des Passworts fehlschlägt, Ticket #165.

#### 1.16.0 ####
- Neue Features
	- Google Aufgabenunterstützung hinzugefügt. Sie können Google-Joblisten mit Outlook-Aufgabenordnern über Google Task Api synchronisieren. Verwenden Sie einfach ein Google-Profil, wählen Sie einen Aufgabenordner aus und führen Sie eine automatische Erkennung durch, um die Google-Jobliste auszuwählen.
	- UpdateChecker verbessert, Schaltfläche hinzufügen, um die neue Version automatisch herunterzuladen, zu extrahieren und das Installationsprogramm zu starten.
	- Verbesserte Synchronisationsberichte mit formatierter Ansicht.
	- Kleine Verbesserungen der Benutzeroberfläche und Layoutänderungen.
	- Link zu Hilfesite und Wiki in About Dialog hinzugefügt.
	- Verbesserte Autodiscovery in Google-Profilen und Schaltfläche zum Hinzufügen einer neuen Autodiscovery.
- Fehlerbehebungen
	- Behobener Workaround für leere Sammlungen des Synology NAS, die fälschlicherweise 404 NotFound zurückgeben. Ticket #203.
	- Löschen durchführen und neu erstellen, wenn ein Update für ein Google-Ereignis den HTTP-Fehler 403 zurückgibt. Ticket #205.
	- Protokollierung der UI der Serverressource in Synchronisierungsberichten korrigiert.
	- Falsche Behandlung von Ordnern in OutlookTaskRepository behoben.
	- Ordnungsgemäßes disposen des WebClients in UpdateChecker- und IsOnline-Prüfung.

#### 1.15.0 ####
- WARNUNG: Diese Version ändert die interne Cache-Struktur. Beim Downgrade auf eine ältere Version wird der Cache gelöscht und eine neue Anfangssynchronisierung durchgeführt!
- Neue Features
	- Verbesserte Behandlung von Uris, Verwendung der benutzerdefinierten Klasse WebResourceName anstelle von System.Uri zum Identifizieren von WebDAV-Ressourcen. Dies sollte verschiedene Probleme mit Dateinamen mit falsch codierten Sonderzeichen wie Schrägstrichen oder Leerzeichen speziell für Owncloud beheben, siehe Ticket #193 und Diskussionen.
	- Erweiterte Option für die präemptive Authentifizierung hinzugefügt und für neue Profile als Standard festgelegt, Feature-Request von Ticket #198.
	- Optionen-Tabs ziehbar gemacht.
	- Löschen von Caches, wenn sie eine andere Version als die erforderliche Version haben, und Implementieren der Cache-Konvertierung von Version 0 in 1.
	- InitialTaskEntityMatcher wurde verbessert und außerdem Start und Fälligkeitsdatum verglichen, falls dies für übereinstimmende Aufgaben verfügbar ist.
- Fehlerbehebungen
	- Setzen des PatternEndDate of Recurrence auf PatternStartDate, wenn es vor dem Start im Ereignis ein ungültiges Datum ist, um die COMException zu vermeiden. Ticket #197.
	- Task nicht in lokaler Zeitzone abschließen, COMPLETED von vtodo muss in UTC sein, Korrektur der Regression in 1.14.0 wurde vorgenommen.
	- UTC-Konvertierung in InitialEventEntityMatcher wurde vermieden und lokale Zeitzone verwendet, um Nullreferenzausnahmen aus der Dday.iCal-Bibliothek in einigen seltsamen Zeitzonenfällen zu vermeiden. (Ticket #154) Korrigiert auch den Abgleich alltäglicher Ereignisse und prüft, ob das Datum passt.
	- COMException abfangen, wenn AddressEntryUserType of Recipient abgerufen wird. Ticket 109 von Github.

#### 1.14.2 ####
- Fehlerbehebungen
	- Behebung jedes Arbeitstages und Vermeidung von INTERVAL = 0, das falsch aus dem Outlook-Objektmodell festgelegt wurde, behebt ein Problem mit bestimmten Versionen von SabreDAV / OwnCloud, wobei INTERVAL = 0 zu einem internen Serverfehler führt
	- Es wurde auch eine mögliche ArgumentException in MapRecurrence1To2 abgefangen, wenn versucht wird, AppointmentItem eines geänderten Vorkommens abzurufen.
	- Verbesserter Umgang mit DECLINED und abgesagten Meetings.
	- Präfix AppointmentItem Betreff mit "Abgebrochen:", wenn der Ereignisstatus ABBRUCH ist.
	- Verwendet die Erweiterung .vcf anstelle von .vcs für neu erstellte Vcards.
	- Verbesserte Zuordnung von Telefonnummern, Zuordnung von Outlook OtherPhoneNumber und OtherFaxNumber und Festlegen von TYPE = MAIN für PrimaryPhoneNumber.
	- Verbesserte Zuordnung von HOME- und WORK-URLs für Vcards.
	- Refactored IsOnline () überprüft, um Probleme in Proxy-Umgebungen zu vermeiden, Ticket #189.

#### 1.14.0 ####
- Neue Features
	- Überspringen der Synchronisierungsläufe. Wenn das Netzwerk nicht verfügbar ist, um in diesem Fall Fehlerberichte zu vermeiden, wurde eine allgemeine Option zum Überprüfen der Internetverbindung mit der DNS-Abfrage zu www.google.com hinzugefügt. Wenn Sie sich in einem lokalen Netzwerk befinden, ohne dns oder google.com blockiert zu haben, deaktivieren Sie diese Option.
	- Implementierte Konfigurationsoptionen für die Ereigniszuordnung zum Synchronisieren des privaten Flags mit CLASS: CONFIDENTIAL und umgekehrt, Feature-Request 15.
- Fehlerbehebungen
	- Das Mapping von Outlook-Taskdaten zu DTSTART und DUE wurde korrigiert. Für den Start wird die lokale Zeitzone und die Uhrzeit 00:00:00 verwendet, für fällige Werte 23:59:59. DURATION wird entfernt, um RFC 5545-kompatibel zu sein. Siehe Ticket #170. Verwendet auch localtime für COMPLETED anstelle von UTC, um konsistent zu sein, und korrigiert VTIMEZONE-DST-Regeln für Aufgaben.
	- Feste jährliche Wiederholung mit Intervall = 1 für Aufgaben.
	- Nicht erkannte PARTSTAT-Behandlung wie bei NEEDS-ACTION gemäß RFC 5545.
	- Zuordnung von Teilnehmern mit Typ Ressource / Raum oder unbekannter Rolle behoben, X-LOCATION der Typ Ressource zuordnen, CUTYPE = RESOURCE für Ressourcen festgelegt.
	- COMException beim Festlegen des Wiederholungsintervalls abgefangen und ungültige Termine für Termine und Aufgaben ignoriert. Ticket #174.
	- Protokollierung der UID von Ereignissen für Wiederholungsfehler behoben.
	- Vermeidung einer COMException für ungültigen Organiser in MapAttendeesAndOrganizer2To1, Überspringen des Organisators, wenn keine E-Mail und kein gültiger CN vorhanden ist.
	- In den VTIMEZONE-Definitionen vor der Deserialisierung von icaldata das Jahr 0001 durch 1970 ersetzt, da DDay.iCal ansonsten extrem langsam ist und für emClient erforderlich ist, siehe Ticket #150.

#### 1.13.2 ####
- Fehlerbehebungen
	- SetOrganizer und GetMailUrl in EventEntityMapper umgeändert, um Nullreferenzausnahmen zu vermeiden und COMExceptions abzufangen.
	- COMExceptions beim Zugriff auf die Zeitzone von AppointmentItem und Fallback auf UTC in diesem Fall abgefangen.
	- COMException abgefangen, wenn AppointmentItem einer Ausnahme nicht vorhanden ist, ignoriert diese Ausnahme, da die Änderungen nicht abgerufen werden können. Dies geschieht, wenn sich das wiederkehrende Ereignis nicht in der lokalen Outlook-Zeitzone befindet.
	- Zeilenumbrüche in newFeaturesTextBox eingestellt, um die neuen Funktionen besser lesbar zu machen, Feature-Request 24.
	- Ungültige DTEND-Werte von Ereignissen geprüft und COMException abgefangen, wenn versucht wird, EndTime festzulegen, verwendet in diesen Fällen DTSTART.
	- COMException in GetEvent Organizer() abgefangen, Probleme mit OL2007 behoben.
	- Mögliche NullReferenceExceptions in MapAttendeesandOrganizer2To1 vermieden.
	- Mögliche COMException in MapOrganizer1To2 abgefangen.
	- UriFormatException wurde auch in Map2To1 abgefangen, wenn der Server ungültige E-Mail-Adressen der Teilnehmer sendet, Ticket #168.

#### 1.13.0 ####
- Neue Features
	- Unterstützung für GMX-Kalender wurde hinzugefügt. In UTC müssen neue Ereignisse erstellt werden. Siehe Abschnitt GMX in README.
	- Konfiguration der Protokoll- und Protokollebene unter "Allgemeine Optionen" anzeigen / löschen. (Feature 22)
	- Hinzufügen von zusätzlich "1 Minute" und "2 Minuten" zu den verfügbaren Synchronisierungsintervallen nach mehrfacher Anforderung.
	- Option zum Deaktivieren der Zuordnung von Kontaktfotos in ContactMappingConfiguration hinzugefügt, da es in OL 2007 nicht ordnungsgemäß funktioniert.
- Fehlerbehebungen
	- EnsureSynchronizationContext bei Rückrufen von Outlook behebt Fehler beim Anzeigen von Synchronisationsberichten, wenn Elemente sofort nach Änderungen synchronisiert werden.
	- Keine leeren Abfragen an Repositorys durchführen, behebt HTTP 400-Fehler mit GMX.
	- Die Verwendung von PR_MESSAGE_CLASS zum Filtern von AppointmentItems / TaskItems in OutlookRepositories sollte Casting-Fehler beheben, wenn sich andere Elemente im Ordner befinden.
	- Das Layout der Tasten in MappingConfiguration und OptionsDisplay wurde korrigiert.
	- EventMappingConfiguration wurde hinzugefügt, um Ereignisse in UTC zu erstellen, die beispielsweise für GMX erforderlich sind, da die lokale Windows-Zeitzone zum HTTP 403-Fehler führt. Ticket #162.
	- System.UnauthorizedAccessExceptions in ContactEntityMapper abfangen.
	- Startcode nur einmal ausgeführt, sollte Fehler in Ticket #161 beheben.
	- Vermeidet die NullreferenceException, wenn AdressEntry des Empfängers nicht abgerufen werden kann, Ticket #163.

#### 1.12.0 ####
- Neue Features
	- Übereinstimmende hinzugefügte Entitäten bei jedem Synchronisierungslauf sollten Verdoppelungen und Fehler vermeiden, wenn dasselbe Ereignis in Server und Client hinzugefügt wird, z. eine (automatisch akzeptierte) Einladung zum Meeting.
	- Schaltfläche "Cache zurücksetzen" hinzugefügt, um den Synchronisierungscache zu löschen und eine neue anfängliche Synchronisierung mit dem nächsten Synchronisierungslauf zu starten.
	- Der zugehörige Geburtstagstermin wird gelöscht, wenn ContactItem in Outlook gelöscht wird. Feature #21.
	- Bereinigt veraltete Synchronisationsberichte mit konfigurierbarer Zeitspanne.
- Fehlerbehebungen
	- Probleme behoben, die aufgrund des Ladeverhaltens von Steuerelementen auftreten konnten.
	- Das Exportieren von DateCompleted für Tasks wurde korrigiert, laut RFC muss es sich um einen DATE-TIME-Wert handeln, siehe Ticket #156.
	- Datum wurde für Aufgaben von UTC in lokales Datum konvertiert, wenn eine Zuordnung zu Outlook vorgenommen wurde.
	- Hinzufügen von Berichten zu ToolBar-Schaltflächen für OL2007.
	- Meeting-Antwort nur aktualisiert, wenn MapAttendees in MappingConfiguration festgelegt ist.
	- Feste jährliche Wiederholung mit Intervall = 1, von Jonathan Westerholt zur Verfügung gestellter Patch, Ticket #159.
	- Zurücksetzen von "Verwenden von GlobalAppointmentID für neue Ereignisse anstelle einer zufälligen Guid, um das Verdoppeln von Ereignissen aus Einladungen für den eigenen Teilnehmer zu vermeiden". Dies führte zu Problemen mit Google, wenn gelöschte Ereignisse mit derselben UID wiederhergestellt wurden.
	- Bereinigt veraltete Synchronisationsberichte.
	- Kontextmenü hinzugefügt, mit dem das Cache-Verzeichnis auch für den Google-Profiltyp geöffnet werden kann.
	- Die neue Registerkarte in OptionsForm ausgewählt, wenn ein neues Profil hinzugefügt wird.

#### 1.11.0 ####
- Neue Features
	- Erweiterte Protokollierung und konfigurierbare Synchronisationsberichte nach jedem Synchronisierungslauf. Sie können konfigurieren, ob Berichte für jeden Synchronisierungslauf erstellt werden sollen oder nur, wenn Fehler oder Warnungen auftreten und ob die Berichte sofort nach dem Synchronisierungslauf angezeigt werden sollen. Sie können Berichte auch im Berichtsfenster löschen oder komprimieren.
	- Unterstützung für Zoho Calendar, Patch von Suki Hirata <thirata@outlook.com>
- Fehlerbehebungen
	- Übliche Mapping-Funktionen für Ereignisse und Aufgaben werden herausgefiltert und die Priorität 1-9 gemäß RFC5545 zugeordnet 

#### 1.10.0 ####
- Neue Features
	- Möglichkeit hinzugefügt, Serverkalenderfarbe auf ausgewählte Kategorienfarbe einzustellen
	- Ermöglicht die Angabe des Tastenkürzels der Kategorie und die Verbesserung der Benutzeroberfläche von EventMappingConfiguration
	- Zeitplanungskonfigurationsoptionen zu EventMappingConfiguration hinzugefügt und RSVP für Teilnehmer festgelegt. (Sie können angeben, ob Sie SCHEDULE-AGENT einstellen möchten: CLIENT oder X-SOGO-SEND-APPOINTMENT-NOTIFICATIONS: NO für SOGo.)
- Fehlerbehebungen
	- Es wurden einfache Anführungszeichen in der Kategorie-Filterzeichenfolge mit Escapezeichen versehen und in EventMappingConfiguration validiert. Es darf keine Kommas oder Semikola enthalten, um Ausnahmen zu vermeiden.
	- Verwenden des DASL-Filters anstelle der JET-Syntax zum Beheben der Kategoriefilterung für OL 2010 (64-Bit)
	- Berücksichtigung relativer Weiterleitungen. (behebt die Autodiscovery für einige Server basierend auf cpanel / horde)
	- UTC-Konvertierung aus der Dday.iCal-Bibliothek für die bevorstehende Erinnerungsprüfung vermeiden.
	- Verwenden von GlobalAppointmentID für neue Ereignisse anstelle einer zufälligen Guid, um das Verdoppeln von Ereignissen aus Einladungen für den eigenen Teilnehmer zu vermeiden.
	
#### 1.9.0 ####
- Neue Features
	- Zuordnen von CalDAV-Serverfarben zu Outlook-Kategorienfarben. Sie können die Kategoriefarbe manuell auswählen oder die Farbe vom Server abrufen und der nächsten unterstützten Outlook-Farbe zuordnen.
- Fehlerbehebungen
	- Verwendet keine umgebungsspezifischen Zeilenumbrüche für Daten, die an den Server gesendet werden.
	- Uris, die in XML-Dokumente eingefügt werden, werden escaped.
	- Nicht verwendete calDavReadWriteTimeout wurde aus der Konfiguration entfernt.

#### 1.8.0 ####
- Neue Features
	- Filterung auf der Outlook-Seite hinzugefügt, so dass mehrere CalDAV-Kalender über eine Outlook-Kategorie in einem Outlook-Kalender synchronisiert werden können
	- Mapping-Konfigurationsoptionen für Kontakte hinzugefügt (Mapping von Geburtstagen aktivieren oder deaktivieren, Feature #12).
	- Entity-Version (Etag) beim Löschen bereitstellen und If-Match-Header festlegen
	- Option hinzugefügt, um gerade anstehende Erinnerungen zu synchronisieren.
	- Verbesserungen bei der AutoErmittlung: Ignoriert XML-Ausnahmen während der AutoErmittlung (wird für einige falsche owncloud-Serverpfade benötigt) und versucht, den Hostnamen auch ohne Pfad zu verwenden, wenn well-known nicht verfügbar, behebt die AutoErmittlung für posteo (https://posteo.de:8443), Anzeigen, wenn keine Ressourcen über bekannte URLs gefunden wurden.
- Fehlerbehebungen
	- Filtert SOGo-Vlists (contenttype text / x-vlist) heraus, da diese momentan nicht analysiert werden können. Dadurch wird vermieden, dass Vlisten mit einer leeren Vcard synchronisiert werden und die Vlist zerstört wird, wenn Sie wieder mit SOGo synchronisieren.
	- Beschneidet Kategorienamen für Ereignisse, Aufgaben und Kontakte bei der Zuordnung zu caldav.
	- Verwendet ENCODING=b anstelle von BASE64 gemäß der vcard 3.0-Spezifikation für binäre Attribute.

#### 1.7.0 ####
- Neue Features
	- GUI-Neugestaltung für Google-Profile zur Vereinfachung der Einrichtung und automatischen Erkennung von Google-Konten. Beim Erstellen eines neuen Synchronisierungsprofils können Sie zwischen einem generischen CalDAV / CardDAV- und einem Google-Profil wählen. Für Google reicht es aus, die E-Mail-Adresse einzugeben. Die automatische Erkennung versucht, nach der Konfiguration von OAuth nach Ressourcen zu suchen.
	- Verbesserungen der Autodisovery-Logik.
	- Kalenderfarben werden jetzt in "AutoErmittlung" angezeigt. SelectResourceForm. Das Synchronisieren von Farben mit Outlook-Kategorien ist in Arbeit.
	- Gruppenbeschriftung im Menüband hinzugefügt und ScreenTips und SuperTips festgelegt.
- Fehlerbehebungen
	- Löscht alte Telefonnummern vor dem Update, behebt die Verdoppelung der Heimat- und Arbeitsnummern, Ticket #142.
	- Änderungen der TabIndex-Ordnung, Ticket #140.
	- Löscht den Profilcache auch bei einer Änderung des Benutzernamens, hilft bei der Änderung der Google-ID, Ticket #141.
	- Löscht den Profil-Cache auch bei einer Änderung oder Deaktivierung des Zeitbereichsfilters. Ticket #138.
	- Korrigiert calDavDateTimeFormatString und verwendet heute anstelle von jetzt Timer-Filter.
	- Fügt Etags an Systemgrenzen fehlende Anführungszeichen hinzu.

#### 1.6.0 ####
- Neue Features:
	- Stellt die Entitätsversion (etag) für das Update bereit und setzt den If-Match-Header
	- Implementiert einen eigenen vCardImprovedWriter, um Serialisierungsprobleme von vCardStandardWriter zu beheben und kostspielige Regex-Workarounds zu vermeiden
	- Fügt TYPE = HOME für persönliche Homepages hinzu
- Fehlerbehebungen:
	- Behebt die Zuordnung von HomeFaxNumber für Vcards, Ticket #134.
	- Protokolliert Ausnahmen während Verbindungstests und versucht nicht, Kalender oder Adressbücher für leere Homesets aufzulisten. Behebt das Problem #82 von Github.
	- Behebt GetContacts für Yandex, da Yandex selbst mit einem etag das Verzeichnis selbst zurückgibt.
	- Verbesserte Fehlerbehandlung.
	- Behebt die für Yandex-Vcards erforderlichen TYPE-Subeigenschaften.
	- Stellt sicher, dass Etag beim Hinzufügen in Entity-Repositorys in doppelte Anführungszeichen gesetzt wird, da einige Caldav-Server wie Yandex ETAGs ohne Anführungszeichen senden.
	
#### 1.5.4 ####
- Neue Features:
	- Allgemeine Optionen in der Benutzeroberfläche zum Ändern von SSL-Optionen und anderen globalen Einstellungen
	- Option hinzugefügt, um Statusinformationen in Appdata\Roaming statt Local zu speichern. Ticket #125.
	- Mapping-Konfigurationsoptionen für Termine hinzugefügt (Mapping von Erinnerungen, Teilnehmern oder Beschreibungstext aktivieren oder deaktivieren).
	- Spendenlink zu About Dialog hinzugefügt.
	- Kontextmenü zu Optionen hinzugefügt, wodurch das Cache-Verzeichnis geöffnet werden kann.
- Fehlerbehebungen:
	- Die Zuordnung der ORG-Eigenschaft zu CompanyName und der Abteilung für Vcards wurde korrigiert. Ticket #127.
	- Fängt COM-Ausnahmen ab, wenn versucht wird, ungültige Outlook-Elemente in Repositorys hinzuzufügen, Ticket #130.
	- Korrekturen für das Ausblenden relativer URLs für Entitäts-IDs, Ticket #129.

#### 1.5.3 ####
- Vermeidet Nullreferenzausnahmen, die die Synchronisierung verhindert, wenn in der Konfigurationsdatei keine Proxy-Einstellungen vorhanden sind, Fehler #124.
- Richten Sie den richtigen Mime-Text / Vcard ein, wenn Sie Kontakte platzieren.

#### 1.5.2 ####
- Löscht den Profil-Cache. Wenn der Outlook-Ordner oder der Caldav-Server-URL geändert wird, Ticket #117. Verhindert den Datenverlust und erzwingt in solchen Fällen eine neue Anfangssynchronisierung.
- Fix für Linebreak-Probleme von OpenX-change, zusammengeführt von Pull-Request #79, danke an bjoernbusch.

#### 1.5.1 ####
- Neue Features:
	- Unterstützung für die Proxy-Konfiguration in der GUI, um manuelle Proxy-Einstellungen festzulegen und Basic Auth- und NTLM-Proxies zuzulassen.
- Fehlerbehebungen:
	- Verwendet ContactItemWrapper und lädt Elemente erneut, um eine zweite Synchronisierung mit einer geänderten Änderungszeit in Outlook zu vermeiden, siehe Ticket #111.
	- Verhindert das Senden von Meeting-Antworten, wenn das Meeting selbst organisiert ist.
	- Vermeidet unnötige Verbindungstests während der automatischen Erkennung, behebt die automatische Erkennung von Google CardDAV.

#### 1.5.0 ####
- Neue Features:
	- Autodiscovery für CardDAV-Adressbücher
	- Änderungsgesteuerte Teilsynchronisierung (Terminelemente sofort nach Änderung in Outlook synchronisieren).
	- Unterstützt den Yandex CalDAV-Server.
	- Viele Verbesserungen für CardDAV.
	- Fügt OAuth Scope für Google CardDAV hinzu.
- Fehlerbehebungen:
	- Korrigieren der Synchronisierung von Kontaktnotizen mit Umlauten.
	- Deaktiviert TimeRangeFiltering, wenn der Kontaktordner ausgewählt wird.
	- Stellt sicher, dass die FN von vcard nicht leer ist, da es ein MUST-Attribut ist (Bug #109).
	- Mappe ZugriffKlassifizierung von Vcards.
	- Stellt sicher, dass die vcard-UID auch in Updates nicht leer ist.
	- Überspringt die Adressbuchsammlung selbst, wenn Vcards von Owncloud abgerufen werden.
	- Verwendet eine vorhandene UID für Dateinamen in PUT-Anforderungen.
	- Ruft ETAG über propfind ab, wenn es nicht im Header zurückgegeben wird, um Nullreferenz zu vermeiden.
	- Überprüft auch das Schreibrecht beim Erkennen von Kalenderzugriffsrechten.
	- Ordnet andere vcard-telefonnummern zu.
	- Erkennt RevisionDate in vcard-Updates, falls verfügbar (Fehler #111).
	- Behebt InitialEventEntityMatcher, wenn DTEnd null ist (Fehler #110).
	- Filtert nur ContactItems in ContactRepository GetTable, um COM-Ausnahmen zu vermeiden, da derzeit keine Gruppen oder Verteilerlisten synchronisiert werden.
	- Vermeidet Ausnahmen beim automatischen Erkennen von DoubleClick EventHandler, wenn Sie auf die Kopfzeile klicken.

#### 1.4.5 ####
- Behebt Regex in der Problemumgehung für die DDay.iCal-Zeitzonenanalyse, sollte Bug #105 für die Synchronisierung mit Owncloud/Davdroid beheben.
- Überarbeitung der Exdate-Generierung, um einige seltsame Elemente der Outlook Exception Collection zu umgehen, Fehler #91 und andere Wiederholungsausnahmen mit komplexen Mustern zu beheben.

#### 1.4.4 ####
- Ein weiterer Fix für die VTIMEZONE-Definition für Google, behebt hoffentlich die Fehler mit den Zeitzonen in den USA und in Moskau.
- Fügt eine UID hinzu, wenn vCard erstellt wird. Die RFC-UID ist obligatorisch.
- Ein weiterer Fix für Wiederholungsausnahmen und -daten für Bug #101.
- Behandelt Ausnahmen beim Aktualisieren von Outlook-Ordnern oder beim Laden des Profils beim Start.

#### 1.4.3 ####
- Eine weitere DDay.iCal Workaround, um die TIMEZONE-Generierung für Zeitzonen mit sich ändernden DST-Regeln wie Moskau oder Kairo festzulegen.
- bugfix: Verwendet die Zeitzonen-ID zum Vergleich und vermeidet den Export von doppelten TIMEZONE-Definitionen.
- Optionen hizugefügt, um Keepalive nicht zu verwenden und ungültige Header zu akzeptieren.

#### 1.4.2 ####
- Verwendet StartTimeZone und EndTimeZone von Ereignissen, wenn sie sich von der Systemzeitzone unterscheiden.
- Ordnet Server-Zeitzonen Windows-Zeitzonen zu und legt die Zeit in StartTimeZone fest, um wiederkehrende Ereignisse zu beheben, die DST-Verschiebungen umfassen (behebt Fehler #94).
- Behebt viele Fälle, in denen Mapping-Wiederholungsausnahmen auftreten und über DST-Änderungen oder wenn sich Outlook und Server in unterschiedlichen Zeitzonen befinden.
- Fix für Bug #101, falsche Exdate-Berechnung.
- Korrektur der ursprünglichen Datumsberechnung für Wiederholungsausnahmen, wenn sie sich am Vortag in UTC befinden.
- Exportiert keine historischen Zeitzonen vor 1970.

#### 1.4.1 ####
- Fügt die Zuordnung von IMAddress für Kontakte hinzu.
- Fügt Zuordnung von Kontaktnotizen hinzu.
- Behebt die vcard-Zuordnung für Faxnummern und andere Adressarten.
- Fügt einen Doppelklick-Ereignishandler für die AutoErmittlung hinzu.
- Das Verhalten von TestConnection wurde korrigiert, so dass das Abbrechen der automatischen Erkennung funktioniert.
- Fügt das Mapping von Kontaktfotos hinzu.
- Zuordnung von FormattedName für Kontakte.
- Fügt Mapping für X509-Zertifikate für Kontakte (z. B. S / MIME) zum Attribut vCard KEY hinzu.
- Implementiert EmailAddress Mapping für Exchange-Kontakte (Typ "EX").

#### 1.4.0 ####
- Anfängliche CardDAV-Unterstützung zum Synchronisieren von Kontakten (Alpha).
- Refactoring des Autodiscovery.
- Korrigiert Optionen und Schaltflächen für Outlook 2007.

#### 1.3.4 ####
- Fügt Unterstützung für Outlook 2007 hinzu, Credits an PierreMarieBaty (Pull-Request #67).
- Refactoring des Autodiscovery.
- Refactoring von URL-Validierung und Testeinstellungen
- Option hinzugefügt, um Synchronisierungseinstellungen automatisch zu korrigieren.
- Verhindert ArgumentOutOfRangeException in der E-Mail-Teilzeichenfolge des Teilnehmers

#### 1.3.3 ####
- Behebt den Erinnerungszeitwert.

#### 1.3.2 ####
- Behebt Erinnerungen für Google
- Klärt die Testeinstellungen für schreibgeschützte Ressourcen und legt den Synchronisationsmodus fest

#### 1.3.1 ####
- Fügt einen Guard hinzu, um zu verhindern, dass ein SynchronizationWorker mehrmals ausgeführt wird.
- Korrigiert die Prioritätszuordnung für Aufgaben.
- Erste Implementierung wiederkehrender Aufgaben.

#### 1.3.0 ####
- Fügt Unterstützung für die automatische Erkennung von CalDAV-URLs hinzu.
- Problemumgehung: Da DDay.iCal keine Ereignisse analysieren kann, die unsortierte TimeZoneComponents enthalten, müssen diese vor der Analyse sortiert werden.

#### 1.2.2 ####
- Fehler in InitialEventEntityMatcher behoben, der zu einer Duplizierung von Ereignissen führte, wenn ein Profil gelöscht und neu erstellt wurde.
- Fängt UriFormatExceptions in Teilnehmer- und Organisatorwerten aus CalDav ab.
- Enthält eine Antwortnachricht in Ausnahmefällen, wenn ein Protokollfehler auftritt.

#### 1.2.1 ####
- HttpClient-Umleitungsproblem behoben, das Auswirkungen auf die Zimbra-Integration hatte.

#### 1.2.0 ####
- Option hinzugefügt, um die neue Version zu ignorieren und auf das nächste Update zu warten.
- Problemumgehung für Group Office hinzugefügt, die leere VALARMs toleriert.
- SynchronizeNowButton während der Synchronisierung deaktiviert.
- Deaktiviert TestConnectionButton, während der Test ausgeführt wird.
- Richtige Entsorgung von Webnachrichten hinzugefügt.

#### 1.1.0 ####
- Unterstützung für Google OAuth.
- Führt alle Weboperationen im Hintergrund aus.

#### 1.0.4 ####
- Korrigiert den TimeRange-Filter für Ereignisse.

#### 1.0.3 ####
- Fügt eine Funktion hinzu, die prüft, ob eine neuere Version verfügbar ist (Ticket 61).

#### 1.0.2 ####
- Bugfix: UID beim Aktualisieren eines Events beibehalten.

#### 0.99.16 ####
- Filterung für Zeitbereich optional.

#### 0.99.15 ####
- Implementiert app.config-Optionen zum Deaktivieren der SSL/TLS-Zertifikatüberprüfung und zum Aktivieren/Deaktivieren von SSL3/TLS12.

#### 0.99.14 ####
- Verwendet BYSETPOS auch für andere Instanzen aus Outlook-Korrekturen erster/zweiter/... Wochentag/Wochenende-Tag im Monat.

#### 0.99.13 ####
- Verwendet BYSETPOS -1, um die monatlichen/jährlichen Wiederholungen des letzten Arbeitstages in Outlook zu beheben.
- Fügt einen UserAgent-Header zur Anforderung hinzu. (z.B. von BAIKAL benötigt).

#### 0.99.12 ####
- Behebt Fehler: Die Zuordnung ist falsch, wenn das Master-Ereignis nicht das erste Ereignis in der CalDAV-Ressource ist.
- Behebt das Protokollierungsproblem
- Behebt die Wiederholung von Outlook für den letzten Wochentag im Monat

#### 0.99.10 ####
- Holt Etag vom Server, wenn es nicht in einer Update-Antwort enthalten ist.
- CalDavWebClient wird aus CalDavDataAccess herausgerechnet.

#### 0.99.9 ####
- Löscht den Ordner in OptionDialog.
- Ruft GarbageCollector nach jedem Synchronizer-Lauf auf, um Probleme mit Wiederholungsausnahmen zu vermeiden.

#### 0.99.8 ####
- Behebt einige Probleme mit dem Zeitlimit von Caldav, um WebRequests ordnungsgemäß zu beseitigen.

#### 0.99.7 ####
- Überprüft, ob die Organiseradresse leer ist, um eine COM-Ausnahme in GetMailUrl zu vermeiden.
- Behebt die Exdate-Berechnung für verschobene Wiederholungsausnahmen.

#### 0.99.6 ####
- Fängt 404-Antwort für leere Caldav-Repositorys von Synology ab.
- Etwas generisches Refactoring.

#### 0.99.4 ####
- Entsorgt Outlook-Ordner nach dem Gebrauch.
- Weitere Fehlerbehebungen für Wiederholungsausnahmen:
- Wenn Outlook eine geänderte Ausnahme und eine gelöschte Ausnahme mit demselben Originaldatum bereitstellt, wird die gelöschte Ausnahme verworfen.
- Verhindert das Überspringen von Terminausnahmen während des Verschiebens.
- Vertauscht die Handhabung von ExeptionDates und RecurrenceIDs.
- Klärt den Protokollierungsfehler.
- Überprüft, ob im Ziel bereits eine neue Ausnahme vorhanden ist.

#### 0.99.3 ####
- Behebt die Definition der Zeitzone.

#### 0.99.2 ####
- Behebt Zeitzonenprobleme bei der Synchronisierung von Outlook mit CalDav für wiederkehrende Ereignisse.
- Fügt den neuen CalDav-Ereignissen lokale Zeitzoneninformationen hinzu.
- Legt das Start- und Enddatum in der lokalen Zeitzone anstelle von utc für CalDav-Ereignisse fest.
- Behebt wiederkehrende Ereignisse, die sich über die Sommerzeit hinweg erstrecken.
- Berechnet Exception-Daten für Wiederholungsausnahmen.
- Behebt die Datumsberechnung für GetOccurence.
- Beachtet BYSETPOS für monatliche und jährliche Wiederholungsregeln.

#### 0.99.1 ####
- Verbesserte Überprüfung der Kalender-URL im Dialogfeld "Optionen".

#### 0.99 ####
- Korrekturen für Google.

#### 0.98 ####
- Fügt SCHEDULE-AGENT = CLIENT für den Organisator hinzu, um zu vermeiden, dass Einladungen in SOGo zweimal gesendet werden, siehe Ticket 45.

#### 0.97.8 ####
- Fügt die Debug-Protokollierung für Caldav-Anforderungen hinzu.

#### 0.97.7 ####
- Weitere Korrekturen für den Austausch von E-Mail-Adressen für Teilnehmer und eine bessere Protokollierung.
- Fängt eine COM-Ausnahme für nicht gefundene Wiederholungsausnahmen ab.

#### 0.97.6 ####
- Weitere Korrekturen für GetMailUrl.
- Verbesserte Handhabung von WebExceptions.

#### 0.97.5 ####
- Korrekturen für GetMailUrl für Exchange und GAL.
- Behebt WebException-Ausnahmen.
- Der Antwortheader "location" darf eine relative Uri enthalten.

#### 0.97.3 ####
- Legt das Intervall für jährliche Wiederholungsregeln fest.

#### 0.97.2 ####
- Fügt einen Synchronisationskontext hinzu, falls er fehlt.
- Korrekturen für die Task-Synchronisierung, wenn Start- und Fälligkeitsdatum gleich sind.

#### 0.97.1 ####
- Vertauscht die Standardwerte für die Synchronisierungszeiträume im Dialogfeld "Optionen".
- Fängt Ausnahmen ab, wenn die PR_SMTP_ADDRESS-Eigenschaft nicht verfügbar ist.
- Stellt den Besprechungsstatus auf Nicht-Treffen ein, wenn nur der eigene Organisator und keine Teilnehmer anwesend sind.

#### 0.97 ####
- Erste Task-Synchronisierungsunterstützung (Alpha)
- Caldav-Anforderungen asynchron machen, Outlook-Benutzeroberfläche reagiert während Caldav-Abrufanforderungen
- Einige Wiederholungskorrekturen
- Verbessert die Handhabung des gesamten Fortschritts

#### 0.96 ####
- Korrekturen für Google.

#### 0.95.1 ####
- Behebt die Einstellung der SMTP-Adresse für Exchange-Benutzer.

#### 0.95 ####
- Implementiert 301.302 Weiterleitungen zur Unterstützung von Zimbra.
- Fügt Validierung für Optionen hinzu.

#### 0.94 ####
- Behebt eine Ausnahme in der anfänglichen Zuordnung, wenn der Betreff oder die Zusammenfassung des Ereignisses null ist

## Benutzerdokumentation ##

Nach der Installation des Plugins wird in Outlook ein neues Menüband mit dem Namen 'Caldav Synchronizer' mit 6 Menüelementen hinzugefügt.
- Jetzt synchronisieren
- Synchronisationsprofile
- Allgemeine Optionen
- Über
- Berichte
- Status

Zur Erleichterung der Zugänglichkeit unterstützt das Menüband auch Tastentipps, die über die ALT-Taste gefolgt von CDS und SN, SP, GO, AB, RE bzw. ST für die 6 Elemente verfügbar sind.

Verwenden Sie das Dialogfeld "Synchronisationsprofile", um verschiedene Synchronisationsprofile zu konfigurieren. Jedes Profil ist für die Synchronisierung eines Outlook-Kalender-/Aufgaben- oder Kontaktordners mit einem Remoteordner eines CalDAV-/CardDAV-Servers verantwortlich.

Ab Version 2.15.0 sind die erweiterten Konfigurationseinstellungen standardmäßig ausgeblendet. Sie können sie aktivieren, indem Sie auf *Erweiterte Einstellungen anzeigen* klicken, und sie wieder deaktivieren, indem Sie auf *Erweiterte Einstellungen ausblenden* klicken. Das Standardverhalten kann auch als allgemeine Option konfiguriert werden, siehe unten.

Die Symbolleiste im linken oberen Teil bietet die folgenden Optionen:

- **Neues Profil hinzufügen** fügt ein neues leeres Profil hinzu
- **Mehrere Profile hinzufügen** Massenprofilerstellung, um mehrere Profile gleichzeitig hinzuzufügen und den Ordner für jede erkannte Serverressource (Kalender, Adressbuch und Aufgabe) auszuwählen.
- **Ausgewähltes Profil löschen** löscht das aktuelle Profil
- **Ausgewähltes Profil kopieren** kopiert das aktuelle Profil in ein neues
- **Ausgewähltes Profil nach oben verschieben** Reihenfolge in der Baumansicht ändern *(nur in den erweiterten Einstellungen)*
- **Ausgewähltes Profil nach unten verschieben** Reihenfolge in der Baumansicht ändern *(nur in den erweiterten Einstellungen)*
- **Datenverzeichnis des ausgewählten Profils öffnen** Verzeichnis mit zwischengespeicherter Beziehungsdatei zum Debuggen im Explorer anzeigen *(nur in den erweiterten Einstellungen)*
- **Cache löschen** Den Sync-Cache löschen und mit dem nächsten Sync-Lauf eine neue Anfangssynchronisierung starten.
- **Alle Knoten erweitern** Alle Knoten in der Strukturansicht erweitern, standardmäßig aktiviert, können aber in den allgemeinen Optionen *geändert werden (nur in den erweiterten Einstellungen)*
- **Alle Knoten ausblenden** Alle Knoten in der Baumansicht *ausblenden (nur in den erweiterten Einstellungen)*
- **Profile in Datei exportieren** und
- **Profile aus Datei importieren** Siehe Profilimport / -export

Beim Hinzufügen eines neuen Profils können Sie zwischen einem generischen CalDAV-/ CardDAV-, einem Google-Profil zur Vereinfachung der Google-Profilerstellung und vordefinierten CalDAV-/CardDAV-Profilen für iCloud Calendar und Kontakte, SOGo, Fruux, Posteo, Yandex, GMX, Sarenet, Sehenswürdigkeiten, Cosy Cloud, Nextcloud, mailbox.org, Open-Xchange, EasyProject, Web.de, SmarterMail, Mail.de, Kolab, Swisscom-Adressbücher, EGroupware und FastMail auwählen, bei denen bereits die DAV-URL für die automatische Erkennung eingetragen ist.

Die folgenden Eigenschaften müssen für ein neues generisches Profil festgelegt werden:

- *Profilname*: Ein beliebiger Name für das Profil, der in der Baumansicht angezeigt wird.
- *Outlook-Einstellungen*:
- **Outlook-Ordner:** Outlook-Ordner, der für die Synchronisierung verwendet werden soll. Sie können einen Kalender, einen Kontakt oder einen Aufgabenordner auswählen. Je nach Ordnertyp muss der entsprechende Serverressourcentyp in den Servereinstellungen verwendet werden.
- **Elemente sofort nach Änderung synchronisieren** Einen Teil-Synchronisationslauf sofort nach dem Erstellen, Ändern oder Löschen eines Elements in Outlook auslösen (mit einer Verzögerung von 10 Sekunden).
- *Server Einstellungen*:
- **DAV-URL:** URL des entfernten CalDAV- oder CardDAV-Servers. Sie sollten hier aus Sicherheitsgründen eine HTTPS-Verbindung verwenden! Die URL muss mit einem **/** enden, z. **https://myserver.com/**
- Wenn Sie nur über ein selbstsigniertes Zertifikat verfügen, fügen Sie das selbstsignierte Zertifikat den vertrauenswürdigen Stammzertifizierungsstellen des lokalen Computers hinzu. Sie können das Zertifikat importieren, indem Sie die MMC als Administrator ausführen. Wenn dies fehlschlägt, siehe Abschnitt *'Erweiterte Optionen'*
- **Benutzername:** Benutzername, um eine Verbindung zum CalDAV-Server herzustellen
- **Passwort:** Passwort für die Verbindung. Das Passwort wird verschlüsselt in der Konfigurationsdatei der Option gespeichert.
- **IMAP / POP3-Kontokennwort verwenden** Anstelle des Kennworts können Sie das IMAP / Pop3-Kennwort aus dem Outlook-Konto verwenden, das dem Ordner zugeordnet ist. Das Kennwort wird aus dem Windows-Registrierungseintrag des Outlook-Profils abgerufen. *(nur in erweiterten Einstellungen)*
- **WebDAV-Synchronisierung verwenden** WebDAV-Sync ist eine Protokollerweiterung, die in RFC 6578 definiert ist und nicht von allen Servern unterstützt wird. Test- oder Discovery-Einstellungen prüfen, ob dies unterstützt wird. Diese Option kann die Erkennung von Serveränderungen erheblich beschleunigen, schließt jedoch die Verwendung des Zeitbereichsfilters aus. *(nur in erweiterten Einstellungen)*
- **E-Mail-Adresse:** E-Mail-Adresse des Kalenderbesitzers, die als Remote-Identität für den CalDAV-Server verwendet wird, zur Identifizierung des tatsächlichen Organisators von Meetings und als Organisator anstelle der Outlook-Identität, wenn die Planungsoption *Für Serveridentität handelt* aktiviert ist. Falls verfügbar, wird die E-Mail-Adresse während der *Test- oder Erkennungseinstellungen* automatisch erkannt. Wenn die DAV-URL leer ist, kann die E-Mail-Adresse auch für die automatische Erkennung über DNS-Lookups verwendet werden, siehe Abschnitt Automatische Erkennung.
- **DAV-Ressource erstellen** Sie können Server-DAV-Ressourcen (Kalender oder Adressbücher) hinzufügen. Sie können den Anzeigenamen der Ressource konfigurieren und festlegen, ob die URL mit einer zufälligen Zeichenfolge oder dem Anzeigenamen erstellt werden soll. Bei Kalendern können Sie auch die Serverkalenderfarbe ändern. *(nur in erweiterten Einstellungen)*

- *Sync-Einstellungen*:
	- Synchronization settings
		- **Outlook -> Server (Replicate):** syncronize everything from Outlook to the server (one way)
		- **Outlook <- Server (Replicate):** synchronize everything from the server to Outlook (one way)
		- **Outlook -> Server (Merge):** synchronize everything from Outlook to the server but don't change events created on the server
		- **Outlook <- Server (Merge):** synchronize everything from the server to Outlook but don't change events created in Outlook
		- **Outlook <-> Server (Two-Way):** Two-Way synchronization between Outlook and the server with one of the following conflict resolution
	- Conflict resolution (only used in Two-Way synchronization mode and only available in *advanced settings*)
		- **Outlook Wins:** If an event is modified in Outlook and in the server since last snyc, use the Outlook version. If an event is modified in Outlook and deleted in the server since last snyc, also use the Outlook version. If an event is deleted in Outlook and modified in the server, also delete it in the server.
		- **Server Wins:** If an event is modified in Outlook and in the server since last snyc, use the server version. If an event is modified in Outlook and deleted in the server since last snyc, also delete it in Outlook. If an event is deleted in Outlook and modified in the server, recreate it in Outlook.
		- **Automatic:** If event is modified in Outlook and in the server since last snyc, use the last recent modified version. If an event is modified in Outlook and deleted in the server since last snyc, delete it also in Outlook. If an event is deleted in Outlook and modified in the server, also delete it in the server
	- **Synchronization interval (minutes):** Choose the interval for synchronization in minutes, if 'Manual only' is choosen, there is no automatic sync but you can use the 'Synchronize now' menu item.
	- **Perform synchronization in chunks** and
	- **Chunk size** perform CalDAV/CardDAV sync in chunks with configurable chunk size to avoid OutOfMemoryEceptions, enabled by default because of lower memory consumption for huge resources. *(only in advanced settings)*
	- **Use time range filter** and
	- **Synchronization timespan past (days)** and
	- **Synchronization timespan future (days)** *(only in advanced settings)* For performance reasons it is useful to sync only a given timespan of a big calendar, especially past events are normally not necessary to sync after a given timespan. But be aware that Outlook and Google and some other CalDAV servers calculate the intersection with the time-range differently for recurring events which can cause doubled or deleted events, so it is recommended to select a time-range which is larger than the largest interval of your recurring events (e.g. 1 year for birthdays). You can't use the time range filter together with WebDAV collection sync.

- **Is active checkbox in the tree view** If deactivated, current profile is not synced anymore without the need to delete the profile.

If you expand the tree view of the profile you can configure network and proxy options and mapping configuration options. *(only in advanced settings)*

- **Network and proxy options**: Here you can configure advanced network options and proxy settings. 
	- **Close connection after each request** Don't use KeepAlive for servers which don't support it. 
	- **Use Preemptive Authentication** Send Authentication header with each request to avoid 401 responses and resending the request, disable only if the server has problems with preemptive authentication.
	- **Force basic authentication** Set basic authentication headers to avoid problems with negotiation or digest authentication with servers like OS X. This is only recommended if you use a secure HTTPS connection, otherwise passwords are sent in cleartext.
	- **Use System Default Proxy** Use proxy settings from Internet Explorer or config file, uses default credentials if available for NTLM authentication.
	- **Use manual proxy configuration** Specify proxy URL as `http://<your-proxy-domain>:<your-proxy-port>` and optional Username and Password for Basic Authentication.
	
- **Mapping Configuration**: Here you can configure what properties should be synced.
	- For appointments you can choose if you want to map reminders (just upcoming, all or none) and the description body.
	- *Export html description X-ALT-DESC converted from RTF Body* If enabled, convert formatted RTF Body of Outlook appointment to html and export it as X-ALT-DESC property. The RTF to html conversion is experimental, inline images and some formatting properties can't be converted! Be aware that some servers like Google Calendar drop this attribute!
	- *Set RTF Body from X-ALT-DESC html description* If enabled, convert X-ALT-DESC description html property to RTF and set Outlook appointment RTF Body. The html to RTF conversion is experimental, not all html formatting options can be converted! This overwrites also the plaintext Body!
	- *Timezone settings* See section Timezone mapping below.
	- *Use GlobalAppointmentID for UID attribute:* Use Outlook GlobalAppointmendID instead of random Guid for UID attribute in new CalDAV events. This can avoid duplicate events from invitations.
	- In *Privacy settings* you can configure if you want to map Outlook private appointments to CLASS:CONFIDENTIAL and vice versa. This could be useful for Owncloud for example, if you share your calendar with others and they should see start/end dates of your private appointments. You can also map all CLASS:PUBLIC events to Outlook private appointments. And for Google calendar it is useful to map all Outlook public events to default visibility instead of PUBLIC.
	- In *Scheduling settings* you can configure if you want to map attendees and organizer and if notifications should be sent by the server. 
	- Use *Don't send appointment notifications for SOGo servers and SCHEDULE-AGENT=CLIENT for other servers if you want to send invitations from Outlook and avoid that the server sends invitations too, but be aware that not all servers (e.g. Google) support the SCHEDULE-AGENT=CLIENT setting.
	- Use *Act on behalf of server identity* to set the server identity (Email Address in the server settings of the sync profile) as the organizer of newly created meetings and the Outlook identity acting on behalf with the SENT-BY property. This can be useful when Outlook and server identity do not match to avoid invites sent by the wrong email or if meetings are created in a shared calendar on behalf of the calendar owner.
	- In *Outlook settings* you can also define a filter category so that multiple CalDAV-Calendars can be synchronized into one Outlook calendar via the defined category (see Category Filter and Color below).
	- *Cleanup duplicate events after each sync run:* removes duplicate Outlook appointments based on start,end and subject of the events after each sync run, be aware of possible performance penalties with this option enabled.
	- For contacts you can configure if birthdays should be mapped or not. If birthdays are mapped, Outlook also creates an recurring appointment for every contact with a defined birthday.  Similar, you can configure if anniversarys should be mapped or not.
	- You can also configure if contact photos should be mapped or not. Contact photo mapping from Outlook to the server doesn't work in Outlook 2007. You can also add an option to not overwrite the contact photo in Outlook when it changes on the server, which could happen due to other mobile clients reducing the resolution for example.
	- Don't overwrite FileAs in Outlook uses the Outlook settings for FileAs and doesn't overwrite the contact FileAs with the FN from the server.
	- Fix imported phone number format adds round brackets to the area code of phone numbers, so that Outlook can show correct phone number details with country and area code, e.g. +1 23 45678 is mapped to +1 (23) 45678.
	- Map OutlookEmailAddress1 to WORK instead of HOME, enable when you need to change the order of email address mapping.
	- Write IM addresses as IMPP attributes. If enabled IMPP is used instead of X-AIM,X-ICQ,X-JABBER etc. for writing Instant messenger addresses in vCards.
	- Default IM protocol. Choose the default IM service type protocol which will be added to the chat address field from Outlook when writing vCards, defaults to AIM. 
	- Map Distribution Lists enables the sync of contact groups / Distribution Lists, right now the DAV contact group format SOGo VLIST, vCards with KIND:group or iCloud groups are available, see **Distribution Lists** below.
	- For tasks (not for Google task profiles) you can configure if you want to map reminders (just upcoming, all or none), the priority of the task, the description body and if recurring tasks should be synchronized.
	- You can also define if task start and due dates should be mapped as floating without timezone to avoid issues with tasks across different timezones.
	- Similar to calendars you can also define a filter category so that multiple CalDAV Tasklists can be synchronized into one Outlook task folder via the defined category.
	
### Timezone settings ###

Outlook and Windows use different Timezone definitions than most CalDAV servers and other clients. When adding new events on the server you have different options how the timezone of the newly created VEVENT is generated. The default setting uses the default Windows Timezone from Outlook (e.g. W. Europe Standard Time) or the selected timezones for the start and end of the appointment. Since some servers have problems with that timezone definitions you can change that behaviour in the event mapping configuration with the following options:

- *Create events on server in UTC* Use UTC instead of Outlook Appointment Timezone for creating events on CalDAV server. Not recommended for general use, because recurrence exceptions over DST changes can't be mapped and Appointments with different start and end timezones can't be represented.
- *Create events on server in downloaded IANA Timezones* Use Iana instead of Windows Timezones for creating events on CalDAV server. Needed for servers which do not accept non standard Windows Timezones like GMX for example. Timezone definitions will be downloaded from [http://tzurl.org.](http://tzurl.org)
- *Use IANA Timezone* Use this IANA timezone for default Outlook/Windows timezone. Manually selected different timezones in Outlook appointments will be mapped to first corresponding IANA timezone.
- *Include full IANA zone with historical data* Use full IANA timezone definition with historical data. Needs more bandwidth and can be incompatible when manually importing in Outlook.

### Managing meetings and invites ###

Outlook can only track meeting responses and invites in the main calender folder. If you schedule meetings from Outlook which are synced with the CalDAV server you have two possibilities to avoid double invitation mails for all attendees. First, you can enable the option *SCHEDULE-AGENT=CLIENT* (or *Don't send appointment notifications (from SOGo)*" for SOGo servers) and let only Outlook send the meeting invites, if the server supports this option. Or you can disable this option and let the server schedule the meetings after syncing the meeting. Then you need to disable the invitation mails sent from Outlook. This is possible by unchecking the checkbox left to the attendee name in the meeting planning dialog. When syncing meetings created in Outlook to the server, the option *Use GlobalAppointmentID for UID attribute* is recommended. This can avoid duplicate events from invitations.

When creating meetings in Outlook you can also use *Act on behalf of server identity* to set the server identity (Email Address in the server settings of the sync profile) as the organizer and the Outlook identity acting on behalf with the SENT-BY property. This can be useful when Outlook and server identity do not match to avoid invites sent by the wrong email or if meetings are created in a shared calendar on behalf of the calendar owner.

The response status of all attendees can be synced from Outlook to the server but only the status of the own Outlook identity (if included in the attendees) can be synced from the server to Outlook due to limitations of the Outlook Object Model.

When receiving invites from the CalDAV server and via Email in your INBOX, Outlook will automatically create a tentative meeting in the main calendar folder (This can be controlled with the Outlook Option 'Automatically process meeting requests and responses to meeting requests and polls').

To avoid double meetings the option *Cleanup duplicate events after each sync run* in event mapping configuration is recommended.

### Free/busy lookups ###

You can configure free/busy lookups globally in the outlook options.
Select Options/Calendar and there free/busy information and use a free/busy url of your server with placeholder like %Name%, e.g. http://myserver/freebusy.php/%Name%
Then every attendee in the outlook planning view gets resolved with that url for a free/busy lookup against your server. 

### Scheduling settings and resources ###

If your server supports resources (for SOGo see [http://wiki.sogo.nu/ResourceConfiguration](http://wiki.sogo.nu/ResourceConfiguration))
disable "set SCHEDULE-AGENT=CLIENT" in Mapping Configuration, so that the server can handle the resource invitation mails, add the resource email adress as attendee in the Outlook appointment and choose type ressource (house icon) for it.
 
### Category Filter and Color ###

If you want to sync multiple CalDAV calendars or tasklists into one Outlook folder you can configure an Outlook category for filtering in the *Mapping Configuration*. You can choose a category from the dropdown list of all available Outlook categories or enter a new category name.
For all events/tasks from the server the defined category is added in Outlook, when syncing back from Outlook to the server only appointments/tasks with that category are considered but the filter category is removed. The category name must not contain any commas or semicolons!
With the checkbox *Sync also Appointments without any category* also all appointments/tasks without a category are synced to the server.
With the checkbox below you can alternatively negate the filter and sync all appointments/tasks except this category.
For calendars it is also possible to choose the color of the category or to fetch the calendar color from the server and map it to the nearest supported Outlook category color with the button *Fetch Color*. With *Set DAV Color* it is also possible to sync the choosen category color back to set the server calendar color accordingly. With *Category Shortcut Key* you can define the shortcut key of the selected category for easier access when creating appointments.

Experimental mapping of the first category color of the appointment to the matching COLOR attribute of the event is also available with the option *Map Event Color to Category*. When mapping a COLOR from the server to Outlook the first matching Outlook category with that color is used, but mapping can be manually changed in the options.xml config file. Together with DAVdroid for Android [https://davdroid.bitfire.at](https://davdroid.bitfire.at) you can map individual event colors from Android to Outlook,but not all calendar apps support it or can even crash, see [https://davdroid.bitfire.at/faq/entry/setting-event-colors-crash/](https://davdroid.bitfire.at/faq/entry/setting-event-colors-crash/)

### Reminders ###

In event and task mapping configuration you can define if you want to map (all/non/just upcoming) reminders. If you get the following error message when trying to set reminders in Outlook 
> The reminder will not appear because the item is in a folder that doesn’t support reminders.

you can try to change the Outlook options as discussed in
[http://answers.microsoft.com/en-us/office/forum/office_2016-outlook/outlook-2016-calendar-reminders/8f40bcdd-e3fc-4f29-acaf-544f48d63992](http://answers.microsoft.com/en-us/office/forum/office_2016-outlook/outlook-2016-calendar-reminders/8f40bcdd-e3fc-4f29-acaf-544f48d63992)
or try the following reported by #Todo18


1. Create a new storage folder in Outlook via the File menu, Info, Account Settings. In the Data Files tab, you can Add a new (.pst) data file. After the file has been added, Make it the default [data file], and close the dialog.
2. Go to the Calendar window, right click on the calendar that's giving you problems, and select Move Calendar. In the dialog, pick the data file that you created in the first step, and confirm. Don't forget to update the storage folder in the CalDav Synchronizer settings!

### Custom properties mapping ###

When you expand the tree view of the profile for events and tasks, you can configure the mapping of custom properties.

- *Map all Outlook custom properties to X-CALDAVSYNCHRONIZER attributes* If enabled, all Outlook custom text properties of the appointment/task are mapped to DAV attributes with the prefix X-CALDAVSYNCHRONIZER- and vice versa.
- You can also define manual mapping pairs of Outlook custom attributes and DAV X-Attributes. This will overrule the general mapping of all Outlook custom properties if both is activated. Outlook properties that don't exist, will be created. DAV properties MUST start with X-. Only Outlook custom properties of type Text can be mapped.  

### Distribution Lists ###

When enabled in Contact Mapping configuration you can now also sync Outlook Distribution Lists with your server contact groups. Since different servers use different formats to store contact groups, you will be able to choose the used DAV contact group format. Right now, the VLIST format for SOGo servers, vCards with KIND:group and iCloud groups are supported. Don't enable any of these options when your server doesn't support it!

Since Outlook Distribution Lists also support list members which aren't in the addressbook but SOGo VLISTs don't, we add them as custom X-Attributes. With this workaround those members aren't displayed in SOGo but won't get lost when syncing back to Outlook.

Since vCard in version 3.0 doesn't support contact groups we use X-ADDRESSBOOK-SERVER attributes for KIND and MEMBER for contact groups and map the member CN and EMAIL for vCards with KIND:group or the member UID for the icloud groups.

### Google Calender / Addressbooks / Tasks settings ###

For Google you can use the new Google type profile which simplifies the setup. You just need to enter the email address of your google account. When testing the settings, you will be redirected to your browser to enter your Google Account password and grant access rights to your Google Calender, Contacts and Tasks for OutlookCalDavSynchronizer via the safe OAuth protocol. After that Autodiscovery will try to find available calendar, addressbook and task resources. 

You can control which calendars are available via CalDAV and shown in autodiscovery in your calendar settings, see [https://calendar.google.com/calendar/syncselect](https://calendar.google.com/calendar/syncselect)

For contacts you should activate the checkbox **Use Google native API**. This will improve performance and other mapping issues, since the Google Contacts API supports more features than the generic CardDAV API. Compared to CardDAV this adds:

- Support for google contact groups, which are synced to Outlook categories.
- Added mapping for anniversary, relations (spouse, child, etc.) and IMs for google contacts (Contribution from Florian Saller, thank you!).

When switching between native API and CardDAV the sync cache is cleared and a complete initial sync is performed during next sync run.

For tasks you can choose the tasklist you want to sync with an Outlook task folder and the id of the task list is shown in the Discovered Url. With the button 'Edit Url' you still can manually change the Url e.g. when you want to sync a shared google calendar from another account.

If you get an error with insufficient access you need to refresh the token by deleting the previous token in 
`C:\Users\<your Username>\AppData\Roaming\Google.Apis.Auth`

### GMX calendar settings ###

For GMX calendar use the GMX Calendar account type, which sets the autodiscovery DAV Url `https://caldav.gmx.net`
Since GMX doesn't allow to create events with the Windows Timezone IDs, for the GMX account type the `Create events on server with downloaded IANA Timezones` checkbox in Mapping Configuration is checked by default to avoid errors when creating events and syncing from Outlook to GMX.

For GMX addressbook use the DAV Url `https://carddav.gmx.net`

### Synology NAS settings ###

When test settings for your synology NAS profile, you can ignore the warning "The specified Url does not support calendar queries. Some features like time range filter may not work!".
But a user reported, that "Disable directory browsing" setting **must not** be enabled for the calendar folder for proper syncing.

For Synology NAS with SSL support use port 5006 and the following settings in your NAS:
In Synology DSM Navigate to control panel > Terminal & SNMP
Select Enable SSH 
Then enter Advanced Settings and set it to High
Now it will work on port 5006 with https.

### iCloud settings ###

Apple changed their security policy recently (June 2017). You need to enable Two-Factor-Authentication and an app-specific password for CalDavSynchronizer, see
[https://support.apple.com/en-us/HT204397](https://support.apple.com/en-us/HT204397)

For syncing iCloud Calendar select the preconfigured iCloud Calendar profile type, which uses     the following CalDAV URL

    https://caldav.icloud.com

Only as a fallback if the autodiscovery fails you can use the following procedur
To find the correct DAV url for iCloud you need some information from the MacOS, where you are connected with your calendar.

Open with Textedit: `~/Library/Calendars/*.caldav/Info.plist` 
(Its in the hidden User-Library)

Check iCloud Path: PrincipalURL 
    `<string>https://p**-caldav.icloud.com/*********/principal/</string>`

Check: DefaultCalendarPath 
    `<string>/*********/calendars/********-****-****-****-************</string>`

Then you get the DAV url of the calendar:
    `https://p**-caldav.icloud.com/*********/calendars/********-****-****-****-************/`

For syncing iCloud contacts select the preconfigured iCloud contacts profile type, which uses the following CardDAV URL

    https://contacts.icloud.com
and press '*Test or discover settings*' for autodiscovery, the final URL should look like
    
    https://contacts.icloud.com:443/<YOUR UNIQUE Apple USER_ID>/carddavhome/card/

There are PHP files available to determine your Apple USER_ID, see

    https://icloud.niftyside.com/

    https://github.com/muhlba91/icloud

### One.com settings ###

The one.com caldav server has problems with escaping, so if your calendar url looks something like

    https://caldav.one.com/calendars/users/USERNAME@DOMAIN.COM/calendar/
use the url

    https://caldav.one.com/calendars/users/USERNAME%40DOMAIN.COM/calendar/

### Autodiscovery ###

When you are using an IMAP/POP3 Account with the same server settings (Username, Email address) you can press *Get IMAP/POP3 account settings* to discover those settings. The DAV url is discovered via DNS lookup from the account email address or the IMAP/POP3/SMTP server url if that fails. Together with the *Use IMAP/POP3 account password* checkbox activated you can fully autoconfigure the server settings from your existing account.

Instead of using the exact calendar/addressbook URL you can use the server address or the principal url and use the 'Test or discover settings' button in the option dialog to try to autodiscover available calendars and addressbooks on the server. 

If the server has calendar-proxy support (calendar-proxy-read-for, calendar-proxy-write-for), see [https://github.com/apple/ccs-calendarserver/blob/master/doc/Extensions/caldav-proxy.txt](https://github.com/apple/ccs-calendarserver/blob/master/doc/Extensions/caldav-proxy.txt) shared calendars can also be discovered. You can then choose one of the found calendars or addressbooks in the new window.

If your server has redirections for well-known Urls (`./well-known/caldav/` and `./well-known/carddav/` ) you need to enter the server name only (without path). If your domain configured DNS SRV and/or TXT lookups it is also possible leave the DAV url empty and discover it from the entered Email Address or Username via DNS lookups, for example:

    _carddavs._tcp 86400 IN SRV 10 20 443 dav.example.org.
    _caldavs._tcp 86400 IN SRV 10 20 443 dav.example.org.

### Proxy Settings ###
You can now set manual proxy settings in the *Network and proxy options* dialog in each profile. To override the default proxy settings from Windows Internet Explorer you can also specify settings in the app config file, see config options below.
More information can be found at
[https://msdn.microsoft.com/en-us/library/sa91de1e%28v=vs.110%29.aspx](https://msdn.microsoft.com/en-us/library/sa91de1e%28v=vs.110%29.aspx)

### General Options and SSL settings ###
In the General Options Dialog you can change settings which are used for all synchronization profiles.

- *Generel Settings*
	- **Automatically check for newer versions** set to false to disable checking for updates.
	- **Check Internet connection before sync run** checks if an interface is up and try DNS query to dns.msftncsi.com first and if that fails try to download http://www.msftncsi.com/ncsi.txt with the configured proxy before each sync run to avoid error reports if network is unavailable after hibernate for example. Disable this option if you are in a local network where DNS and that URL is blocked.
	- **Include custom message classes in Outlook filter** Disabled by default, enable only if you have custom forms with message_classes other than the default IPM.Appointment/Contact/Task. For better performance, Windows Search Service shouldn't be deactivated if this option is enabled.
	- **Use fast queries for Outlook folders** Enabled by default, uses fast GetTable queries when accessing Outlook folders. Disable only if you get errors in GetVersions, when disabled every item needs to be requested which causes a performance penalty!
	- **Trigger sync after Outlook Send/Receive and on Startup** If checked a manual sync is triggered after the Outlook Send/Receive finishes and on Outlook startup.
	- **Store data in roaming folder** set to true if you need to store state and profile data in the AppData\Roaming\ directory for roaming profiles in a AD domain for example. When changing this option, a restart of Outlook is required.
- *UI Settings*
	- **Show advanced settings as default** Show the advanced settings in synchronization profiles as default if enabled.
	- **Expand all nodes in Synchronization profiles** Enabled by default, expands all nodes in the synchronization profiles to see the suboptions for network settings and mapping configuration.
	- **Enable Tray Icon** Enabled by default, you can disable the tray icon in the Windows Taskbar if you don't need it.
	- **Show Sync Progress Bar** and **Sync Progress Bar Threshold (Items)** Enabled by default, show a progress bar if more than the treshold of items need to be loaded during a synchronization run. If disabled, no progress bar is shown but be aware that for larger changes Outlook can freeze, since some operations need to be performed in the Outlook main thread.
	- **Language** Select UI language. When changing this option, a restart of Outlook is required.
- *Server Settings*
	- **Accept invalid chars in server response** If checked invalid characters in XML server responses are allowed. A typical invalid char, sent by some servers is Form feed (0x0C).
	- ** Enable useUnsafeHeaderParsing** Enable, if the server sends invalid http headers, see common network errors. Needed for Yahoo and cPanel Horde servers for example. The general option overrides the setting in the app.config file.
	- **CalDav Connection Timeout (secs)** For slow server connections you can increaste the timeout value (default 90 secs).
- *SSL/TLS Settings*
	- If you have problems with SSL/TLS and self-signed certificates, you can change the following settings at your own risk. The recommended way would be to add the self signed cert to the Local Computer Trusted Root Certification Authorities. You can import the cert by running the MMC as Administrator.
	- **Disable Certificate Validation** set to true to disable SSL/TLS certificate validation, major security risk, use with caution!
	- **Enable Client Certificates** If enabled, the available client certificates from the Windows user certificate store will automatically be provided.
	- **Enable Tls12** set to false to disable TLS12, not recommended 
	- **Enable Ssl3** set to true to enable deprecated SSLv3, major security risk, use with caution!
- *Synchronization Reports*
	- See **Reports of sync runs** below. 
- *General Logging*
	- In the **General Logging** section you can show or clear the log file and define the log level. Possible log levels are `INFO` and  `DEBUG`.

### Profile Import/Export ###

In the toolbar of the synchronization profiles you can export all profiles to a file and import profiles from an earlier exported file. When exporting, you can choose a filename, the extension is *.cdsp and all options are saved in an xml format into this file. When importing the file, existing profiles are merged with the imported ones. If the selected Outlook folder for the profile doesn't exist during import, you need to manually select a folder before you can save the options, they are not automatically created. You need also be aware of the fact, that saved profile passwords won't work on other accounts or machines, since the encryption is dependant on the current user. But you can use the account password from the IMAP/POP3 account if available. General options are not saved in that file, but in the registry in `HKEY_CURRENT_USER\Software\CalDavSynchronizer`.

### Reports of sync runs ###

You can also configure Synchronization reports for all profiles, this can be configured via general Options:

- **Log** You can choose if you want to generate reports for *"Only sync runs with errors"* or *"Sync runs with errors or warnings"* or *"All sync runs"*.
- **Show immediately** configures if the Sync reports should be shown immediately after a sync run with errors, with warnings or errors, or not at all.
- **Delete reports older than (days)** Automatically delete reports which are older than the days configured.
- **Log Entity Names** Enable to display the summary of the event or task or the name of the contact to identify the entity in the sync report.
- 
- **Log all entities, even without warnings or errors** Enable if a full report of all modified entities is needed.

You can show reports manually with the **Reports** button in the CalDav Synchronizer Ribbon. There you can choose from available reports (shown as profile name with timestamp of the sync run) and see informations about items synced and if there were any warnings or errors. You can also delete reports or add them to a zip file via the context menu. If the last sync run lead to any errors, a warning symbol is shown in the Ribbon or the Report window opens if configured in the general options.

### Synchronization Status and System TrayIcon with Notifications ###

With the **Status** button in the CalDav Synchronizer Ribbon or via doubleclick from the TrayIcon you can access the status of the active sync profiles with their last sync run shown in minutes ago and the status OK, error, or warning. When clicking on the profile name you get to the according sync profile settings, when clicking the status icon, you can open the according sync report. When a sync run has any errors or warnings you will get a notification from the CalDav Synchronizer TrayIcon.

## Trouble Shooting ##

Options and state information is normally stored in the following folder:

    C:\Users\<Your Username>\AppData\Local\CalDavSychronizer
If you activated Store data in roaming folder the location is changed to the following folder:

    C:\Users\<Your Username>\AppData\Roaming\CalDavSychronizer

There is one `options_<your outlook profile>.xml` file which stores the options for each outlook profile.
For each sync profile there is a subfolder with state information stored in a relations.xml file after the inital sync. If you delete that folder, a fresh inital sync is performed. In the Synchronization profiles dialog a context menu is available in each profile (right click), which allows to open the cache directory and read the relations.xml file.

Each synchronization attempt is logged in the `log.txt` file. There you can find information about sync duration and the amount of added, deleted or modified events. Errors and Exceptions are logged aswell. You can view and clear the log file in **General Options**. There you can also change the log level from `INFO` to `DEBUG`. 

 
### Debugging and more config options ###

In the install dir (The default is `'C:\Program Files (x86)\CalDavSynchronizer'`) you will find the app config file

    CalDavSynchronizer.dll.config

In that xml file you can config timeout parameters and config options in the section `appSettings`
After changing parameters you have to restart Outlook.

- **wpfRenderModeSoftwareOnly**: When set to true, turn off hardware acceleration and use Software Rendering only. Useful if you have issues with WPF and your graphics card driver.

You can also change defaults for some of the general options like CheckForNewVersions, StoreAppDatainRoamingFolder, IncludeCustomMessageClasses and SSL/TLS options, useful for All Users deployment, because general options are stored per user in the HKCU registry hive.

In the section `system.net` you can define proxy settings, e.g. use of NTLM credentials

    <defaultProxy useDefaultCredentials="true">
    </defaultProxy>

In this section you can also allow UnsafeHeaderParsing if the server sends invalid http headers.

    <system.net>
    	<settings>
    		<servicePointManager expect100Continue="false" />
    		<httpWebRequest useUnsafeHeaderParsing="true" />
    	</settings>
    </system.net>

This setting can also be enabled in the general options, starting with version 2.10.0.

In the section `log4net` you can define the log level for the main log (also possible in general options now) and for the caldav data access, 
    level value can be DEBUG or INFO, e.g. :

	<root>
      <level value="DEBUG" />
      <appender-ref ref="MainLogAppender" />
    </root>
    
### Common network errors ###

- System.Net.Http.HttpRequestException: Response status code does not indicate success: '401' ('Unauthorized').
	- Wrong Username and/or Password provided.
- System.Net.Http.HttpRequestException: An error occurred while sending the request. ---> System.Net.WebException: The underlying connection was closed: A connection that was expected to be kept alive was closed by the server.
	- The server has KeepAlive disabled. Use *"Close connection after each request"* in **Network and proxy options**.
- System.Net.Http.HttpRequestException: An error occurred while sending the request. ---> System.Net.WebException: The server committed a protocol violation. Section=ResponseStatusLine
	- The server sends invalid headers. Enable the general option **Enable useUnsafeHeaderParsing** or the commented out option **useUnsafeHeaderparsing** in the app config file, see **Debugging and more config options** above.
