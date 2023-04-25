## 🚀 Integración Continua con GitHub Actions, Docker y Jenkins 🚀

Este repositorio contiene el código fuente del proyecto explicado en el video "[Maquina de Integración Continua con Google Cloud, GitHub Actions, Docker y Jenkins](https://youtu.be/kC2-fSGzKS0)". En este tutorial, te enseñamos cómo construir una máquina de integración continua básica, pero completamente funcional, utilizando GitHub Actions, Docker, el registro de GitHub (GitHub Packages) y Jenkins.

### 📁 Estructura del repositorio

El archivo principal de configuración de GitHub Actions se encuentra en la siguiente ruta: `example-cicd-integration/.github/workflows/main.yml`

### 🌟 Flujo de trabajo

Este flujo de trabajo realiza las siguientes acciones:

1. Configura un entorno de ejecución basado en Ubuntu 20.04.
2. Utiliza Node.js en la versión especificada en la matriz de estrategia.
3. Inicia sesión en el registro de contenedores de GitHub (ghcr.io) utilizando las credenciales proporcionadas.
4. Construye y sube la imagen de Docker con la etiqueta correspondiente al nombre de la referencia (rama o etiqueta) actual.
5. Construye y sube la imagen de Docker con la etiqueta "latest".
6. Ejecuta un trabajo en Jenkins mediante una solicitud HTTP POST al webhook genérico.

### 📚 Recursos adicionales

Si deseas obtener más información sobre cómo configurar y utilizar GitHub Actions, Docker, GitHub Packages y Jenkins, consulta la [documentación oficial](https://docs.github.com/en/actions) y no olvides ver el video tutorial en el siguiente enlace: [Maquina de Integración Continua con Google Cloud, GitHub Actions, Docker y Jenkins](https://youtu.be/kC2-fSGzKS0)

