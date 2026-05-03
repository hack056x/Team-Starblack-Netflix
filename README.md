📋 Requisitos previos
Antes de comenzar, asegúrate de tener:

Una cuenta en GitHub (gratuita)

Una cuenta en Render.com (puedes registrarte con GitHub)

Tu proyecto funcionando localmente

🚀 Paso 1: Preparar los archivos para producción

Asegúrate de que tu proyecto tenga esta estructura exacta:

Team-Starblack-Netflix/

├── app.py                 # Tu aplicación Flask

├── requirements.txt       # Dependencias de Python

├── Procfile               # ¡IMPORTANTE! Comando de inicio

├── users.txt              # Se creará automáticamente

├── templates/login.html, register.html, index.html.

└── static/style.css, login.css, register.css
    

🚀 Paso 2: Subir el código a GitHub

este paso no explico porque si leer esto ya sabe como hacerlo


🚀 Paso 3: Desplegar en Render

3.1 Crear el Web Service
Inicia sesión en render.com (usa "Sign in with GitHub")

Haz clic en "New +" → "Web Service" 

Conecta tu repositorio de GitHub:

Si es la primera vez, autoriza a Render a acceder a tus repos

Busca y selecciona Team-Starblack-Netflix


3.2 Configurar el servicio
Completa el formulario con estos valores:

Campo	Valor

Name	netflix-token-generator (o el nombre que quieras)

Root Directory	Déjalo vacío (tu proyecto está en la raíz)

Environment	Python 3 

Build Command	pip install -r requirements.txt

Start Command	gunicorn app:app



    
