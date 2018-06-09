# Beschreibung

Neuer Style für web.de - realisiert durch CSS, welches durch ein Browseraddon wie [Stylus](https://add0n.com/stylus.html) injiziert wird.

Reduziert web.de auf das Wesentliche, erweitert so die nutzbare Fläche und macht es übersichtlicher.  
Auch gut für unerfahrene Benutzer, um versehentliche "Upgrade" Bestellungen zu vermeiden.  
Optionaler Darkstyle in den Settings nach der Installation verfügbar.



# Installation

1. Installiere die [Browsererweiterung Stylus](https://add0n.com/stylus.html) (Direktlinks auf der Seite oben rechts)
2. Klicke hier: [![Install directly with Stylus](https://img.shields.io/badge/Install%20directly%20with-Stylus-238b8b.svg)](https://raw.githubusercontent.com/stonecrusher/stylus-UserCSS/master/WEBde/webde-geputzt.user.css)



# Weitere Informationen

## Ladezeiten verkürzen / Ressourcen ganz blockieren

Stylus kann Elemente nur ausblenden. Wenn sie gar nicht erst geladen werden sollen, dann braucht man ein Werbeblocker-Addon wie [uBlock Origin](https://github.com/gorhill/uBlock/wiki) (schaue bei "Install from" nach deinem Browser) oder [AdblockPlus](https://adblockplus.org/).  
Die Ladezeiten (hauptsächlich für geputzte Login & Logoutseite) können signifikant verkürzt werden, indem man die entsprechende Filterliste abonniert.

### Anleitung zum abonnieren von Filterlisten
Füge folgende URL als Filterliste in deinem Adblocker hinzu:  
https://raw.githubusercontent.com/stonecrusher/stylus-UserCSS/master/gmx/blockierregeln-gmx-webde

- **uBlock Origin**:  
  Dashboard öffnen --> Filterlisten --> Importieren --> URL einfügen --> Änderungen anwenden
- **Adblock Plus**:  
  Optionen --> Erweitert --> Neue Filterliste hinzufügen --> Beliebigen Titel und URL einfügen --> Filterliste hinzufügen


## Weitere Skripte

Für funktionelle Erweiterung per JavaScript (z.B. mit [Greasemonkey](https://www.greasespot.net/) / [Tampermonkey](https://tampermonkey.net/) oder ähnlichen Addons) stehen folgende praktische Skripte zur Verfügung:

- [Automatische Weiterleitung zum Posteingang](https://greasyfork.org/de/scripts/32227)
- [Farbige Markierung von Zitaten](https://greasyfork.org/de/scripts/40783)


## Sonstiges

Getestet mit Firefox59 & Chrome65 auf dem Desktop (bin dankbar für [Feedback](https://github.com/stonecrusher/stylus-UserCSS/issues)).  
Nur kostenloses FreeMail. Die Bezahlvariante "web.de CLUB" ist ungetestet!

# Changelog

- 2018-05-30: Standardfarben, Optionenreihenfolge und Label geändert #1; Login & Logout Hintergrund fix.
- 2018-05-26: Virenschutz im Menü hat Platz gewechselt.
- 2018-05-02: Update Additional Info; Jetzt auch als UserCSS auf GitHub verfügbar.
- 2018-04-28: Online-Speicher Vollbild overlay Werbung
- 2018-04-09: Fix Startseite wurde nicht gespeichert.
- 2018-04-07: Update Navibuttons.
- 2018-03-28: Es ist geschafft, aber schon hat sich die Loginseite verändert (.weather, #rightnav, weiße Unterstriche, andere uBO Blockierregeln).
- 2018-03-26: Ganz toll, dank eines Fehlers mit meinem Javascript-Blocker und der neuen USO Seite sind jetzt die Einstellungen alle flöten gegangen. Neu machen :(
- 2018-03-26: Bigger width for email list on start page; Ab jetzt alles auf deutsch; Beschreibung geändert.
- Update: Removed new .promo class; Removed promo list on start page; Added cloud.web.de to RegEx; Bigger height for email list on start page and mailbox (need feedback).
- Update: Removed new De-Mail item in top menu.
- Update: Fix for changed structure (top menu buttons and feedback slider).
- Update: Removed vertical-align from #main.splash-agb .layer-close (linter error); Removed Fax and Virenschutz from sidebar menu.
- Update: Small fix in RegEx for "login failed" (just for consistency); added darkstyle (see above).
- Update: Made lowwidth-adaption optional (default:no) to bring back missing answer button; Depending on browser/OS style, horizontal scrollbar still could pop up depending on content of html-mail: lowered allowed maxwidth; Added option to hide instant reply.
- Update: After logout google search popped up again; Removed "Browser-update" top bar again.
- Update: Changed description.
- Update: RegEx update (bap subdomain optional); Removed Internet TV; Removed "XL-Speicher" in toolbar when writing e-mail.
- Update: Removed grey "browser update" top bar on login page when JS is enabled (seen in Opera).
- Update: Removed namespace (was global); Removed Club button on top menu.
- Update: Splashpage update; Auto-Logout cleaned; Logout security hint update.
- Update: Removed "Einschreiben" in options when writing email; Removed "Zeitversetzt senden" ad when sending email.
- Update: Removed new "specialad" and All-Net button.
- Update: Fixed new splash site.
- Update: Removed more stuff from the left menu (SMS, Pinwand, Fax).
- Update: Updated RegExp AND fixed issue with waybackmachine.org / archive.org
- Update: web.de changed something with the wrappers, so a little fix was necessary
- Update: Removed "XXL-Speicher" ad when writing email; Changed weather option default to "yes".
- Update: Corrected message on login failed; Removed stuff after sending an e-mail.
- Update: Replaced many domain rules by RegEx; Removed Webcent overlay and flyoutFeatureTeaser; Small code changes regarding hints; Removed some legacy code; Updated screenshots; Added message on Login failed.
- Update: Made rules for splash pages more general (--> fixes webcent splash page); added option to show weather on login screen.
- Update: Added linebreaks in the sourcecode to get rid of long lines.
- Update: Added pointless menu option for "ludor" ... (is klar, ne)
- Update: Removed double domain rules.
- Update: Credits added (thanks Norwin); corrections for mailbox on small-width devices added (thanks "Johnny English"); description and name updated; screenshots added; small corrections regarding footer and splash screens as well as collapsed navigation; Corrected login and logout for smaller devices; Fixed horizontal scrollbars at start page.
- Update: Major code changes for more convenience.
