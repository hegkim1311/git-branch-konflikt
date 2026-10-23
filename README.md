# Beispiel 2: Merge-Konflikt lösen

## Verwendete Befehle
```bash
git switch -c feature-konflikt
git add README.md
git commit -m "Änderung im Feature-Branch"

git switch main
git add README.md
git commit -m "Änderung im Main-Branch"

git merge feature-konflikt
```

## Beobachtung
```Ich habe im Branch feature-konflikt und im Branch main dieselbe Stelle der Datei README.md unterschiedlich geändert. Beim Zusammenführen mit git merge trat ein Merge-Konflikt auf, da Git nicht automatisch entscheiden konnte, welche Änderung übernommen werden soll. Nach dem manuellen Beheben des Konflikts und einem weiteren Commit konnten die Branches erfolgreich zusammengeführt werden```
