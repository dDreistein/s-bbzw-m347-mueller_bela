# Fragen – Konfiguration und Umgebungsvariablen (DL11)

Name: <Nachname> <Vorname>
Klasse: <Klasse>

---

## 1. Konfiguration

Welche Werte waren ursprünglich hardcoded in `compose.yml` und `app/main.py`?

Antwort: Alle env variabeln z.B. DATABASE_URL, POSTGRES_PASSWORD...

---

Warum ist es ein Problem, Passwörter direkt in `compose.yml` einzutragen?

Antwort: Weil das compose.yml in die versionskontrolle kommt und so auch die passwörter öffentlich sind.

---

Was ist der Unterschied zwischen `.env` und `.env.example`?

Antwort: example enthält für private angaben nur platzhalter

---

Warum muss `.env` in `.gitignore` eingetragen sein?

Antwort: dass die secrets auf der lokalen maschine bleiben

---

## 2. Variablen in Compose

Wie referenziert man eine Variable aus `.env` in `compose.yml`?

Antwort:

---

Was passiert, wenn eine Variable in `.env` fehlt, aber in `compose.yml` verwendet wird?

Antwort:

---

Was zeigt der Befehl `docker compose config`? Wann ist er nützlich?

Antwort:

---

## 3. Dockerfile und Build

Warum wird `requirements.txt` in einem eigenen `COPY`-Schritt vor dem App-Code kopiert?

Antwort:

---

Was bewirkt `.dockerignore`? Welche Dateien sollten darin stehen?

Antwort:

---

## 4. Systemtest

Funktioniert `/db-check` nach Ihrer Konfigurationsanpassung?

Antwort:

---

Was zeigt der Endpunkt `/db-check` an, wenn die Verbindung funktioniert?

Antwort:

---

## 5. Reflexion

Was war der wichtigste Schritt in dieser Woche?

Antwort:

---

Was ist noch unklar oder möchten Sie besser verstehen?

Antwort:
