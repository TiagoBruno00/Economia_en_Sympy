# Economia en Sympy
Este repositorio demuestra la potencia de la librería **SymPy** para la resolución de modelos de teoría económica y aplicaciones econométricas. El objetivo es automatizar el álgebra compleja, resolver sistemas dinámicos y optimizar funciones de pérdida mediante cálculo simbólico.

## Contenido del Proyecto

### 1. Incertidumbre y Política Económica (Brainard, 1967)
Implementación del modelo clásico de **William Brainard**.
- **El problema:** La incertidumbre sobre la estructura de la economía genera incentivos para que los *policymakers* actúen con cautela ("gradualismo").
- **La solución:** Se demuestra computacionalmente cómo la función de pérdida esperada se vuelve convexa bajo incertidumbre, llevando a respuestas de política atenuadas en lugar de cambios discretos grandes.

### 2. Crecimiento Endógeno con Capital Público (Heijdra, 2017)
Resolución del **Intermezzo 14.1** de *Foundations of Modern Macroeconomics*, como tarea en mi puesto de auxiliar de investigación.
- **El modelo:** Un modelo de crecimiento endógeno donde el capital público genera externalidades positivas en la producción.
- **Implementación:** Se resuelven simbólicamente:
  - El Hamiltoniano y las condiciones de primer orden (CPO).
  - Las ecuaciones de Euler del consumidor y la firma.
  - La **linealización del sistema dinámico** (Matriz Jacobiana) para analizar la estabilidad del equilibrio a largo plazo.

### 3. Algoritmo Newton-Raphson para Mínimos Cuadrados No Lineales (Judge et al., 1988)
Esta es una clase que realicé para la cátedra de **Econometría III** en mi rol de adscripto.
- **Aplicación:** Estimación de parámetros mediante la minimización de la Suma de Cuadrados de los Residuos (SSR).
- **Técnica:** Se utiliza SymPy para calcular dinámicamente el **Gradiente** y el **Hessiano** de la función objetivo, automatizando el algoritmo de optimización sin necesidad de derivar manualmente.

## Herramientas
* **Python 3.x**
* **SymPy:** Cálculo simbólico y álgebra computacional.
* **NumPy:** Computación numérica (vía `lambdify`).
* **Matplotlib:** Visualización de resultados y fronteras de optimización.

## Referencias
1.  **Brainard, W. C. (1967).** Uncertainty and the effectiveness of policy. *American Economic Review*, 57(2), 411–425.
2.  **Heijdra, B. J. (2017).** Endogenous economic growth (Cap. 14). En *Foundations of Modern Macroeconomics* (3.ª ed.). Oxford University Press.
3.  **Judge, G. G., et al. (1988).** Nonlinear least squares and nonlinear maximum likelihood estimation (Cap. 12). En *Introduction to the Theory and Practice of Econometrics*. John Wiley & Sons.
