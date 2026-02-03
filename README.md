# 🚀 Ejercicio: Integración continua de una imagen Docker con GitHub Actions


## 🎯 Contexto  
El objetivo de este ejercicio es aprender a configurar un flujo de **integración continua (CI)** que construya automáticamente una imagen Docker de una aplicación Node.js monolítica (basada en Express.js) y la publique en **Docker Hub** usando **GitHub Actions**.

---

## 🥅 Objetivo  
Obtener una **imagen Docker lista para producción**, generada y publicada automáticamente en Docker Hub cada vez que se haga un push a la rama principal del repositorio.

---

## 📦 Tipo de aplicación  
- Arquitectura: **Monolítica**  
- Backend: **Node.js**  
- Framework: **Express.js**

---

## User Interface
![Home](./public/ss/home.png)

## Prerequisites 
1. GitHub Account
2. Docker Account

---

## 🛠️ Pasos a seguir

---

## 1. 🧱 Creación del `Dockerfile`

Crea un archivo llamado `Dockerfile` en la raíz del proyecto.

---

## 2. 🤖 Crear el workflow de GitHub Actions  
Este workflow construirá la imagen y la publicará en Docker Hub. Deberías iniciar con la plantilla proporcionada por GitHub.

Crea el archivo:

```
.github/workflows/docker-image.yml
```


### 🔐 Recuerda configurar los secretos en GitHub:
- `DOCKERHUB_USERNAME`
- `DOCKERHUB_TOKEN` (token de acceso generado en Docker Hub)

---

## 3. ✅ Comprobar la ejecución correcta

### Verificación en GitHub Actions
1. Ve a **Actions** en tu repositorio.  
2. Selecciona el workflow **Build and Push Docker Image**.  
3. Comprueba que todos los pasos aparecen en verde.

### Verificación en Docker Hub
1. Entra en tu cuenta de Docker Hub.  
2. Busca la imagen en tu repositorio.  

---

## 🎉 Resultado final  
Al completar este ejercicio, tendrás un pipeline funcional que:

- Construye automáticamente una imagen Docker de tu aplicación Node.js.  
- La publica en Docker Hub sin intervención manual.  
- Garantiza que siempre haya una versión lista para producción.

---