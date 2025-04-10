# 🖥️ Simulador de Arquitectura de von Neumann

Este simulador emula el comportamiento básico de una **máquina de von Neumann**, permitiendo la ejecución de operaciones aritméticas y lógicas simples con una arquitectura secuencial clásica. Ha sido desarrollado como herramienta educativa para visualizar cómo una CPU procesa instrucciones paso a paso dentro de un entorno controlado.

---

## 🚀 ¿Qué hace este simulador?

- Simula el ciclo de instrucción **Fetch - Decode - Execute**.
- Permite ejecutar **programas precargados** con instrucciones básicas.
- Muestra cómo se mueven los datos entre la **memoria**, el **registro de instrucciones**, la **unidad de control** y la **ALU (unidad aritmético-lógica)**.
- Detecta condiciones especiales como **overflow**.

---

## 📦 Programas precargados

A continuación, se describen los programas que vienen incluidos por defecto en el simulador:

| Programa                          | Descripción                                               | Resultado   |
|----------------------------------|-----------------------------------------------------------|-------------|
| `5 + 2`                          | Suma directa entre dos operandos.                         | `7`         |
| `(1 + 1) ^ 5`                    | Potenciación anidada: se suma 1+1 y se eleva a la 5ta.    | `32`        |
| `01001011 OR 01010101`          | Operación lógica OR entre dos números binarios.           | `01011111`  |
| `01001011 AND 01010101`         | Operación lógica AND entre dos números binarios.          | `01000001`  |
| `255 + 1`                        | Suma que provoca **overflow** en un sistema de 8 bits.    | `OVERFLOW`  |
| `((2 ^ 2) + 2) ^ 2`              | Operación combinada con suma y potencia anidada.          | `36`        |
| `(8 - 3) ^ 3`                    | Resta seguida de potenciación.                            | `125`       |

---

## ⚙️ ¿Cómo funciona?

1. **Carga de instrucciones**: Las instrucciones se cargan en memoria, imitando un programa.
2. **Ciclo de instrucción**:
   - **Fetch**: Se obtiene la siguiente instrucción desde la memoria.
   - **Decode**: Se decodifica para identificar operación y operandos.
   - **Execute**: Se ejecuta la operación en la ALU.
3. **Resultado**: El resultado se almacena en un registro y puede visualizarse en pantalla.

---

## 🧠 ¿Qué es la arquitectura de von Neumann?

Es un modelo computacional que define una arquitectura basada en:
- **Memoria única compartida** para instrucciones y datos.
- **Ejecución secuencial** de instrucciones.
- Un ciclo de instrucción repetitivo para procesar datos.

Este simulador replica esa idea de forma sencilla y visual.

---

## 🛠️ Posibles mejoras

- Soporte para programas personalizados.
- Visualización paso a paso del ciclo completo.
- Control del tamaño de los registros para simular más bits.

---
