# screenLocker-installer

# Inicialización de Base de Datos (JSON)

Este proyecto utiliza un **JSON de configuración** para la **creación e inicialización de la base de datos** de comandos.

Toda la edición puede hacerse **directamente desde este README**, abriendo el enlace incluido más abajo.

---

## 📦 Ejemplo de JSON de creación de la base de datos

```json
{
  "pc_alejandro": {
    "command": "unlock",
    "message": "Hora de ayudar a poner la mesa"
  }
}

Este JSON define:
- **pc_alejandro** → identificador del dispositivo
- **command** → acción a ejecutar
- **message** → mensaje mostrado al usuario

---

## ✏️ Edición online del JSON (desde este README)

Puedes **editar este JSON directamente en el navegador** usando el siguiente enlace:

👉 **[Abrir editor online con el JSON precargado](https://jsoneditoronline.org/?json=%7B%22pc_alejandro%22%3A%7B%22command%22%3A%22unlock%22%2C%22message%22%3A%22Hora%20de%20ayudar%20a%20poner%20la%20mesa%22%7D%7D)**

Al abrir el enlace:
- El JSON se carga automáticamente
- Puedes editarlo en vista **árbol** o **texto**
- Copia el resultado final para guardarlo o usarlo en la aplicación

---
