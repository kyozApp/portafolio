# 🌟 Despliegue de un Portafolio con Astro y Cloudflare Pages

---

## 1️⃣ **Crear un Proyecto con Astro**

Inicia un nuevo proyecto utilizando Astro:  

```bash
pnpm create astro@latest
```

---

## 2️⃣ **Configurar el Proyecto**

1. Navega al directorio del proyecto creado:

   ```bash
   cd portafolio
   ```

2. Ejecuta la herramienta de actualización de Astro:

   ```bash
   pnpm dlx @astrojs/upgrade
   ```

3. Instala para procesar las imagenes de Astro:

   ```bash
   pnpm add sharp
   ```

4. Instala para los iconos de Astro:

   ```bash
   pnpm astro add astro-icon
   ```

---

## 3️⃣ **Inicializar Git y Configurar el Repositorio**

1. Inicializa un repositorio Git:  

   ```bash
   git init
   ```

2. Agrega los archivos al repositorio:  

   ```bash
   git add .
   ```

3. Realiza un commit inicial:  

   ```bash
   git commit -m "Desplegando mi portafolio"
   ```

4. Crea un nuevo repositorio privado en GitHub vinculado al proyecto:  

   ```bash
   gh repo create portafolio --public --source=.
   ```

5. Cambia la rama predeterminada a `main` si esta en master:  

   ```bash
   git branch -m master main
   ```

6. Empuja los cambios a GitHub:  

   ```bash
   git push -u origin main
   ```

---

## 4️⃣ **Configurar Cloudflare Pages**

1. Accede al panel de control de Cloudflare Pages:  
   [Cloudflare Pages Dashboard](https://dash.cloudflare.com/f1b2dc87d8ae478eb50f53d0a9193523/workers-and-pages)  

2. Configura los siguientes parámetros:  
   - **Rama:** `main`
   - **Comando de compilación:**  
     ```bash
     pnpm astro build
     ```
   - **Directorio de salida:** `/dist`

---

### 🚀 ¡Tu portafolio estará desplegado en Cloudflare Pages!
- Aprovecha la velocidad de Astro y la infraestructura de Cloudflare para obtener un sitio web optimizado y rápido.

