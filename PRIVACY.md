# 🔒 Datenschutzerklärung (Privacy Policy)

**Letzte Aktualisierung:** 19. September 2026  
**Bot:** Eazykiller Bot

Diese Datenschutzerklärung informiert die Nutzer des Eazykiller Bots darüber, welche Daten bei der Nutzung erhoben, wie sie verarbeitet und wie lange sie gespeichert werden.

---

## 1. Grundsatz: Keine Speicherung von Nutzerprofilen außerhalb von Discord
Der Bot speichert **keine personenbezogenen Nutzerprofile oder Namenshistorien** dauerhaft in externen Datenbanken oder Dateisystemen. 
Alle Namensänderungen werden bei Erkennung unmittelbar in einen vom Server-Administrator frei wählbaren Textkanal auf Discord weitergeleitet und verbleiben ausschließlich innerhalb des Discord-Ökosystems.

---

## 2. Welche Daten werden verarbeitet?

Der Bot verarbeitet ausschließlich Daten, die für die technischen Kernfunktionen notwendig sind:

### a) Namensänderungs-Benachrichtigungen (Echtzeit-Alerts)
* **Verarbeitete Daten bei Änderung:**
  * Discord User-ID (zur Erwähnung des Nutzers)
  * Vorheriger und neuer Benutzername (Username)
  * Vorheriger und neuer globaler Anzeigename (Display Name)
  * Vorheriger und neuer Server-Nickname
* **Zweck:** Moderation und Transparenz gegen Trolling/Identitätstäuschung auf dem jeweiligen Server.
* **Verarbeitung:** Der Bot hält lediglich zur Laufzeit im flüchtigen Arbeitsspeicher (RAM) den zuletzt gesehenen Namen vor, um Differenzen festzustellen. Sobald eine Namensänderung auftritt, wird diese als Nachricht in den konfigurierten Log-Kanal gesendet. **Es erfolgt keine persistente Speicherung in einer Datenbank.**

### b) Temporäre Sprachkanäle (Voice Management)
* **Verarbeitete Daten:**
  * Kanal-ID und Owner-ID (Discord User-ID)
  * Aktuelle Mitglieder im Sprachkanal samt Beitrittszeitpunkt (`join_time`)
  * Konfigurierte Kanal-Einstellungen (Gesperrt-Status, Sichtbarkeit)
  * Spezifische Kanal-Berechtigungen (Whitelist / Blacklist je Nutzer-ID)
* **Zweck:** Bereitstellung temporärer Sprachkanäle ("Join-to-Create"), gerechter Owner-Transfer beim Verlassen des Raums und Zugriffskontrolle.
* **Speicherdauer:** Werden **automatisch und restlos gelöscht**, sobald der temporäre Sprachkanal leer ist und aufgelöst wird.

### c) Server-Konfiguration
* **Gespeicherte Daten:**
  * Server-ID (`guild_id`)
  * ID des ausgewählten Text-Logkanals (`name_log_channel_id`)

---

## 3. Rechtsgrundlage und Berechtigtes Interesse (DSGVO)
Die Verarbeitung erfolgt auf Grundlage von Art. 6 Abs. 1 lit. f DSGVO (Berechtigtes Interesse). Das berechtigte Interesse des Serverbetreibers besteht in der Gewährleistung eines sicheren, geordneten Serverbetriebs sowie der Bereitstellung automatisierter Sprachkanäle.

---

## 4. Weitergabe von Daten an Dritte
Es findet **keine Weitergabe oder ein Verkauf** von Nutzerdaten an Dritte statt. Alle Daten verbleiben auf Discord bzw. der Server-Instanz des Bots.

---

## 5. Konfiguration & Steuerung durch Administratoren
Server-Administratoren mit der Berechtigung *Server verwalten* können das Namenslogging jederzeit konfigurieren:
* `/namelog set #kanal`: Legt den Log-Kanal fest.
* `/namelog disable`: Deaktiviert das Namenslogging vollständig.
* `/namelog status`: Zeigt den aktuellen Logging-Kanal an.

---

## 6. Kontakt & Fragen
Bei Fragen wende dich bitte an die Administration des jeweiligen Discord-Servers oder den Bot-Entwickler.
