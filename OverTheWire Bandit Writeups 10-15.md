Level 10 → 11

Ziel: Die in Base64 kodierten Daten in der Datei data.txt dekodieren.

Befehl: base64 -d data.txt

Passwort: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

Level 11 → 12

Ziel: Einen Rot13-verschlüsselten Text in data.txt entschlüsseln.

Befehl: cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'

Passwort: 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

Level 12 → 13

Ziel: Eine Hexdump-Datei wiederholt dekomprimieren, um an das Passwort zu gelangen.

Lösung: Mit dem Befehl file [Dateiname] kann man prüfen, um was für eine Datei es sich handelt und welche Kompilierung/Kompression sie hat. Die Datei entsprechend umbenennen und entpacken.

Passwort: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn

Level 13 → 14

Ziel: Den privaten SSH-Key nutzen, um sich ohne Passwort als bandit14 anzumelden.

Lösung: Speichere den privaten SSH-Schlüssel in einer Datei namens mykey, passe die Rechte an und verbinde dich mit dem Server.

Befehl: ssh -i mykey bandit14@bandit.labs.overthewire.org -p 2220

Level 14 → 15

Ziel: Das aktuelle Passwort auslesen und an Port 30000 auf localhost senden, um das nächste Passwort abzurufen.

Befehl (Passwort holen): cat /etc/bandit_pass/bandit14

Befehl (Passwort senden): echo "MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS" | nc localhost 30000

Passwort: 8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
