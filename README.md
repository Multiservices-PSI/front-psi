# Frontend - Microservicios UI

Este repositorio contiene la interfaz de usuario del proyecto, construida con **Vue 3** y el motor **Vite**. Está diseñada para interactuar de forma concurrente con un backend de microservicios (Java/Spring Boot y C#/.NET) a través de un API Gateway configurado en Nginx.

## Stack Tecnológico

- **Framework Core:** Vue 3
- **Entorno y Build:** Vite
- **Gestor de Paquetes:** pnpm
- **Manejo del Estado:** Pinia
- **Enrutamiento:** Vue Router
- **Peticiones HTTP:** Axios

## Requisitos Previos

Para levantar este proyecto necesitas tener instalado Node.js. Además, este proyecto utiliza **pnpm** por su velocidad y eficiencia en el manejo de dependencias.

Si no tienes `pnpm` instalado en tu máquina, instálalo globalmente ejecutando:

```bash
npm install -g pnpm
```

1. Instalar dependencias

Una vez clonado el repositorio, entra a la carpeta raíz y descarga todas las librerías necesarias:

```bash
pnpm install
```

2. Entorno de Desarrollo

Levanta el servidor local de Vite. Esto habilitará la recarga rápida (HMR) para ver los cambios en tiempo real mientras programas:

```bash
pnpm dev
```

3. Compilación para Producción (Nginx / Docker)

Cuando el código esté listo para integrarse al pipeline de CI/CD, ejecuta el siguiente comando. Esto empaquetará, minificará y optimizará los archivos estáticos dentro de una nueva carpeta llamada dist:

```bash
pnpm build
```

4. Previsualizar Producción Localmente

Si quieres asegurarte de que la compilación de la carpeta dist funciona correctamente antes de desplegar al servidor Ubuntu, puedes simular un entorno de producción con:

```bash
pnpm preview
```
