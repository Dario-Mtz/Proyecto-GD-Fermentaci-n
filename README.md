[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=Dario-Mtz/Proyecto-GD-Fermentaci-n)

# Proyecto: Simulación dinámica de un proceso de fermentación mediante un sistema de ecuaciones diferenciales ordinarias

## Información general

**Alumno:** Dario Antonio Martinez Camarena  
**Número de control:** 21210684  
**Correo institucional:** l21210684@tectijuana.edu.mx  
**Asignatura:** Gemelos Digitales  
**Docente:** Dr. Paul Antonio Valle Trujillo  
**Institución:** Tecnológico Nacional de México / Instituto Tecnológico de Tijuana  
**Departamento:** Ingeniería Eléctrica y Electrónica  
**Carrera:** Ingeniería Biomédica  

---

## Descripción del proyecto

Este proyecto desarrolla un gemelo digital basado en un sistema de ecuaciones diferenciales ordinarias no lineales para simular la dinámica de un proceso de fermentación. El modelo considera tres variables principales: biomasa microbiana, producto generado y sustrato disponible.

La finalidad del modelo es representar la evolución dinámica del sistema, analizar su comportamiento mediante simulaciones numéricas, estudiar sus puntos de equilibrio y evaluar su estabilidad local. Además, se implementa una perturbación externa en Simulink para observar la respuesta del sistema ante cambios simulados en la alimentación del sustrato.

---

## Objetivo

Desarrollar un gemelo digital basado en ecuaciones diferenciales ordinarias para simular el comportamiento dinámico de un proceso de fermentación, considerando la evolución de la biomasa, el consumo de sustrato y la generación de producto, con el propósito de analizar el comportamiento del sistema y apoyar la toma de decisiones en condiciones simuladas de operación.

---

## Variables del modelo

| Variable | Descripción |
|---|---|
| `x(t)` | Biomasa microbiana |
| `y(t)` | Producto generado durante la fermentación |
| `z(t)` | Sustrato o nutriente disponible |

---

## Modelo matemático

El sistema dinámico utilizado está formado por tres ecuaciones diferenciales ordinarias no lineales de primer orden:

```math
\frac{dx}{dt}=a_1+a_2y-a_3x-a_4y^2
