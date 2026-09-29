# Secure Lab App

Aplicación Node.js/Express de laboratorio para la práctica de Git, GitHub y Docker (DevSecOps).

## Ejecución local
    npm install
    npm start

## Ejecución con Docker
    docker build -t secure-lab-app:1.0 .
    docker run -d --name secure-lab-app -p 8080:3000 -e APP_ENV=lab secure-lab-app:1.0

## Endpoints
- `GET /` — información básica y entorno
- `GET /health` — estado de salud (`{"status":"UP"}`)
