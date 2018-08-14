RSS-Reader 1.3.1
================

Das PHP-Script "RSS Reader" liest ein News Feed und gibt es auf der Webseite
formatiert aus.

Unterst�tzt werden die Formate RSS, Atom, RDF und SMF XML-Feed.



�nderungen:
-----------

Version 1.3.1:
  [+] Sonderzeichen im Feed werden jetzt kodiert, was Probleme bei
	    unterschiedlichen Zeichens�tzen vermeidet.
  [*] Diverse kleinere �nderungen im Quellcode.

Version 1.3:
  [+] Es werden jetzt auch Atom-Feeds unterst�tzt.
  [*] Kleinere �nderungen am Programmcode und der Ausgabe.

Version 1.2.1:
  [+] Die Beschreibung der Feed-Eintr�ge kann mit einer Variable ausgeblendet
      werden.
  [+] Die Eintragsinformationen, wie z.B. der Autor oder das Datum, k�nnen
      ausgebledet werden.
  [+] Die maximal anzuzeigende Anzahl der Feed-Eintr�ge kann jetzt mit einer
      Variable festgelegt werden.
  [*] In RSS-Feeds wird jetzt nur das Datum angezeigt, wenn im Feed keine
      Uhrzeit angegeben oder auf "00:00:00" gesetzt wurde.

Version 1.2:
  [+] Bei RSS Feeds kann jetzt optional der Link zu einer angeschlossenen Datei
      (mit dem enclosure-Tag) angezeigt werden.
  [+] Eine Stylesheet-Datei wurde hinzugef�gt, mit der das Style individuell
      angepasst werden kann.
  [+] Ist in einem Feed-Eintrag kein Titel angegeben, kann nun ein vorgegebener
      Text angezeigt werden.

Version 1.1:
  [+] Es k�nnen jetzt auch News-Feeds von Simple Machines Foren ("smf:xml-feed")
      gelesen werden.
  [+] Jetzt werden auch RDF-Feeds ("rdf:RDF") unterst�tzt.

--------------------------------------------------------------------------------
Copyright (c) 2007-2010 Werner Rumpeltesz (www.gaijin.at)
