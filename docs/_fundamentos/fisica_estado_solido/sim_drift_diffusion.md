---
layout: simulation
title: "Simulación: Transporte de Portadores - Difusión y Deriva"
subject: "Física de Semiconductores"
complexity: "Avanzado"
tech_stack: ["JavaScript", "D3.js", "WebGL"]
last_updated: 2025-03-12
description: "Esta simulación interactiva permite visualizar los mecanismos de transporte de portadores (electrones y huecos) en un semiconductor bajo diferentes condiciones de campo eléctrico, gradiente de concentración y temperatura."
theory: |
  El transporte de portadores en semiconductores se rige principalmente por dos mecanismos:
  
  1. **Deriva (Drift)**: Movimiento de portadores debido a un campo eléctrico aplicado. La velocidad de deriva está dada por:
     
     $$v_d = \mu E$$
     
     donde $\mu$ es la movilidad del portador y $E$ es el campo eléctrico.
  
  2. **Difusión**: Movimiento de portadores debido a un gradiente de concentración. La densidad de corriente de difusión está dada por:
     
     $$J_{\text{difusión}} = qD\nabla n$$
     
     donde $D$ es el coeficiente de difusión, $n$ es la concentración de portadores, y $q$ es la carga elemental.
js_component: "drift_diffusion_sim.js"
exercises:
  - "Modifique el campo eléctrico a 10⁴ V/m y observe el comportamiento de los electrones. ¿Cómo cambia la velocidad media? Compare con el valor teórico calculado usando la movilidad del silicio."
  - "Establezca un gradiente de concentración y desactive el campo eléctrico. Observe el proceso de difusión y estime el coeficiente de difusión comparando con la evolución teórica."
  - "Active simultáneamente el campo eléctrico y el gradiente de concentración en direcciones opuestas. Encuentre el punto de equilibrio donde la corriente neta sea cero."
references:
  - "Sze, S.M., Ng, K.K. (2006). Physics of Semiconductor Devices. 3rd Edition. Wiley."
  - "Lundstrom, M. (2000). Fundamentals of Carrier Transport. 2nd Edition. Cambridge University Press."
---

## Controles de la Simulación

### Parámetros del Material
- **Material**: Seleccione el semiconductor (Si, Ge, GaAs)
- **Temperatura**: Ajuste entre 200K y 500K
- **Dopaje**: Configure tipo (N o P) y concentración

### Condiciones Eléctricas
- **Campo Eléctrico**: Ajuste magnitud y dirección
- **Potencial de Barrera**: Configure barreras de potencial

### Distribución de Portadores
- **Concentración Inicial**: Uniforme o con gradiente
- **Inyección de Portadores**: Puntual o en región específica

### Visualización
- **Modo de Visualización**: Partículas individuales o densidad
- **Escala de Tiempo**: Ajuste la velocidad de la simulación
- **Trayectorias**: Muestre/oculte el camino de los portadores

## Interpretación de Resultados

La visualización muestra el movimiento de los portadores con código de colores:
- **Rojo**: Huecos
- **Azul**: Electrones

El panel inferior muestra gráficas en tiempo real de:
- Distribución espacial de portadores
- Densidad de corriente
- Velocidad media vs. Campo eléctrico

Para guardar los resultados de la simulación, utilice el botón "Exportar datos" que generará un archivo CSV con los valores numéricos.