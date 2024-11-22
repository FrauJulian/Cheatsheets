# Git Befehle im Terminal

## 1. Git Befehle

### 1.1 Repository erstellen oder klonen

| Befehl | Beschreibung |
|--------|--------------|
| `git init` | Neues lokales Git-Repository erstellen. |
| `git clone <repository-url>` | Remote Repository klonen. |

### 1.2 Status und Log

| Befehl | Beschreibung |
|--------|--------------|
| `git status` | Status der Änderungen anzeigen. |
| `git log` | Log der Commits anzeigen. |
| `git log --oneline` | Log in komprimierter Form anzeigen. |

### 1.3 Änderungen tracken

| Befehl | Beschreibung |
|--------|--------------|
| `git add <file>` | Datei zum Staging-Bereich hinzufügen. |
| `git add .` | Alle Änderungen hinzufügen. |
| `git commit -m "Nachricht"` | Änderungen mit einer Nachricht committen. |
| `git commit -a -m "Nachricht"` | Alle geänderten Dateien direkt committen (ohne `git add`). |

### 1.4 Branches

| Befehl | Beschreibung |
|--------|--------------|
| `git branch` | Alle lokalen Branches anzeigen. |
| `git branch <branch-name>` | Neuen Branch erstellen. |
| `git checkout <branch-name>` | Zu einem bestehenden Branch wechseln. |
| `git checkout -b <branch-name>` | Neuen Branch erstellen und wechseln. |

### 1.5 Commit Nachrichten bearbeiten

| Befehl | Beschreibung |
|--------|--------------|
| `git commit --amend` | Die letzte Commit-Nachricht ändern. |

### 1.6 Git Aliase erstellen

| Befehl | Beschreibung |
|--------|--------------|
| `git config --global alias.<alias-name> '<git-command>'` | Alias für einen Git-Befehl erstellen. Zum Beispiel: `git config --global alias.co 'checkout'`. |

### 1.7 Temporäre Commits entfernen (Reflog)

| Befehl | Beschreibung |
|--------|--------------|
| `git reflog` | Übersicht über alle Änderungen am Branch. |
| `git reset --hard HEAD@{n}` | Zum bestimmten Punkt in der Historie zurückkehren, basierend auf der Reflog-Referenz. |

### 1.8 Git Cherry-Pick

| Befehl | Beschreibung |
|--------|--------------|
| `git cherry-pick <commit-id>` | Einen bestimmten Commit aus einem anderen Branch anwenden. |

### 1.9 Git Bisect (Fehlersuche)

| Befehl | Beschreibung |
|--------|--------------|
| `git bisect start` | Startet die Fehlersuche mithilfe der Bisect-Funktion. |
| `git bisect good <commit>` | Markiert einen Commit als funktionierend. |
| `git bisect bad <commit>` | Markiert einen Commit als fehlerhaft. |

### 1.10 Git Blame (Dateiänderungen nachvollziehen)

| Befehl | Beschreibung |
|--------|--------------|
| `git blame <file>` | Zeigt an, welche Commits welche Zeilen einer Datei geändert haben. |

### 1.11 Git Clean (Unversionierte Dateien entfernen)

| Befehl | Beschreibung |
|--------|--------------|
| `git clean -f` | Löscht unversionierte Dateien. |
| `git clean -fd` | Löscht unversionierte Dateien und Verzeichnisse. |

## 2. Arbeiten mit Remote Repositories

### 2.1 Push & Pull

| Befehl | Beschreibung |
|--------|--------------|
| `git remote add origin <url>` | Remote Repository hinzufügen. |
| `git push -u origin <branch>` | Lokalen Branch das erste Mal pushen. |
| `git push` | Änderungen pushen. |
| `git pull` | Änderungen vom Remote-Repository holen. |

### 2.2 Fetch und Merge

| Befehl | Beschreibung |
|--------|--------------|
| `git fetch` | Änderungen vom Remote holen, aber nicht mergen. |
| `git merge <branch-name>` | Änderungen von einem Branch in den aktuellen Branch mergen. |

## 3. Konflikte und Zurücksetzen

### 3.1 Konflikte lösen

Konflikte manuell lösen und Dateien committen.

### 3.2 Änderungen rückgängig machen

| Befehl | Beschreibung |
|--------|--------------|
| `git revert <commit-id>` | Einen Commit rückgängig machen, ohne die Historie zu ändern. |
| `git reset --hard <commit-id>` | Zum angegebenen Commit zurücksetzen, alle Änderungen verwerfen. |
| `git reset --soft <commit-id>` | Zum angegebenen Commit zurücksetzen, Änderungen aber im Staging-Bereich behalten. |
| `git reset --mixed <commit-id>` | Zum angegebenen Commit zurücksetzen, Änderungen behalten, aber aus dem Staging-Bereich entfernen. |
| `git checkout -- <file>` | Änderungen an einer Datei verwerfen (seit letztem Commit). |
| `git reset HEAD <file>` | Datei vom Staging-Bereich entfernen. |

## 4. Stashing (Änderungen zwischenlagern)

| Befehl | Beschreibung |
|--------|--------------|
| `git stash` | Änderungen zwischenlagern. |
| `git stash apply` | Änderungen wiederherstellen. |
| `git stash drop` | Gestashte Änderungen verwerfen. |
| `git stash list` | Alle Stashes anzeigen. |

## 5. Tags erstellen

| Befehl | Beschreibung |
|--------|--------------|
| `git tag <tagname>` | Einen neuen Tag erstellen. |
| `git tag` | Alle Tags anzeigen. |
| `git push origin <tagname>` | Einen Tag pushen. |

## 6. Erweiterte Git Funktionen

### 6.1 Zusammenführen und Squashen

| Befehl | Beschreibung |
|--------|--------------|
| `git rebase <branch>` | Änderungen von einem Branch auf einen anderen umschreiben. |
| `git rebase -i HEAD~n` | Interaktives Rebase für die letzten `n` Commits (z. B. um Commits zusammenzuführen). |

### 6.2 Remote Branch löschen

| Befehl | Beschreibung |
|--------|--------------|
| `git push origin --delete <branch-name>` | Löscht einen Remote-Branch. |
