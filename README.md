# ScreenLocker – Installer (Beta)

ScreenLocker es una pequeña aplicación para **bloquear la pantalla de un ordenador Windows** y mostrar un **mensaje personalizado** (por ejemplo: *“Hora de cenar”* o *“Se acabó el ordenador”*).

Está pensada para ayudar a los padres a **evitar discusiones cuando se acaba el tiempo de uso del PC**.

⚠️ **Estado actual**: versión Beta / pruebas.  
Funciona bien, pero es sencilla y mejorable. El objetivo es probarla y recoger feedback.

---

## 🧠 ¿Cómo funciona ScreenLocker?

1. El ordenador tiene instalada la aplicación ScreenLocker.
2. El padre/madre accede a una **base de datos online** (Firebase).
3. En esa base de datos:
   - Se indica si el ordenador debe estar **bloqueado (`lock`)** o **desbloqueado (`unlock`)**
   - Se puede cambiar el **mensaje** que verá el niño en pantalla
4. La aplicación consulta esa base de datos y:
   - Bloquea la pantalla
   - Muestra el mensaje configurado

👉 El control se hace **desde cualquier dispositivo** (móvil, tablet, otro ordenador).

---

## 🔄 Importante
- Tras instalar la aplicación es necesario **reiniciar el ordenador una vez**.
- El ordenador debe estar **conectado a Internet**.
- El bloqueo/desbloqueo es **manual**: hay que cambiar el valor `lock / unlock` en la base de datos.

---

## 🎥 Vídeo: cómo configurar el backend (Firebase)

Antes de usar ScreenLocker necesitas crear una **base de datos en Firebase**.

En este vídeo se explica **paso a paso** cómo hacerlo:

<a href="https://youtu.be/KFYa1E_6j00?si=JoEpb40r53uDv_Wt" target="_blank" rel="noopener noreferrer">
🎥 Ver vídeo: Configuración del backend con Firebase
</a>

---

## 🗄️ Inicialización de la Base de Datos (JSON)

La base de datos se define con un **JSON** como el siguiente:

```json
{
  "pc_alejandro": {
    "command": "unlock",
    "message": "Hora de ayudar a poner la mesa"
  }
}
```

Este JSON define:
- **pc_alejandro** → identificador del dispositivo
- **command** → acción a ejecutar
- **message** → mensaje mostrado al usuario

---

## ✏️ Edición online del JSON (desde este README)

Puedes **editar este JSON directamente en el navegador** usando el siguiente enlace:

<a href="https://jsoneditoronline.org/?json=%7B%22pc_alejandro%22%3A%7B%22command%22%3A%22unlock%22%2C%22message%22%3A%22Hora%20de%20ayudar%20a%20poner%20la%20mesa%22%7D%7D" target="_blank" rel="noopener noreferrer">
👉 Abrir editor online con el JSON precargado
</a>

Al abrir el enlace:
- El JSON se carga automáticamente
- Puedes editarlo en vista **árbol** o **texto**
- Copia el resultado final para guardarlo o usarlo en la aplicación

---
