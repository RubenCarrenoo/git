# Proyecto Git Flow

## Objetivo
Aplicar el flujo de trabajo Git Flow utilizando Conventional Commits en un proyecto Python simple.

---

## 1. Creación del proyecto

Se creó una nueva carpeta en Documents:

mkdir git
Se inicializó el repositorio:

git init

---

## 2. Inicialización de Git Flow

Se ejecutó:

git flow init

Se aceptaron todas las configuraciones por defecto:
- main
- develop
- feature/
- release/
- hotfix/

---

## 3. Creación de Feature

git flow feature start saludo

Se realizaron dos commits usando Conventional Commits:

git commit -m "feat: add saludar function"
git commit -m "feat: add despedir function"

Se finalizó la feature:

git flow feature finish saludo

---

## 4. Creación de Release

git flow release start 1.0.0

Se actualizó el README:

git commit -m "docs: update README for release 1.0.0"

Finalización:

git flow release finish 1.0.0

Se creó el tag 1.0.0

---

## 5. Creación de Hotfix

git flow hotfix start 1.0.1

Se corrigió un error menor:

git commit -m "fix: correct despedir message format"

Finalización:

git flow hotfix finish 1.0.1

Se creó el tag 1.0.1

---

## Estructura final del proyecto

- app.py
- README.md

---

## Conventional Commits utilizados

- feat
- fix
- docs
- chore
