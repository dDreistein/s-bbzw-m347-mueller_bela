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
env_file:
-   .env

und dann die werte mit ${KEY} platzhaltern

---

Was passiert, wenn eine Variable in `.env` fehlt, aber in `compose.yml` verwendet wird?

Antwort: sie kann nicht gelesen werden und es gibt einen fehler

---

Was zeigt der Befehl `docker compose config`? Wann ist er nützlich?

Antwort: zeigt das compose.yml mit eingesetzten env variablen

---

## 3. Dockerfile und Build

Warum wird `requirements.txt` in einem eigenen `COPY`-Schritt vor dem App-Code kopiert?

Antwort: da dieses erst die pip packages checkt welche tendenziell weniger changes haben.

---

Was bewirkt `.dockerignore`? Welche Dateien sollten darin stehen?

Antwort: Es sorgt dafür das bestimmte files vom dockefile ignoriert werden. darin gehören files wie packages, welche im buildprozess generiert werden.

---

## 4. Systemtest

Funktioniert `/db-check` nach Ihrer Konfigurationsanpassung?

Antwort: JA

---

Was zeigt der Endpunkt `/db-check` an, wenn die Verbindung funktioniert?

Antwort: {"db":"connected"}

---

## 5. Reflexion

Was war der wichtigste Schritt in dieser Woche?

Antwort: .env files erstellen

---

Was ist noch unklar oder möchten Sie besser verstehen?

Antwort: -
