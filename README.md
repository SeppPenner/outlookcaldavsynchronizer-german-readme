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

#### 3.6.1 ####
- Erschienen am 23.04.2019
- Bug fixes
	- Google-Kontakte-Synchronisierung aufgrund geänderter nativer API gefixt.
	- Aktualisierung der Google API NuGet-Pakete.
	- Angepasste Google-Integrationstests.

#### 3.6.0 ####
- Erschienen am 10.04.2019
- Neue Features
	- Zuordnung für Outlook-Kontakte AssistantName, Gatte und ManagerName zu vCard X-ASSISTANT, X-SPOUSE und X-MANAGER hinzugefügt.
	- Aktualisiertes Profillogo von mailbox.org.
	- Aktualisierte NuGet-Pakete.
- Fehlerbehebungen
	- Übernimmt die vorhandene Farbe aus der vorhandenen Kategorie anstelle des Wörterbuchs, um eine KeyNotFoundException zu verhindern. Github-Issue #251.
	- Reduzierung der Höhe des Optionsfensters zur Verbesserung der Anzeige für kleinere Bildschirmgrößen.

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
	- Synchronisationseinstellungen
- **Outlook -> Server (Replikat):** Alles von Outlook zum Server synchronisieren (one way).
- **Outlook <- Server (Replikat):** Alles vom Server nach Outlook synchronisieren (one way).
- **Outlook -> Server (Merge):** Synchronisiert alles von Outlook auf den Server, ändert jedoch keine auf dem Server erstellten Ereignisse.
- **Outlook <- Server (Merge):** Synchronisiert alles vom Server mit Outlook, ändert jedoch keine in Outlook erstellten Ereignisse.
- **Outlook <-> Server (bidirektional):** Bidirektionale Synchronisierung zwischen Outlook und dem Server mit einer der folgenden Konfliktlösungen.
- Konfliktlösung (wird nur im bidirektionalen Synchronisationsmodus verwendet und ist nur in den *erweiterten Einstellungen verfügbar*)
- **Outlook gewinnt:** Wenn seit dem letzten Snyc ein Ereignis in Outlook und auf dem Server geändert wurde, wird die Outlook-Version verwendet. Wenn ein Ereignis in Outlook geändert und seit dem letzten Snyc auf dem Server gelöscht wurde, wird auch die Outlook-Version verwendet. Wenn ein Ereignis in Outlook gelöscht und auf dem Server geändert wird, wird es auch auf dem Server gelöscht.
- **Server gewinnt:** Wenn seit dem letzten Snyc ein Ereignis in Outlook und auf dem Server geändert wurde, verwendet es die Serverversion. Wenn ein Ereignis in Outlook geändert und seit dem letzten Snyc auf dem Server gelöscht wird, wird es auch in Outlook gelöscht. Wenn ein Ereignis in Outlook gelöscht und auf dem Server geändert wird, wird es in Outlook neu erstellt.
- **Automatisch:** Wenn das Ereignis in Outlook und auf dem Server seit dem letzten Snyc geändert wurde, verwendet es die zuletzt aktualisierte Version. Wenn ein Ereignis in Outlook geändert und seit dem letzten Snyc auf dem Server gelöscht wird, wird es auch in Outlook gelöscht. Wenn ein Ereignis in Outlook gelöscht und auf dem Server geändert wird, wird es auch auf dem Server gelöscht.
- **Synchronisationsintervall (Minuten):** Wählen Sie das Synchronisationsintervall in Minuten aus. Wenn Sie die Option "Nur manuell" auswählen, wird keine automatische Synchronisierung durchgeführt. Sie können jedoch den Menüpunkt "Jetzt synchronisieren" verwenden
- **Synchronisation in Abschnitten** und durchführen
- **Chunk-Größe** Durchführen der CalDAV- / CardDAV-Synchronisierung in Chunks mit konfigurierbarer Chunk-Größe, um OutOfMemoryEceptions zu vermeiden, die standardmäßig aktiviert sind, da der Speicherverbrauch bei großen Ressourcen geringer ist. *(nur in erweiterten Einstellungen)*
- **Verwenden Sie den Zeitbereichsfilter** und
- **Synchronisationszeit vergangene (Tage)** und
- **Zukünftige Synchronisierungszeit (Tage)** *(nur in den erweiterten Einstellungen)* Aus Leistungsgründen ist es sinnvoll, nur eine bestimmte Zeitspanne eines großen Kalenders zu synchronisieren. Insbesondere vergangene Ereignisse sind normalerweise nicht erforderlich, um nach einer bestimmten Zeit zu synchronisieren. Beachten Sie jedoch, dass Outlook und Google sowie einige andere CalDAV-Server die Schnittmenge mit dem Zeitbereich für wiederkehrende Ereignisse unterschiedlich berechnen, was zu doppelten oder gelöschten Ereignissen führen kann. Es wird daher empfohlen, einen Zeitbereich auszuwählen, der größer als das größte Intervall Ihrer wiederkehrenden Ereignisse ist (z. B. 1 Jahr für Geburtstage). Sie können den Zeitbereichsfilter nicht zusammen mit der Synchronisierung der WebDAV-Sammlung verwenden.

- **Aktiviertes Kontrollkästchen in der Baumansicht** Wenn deaktiviert, wird das aktuelle Profil nicht mehr synchronisiert, ohne dass das Profil gelöscht werden muss.

Wenn Sie die Baumansicht des Profils erweitern, können Sie Netzwerk- und Proxyoptionen sowie Zuordnungskonfigurationsoptionen konfigurieren. *(nur in erweiterten Einstellungen)*

- **Netzwerk- und Proxy-Optionen**: Hier können Sie erweiterte Netzwerkoptionen und Proxy-Einstellungen konfigurieren.
- **Verbindung nach jeder Anforderung schließen** Verwenden Sie KeepAlive nicht für Server, die diese nicht unterstützen.
- **Präventive Authentifizierung verwenden** Senden des Authentication-Header mit jeder Anforderung, um 401-Antworten zu vermeiden und die Anforderung erneut zu senden. Deaktivieren Sie diese Option nur, wenn der Server Probleme mit der präemptiven Authentifizierung hat.
- **Standardauthentifizierung erzwingen** Legen Sie Standardauthentifizierungsheader fest, um Probleme mit der Aushandlung oder Digestauthentifizierung bei Servern wie OS X zu vermeiden. Dies wird nur empfohlen, wenn Sie eine sichere HTTPS-Verbindung verwenden. Andernfalls werden Passwörter im Klartext gesendet.
- **System Default Proxy verwenden** Proxy-Einstellungen aus Internet Explorer oder Konfigurationsdatei verwenden, verwendet Standardberechtigungsnachweise, falls für die NTLM-Authentifizierung verfügbar.
- **Verwenden der manuellen Proxy-Konfiguration.** Geben Sie die Proxy-URL als http://<Ihre-Proxy-Domäne>:<Ihr-Proxy-Port> und optional Benutzername und Kennwort für die Basisauthentifizierung an.
	
- **Zuordnungskonfiguration**: Hier können Sie konfigurieren, welche Eigenschaften synchronisiert werden sollen.
	- Bei Terminen können Sie auswählen, ob Sie Erinnerungen (nur kommende, alle oder keine) und den Beschreibungstext zuordnen möchten.
	- *Exportiere HTML-Beschreibung X-ALT-DESC konvertiert aus RTF-Body* Wenn diese Option aktiviert ist, konvertieren Sie den formatierten RTF-Body eines Outlook-Termins in HTML und exportieren Sie ihn als X-ALT-DESC-Eigenschaft. Die Konvertierung von RTF in HTML ist experimentell. Inline-Bilder und einige Formatierungseigenschaften können nicht konvertiert werden! Beachten Sie, dass einige Server wie Google Calendar dieses Attribut verwerfen!
	- *RTF-Body aus X-ALT-DESC-HTML-Beschreibung festlegen* Wenn aktiviert, konvertieren Sie die X-ALT-DESC-Beschreibung für die HTML-Eigenschaft in RTF und legen Sie den RTF-Body für Outlook-Termine fest. Die Konvertierung von HTML in RTF ist experimentell. Es können nicht alle HTML-Formatierungsoptionen konvertiert werden! Dies überschreibt auch den Klartext-Body!
	- *Zeitzoneneinstellungen* Siehe Abschnitt Zeitzonen-Mapping unten.
	- *Verwenden der GlobalAppointmentID für das UID-Attribut:* Verwenden Sie Outlook GlobalAppointmendID anstelle der zufälligen Guid für das UID-Attribut in neuen CalDAV-Ereignissen. Dadurch können doppelte Ereignisse von Einladungen vermieden werden.
	- In *Datenschutzeinstellungen* können Sie konfigurieren, ob private Outlook-Termine CLASS: CONFIDENTIAL und umgekehrt zugeordnet werden sollen. Dies kann beispielsweise für Owncloud nützlich sein, wenn Sie Ihren Kalender für andere Personen freigeben und deren Anfangs- und Enddatum Ihrer privaten Termine angezeigt werden. Sie können auch alle CLASS: PUBLIC-Ereignisse privaten Outlook-Terminen zuordnen. Für Google Kalender ist es nützlich, alle öffentlichen Outlook-Ereignisse der Standardsichtbarkeit anstelle von PUBLIC zuzuordnen.
	- In *Zeitplaneinstellungen* können Sie konfigurieren, ob Sie Teilnehmer und Organisator zuordnen möchten und ob Benachrichtigungen vom Server gesendet werden sollen. 
	- Verwenden Sie *Keine Terminbenachrichtigungen für SOGo-Server senden* und SCHEDULE-AGENT=CLIENT für andere Server, wenn Sie Einladungen aus Outlook senden und vermeiden wollen, dass der Server auch Einladungen sendet. Beachten Sie jedoch, dass nicht alle Server (z. B. Google) die SCHEDULE-AGENT=CLIENT-Einstellung unterstützen.
	- Verwenden Sie *Im Auftrag der Serveridentität handeln*, um die Serveridentität (E-Mail-Adresse in den Servereinstellungen des Synchronisierungsprofils) als Organisator neu erstellter Besprechungen und die Outlook-Identität festzulegen, die im Auftrag der SENT-BY-Eigenschaft agiert. Dies kann nützlich sein, wenn Outlook und Serveridentität nicht übereinstimmen, um Einladungen zu vermeiden, die von der falschen E-Mail gesendet werden, oder wenn Besprechungen in einem freigegebenen Kalender im Auftrag des Kalenderbesitzers erstellt werden.
	- In *Outlook-Einstellungen* können Sie auch eine Filterkategorie definieren, so dass mehrere CalDAV-Kalender über die definierte Kategorie in einen Outlook-Kalender synchronisiert werden können (siehe Kategorie Filter und Farbe unten).
	- *Bereinigen doppelter Ereignisse nach jedem Synchronisierungslauf:* Entfernt doppelte Outlook-Termine basierend auf Start-, End- und Betreff der Ereignisse nach jedem Synchronisierungslauf. Beachten Sie mögliche Performance-Probleme bei aktivierter Option.
	- Für Kontakte können Sie konfigurieren, ob Geburtstage zugeordnet werden sollen oder nicht. Wenn Geburtstage zugeordnet werden, erstellt Outlook für jeden Kontakt mit einem definierten Geburtstag außerdem einen wiederkehrenden Termin. Ähnlich können Sie konfigurieren, ob Jubiläen zugeordnet werden sollen oder nicht.
	- Sie können auch konfigurieren, ob Kontaktfotos zugeordnet werden sollen oder nicht. Das Zuordnen von Kontaktfotos von Outlook zum Server funktioniert in Outlook 2007 nicht. Sie können auch eine Option hinzufügen, um das Kontaktfoto in Outlook nicht zu überschreiben, wenn es auf dem Server geändert wird. Dies kann beispielsweise passieren, wenn andere mobile Clients die Auflösung reduzieren.
	- Überschreibt FileAs in Outlook nicht, verwendet die Outlook-Einstellungen für FileAs und überschreibt die Kontakt-FileAs nicht mit dem FN vom Server.
	- Das importierte Telefonnummernformat wird korrigiert und fügt der Ortskennzahl der Telefonnummern runde Klammern hinzu, sodass Outlook korrekte Telefonnummerndetails mit Länder- und Ortskennzahl anzeigen kann, z.B. +1 23 45678 wird auf +1 (23) 45678 abgebildet.
	- Ordnet OutlookEmailAddress1 auf WORK anstelle von HOME zu. Aktivieren Sie diese Option, wenn Sie die Reihenfolge der E-Mail-Adresszuordnung ändern müssen.
	- Schreibt IM-Adressen als IMPP-Attribute. Wenn aktiviert, wird IMPP anstelle von X-AIM, X-ICQ, X-JABBER usw. zum Schreiben von Instant Messenger-Adressen in vCards verwendet.
	- Standard-IM-Protokoll. Wählen Sie das Standardprotokoll für den IM-Servicetyp aus, das beim Schreiben von vCards aus Outlook in das Chat-Adressfeld eingefügt wird. Der Standardwert ist AIM.
	- Kartenverteilungslisten ermöglichen die Synchronisierung von Kontaktgruppen-/Verteilerlisten. Die DAV-Kontaktgruppenformate SOGo VLIST, vCards mit KIND:Gruppe oder iCloud-Gruppen sind verfügbar, siehe **Verteilerlisten** unten.
	- Für Aufgaben (nicht für Google-Aufgabenprofile) können Sie konfigurieren, ob Sie Erinnerungen (nur anstehende, alle oder keine) zuordnen möchten, die Priorität der Aufgabe, den Beschreibungstext und ob wiederkehrende Aufgaben synchronisiert werden sollen.
	- Sie können auch definieren, ob Aufgabenbeginn und Fälligkeitsdatum als Floating ohne Zeitzone zugeordnet werden sollen, um Probleme mit Aufgaben in verschiedenen Zeitzonen zu vermeiden.
	- Ähnlich wie Kalender können Sie auch eine Filterkategorie definieren, so dass mehrere CalDAV-Joblisten über die definierte Kategorie in einen Outlook-Aufgabenordner synchronisiert werden können.
	
### Zeitzoneneinstellungen ###

Outlook und Windows verwenden andere Zeitzonen als die meisten CalDAV-Server und anderen Clients. Beim Hinzufügen neuer Ereignisse auf dem Server haben Sie verschiedene Möglichkeiten, wie die Zeitzone des neu erstellten VEVENT generiert wird. In der Standardeinstellung werden die Standard-Windows-Zeitzone von Outlook (z. B. Westeuropa-Standardzeit) oder die ausgewählten Zeitzonen für den Beginn und das Ende des Termins verwendet. Da einige Server Probleme mit diesen Zeitzonen-Definitionen haben, können Sie dieses Verhalten in der Ereigniszuordnungskonfiguration mit den folgenden Optionen ändern:

- *Erstelle Ereignisse auf dem Server in UTC* Verwendet UTC anstelle von Outlook Appointment Timezone zum Erstellen von Ereignissen auf dem CalDAV-Server. Nicht für die allgemeine Verwendung empfohlen, da Wiederholungsausnahmen über DST-Änderungen nicht zugeordnet werden können und Termine mit unterschiedlichen Start- und Endzeitzonen nicht dargestellt werden können.
- *Erstelle Ereignisse auf dem Server in heruntergeladenen IANA-Zeitzonen* Verwendet Iana anstelle von Windows-Zeitzonen zum Erstellen von Ereignissen auf dem CalDAV-Server. Wird für Server benötigt, die keine Standard-Windows-Zeitzonen wie beispielsweise GMX akzeptieren. Zeitzonen-Definitionen werden von heruntergeladen von [http://tzurl.org.](http://tzurl.org).
- *Verwende die IANA-Zeitzone* Verwendet diese IANA-Zeitzone für die Standardzeitzone von Outlook / Windows. Manuell ausgewählte andere Zeitzonen in Outlook-Terminen werden der ersten entsprechenden IANA-Zeitzone zugeordnet.
- *Vollständige IANA-Zone mit historischen Daten einschließen* Verwendet die vollständige Definition der IANA-Zeitzone mit historischen Daten. Benötigt mehr Bandbreite und kann beim manuellen Import in Outlook inkompatibel sein.

### Verwalten von Meetings und Einladungen ###

Outlook kann nur Meeting-Antworten und Einladungen im Hauptkalenderordner nachverfolgen. Wenn Sie Besprechungen von Outlook aus planen, die mit dem CalDAV-Server synchronisiert werden, haben Sie zwei Möglichkeiten, doppelte Einladungsmails für alle Teilnehmer zu vermeiden. Erstens können Sie die Option *SCHEDULE-AGENT=CLIENT* (oder *Keine Terminbenachrichtigungen (von SOGo) senden* für SOGo-Server) aktivieren und nur die Besprechungseinladungen von Outlook senden, wenn der Server diese Option unterstützt. Zweitens können Sie diese Option deaktivieren und den Server die Besprechungen nach der Synchronisierung der Besprechung planen lassen. Anschließend müssen Sie die von Outlook gesendeten Einladungs-E-Mails deaktivieren. Dies ist möglich, indem Sie das Kontrollkästchen links neben dem Namen des Teilnehmers im Besprechungsplanungsdialogfeld deaktivieren. Wenn Sie Besprechungen auf den Server in Outlook synchronisieren, wird die Option *Nutze GlobalAppointmentID für UID-Attribut* empfohlen, um doppelte Ereignisse durch Einladungen zu vermeiden.

Wenn Sie Besprechungen in Outlook erstellen, können Sie auch *Achte auf die Namen der Serveridentität* verwenden, um die Serveridentität (E-Mail-Adresse in den Servereinstellungen des Synchronisierungsprofils) als Organisator festzulegen und die Outlook-Identität unter Berücksichtigung der SENT-BY-Eigenschaft festzulegen. Dies kann nützlich sein, wenn Outlook und Serveridentität nicht übereinstimmen, um Einladungen zu vermeiden, die von der falschen E-Mail gesendet werden oder wenn Besprechungen in einem freigegebenen Kalender im Auftrag des Kalenderbesitzers erstellt werden.

Der Antwortstatus aller Teilnehmer kann von Outlook mit dem Server synchronisiert werden. Aufgrund der Einschränkungen des Outlook-Objektmodells kann jedoch nur der Status der eigenen Outlook-Identität (sofern in den Teilnehmern enthalten) vom Server mit Outlook synchronisiert werden.

Wenn Sie Einladungen vom CalDAV-Server und per E-Mail in Ihrer INBOX empfangen, erstellt Outlook automatisch eine vorläufige Besprechung im Hauptkalenderordner (Dies kann mit der Outlook-Option "Besprechungsanfragen und Antworten auf Besprechungsanfragen und Abfragen automatisch bearbeiten" gesteuert werden).

Um Doppelbesprechungen zu vermeiden, wird die Option *Bereinigen doppelter Ereignisse nach jedem Synchronisierungslauf* in der Ereigniszuordnungskonfiguration empfohlen.

### Frei-/Gebucht-Lookups ###

Sie können Frei-/Gebucht-Lookups global in den Outlook-Optionen konfigurieren.
Wählen Sie Optionen/Kalender und dort Frei-/Gebucht-Informationen aus und verwenden Sie eine Frei-/Gebucht-URLs Ihres Servers mit einem Platzhalter wie%Name%, z. http://myserver/freebusy.php/%Name%
Dann wird jeder Teilnehmer in der Outlook-Planungsansicht mit dieser URL aufgelöst, um eine Frei-/Gebucht-Suche nach Ihrem Server durchzuführen.

### Planen von Einstellungen und Ressourcen ###

Wenn Ihr Server Ressourcen unterstützt (für SOGo siehe [http://wiki.sogo.nu/ResourceConfiguration](http://wiki.sogo.nu/ResourceConfiguration)), deaktivieren Sie "set SCHEDULE-AGENT=CLIENT" in der Zuordnungskonfiguration, damit der Server die Ressourceneinladungsmails verarbeiten kann, fügen Sie die Ressourcen-E-Mail-Adresse im Outlook-Termin als Teilnehmer hinzu und wählen Sie den Typ Ressource (Haussymbol).
 
### Kategoriefilter und Farbe ###

Wenn Sie mehrere CalDAV-Kalender oder -Tasklisten in einem Outlook-Ordner synchronisieren möchten, können Sie in der *Mapping-Konfiguration* eine Outlook-Kategorie für die Filterung konfigurieren. Sie können eine Kategorie aus der Dropdown-Liste aller verfügbaren Outlook-Kategorien auswählen oder einen neuen Kategorienamen eingeben.
Für alle Ereignisse/Aufgaben vom Server wird die definierte Kategorie in Outlook hinzugefügt. Wenn Sie eine Synchronisierung von Outlook auf den Server durchführen, werden nur Termine / Aufgaben mit dieser Kategorie berücksichtigt, die Filterkategorie wird jedoch entfernt. Der Kategoriename darf keine Kommas oder Semikolons enthalten!
Mit der Checkbox *Synchronisiere auch Termine ohne Kategorie* werden auch alle Termine/Aufgaben ohne Kategorie mit dem Server synchronisiert.
Mit der Checkbox unten können Sie alternativ den Filter negieren und alle Termine/Aufgaben außer dieser Kategorie synchronisieren. Bei Kalendern ist es auch möglich, die Farbe der Kategorie auszuwählen oder die Kalenderfarbe vom Server abzurufen und sie der nächstgelegenen unterstützten Outlook-Kategorienfarbe mit der Schaltfläche *Wähle Farbe* zuzuordnen. Mit *Setze DAV-Farbe* ist es auch möglich, die ausgewählte Kategoriefarbe wieder zu synchronisieren, um die Serverkalenderfarbe entsprechend einzustellen. Mit *Kategorie-Tastenkombination* können Sie die Tastenkombination der ausgewählten Kategorie definieren, um beim Erstellen von Terminen den Zugriff zu erleichtern.

Die experimentelle Zuordnung der ersten Kategoriefarbe des Termins auf das entsprechende COLOR-Attribut des Ereignisses ist auch mit der Option *Zuordnen der Ereignisfarbe zur Kategorie* verfügbar. Beim Zuordnen einer FARBE vom Server zu Outlook wird die erste übereinstimmende Outlook-Kategorie mit dieser Farbe verwendet. Die Zuordnung kann jedoch manuell in der Konfigurationsdatei options.xml geändert werden. Zusammen mit DAVdroid für Android [https://davdroid.bitfire.at](https://davdroid.bitfire.at) können Sie einzelne Ereignisfarben von Android nach Outlook zuordnen, aber nicht alle Kalender-Apps unterstützen dies oder können sogar abstürzen. Siehe auch [https://davdroid.bitfire.at/faq/entry/setting-event-colors-crash](https://davdroid.bitfire.at/faq/entry/setting-event-colors-crash/).

### Erinnerungen ###

In der Konfiguration der Ereignis- und Aufgabenzuordnung können Sie festlegen, ob Sie Erinnerungen (alle/nicht/nur bevorstehende Ereignisse) zuordnen möchten. Wenn Sie folgende Fehlermeldung erhalten, wenn Sie versuchen, Erinnerungen in Outlook festzulegen
> Die Erinnerung wird nicht angezeigt, da sich das Element in einem Ordner befindet, der keine Erinnerungen unterstützt.

Sie können versuchen, die Outlook-Optionen wie in [http://answers.microsoft.com/en-us/office/forum/office_2016-outlook/outlook-2016-calendar-reminders/8f40bcdd-e3fc-4f29-acaf-544f48d63992](http://answers.microsoft.com/en-us/office/forum/office_2016-outlook/outlook-2016-calendar-reminders/8f40bcdd-e3fc-4f29-acaf-544f48d63992) beschrieben zu ändern oder probieren Sie folgendes aus, das von #Todo18 berichtet wurde.

1. Erstellen Sie in Outlook über das Menü Datei, Info, Kontoeinstellungen einen neuen Speicherordner. Auf der Registerkarte Datendateien können Sie eine neue (.pst-)Datendatei hinzufügen. Nachdem die Datei hinzugefügt wurde, legen Sie sie als Standarddatei fest, und schließen Sie den Dialog.
2. Gehen Sie zum Kalenderfenster, klicken Sie mit der rechten Maustaste auf den Kalender, der Probleme bereitet, und wählen Sie Kalender verschieben. Wählen Sie im Dialogfeld die Datendatei aus, die Sie im ersten Schritt erstellt haben, und bestätigen Sie die Auswahl. Vergessen Sie nicht, den Speicherordner in den CalDav Synchronizer-Einstellungen zu aktualisieren!

### Benutzerdefinierte Eigenschaftszuordnung ###

Wenn Sie die Strukturansicht des Profils für Ereignisse und Aufgaben erweitern, können Sie die Zuordnung von benutzerdefinierten Eigenschaften konfigurieren.

- *Ordnen Sie alle benutzerdefinierten Eigenschaften von Outlook den X-CALDAVSYNCHRONIZER-Attributen zu* Wenn diese Option aktiviert ist, werden alle benutzerdefinierten Outlook-Texteigenschaften des Termins/Tasks den DAV-Attributen mit dem Präfix X-CALDAVSYNCHRONIZER- und umgekehrt zugeordnet.
- Sie können auch manuelle Zuordnungspaare aus benutzerdefinierten Outlook-Attributen und DAV-X-Attributen definieren. Dadurch wird die allgemeine Zuordnung aller benutzerdefinierten Outlook-Eigenschaften überschrieben, wenn beide aktiviert sind. Outlook-Eigenschaften, die nicht vorhanden sind, werden erstellt. DAV-Eigenschaften MÜSSEN mit X- beginnen. Nur benutzerdefinierte Outlook-Eigenschaften des Typs Text können zugeordnet werden.  

### Verteilerliste ###

Wenn diese Option in der Kontaktzuordnungskonfiguration aktiviert ist, können Sie jetzt auch Outlook-Verteilerlisten mit Ihren Serverkontaktgruppen synchronisieren. Da verschiedene Server unterschiedliche Formate zum Speichern von Kontaktgruppen verwenden, können Sie das verwendete DAV-Kontaktgruppenformat auswählen. Derzeit wird das VLIST-Format für SOGo-Server, vCards mit KIND:Gruppe- und iCloud-Gruppen unterstützt. Aktivieren Sie keine dieser Optionen, wenn Ihr Server dies nicht unterstützt!

Da Outlook-Verteilerlisten auch Listenmitglieder unterstützen, die nicht im Adressbuch enthalten sind, SOGo-VLISTs jedoch nicht, werden diese als benutzerdefinierte X-Attribute hinzugefügt. Mit dieser Problemumgehung werden diese Mitglieder nicht in SOGo angezeigt, gehen jedoch beim Synchronisieren mit Outlook nicht verloren.

Da vCard in Version 3.0 keine Kontaktgruppen unterstützt, verwenden wir X-ADDRESSBOOK-SERVER-Attribute für KIND und MEMBER für Kontaktgruppen und ordnen das Mitglied CN und EMAIL für vCards mit KIND:Gruppe oder die Member-UID für die icloud-Gruppen zu.

### Einstellungen für Google Kalender/Adressbücher/Aufgaben ###

Für Google können Sie das neue Google-Typenprofil verwenden, das die Einrichtung vereinfacht. Sie müssen nur die E-Mail-Adresse Ihres Google-Kontos eingeben. Beim Testen der Einstellungen werden Sie zu Ihrem Browser umgeleitet, um das Kennwort Ihres Google-Kontos einzugeben und über das sichere OAuth-Protokoll Zugriffsrechte für Ihren Google Kalender, Kontakte und Aufgaben für OutlookCalDavSynchronizer zu erteilen. Nach dieser automatischen Suche wird versucht, verfügbare Kalender-, Adressbuch- und Aufgabenressourcen zu finden. 

Sie können steuern, welche Kalender über CalDAV verfügbar sind und in den Kalendereinstellungen automatisch erkannt werden, siehe [https://calendar.google.com/calendar/syncselect](https://calendar.google.com/calendar/syncselect)

Aktivieren Sie für Kontakte das Kontrollkästchen **Google native API verwenden**. Dies verbessert die Leistung und andere Zuordnungsprobleme, da die Google Contacts-API mehr Funktionen als die generische CardDAV-API unterstützt. Im Vergleich zu CardDAV wird Folgendes hinzugefügt:

- Unterstützung für Google-Kontaktgruppen, die mit Outlook-Kategorien synchronisiert werden.
- Mapping für Jubiläum, Verwandte (Ehepartner, Kind usw.) und IMs für Google-Kontakte hinzugefügt (Beitrag von Florian Saller, vielen Dank!).

Beim Umschalten zwischen der nativen API und CardDAV wird der Synchronisierungscache gelöscht und beim nächsten Synchronisierungslauf wird eine vollständige anfängliche Synchronisierung durchgeführt.

Für Aufgaben können Sie die Jobliste auswählen, die Sie mit einem Outlook-Aufgabenordner synchronisieren möchten. Die ID der Aufgabenliste wird in der erkannten URL angezeigt. Mit der Schaltfläche "Url bearbeiten" können Sie die Url noch manuell ändern, z. Wenn Sie einen freigegebenen Google-Kalender mit einem anderen Konto synchronisieren möchten.

Wenn Sie bei unzureichendem Zugriff einen Fehler erhalten, müssen Sie das Token aktualisieren, indem Sie das vorherige Token in `C:\Users\<your Username>\AppData\Roaming\Google.Apis.Auth` löschen.

### GMX-Kalendereinstellungen ###

Für GMX-Kalender verwenden Sie den GMX-Kalender-Kontotyp, der die automatische Ermittlungs-DAV-URL `https://caldav.gmx.net` festlegt. Da GMX das Erstellen von Ereignissen mit den Windows-Zeitzonen-IDs nicht zulässt, ist für das GMX-Konto das Kontrollkästchen `Ereignisse auf Server mit heruntergeladenen IANA-Zeitzonen erstellen` in Zuordnungskonfiguration standardmäßig aktiviert, um Fehler beim Erstellen von Ereignissen und beim Synchronisieren von Outlook nach GMX zu vermeiden.

Verwenden Sie für das GMX-Adressbuch die DAV-URL `https://carddav.gmx.net`

### Synology-NAS-Einstellungen ###

Bei den Testeinstellungen für Ihr Synology NAS-Profil können Sie die Warnung ignorieren "Die angegebene URL unterstützt keine Kalenderabfragen. Einige Funktionen wie der Zeitbereichsfilter funktionieren möglicherweise nicht!".Ein Benutzer meldete jedoch, dass die Einstellung "Verzeichnis durchsuchen deaktivieren" **für den Kalenderordner nicht aktiviert werden darf**, damit der Kalenderordner ordnungsgemäß synchronisiert werden kann.

Für Synology NAS mit SSL-Support nutzen Sie Port 5006 und die folgenden Einstellungen auf ihrem NAS:
In Synology DSM Navigieren Sie zu Systemsteuerung > Terminal & SNMP
Wählen Sie SSH aktivieren
Gehen Sie zu Erweiterte Einstellungen und setzen Sie es auf Hoch.
Nun wird es auf Port 5006 mit https funktionieren.

### iCloud-Einstellungen ###

Apple hat kürzlich (Juni 2017) seine Sicherheitsrichtlinie geändert. Sie müssen die Zwei-Faktor-Authentifizierung und ein app-spezifisches Kennwort für CalDavSynchronizer aktivieren, siehe [https://support.apple.com/en-us/HT204397](https://support.apple.com/en-us/HT204397).

Wählen Sie zum Synchronisieren von iCloud Calendar den vorkonfigurierten Profiltyp des iCloud Calendar aus, der die folgende CalDAV-URL verwendet

    https://caldav.icloud.com

Nur als Fallback, wenn die automatische Erkennung fehlschlägt, können Sie das folgende Verfahren verwenden.
Um die richtige DAV-URL für iCloud zu finden, benötigen Sie einige Informationen von MacOS, mit dem Sie mit Ihrem Kalender verbunden sind.

Mit Textedit öffnen: `~/Library/Calendars/*.caldav/Info.plist` 
(Es befindet sich in der verborgenen Benutzerbibliothek)

Überprüfen Sie den iCloud-Pfad: PrincipalURL 
    `<string>https://p**-caldav.icloud.com/*********/principal/</string>`

Prüfen Sie: DefaultCalendarPath 
    `<string>/*********/calendars/********-****-****-****-************</string>`

Dann erhalten Sie die DAV-URL des Kalenders:
    `https://p**-caldav.icloud.com/*********/calendars/********-****-****-****-************/`

Wählen Sie zum Synchronisieren von iCloud-Kontakten den vorkonfigurierten Profiltyp für iCloud-Kontakte aus, der die folgende CardDAV-URL verwendet

    https://contacts.icloud.com
und drücken Sie '*Testen oder entdecken Sie die Einstellungen*' für die automatische Erkennung. Die endgültige URL sollte folgendermaßen aussehen
    
    https://contacts.icloud.com:443/<YOUR UNIQUE Apple USER_ID>/carddavhome/card/

Es gibt PHP-Dateien, die Ihre Apple-USER_ID ermitteln, siehe

    https://icloud.niftyside.com/

    https://github.com/muhlba91/icloud

### One.com-Einstellungen ###

Der caldav-Server von one.com hat Probleme mit der Escape-Funktion. Wenn also Ihre Kalender-URL in etwa so aussieht

    https://caldav.one.com/calendars/users/USERNAME@DOMAIN.COM/calendar/
Verwenden Sie die URL

    https://caldav.one.com/calendars/users/USERNAME%40DOMAIN.COM/calendar/

### Autodiscovery ###

Wenn Sie ein IMAP-/POP3-Konto mit denselben Servereinstellungen (Benutzername, E-Mail-Adresse) verwenden, können Sie *IMAP-/ POP3-Kontoeinstellungen abrufen* aufrufen, um diese Einstellungen zu ermitteln. Die DAV-URL wird über die DNS-Suche von der E-Mail-Adresse des Kontos oder der IMAP-/ POP3-/SMTP-Server-URL ermittelt, falls dies fehlschlägt. Zusammen mit dem Kontrollkästchen *IMAP-/POP3-Kontokennwort verwenden* können Sie die Servereinstellungen von Ihrem vorhandenen Konto aus vollständig automatisch konfigurieren.

Anstatt die genaue Kalender-/Adressbuch-URL zu verwenden, können Sie die Serveradresse oder die URL des Prinzipals verwenden und die Schaltfläche "Einstellungen testen oder ermitteln" im Optionsdialogfeld verwenden, um zu versuchen, verfügbare Kalender und Adressbücher auf dem Server automatisch zu erkennen. 

Wenn der Server Kalender-Proxy-Unterstützung bietet (Calendar-Proxy-Read-For, Calendar-Proxy-Write-For), siehe [https://github.com/apple/ccs-calendarserver/blob/master/doc/Extensions/caldav-proxy.txt](https://github.com/apple/ccs-calendarserver/blob/master/doc/Extensions/caldav-proxy.txt), kann der freigegebene Kalender auch entdeckt werden. Sie können dann im neuen Fenster einen der gefundenen Kalender oder Adressbücher auswählen.

Wenn Ihr Server über Weiterleitungen für bekannte URLs verfügt (`./well-known/caldav/` und `./well-known/carddav/`), müssen Sie nur den Servernamen eingeben (ohne Pfad). Wenn Ihre Domäne DNS SRV- und/oder TXT-Suchvorgänge konfiguriert hat, können Sie die DAV-URL auch leer lassen und anhand der eingegebenen E-Mail-Adresse oder des Benutzernamens über DNS-Suchvorgänge ermitteln. Beispiel:

    _carddavs._tcp 86400 IN SRV 10 20 443 dav.example.org.
    _caldavs._tcp 86400 IN SRV 10 20 443 dav.example.org.

### Proxy-Einstellungen ###
Sie können jetzt manuelle Proxy-Einstellungen im Dialogfeld *Netzwerk- und Proxy-Optionen* in jedem Profil festlegen. Um die Standard-Proxy-Einstellungen von Windows Internet Explorer zu überschreiben, können Sie auch Einstellungen in der App-Konfigurationsdatei angeben. Weitere Informationen finden Sie unter Konfigurationsoptionen.
Weitere Informationen finden Sie unter [https://msdn.microsoft.com/en-us/library/sa91de1e%28v=vs.110%29.aspx](https://msdn.microsoft.com/en-us/library/sa91de1e%28v=vs.110%29.aspx)

### Allgemeine Optionen und SSL-Einstellungen ###
Im Dialogfeld "Allgemeine Optionen" können Sie Einstellungen ändern, die für alle Synchronisationsprofile verwendet werden.

- *Allgemeine Einstellungen*
	- **Automatisch nach neueren Versionen suchen** Auf false setzen, um die Suche nach Updates zu deaktivieren.
	- **Überprüfen Sie die Internetverbindung vor dem Synchronisierungslauf** Prüft, ob eine Schnittstelle aktiv ist, und probiert zuerst die DNS-Abfrage an dns.msftncsi.com. Wenn dies fehlschlägt, versuchen Sie, vor jedem Synchronisierungslauf http://www.msftncsi.com/ncsi.txt mit dem konfigurierten Proxy herunterzuladen, um Fehlerberichte zu vermeiden, wenn das Netzwerk beispielsweise nach dem Ruhezustand nicht verfügbar ist. Deaktivieren Sie diese Option, wenn Sie sich in einem lokalen Netzwerk befinden, in dem DNS und diese URL blockiert sind.
	- **Fügen Sie benutzerdefinierte Nachrichtenklassen in den Outlook-Filter ein** Diese Option ist standardmäßig deaktiviert, wenn Sie über benutzerdefinierte Formulare mit anderen Nachrichtenklassen als dem Standard-IPM.Appointment/Contact/Task verfügen. Für eine bessere Leistung sollte der Windows-Suchdienst nicht deaktiviert werden, wenn diese Option aktiviert ist.
	- **Verwenden Sie schnelle Abfragen für Outlook-Ordner** Standardmäßig aktiviert, es werden beim Zugriff auf Outlook-Ordner schnelle GetTable-Abfragen verwendet. Deaktivieren Sie nur, wenn Sie Fehler in GetVersions erhalten. Wenn diese Option deaktiviert ist, muss jedes Element angefordert werden, was zu einer Leistungsverschlechterung führt!
	- **Synchronisation nach Outlook Senden/Empfangen und beim Start auslösen** Wenn diese Option aktiviert ist, wird eine manuelle Synchronisierung ausgelöst, nachdem das Senden/Empfangen von Outlook und der Start von Outlook abgeschlossen sind.
	- **Speichern Sie die Daten im Roaming-Ordner** Setzen Sie den Wert auf true, wenn Sie Status- und Profildaten im Verzeichnis AppData\Roaming\ für servergespeicherte Profile in einer AD-Domäne speichern müssen. Beim Ändern dieser Option ist ein Neustart von Outlook erforderlich.
- *UI-Einstellungen*
	- **Erweiterte Einstellungen als Standard anzeigen** Zeigt die erweiterten Einstellungen standardmäßig in Synchronisationsprofilen an, sofern aktiviert.
	- **Erweitern Sie alle Knoten in Synchronisationsprofilen** Diese Option ist standardmäßig aktiviert und erweitert alle Knoten in den Synchronisationsprofilen, um die Unteroptionen für die Netzwerkeinstellungen und die Mapping-Konfiguration anzuzeigen.
	- **Taskleistensymbol aktivieren** Standardmäßig aktiviert, Sie können das Taskleistensymbol in der Windows-Taskleiste deaktivieren, wenn Sie es nicht benötigen.
	- **Sync-Fortschrittsbalken anzeigen** und **Schwellenwert für die Sync-Fortschrittsleiste (Elemente)** Standardmäßig aktiviert, zeigen Sie eine Fortschrittsleiste an, wenn während eines Synchronisierungslaufs mehr als der Schwellenwert von Elementen geladen werden muss. Wenn diese Option deaktiviert ist, wird keine Fortschrittsleiste angezeigt. Beachten Sie jedoch, dass Outlook bei größeren Änderungen einfrieren kann, da einige Vorgänge im Outlook-Hauptthread ausgeführt werden müssen.
	- **Sprache** Wählen Sie die Sprache der Benutzeroberfläche. Beim Ändern dieser Option ist ein Neustart von Outlook erforderlich.
- *Server-Einstellungen*
	- **Akzeptieren Sie ungültige Zeichen in der Serverantwort** Wenn aktiviert, sind ungültige Zeichen in XML-Serverantworten zulässig. Ein typisches ungültiges Zeichen, das von einigen Servern gesendet wird, ist der Formfeed (0x0C).
	- **Aktivieren Sie useUnsafeHeaderParsing** Aktivieren Sie diese Option, wenn der Server ungültige http-Header sendet. Weitere Informationen finden Sie unter Häufige Netzwerkfehler. Wird beispielsweise für Yahoo- und cPanel-Horde-Server benötigt. Die allgemeine Option überschreibt die Einstellung in der Datei app.config.
	- **CalDav-Verbindungszeitlimit (secs)** Bei langsamen Serververbindungen können Sie den Timeout-Wert erhöhen (Standardeinstellung 90 Sekunden).
- *SSL/TLS-Einstellungen*
	- Wenn Sie Probleme mit SSL-/TLS und selbstsignierten Zertifikaten haben, können Sie die folgenden Einstellungen auf eigene Gefahr ändern. Die empfohlene Methode wäre, das selbst signierte Zertifikat den vertrauenswürdigen Stammzertifizierungsstellen des lokalen Computers hinzuzufügen. Sie können das Zertifikat importieren, indem Sie die MMC als Administrator ausführen.
	- **Zertifikatsüberprüfung deaktivieren** Setzen Sie diese Option auf "true", um die Validierung von SSL-/ ´TLS-Zertifikaten zu deaktivieren. Große Sicherheitsrisiken. Vorsicht!
	- **Aktiviere Client-Zertifikate** Wenn aktiviert, werden die verfügbaren Clientzertifikate aus dem Windows-Benutzerzertifikatspeicher automatisch bereitgestellt.
	- **Aktiviere Tls12** Auf false setzen, um TLS12 zu deaktivieren, nicht empfohlen .
	- **Aktiviere Ssl3** Setzen Sie diese Option auf true, um veraltetes SSLv3 zu aktivieren, ein großes Sicherheitsrisiko, mit Vorsicht verwenden!
- *Synchronisationsberichte*
	- Siehe **Berichte über Synchronisierungsläufe** unten. 
- *Allgemeine Protokollierung*
	- In der **Allgemeine Protokollierung**-Sektion können Sie die Protokolldatei anzeigen oder löschen und die Protokollebene festlegen. Mögliche Loglevel sind `INFO` und `DEBUG`.

### Profil-Import/Export ###

In der Symbolleiste der Synchronisationsprofile können Sie alle Profile in eine Datei exportieren und Profile aus einer zuvor exportierten Datei importieren. Beim Exportieren können Sie einen Dateinamen auswählen, die Erweiterung ist *.cdsp und alle Optionen werden im XML-Format in dieser Datei gespeichert. Beim Importieren der Datei werden vorhandene Profile mit den importierten zusammengeführt. Wenn der ausgewählte Outlook-Ordner für das Profil während des Imports nicht vorhanden ist, müssen Sie einen Ordner manuell auswählen, bevor Sie die Optionen speichern können. Diese Optionen werden nicht automatisch erstellt. Sie müssen auch wissen, dass gespeicherte Profilkennwörter auf anderen Konten oder Computern nicht funktionieren, da die Verschlüsselung vom aktuellen Benutzer abhängt. Sie können jedoch das Kontokennwort aus dem IMAP-/POP3-Konto verwenden, sofern verfügbar. Allgemeine Optionen werden nicht in dieser Datei gespeichert, sondern in der Registry unter `HKEY_CURRENT_USER\Software\CalDavSynchronizer`.

### Berichte über Synchronisierungsläufe ###

Sie können auch Synchronisationsberichte für alle Profile konfigurieren. Dies kann über allgemeine Optionen konfiguriert werden:

- **Log** Sie können wählen, ob Sie Berichte für erstellen möchten für *"Nur Synchronisierungsläufe mit Fehlern loggen"* or *"Nur Synchronisierungsläufe mit Fehlern oder Warnungen loggen"* or *"Alle Synchronisierungsläufe loggen"*.
- **Zeige sofort** Konfiguriert, ob die Sync-Berichte sofort nach einem Sync-Lauf mit Fehlern, Warnungen oder Fehlern angezeigt werden sollen oder nicht.
- **Berichte löschen, die älter als (Tage) sind** Löscht automatisch Berichte, die älter sind als die konfigurierten Tage.
- **EntityNamen loggen** Aktivieren Sie diese Option, um die Zusammenfassung des Ereignisses oder der Aufgabe oder den Namen des Kontakts anzuzeigen, um die Entität im Synchronisierungsbericht zu identifizieren.
- **Alle Entitäten protokollieren, auch ohne Warnungen oder Fehler** Aktivieren Sie diese Option, wenn ein vollständiger Bericht aller geänderten Entitäten benötigt wird.

Sie können Berichte manuell mit der Schaltfläche **Berichte** in der CalDav Synchronizer-Multifunktionsleiste anzeigen. Dort können Sie aus verfügbaren Berichten (angezeigt als Profilname mit Zeitstempel des Synchronisierungslaufs) auswählen und Informationen zu synchronisierten Elementen sowie zu Warnungen oder Fehlern anzeigen. Sie können Berichte auch löschen oder über das Kontextmenü zu einer ZIP-Datei hinzufügen. Wenn der letzte Synchronisierungslauf zu Fehlern führte, wird ein Warnsymbol in der Multifunktionsleiste angezeigt oder das Berichtsfenster wird geöffnet, sofern dies in den allgemeinen Optionen konfiguriert ist.

### Synchronisationsstatus und System TrayIcon mit Benachrichtigungen ###

Mit der Schaltfläche **Status** in der CalDav Synchronizer-Multifunktionsleiste oder per Doppelklick über TrayIcon können Sie auf den Status der aktiven Synchronisationsprofile zugreifen, wobei der letzte Synchronisierungslauf in Minuten zuvor angezeigt wurde und der Status OK, Fehler oder Warnung angezeigt wird. Wenn Sie auf den Profilnamen klicken, gelangen Sie zu den entsprechenden Synchronisationsprofileinstellungen. Wenn Sie auf das Statussymbol klicken, können Sie den entsprechenden Synchronisierungsbericht öffnen. Wenn bei einem Synchronisierungslauf Fehler oder Warnungen angezeigt werden, erhalten Sie eine Benachrichtigung von CalDav Synchronizer TrayIcon.

## Fehlerbehebung ##

Optionen und Statusinformationen werden normalerweise im folgenden Ordner gespeichert:

    C:\Users\<Your Username>\AppData\Local\CalDavSychronizer
Wenn Sie "Daten in Roaming-Ordner speichern" aktiviert haben, wird der Speicherort in den folgenden Ordner geändert:

    C:\Users\<Your Username>\AppData\Roaming\CalDavSychronizer

Es gibt eine `options_<Ihr Outlook-Profil>.xml`-Datei, in der die Optionen für jedes Outlook-Profil gespeichert werden. Für jedes Synchronisationsprofil gibt es einen Unterordner mit Statusinformationen, die nach der ersten Synchronisierung in einer Datei `relations.xml` gespeichert sind. Wenn Sie diesen Ordner löschen, wird eine neue Anfangssynchronisierung durchgeführt. Im Dialogfeld "Synchronisationsprofile" ist in jedem Profil ein Kontextmenü (rechte Maustaste) verfügbar, mit dem das Cache-Verzeichnis geöffnet und die Datei `relations.xml` gelesen werden kann.

Jeder Synchronisationsversuch wird in der `log.txt`-Datei protokolliert. Dort finden Sie Informationen zur Dauer der Synchronisierung und die Anzahl der hinzugefügten, gelöschten oder geänderten Ereignisse. Fehler und Ausnahmen werden ebenfalls protokolliert. Sie können die Protokolldatei in **Allgemeine Optionen** anzeigen und löschen. Dort können Sie auch den Log-Level von `INFO` in `DEBUG` ändern.

### Debugging und weitere Konfigurationsoptionen ###

Im Installationsverzeichnis (Die Standardeinstellung ist `'C:\Program Files (x86)\CalDavSynchronizer'`) finden Sie die App-Konfigurationsdatei

    CalDavSynchronizer.dll.config
In dieser XML-Datei können Sie Timeout-Parameter und Konfigurationsoptionen im Abschnitt `appSettings` konfigurieren. Nach dem Ändern der Parameter müssen Sie Outlook neu starten.

- **wpfRenderModeSoftwareOnly**: Deaktivieren Sie mit true die Hardwarebeschleunigung und verwenden Sie nur Software-Rendering. Nützlich bei Problemen mit WPF und dem Grafikkartentreiber.

Sie können auch die Standardeinstellungen für einige der allgemeinen Optionen wie CheckForNewVersions, StoreAppDatainRoamingFolder, IncludeCustomMessageClasses und SSL-/TLS-Optionen ändern. Diese Optionen sind für die Bereitstellung für alle Nutzer nützlich, da allgemeine Optionen pro Benutzer in der HKCU-Registrierungsstruktur gespeichert werden.

Im Abschnitt `system.net` können Sie Proxy-Einstellungen definieren, z. Verwendung von NTLM-Anmeldeinformationen

    <defaultProxy useDefaultCredentials="true">
    </defaultProxy>

In diesem Abschnitt können Sie auch UnsafeHeaderParsing zulassen, wenn der Server ungültige http-Header sendet.

    <system.net>
    	<settings>
    		<servicePointManager expect100Continue="false" />
    		<httpWebRequest useUnsafeHeaderParsing="true" />
    	</settings>
    </system.net>

Diese Einstellung kann ab Version 2.10.0 auch in den allgemeinen Optionen aktiviert werden.

Im Abschnitt `log4net` können Sie die Protokollebene für das Hauptprotokoll festlegen (jetzt auch in den allgemeinen Optionen möglich). Für den Caldav-Datenzugriff kann der Wert für die Ebene DEBUG oder INFO sein, z. B.:

	<root>
      <level value="DEBUG" />
      <appender-ref ref="MainLogAppender" />
    </root>
    
### Häufige Netzwerkfehler ###

- System.Net.Http.HttpRequestException: Der Antwortstatuscode gibt keinen Erfolg an: '401' ('Unauthorized').
	- Falscher Benutzername und/oder Passwort angegeben.
- System.Net.Http.HttpRequestException: Beim Senden der Anfrage ist ein Fehler aufgetreten. ---> System.Net.WebException: Die zugrunde liegende Verbindung wurde geschlossen: Eine Verbindung, von der erwartet wurde, dass sie am Leben bleibt, wurde vom Server geschlossen.
	- Der Server hat KeepAlive deaktiviert. Benutzen Sie *"Verbindung nach jeder Anfrage schließen"* in den **Netzwerk- und Proxy-Optionen**.
- System.Net.Http.HttpRequestException: Beim Senden der Anfrage ist ein Fehler aufgetreten. ---> System.Net.WebException: Der Server hat eine Protokollverletzung begangen. Section=ResponseStatusLine
	- Der Server sendet ungültige Header. Aktivieren Sie die allgemeine Option **Aktiviere useUnsafeHeaderParsing** oder die auskommentierte Option **useUnsafeHeaderparsing** in der App-Konfigurationsdatei, siehe **Debugging und weitere Konfigurationsoptionen** oben.
