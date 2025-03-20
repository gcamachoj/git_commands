# 🚀 Comandos Esenciales de Git

Este repositorio contiene una guía rápida de los comandos más utilizados en **Git**, útil para consultar en el día a día.

---

## 📌 Tabla de Contenidos
1. [Inicialización y Configuración](#inicialización-y-configuración)
2. [Trabajando con Repositorios Remotos](#trabajando-con-repositorios-remotos)
3. [Seguimiento de Cambios](#seguimiento-de-cambios)
4. [Trabajando con Ramas](#trabajando-con-ramas)
5. [Fusión y Rebase](#fusión-y-rebase)
6. [Historial y Estado del Repositorio](#historial-y-estado-del-repositorio)
7. [Otras Utilidades](#otras-utilidades)

---

## 1️⃣ Inicialización y Configuración

### 🛠 **Inicializar un Repositorio**
```bash
git init
```
Inicializa un nuevo repositorio en la carpeta actual, creando la estructura necesaria de Git.

### 🔍 **Configurar Usuario y Correo**
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```
Establece el nombre y correo que aparecerán en los commits.

---

## 2️⃣ Trabajando con Repositorios Remotos

### 🔄 **Clonar un Repositorio**
```bash
git clone <URL_DEL_REPOSITORIO>
```
Crea una copia local de un repositorio remoto.

### 🔗 **Ver los Repositorios Remotos Asociados**
```bash
git remote -v
```
Muestra la lista de repositorios remotos configurados.

### 🔄 **Actualizar el Repositorio Local con Cambios Remotos**
```bash
git pull origin main
```
Descarga y fusiona cambios del repositorio remoto en la rama local.

### 🚀 **Enviar Cambios al Repositorio Remoto**
```bash
git push origin main
```
Sube los cambios locales a la rama `main` del repositorio remoto.

---

## 3️⃣ Seguimiento de Cambios

### 📌 **Añadir Cambios al Área de Preparación (Staging)**
```bash
git add <archivo>
git add .
```
Agrega archivos específicos o todos los archivos modificados al área de preparación.

### 📝 **Confirmar Cambios en el Repositorio**
```bash
git commit -m "Mensaje descriptivo del cambio"
```
Guarda los cambios en el historial con un mensaje.

---

## 4️⃣ Trabajando con Ramas

### 🌱 **Listar Ramas Disponibles**
```bash
git branch
```
Muestra todas las ramas del repositorio.

### ➕ **Crear una Nueva Rama**
```bash
git branch <nombre_de_la_rama>
```
Crea una nueva rama a partir de la rama actual.

### 🔄 **Cambiar de Rama**
```bash
git checkout <nombre_de_la_rama>
```
Cambia a una rama específica.

### 🏎️ **Crear y Moverse a una Nueva Rama**
```bash
git checkout -b <nombre_de_la_rama>
```
Crea una nueva rama y cambia a ella en un solo paso.

---

## 5️⃣ Fusión y Rebase

### 🔀 **Fusionar Ramas**
```bash
git merge <nombre_de_la_rama>
```
Une los cambios de una rama en la rama actual.

### ♻ **Rebase (Reorganizar Commits)**
```bash
git rebase <rama_base>
```
Reaplica los commits de una rama sobre otra base para mantener un historial más limpio.

---

## 6️⃣ Historial y Estado del Repositorio

### 🔍 **Ver el Estado del Repositorio**
```bash
git status
```
Muestra información sobre los archivos modificados y no confirmados.

### 📜 **Ver el Historial de Commits**
```bash
git log --oneline --graph --decorate --all
```
Muestra un historial resumido de commits con una representación gráfica de las ramas.

---

## 7️⃣ Otras Utilidades

### ❌ **Eliminar una Rama**
```bash
git branch -d <nombre_de_la_rama>
```
Elimina una rama local si ya se ha fusionado.

```bash
git branch -D <nombre_de_la_rama>
```
Elimina una rama local forzosamente.

### ⏪ **Deshacer Último Commit (Manteniendo Cambios)**
```bash
git reset --soft HEAD~1
```
Deshace el último commit pero mantiene los archivos en el área de preparación.

### 🔥 **Descartar Cambios en un Archivo**
```bash
git checkout -- <archivo>
```
Revierte los cambios de un archivo al último commit confirmado.

---

## 🚀 Conclusión
Este archivo proporciona un conjunto de comandos esenciales para gestionar proyectos con Git. Puedes usarlo como referencia rápida o complementarlo con más comandos según tus necesidades.

📌 **¡Sigue practicando y mejora tu flujo de trabajo con Git!** 🚀
