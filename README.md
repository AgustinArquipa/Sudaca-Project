# Sudaca Box-Billing Project

<img src="sudaca.PNG" alt="Sudaca Logo" width="300" style="background-color:#dddcdc; padding: 10px; border-radius: 10px;">

Este es un proyecto base de **Django** diseñado para gestionar una caja registradora con funcionalidades de movimientos y arqueos. Proporciona una estructura escalable y está preparado para ser utilizado con una base de datos PostgreSQL.

---

## 🚀 Pasos de Instalación

### 1. Crear un Entorno Virtual

Utilizamos `venv` para manejar entornos virtuales. Para crear un nuevo entorno virtual llamado `sudaca-env`, ejecuta:

```bash
python3.11 -m venv sudaca-env
# o
python3 -m venv sudaca-env
```

Activar el entorno virtual:

- **Linux o Mac**:

```bash
source sudaca-env/bin/activate
```

- **Windows**:

```bash
sudaca-env\Scripts\activate
```

---

### 2. Instalación de Dependencias

Una vez dentro del entorno virtual, navega hasta la raíz del proyecto y ejecuta:

```bash
pip install -r requirements.txt
```

---

### 3. Configuración de Credenciales

Dentro de la raíz del proyecto, crea un archivo llamado `secret.json` con la siguiente estructura:

```json
{
    "FILENAME": "secret.json",
    "SECRET_KEY": "clave_secreta_pedir_administrador_del_sistema",
    "DB_NAME": "sudaca_db",
    "DB_USER": "postgres",
    "DB_PASSWORD": "your_password",
    "DB_HOST": "localhost",
    "DB_PORT": 5432,

    "EMAIL_HOST": "smtp.gmail.com",
    "EMAIL_HOST_USER": "sudaca@gmail.com",
    "EMAIL_HOST_PASSWORD": "<<password>>"
}
```

> **Nota**: Asegúrate de cambiar los valores de `SECRET_KEY`, `DB_NAME`, `DB_USER` y `DB_PASSWORD` a los apropiados para tu configuración.

---

### 4. Configuración de la Base de Datos

Dado que utilizamos PostgreSQL como base de datos, asegúrate de tenerlo instalado y en ejecución.

---

### 5. Crear y Aplicar Migraciones

Para crear las migraciones y aplicarlas, ejecuta:

```bash
python manage.py makemigrations
python manage.py migrate
```

---

### 6. Configuración de Variables de Entorno

Configura la variable de entorno necesaria antes de ejecutar la aplicación:

- **En sistemas Unix/Linux/Mac**:

```bash
export DEVELOPMENT_ENVIRONMENT=True
```

- **En Windows (CMD)**:

```cmd
set DEVELOPMENT_ENVIRONMENT=True
```

- **En Windows (PowerShell)**:

```powershell
$env:DEVELOPMENT_ENVIRONMENT = "True"
```

---

### 7. Ejecutar el Proyecto

Inicia el servidor de desarrollo:

```bash
python manage.py runserver
```

Accede a tu proyecto desde [http://localhost:8000/](http://localhost:8000/).

---
## 🎨 Paleta de Colores

<table>
  <tr>
    <td><div style="width: 40px; height: 40px; background-color: #db1010; border: 1px solid #000;"></div></td>
    <td><b>#db1010 (Rojo)</b>: Utilizado para elementos destacados, botones de acción y alertas importantes.</td>
  </tr>
  <tr>
    <td><div style="width: 40px; height: 40px; background-color: #b75151; border: 1px solid #000;"></div></td>
    <td><b>#b75151 (Rosado Fondo)</b>: Ideal para fondos suaves y contextos secundarios que no distraigan.</td>
  </tr>
  <tr>
    <td><div style="width: 40px; height: 40px; background-color: #dddcdc; border: 1px solid #000;"></div></td>
    <td><b>#dddcdc (Blanco Huesi)</b>: Para fondos principales y elementos neutrales, dando un aspecto limpio.</td>
  </tr>
</table>

Puedes ajustar esta paleta para mejorar el diseño visual según tus necesidades.


## ¡Listo!

Ahora puedes utilizar tu sistema **Sudaca Box-Billing** para gestionar movimientos y arqueos. Si necesitas ayuda adicional, no dudes en contactarnos.

