# Beschreibung

Neuer Style für gmx.net - realisiert durch CSS, welches durch ein Browseraddon wie [Stylus](https://add0n.com/stylus.html) injiziert wird.

Login-, Logout-, Vorschalt- und Errorseite sowie Posteingang für gmx.net / .de / .at / .ch radikal geputzt und sämtliche (Eigen)werbung entfernt.

Optionaler "darkstyle" und Einblenden bestimmter Features (siehe style settings nach der Installation).

*** Not working for gmx.fr / CaraMail / gmx.com ***


# Installation

1. Installiere die [Browsererweiterung Stylus](https://add0n.com/stylus.html) (Direktlinks auf der Seite oben rechts)
2. Klicke hier: [![Install directly with Stylus](https://img.shields.io/badge/Install%20directly%20with-Stylus-238b8b.svg)](https://raw.githubusercontent.com/stonecrusher/stylus-UserCSS/master/gmx/gmx-geputzt.user.css)


# Screenshots

![login hell](./screenshots/2019-04-27%2021_19_37.png)
![postfach dark](./screenshots/2019-04-27%2021_20_46.png)
![style optionen](./screenshots/2025-02-22%2017_51_08.png)


# Weitere Informationen

## Ladezeiten verkürzen / Ressourcen ganz blockieren

Stylus kann Elemente nur ausblenden. Wenn sie gar nicht erst geladen werden sollen, dann braucht man ein Werbeblocker-Addon wie [uBlock Origin](https://github.com/gorhill/uBlock/wiki) (schaue bei "Install from" nach deinem Browser) oder [AdblockPlus](https://adblockplus.org/).  
Die Ladezeiten (hauptsächlich für geputzte Login & Logoutseite) können signifikant verkürzt werden, indem man die entsprechende Filterliste abonniert.

### Anleitung zum abonnieren von Filterlisten
Füge folgende URL als Filterliste in deinem Adblocker hinzu:  
https://raw.githubusercontent.com/stonecrusher/filterlists/master/gmx-webde-turbo.txt

- **uBlock Origin**:  
  Dashboard öffnen --> Filterlisten --> Importieren --> URL einfügen --> Änderungen anwenden
- **Adblock Plus**:  
  Optionen --> Erweitert --> Neue Filterliste hinzufügen --> Beliebigen Titel und URL einfügen --> Filterliste hinzufügen


## Weitere Skripte

Für funktionelle Erweiterung per JavaScript (z.B. mit [Greasemonkey](https://www.greasespot.net/) / [Tampermonkey](https://tampermonkey.net/) oder ähnlichen Addons) stehen folgende praktische Skripte zur Verfügung:

- [Automatische Weiterleitung zum Posteingang](https://greasyfork.org/de/scripts/32228)
- [Überspringen der Weiterleitungsseite bei Dateianhängen](https://greasyfork.org/de/scripts/37084)


## Known Bugs / "Features"

- Darkstyle ist nicht mit "ungeputzter" Login-Seite kombinierbar.
- Darkstyle beachtet die gewählte Logoutbuttonfarbe nur eingeschränkt.
- Kurzes Ausblenden des Logos / des Fehlerkastens beim Logout in Chrome durch GMX-Scripte möglich. Lässt sich nur durch Verwenden oben genannter Blockierregeln beheben.
- Fehlerfrei nur mit User-Agent für Desktop (Desktopvariante der Webseite).


## Sonstiges

Getestet mit Firefox135 & Chrome65 auf dem Desktop (bin dankbar für [Feedback](https://github.com/stonecrusher/stylus-UserCSS/issues)).  
Nur kostenloses FreeMail. ProMail / TopMail sind ungetestet!


## Changelog

- Der Changelog wird nicht mehr gepflegt. Siehe stattdessen die [commit history auf Github](https://github.com/stonecrusher/stylus-UserCSS/commits/master/gmx).
- 2018-06-17: Scroll shadow fix.
- 2018-05-30: Optionsreihenfolge; Inaktive items: Schriftfarbe abdunkeln statt Hintergrund aufhellen.
- 2018-05-30: Farbvariablen hinzugefügt und Standardfarben aufgehellt.
- 2018-05-26: GMX-Struktur hat sich geändert: Linke Navi, Übersichtsbreite, Hover-Farben (Darkstyle), Obere Navi.
- 2018-05-05: Unteren Rand bei Posteingang entfernt wenn kein Adblocker erkannt wurde.
- 2018-04-07: Update Startseite.
- 2018-03-26: Update der Beschreibung.
- 2018-03-07: Fix für neues Logo; Ein bisschen alten Code entfernt; Loginfehler Hintergrundfarbe wieder rot; Neues Overlay entfernt; Erste Verbesserungen Darkstyle Adressbuch; Kommentare nur innerhalb der @-moz-Regeln, damit sie bei Import nicht verworfen werden; Scrollen bei geputztem login zuverlässiger verhindern (sonst kommt Sprung zu fixed header); Neuer Feedback-Reiter unten rechts.
- 2018-02-26: Darkstyle Logout Buttonfarbe.
- 2018-02-06: Anpassung Top-Toolbar.
- 2017-12-30: Schriftfarbe von input-Feldern im Darkstyle geändert, damit auf dunklen und hellen Hintergründen lesbar.
- 2017-12-06: Loginbutton Hintergrund korrigiert.
- 2017-09-26: WEB.cent auf Startseite ausgeblendet.
- 2017-08-12: Beschreibung bearbeitet.
- 2017-07-11: Update Vorschaltseite.
- 2017-06-30: Update Vorschaltseite.
- 2017-06-19: Update neue Vorschaltseite, neues MailCheck-Overlay.
- 2017-06-14: Style Beschreibung geändert. Darkstyle für .ch und .at gefixed.
- 2017-05-10: Update Vorschaltseite; Meldung "Werbung entfernt." hinzugefügt; Name geändert in "GMX FreeMail ausgeputzt"; Die Style style settings sind endlich zurück! Leider momentan noch ganz unten auf der Seite versteckt...
- 2017-05-04: Update Vorschaltseite.
- 2017-04-24: Email schreiben Darkstyle Unterkante Optionsbuttons entfernt.
- 2017-04-22: Kleine Fixes auf Startseite bezüglich Scrollbalken; Darkstyle Logout Notification Farben gefixed; uBlock Origin Anleitung in den Anmerkungen ergänzt.
- 2017-03-30: "Einschreiben" Werbung aus Email senden Optionen entfernt.
- 2017-03-28: Neue Werbung entfernt (.specialad).
- 2017-02-08: Neue Fake-Emails in Posteingang entfernt.
- 2017-02-06: Smileys wurden im Darkstyle nicht angezeigt; Darkstyle GMX-Logo neu.
- 2017-01-27: Navi-Items wurden geändert (kein Fotoalbum mehr, kein Online-Office, andere Reihenfolge) --> Anpassung nötig.
- 2017-01-20: Darkstyle Favoritenstern; Darkstyle Email-Details toggle icon; Darkstyle dropdown Pfeil bei Emailansicht.
- 2017-01-11: featureFlyoutTeaser ausgeblendet; Darkstyle: Schriftfarbe beim Login, Betreff, Icons Adressbuch.
- 2017-01-10: Darkstyle - Schriftfarbe beim Email schreiben und weitere Icons eingeblendet.
- 2017-01-09: Kosmetische Änderungen im Code; Regeln für Vorschaltseiten verallgemeinert; Mailcheck-Werbung bei Auto-Logoff entfernt; Posteingang dehnen funktioniert auch endlich auf der Startseite; Steuerung navcollapse im Darkstyle eingeblendet; "Overflow-rechts verhindern" testweise entfernt; Weitere kleine Optimierungen.
- 2017-01-03: Darkstyle: GMX-Logo geändert; expandnav eingeblendet; Mehr RegEx (yay! :).
- 2017-01-02: Formatierung für Login-(Fehler)meldungen geändert & "Passwort vergessen" eingeblendet; Option für Darkstyle hinzugefügt; Beschreibung geändert.
- 2016-12-25: Neue URL bei session expired hinzugefügt; Konsistent double statt single quotes eingefügt; Logo auch bei Zwangslogout zurückgesetzt; Error bei session expired für Smartphones gefixed; Overflow rechts bei Startseite verbessert.
- 2016-12-23: GMX Logo bei Login auf Orginalgröße zurückgesetzt und Kontrast erhöht.
- 2016-12-22: Anleitung Adblock Filter präzisiert.
- 2016-12-16: Adblock Plus Regeln verbessert; Footer Eigenwerbung entfernt.
- 2016-12-14: Adblock Plus Regeln in der Beschreibung verbessert; Logoposition bei Login & Logout angepasst; Kommentare bei ausgeschalteten Optionen eingefügt; Lizenz auf CC BY-NC-SA geändert (Angabe der Quelle, Freie Bearbeitung/Wiederverwertung etc., Nicht-kommerzielle Nutzung, Weitergabe unter gleichen Bedingungen).
- 2016-12-09: Noch mehr Werbung getarnt als Emails ausgeblendet.
- 2016-12-06: https bei Logout-Adressen ergänzt; .ch und .at bei Loginseite hinzugefügt; Beschreibung geändert; Weitere Info geändert.
- 2016-11-29: Falsches Datum entfernt, URL hinzugefügt.
- 2016-11-24: Nochmal Vorschaltseiten gefixed (lässt sich so schlecht testen) & Infotext "Werbung entfernt." hinzugefügt; Sofort-Antwort default Einstellung auf "zeigen" geändert; ".mailcheck" versteckt.
- 2016-11-20: Vorschaltseiten gefixed, linke Navi gefixed.
