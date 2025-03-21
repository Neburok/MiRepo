---
layout: assessment
title: "Ejercicios: Estructura de Bandas y Propiedades Electrónicas"
subject: "Física del Estado Sólido"
difficulty: "Intermedio-Avanzado"
estimated_time: "2 horas"
last_updated: 2025-03-12
description: "Conjunto de problemas para reforzar la comprensión de la estructura de bandas en semiconductores y sus propiedades electrónicas derivadas."
prerequisites:
  - "Teoría de bandas de energía"
  - "Estadística de Fermi-Dirac"
  - "Ecuación de Schrödinger para potenciales periódicos"
solutions_available: true
solutions:
  - |
    Para resolver este problema, aplicamos la ecuación de la densidad de estados:
    
    $$D(E) = \frac{1}{2\pi^2}\left(\frac{2m^*}{\hbar^2}\right)^{3/2}\sqrt{E-E_c}$$
    
    Sustituyendo los valores dados:
    $m^* = 0.26m_0 = 0.26 \times 9.11 \times 10^{-31} \text{ kg}$
    $E - E_c = 0.1 \text{ eV} = 0.1 \times 1.602 \times 10^{-19} \text{ J}$
    
    Obtenemos $D(E) = 8.32 \times 10^{21} \text{ estados/m}^3\text{/eV}$
  - |
    La masa efectiva se relaciona con la curvatura de la banda mediante:
    
    $$\frac{1}{m^*} = \frac{1}{\hbar^2}\frac{d^2E}{dk^2}$$
    
    La banda parabólica dada por $E(k) = E_0 + \alpha k^2$ tiene $\frac{d^2E}{dk^2} = 2\alpha$
    
    Por lo tanto, $m^* = \frac{\hbar^2}{2\alpha}$
    
    Con $\alpha = 6.8 \times 10^{-20} \text{ J}\cdot\text{m}^2$, obtenemos $m^* = 0.32m_0$
references:
  - "Kittel, C. (2018). Introduction to Solid State Physics. 8th Edition. Wiley."
  - "Yu, P.Y., Cardona, M. (2010). Fundamentals of Semiconductors: Physics and Materials Properties. 4th Edition. Springer."
---

# Ejercicios sobre Estructura de Bandas y Propiedades Electrónicas

## Problemas Teóricos

### Ejercicio 1
Calcule la densidad de estados en la banda de conducción del silicio a una energía 0.1 eV por encima del borde de la banda. Considere que la masa efectiva de los electrones es $m^* = 0.26m_0$, donde $m_0$ es la masa del electrón libre.

### Ejercicio 2
Se ha determinado experimentalmente que la relación de dispersión para electrones cerca del mínimo de la banda de conducción en un semiconductor puede aproximarse mediante $E(k) = E_0 + \alpha k^2$, donde $\alpha = 6.8 \times 10^{-20} \text{ J}\cdot\text{m}^2$. Calcule la masa efectiva de estos electrones.

### Ejercicio 3
Un semiconductor tiene una brecha de energía directa de 1.5 eV a 300 K. Si el coeficiente de temperatura de la brecha de energía es de $-4 \times 10^{-4}$ eV/K, ¿cuál será el valor de la brecha de energía a 400 K?

## Problemas Numéricos

### Ejercicio 4
La densidad de estados efectiva en la banda de conducción de un semiconductor está dada por:

$$N_c = 2\left(\frac{2\pi m_e^*kT}{h^2}\right)^{3/2}$$

Calcule $N_c$ para el GaAs a temperatura ambiente (300 K), sabiendo que $m_e^* = 0.067m_0$.

### Ejercicio 5
Considere un semiconductor intrínseco a 300 K con una brecha de energía de 1.1 eV. Si las masas efectivas son $m_e^* = 1.08m_0$ y $m_h^* = 0.56m_0$, calcule la concentración intrínseca de portadores.

## Problemas Aplicados

### Ejercicio 6
Un cristal semiconductor tiene la siguiente estructura de bandas en el punto Γ (k = 0):
- La banda de valencia máxima está en E = 0 eV
- Existen tres bandas de conducción con mínimos en:
  - E = 2.0 eV, con masa efectiva $m_1^* = 0.2m_0$
  - E = 2.3 eV, con masa efectiva $m_2^* = 0.3m_0$
  - E = 2.8 eV, con masa efectiva $m_3^* = 0.5m_0$

a) ¿Cuál es la brecha de energía de este semiconductor?
b) Calcule la densidad efectiva de estados en la banda de conducción a 300 K.
c