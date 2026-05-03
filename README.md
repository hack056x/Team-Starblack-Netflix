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

├── templates/

│             ├── login.html

│             ├── register.html

│             └── index.html

└── static/

           ├── style.css
    
           ├── login.css
    
           └── register.css
    

    
