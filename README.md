# Safe ID - Protección de DNI Argentino 🇦🇷

Una herramienta web segura para proteger documentos de identidad mediante marcas de agua y ofuscación de datos sensibles.

## 🔗 Acceso

Accede a la herramienta en: https://datosargentinos.com

## 🌟 Características

- ✨ Procesamiento 100% local (no se suben archivos a ningún servidor)
- 🔒 Ofuscación de datos sensibles con control de intensidad
- 💧 Marca de agua personalizada con texto y patrones
- 🎨 Interfaz moderna y fácil de usar
- 📱 Totalmente responsive (funciona en móviles y tablets)
- 🔍 Vista previa en tiempo real
- ↔️ Comparador visual antes/después
- 📲 Compatible con PWA (instalable como app)
- 🌐 Funciona sin conexión (offline)

## ��️ Seguridad

- Todo el procesamiento se realiza en el navegador del usuario
- No se almacena ninguna imagen en servidores externos
- Las imágenes nunca abandonan el dispositivo del usuario
- Proceso de ofuscación irreversible
- Marcas de agua persistentes y difíciles de remover

## 🚀 Uso

1. **Subir Imagen**
   - Arrastra y suelta o selecciona una imagen de tu DNI
   - Formatos soportados: JPG y PNG

2. **Agregar Marca de Agua**
   - Ingresa el texto para la marca de agua (máx. 60 caracteres)
   - Recomendación: incluye destinatario y propósito específico

3. **Ofuscar Datos Sensibles**
   - Activa el modo ofuscación
   - Ajusta la intensidad del efecto
   - Dibuja sobre las áreas que deseas proteger

4. **Descargar Resultado**
   - Previsualiza el resultado final
   - Descarga la imagen protegida

5. **Instalar como App (Opcional)**
   - En Chrome/Edge: Haz clic en el ícono "Instalar" en la barra de direcciones
   - En móviles: Selecciona "Agregar a pantalla principal"
   - Usa la app sin conexión cuando la necesites

## 💡 Recomendaciones de Uso

- **Datos a Ofuscar:**
  - Número de trámite
  - Códigos de barras y QR
  - Información no necesaria para el trámite específico

- **Marca de Agua:**
  - Incluye el nombre del destinatario
  - Especifica el propósito del trámite
  - Agrega la fecha
  - Ejemplo: "Para Banco XYZ - Validación de identidad - 16/02/2024"

## ❓ Preguntas Frecuentes

- **¿Es seguro usar esta herramienta?**
  - Sí, la marca de agua se procesa localmente en tu navegador. Ninguna imagen se sube a servidores externos, garantizando la privacidad de tus datos.

- **¿Por qué debo proteger mi DNI al compartirlo?**
  - Compartir tu DNI sin protección puede llevar a suplantación de identidad y fraudes. Al agregar una marca de agua y ofuscar datos sensibles, reduces significativamente estos riesgos.

- **¿Qué datos debo ofuscar de mi DNI?**
  - Se recomienda ofuscar el número de trámite, los códigos de barras y QR, y cualquier otro dato que no sea necesario para el propósito específico del trámite.

- **¿Qué texto debo usar en la marca de agua?**
  - Es recomendable incluir el nombre del destinatario y el propósito específico, por ejemplo: "Para Banco XYZ - Validación de identidad - DD/MM/AAAA".

- **¿Las imágenes procesadas son válidas para trámites?**
  - Sí, siempre que los datos principales (foto, nombre, número de DNI) sean claramente visibles. Consulta con la entidad específica sobre sus requisitos.

- **¿Dónde puedo ver el código fuente del proyecto?**
  - El código es open source y está disponible en [GitHub](https://github.com/Xyborg/datosargentinos.com). Puedes revisarlo, contribuir o reportar problemas.

- **¿Puedo usar la herramienta sin internet?**
  - Sí, una vez instalada como PWA (Progressive Web App) en tu dispositivo, puedes usar todas las funciones sin conexión a internet.

- **¿Cómo instalo la app en mi dispositivo?**
  - En navegadores de escritorio: Busca el ícono de instalación en la barra de direcciones
  - En dispositivos móviles: Selecciona "Agregar a pantalla principal" en el menú del navegador
  - La app se instalará y podrás acceder directamente desde tu escritorio o pantalla de inicio

## 🔧 Tecnologías Utilizadas

- HTML5 Canvas para procesamiento de imágenes
- JavaScript puro (vanilla) para manipulación de imágenes
- CSS moderno con Tailwind-like utilities
- Diseño responsive y mobile-first

## 💻️ Deploy en local

### Usando docker

1. Clonar repositorio
```bash
git clone https://github.com/xyborg/datosargentinos.com --depth 1
```
2. Crear archivo compose.yml con el siguiente contenido:
```docker
services:
   app:
      image: httpd:latest
      volumes:
         - ./datosargentinos.com:/usr/local/apache2/htdocs/
      ports:
         - 1234:80
      restart: always
```
3. Levantar el server
```bash
docker compose up -d
```
4. Acceder a [localhost:1234](http://localhost:1234) (o el puerto que hayas elegido) y usar
5. Actualizar el sitio
Simplemente accedes al directorio del repositorio y haces un `git pull`

## 👨‍💻 Desarrollo

Este proyecto fue desarrollado por [Martin Aberastegue](https://www.martinaberastegue.com), inspirado en [Saferlayer.com](https://saferlayer.com) y adaptado específicamente para el caso de uso del DNI Argentino.

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🔐 Privacidad

Para más información sobre nuestra política de privacidad, visita [nuestra política de privacidad](https://www.iubenda.com/privacy-policy/69980701). 
