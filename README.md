<div align="center">
  <p align="center">
    <h1> 🧠🖥️ Lomina </h1>
  </p>
  <p>
    Asistente Inteligente para Gestión de Conocimiento Empresarial
  </p>
  
  [![English Docs](https://img.shields.io/badge/README-English-blue?style=for-the-badge)](./README.en.md)

</div>




## 🎯 Objetivo del Proyecto
Diseñar y desarrollar una aplicación web que funcione como un asistente inteligente interno para empresas, capaz de responder preguntas sobre documentación interna, políticas, manuales, y otros recursos, utilizando un modelo de lenguaje grande (LLM) ejecutado localmente. La arquitectura debe estar basada en microservicios, utilizar Angular para el frontend, y desplegarse completamente en un clúster de Kubernetes.

## 📘 Descripción del Problema
Las empresas acumulan grandes cantidades de documentos, manuales y políticas que muchas veces resultan difíciles de consultar por los empleados. Los buscadores tradicionales no son eficientes para responder preguntas complejas o contextuales. La dirección de la empresa ha decidido implementar una solución moderna basada en un asistente inteligente que funcione sin depender de servicios externos por razones de privacidad y confidencialidad.

## 🧱 Requisitos Técnicos
### 🖼️ 1. Frontend (Angular)
Interfaz simple donde el usuario pueda:

- Ingresar preguntas en lenguaje natural.
- Ver respuestas generadas por el LLM.
- Ver historial de preguntas y respuestas.

### 🗃️ 2. Backend y Microservicios
- **API Gateway:** Encargado de recibir las peticiones del frontend y orquestar las llamadas al resto de microservicios.
- **Servicio LLM:** Encapsula un modelo como LLaMA 3 o Mistral utilizando una herramienta local como ollama o llama.cpp.
- **Servicio de Indexación y Documentos:**
Permite cargar y preprocesar documentos empresariales (PDF, DOCX, etc.).
- **Servicio de autenticación:** Acceso mediante credenciales.
- Utiliza embeddings para indexarlos (opcional).

### 🎢 3. Despliegue en Kubernetes
Todos los servicios deben estar dockerizados y desplegados en Kubernetes.

Incluye:
- Archivos Deployment, Service y Ingress.
- Configuración de volúmenes persistentes para el LLM y almacenamiento de documentos.
- Escalabilidad: los microservicios deben ser escalables horizontalmente.

## 🧪 Hitos
- [ ] Correcta separación de responsabilidades entre microservicios.
- [ ] Capacidad del LLM para responder preguntas reales.
- [ ] Despliegue funcional en Kubernetes.
- [ ] Calidad de la interfaz de usuario.
- [ ] Uso de buenas prácticas:
  - [ ]  Código limpio.
  - [ ]  Documentación
  - [ ]  CI/CD.
