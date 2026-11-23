# Guestbook Application on Kubernetes

Este proyecto es una aplicación de libro de visitas (Guestbook) simple, desarrollada como parte del proyecto final del curso de Kubernetes. La aplicación consiste en un front-end web estático servido a través de Nginx y está diseñada para demostrar conceptos fundamentales de Kubernetes como Deployments, Pods, Horizontal Pod Autoscaling (HPA), Rolling Updates y Rollbacks en IBM Cloud.

## Características del Proyecto
- Contenedorización de la aplicación con Docker (Nginx Alpine).
- Despliegue en un clúster de Kubernetes (IBM Cloud Kubernetes Service).
- Escalado automático basado en el uso de CPU mediante HPA (Horizontal Pod Autoscaler).
- Actualizaciones continuas sin tiempo de inactividad (Rolling Updates).
- Reversión a versiones anteriores en caso de fallos (Rollbacks).

## Estructura de Archivos
```text
guestbook-project/
├── Dockerfile          # Configuración para construir la imagen de Nginx con la app
├── index.html          # Versión 1 de la aplicación web
├── index_v2.html       # Versión 2 de la aplicación web (actualización)
├── deployment.yml      # Manifiesto de Kubernetes para el Deployment
├── hpa.yml             # Manifiesto para el Horizontal Pod Autoscaler
└── README.md           # Documentación del proyecto