## Level 0 → 1
**Ziel:** Verbindung zum Server herstellen und die `readme`-Datei lesen.
- **Befehl:** `cat readme`
- **Passwort:** `bandit0`

## Level 1 → 2
**Ziel:** Eine Datei mit dem Namen `-` lesen (Sonderzeichen-Handling).
- **Lösung:** Da `-` oft als Operator für STDIN/STDOUT interpretiert wird, muss der Pfad explizit angegeben werden.
- **Befehl:** `cat ./-`

## Level 5 → 6
**Ziel:** Eine Datei finden, die menschlich lesbar ist, genau 1033 Bytes groß und nicht ausführbar.
- **Befehl:** `find . -size 1033c ! -executable`
- **Passwort:** `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`

## Level 6 → 7
- **Passwort:** `morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`

## Level 7 → 8
**Ziel:** Das Passwort in `data.txt` neben dem Wort "millionth" finden.
- **Befehl:** `grep "millionth" data.txt`
- **Passwort:** `dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc`

## Level 8 → 9
**Ziel:** Die einzige Zeile finden, die nicht dupliziert wurde.
- **Befehl:** `sort data.txt | uniq -u`
- **Passwort:** `4CKMh1JI91bUIZZPXDqGanal4xvAg0JM`

## Level 9 → 10
**Ziel:** Menschlich lesbare Zeichenketten in einer Binärdatei finden.
- **Befehl:** `strings data.txt | grep "==="`
- **Passwort:** `FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey`