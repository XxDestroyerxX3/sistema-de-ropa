# Proyecto Tienda de Ropa - Django

Aplicación web desarrollada con Django para gestionar una tienda de ropa, incluyendo administración de productos, variantes, imágenes, stock, órdenes de compra y funcionalidades de carrito y lista de deseos.

---

## Requisitos

- Python 3.10 o superior
- Django 4.x
- pip (gestor de paquetes)
- Virtualenv (recomendado para entornos aislados)

---

## Instalación

### 1. Clonar el repositorio

```bash
git clone https://github.com/restreh/ST0261-TEIS-Proyecto.git
cd ST0261-TEIS-Proyecto
2. Crear y activar entorno virtual
Linux/macOS:

bash
Copiar
python3 -m venv env
source env/bin/activate
Windows PowerShell:

powershell
Copiar
python -m venv env
.\env\Scripts\activate
3. Instalar dependencias
bash
Copiar
pip install -r requirements.txt
4. Configurar variables de entorno
Crear un archivo .env en la raíz del proyecto con el siguiente contenido:

env
Copiar
DEBUG=True
SECRET_KEY=tu_clave_secreta_generada
EMAIL_BACKEND=django.core.mail.backends.smtp.EmailBackend
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USE_TLS=True
EMAIL_HOST_USER=tu_email@gmail.com
EMAIL_HOST_PASSWORD=tu_contraseña_de_aplicación
Nota: Genera la clave secreta con:

bash
Copiar
python -c "import secrets; print(secrets.token_urlsafe(50))"
Para la contraseña de aplicación en Gmail, habilita la verificación en dos pasos y crea una contraseña de aplicación en tu cuenta Google.

5. Aplicar migraciones
bash
Copiar
python manage.py makemigrations
python manage.py migrate
6. Crear superusuario (para acceso a admin)
bash
Copiar
python manage.py createsuperuser
Sigue las instrucciones para crear un usuario administrador.

7. Ejecutar el servidor
bash
Copiar
python manage.py runserver
Abre tu navegador en http://127.0.0.1:8000

Funcionalidades
Navegación y búsqueda de productos

Gestión avanzada de variantes y stock

Carrito de compras y lista de deseos

Panel administrativo para gestionar productos, órdenes y usuarios

Integración con sistema de envío de correo para notificaciones

Solución de problemas comunes
Error: No se encuentra variable de entorno SECRET_KEY
Verifica que el archivo .env esté en la raíz del proyecto y que contenga la variable SECRET_KEY.
Además, asegúrate de que django-environ esté instalado (pip install django-environ).

Problemas con activación del entorno virtual en Windows
Usa PowerShell y ejecuta:

powershell
Copiar
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
para permitir la ejecución de scripts.

Contacto
Para dudas o reportar problemas, abre un issue en el repositorio o contacta a [tu correo].

Licencia
Este proyecto está bajo la licencia MIT.

yaml
Copiar

---

¿Quieres que te lo guarde en un archivo `.md` para que puedas descargarlo?
