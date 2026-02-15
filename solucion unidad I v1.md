A continuación se presenta la **HOJA DE RESPUESTAS PARA EL DOCENTE**, alineada exactamente con el examen/práctica anterior, lista para **revisión y calificación**.

---

# **HOJA DE RESPUESTAS – DOCENTE**

**Tema:** Decisiones simples y compuestas
**Nivel:** Preparatoria

---

## **Parte A. Identificación de variables (3 pts)**

| Variable        | Tipo de dato | Descripción                                |
| --------------- | ------------ | ------------------------------------------ |
| horasTrabajadas | Entero       | Número de horas trabajadas por el empleado |
| sueldoBase      | Real         | Sueldo calculado antes de descuentos       |
| descuento       | Real         | Monto del descuento o retención aplicada   |
| sueldoFinal     | Real         | Sueldo final a pagar al empleado           |

---

## **Parte B. Desarrollo de fórmulas (3 pts)**

1. **Sueldo base (40 horas o menos):**
   [
   \text{sueldoBase} = \text{horasTrabajadas} \times 45
   ]

2. **Sueldo base (más de 40 horas):**
   [
   \text{sueldoBase} = (40 \times 45) + ((\text{horasTrabajadas} - 40) \times 22)
   ]

3. **Descuento o retención:**

* Si sueldoBase ≤ 1800
  [
  \text{descuento} = \text{sueldoBase} \times 0.10
  ]

* Si sueldoBase > 1800
  [
  \text{descuento} = \text{sueldoBase} \times 0.15
  ]

4. **Sueldo final:**
   [
   \text{sueldoFinal} = \text{sueldoBase} - \text{descuento}
   ]

---

## **Parte C. Estructura de decisión (2 pts)**

**Tipo de estructura:**
Estructura condicional *Si – Sino*

**Explicación esperada:**
Permite tomar una decisión dependiendo de si se cumple o no una condición, en este caso, el número de horas trabajadas y el monto del sueldo base para aplicar el pago y descuento correspondiente.

---

## **Parte D. Pseudocódigo (4 pts)**

```text
Inicio

  Leer horasTrabajadas
  pagoHoraNormal ← 45
  pagoHoraExtra ← 22

  Si horasTrabajadas <= 40 Entonces
      sueldoBase ← horasTrabajadas * pagoHoraNormal
  Sino
      horasExtras ← horasTrabajadas - 40
      sueldoBase ← (40 * pagoHoraNormal) + (horasExtras * pagoHoraExtra)
  FinSi

  Si sueldoBase <= 1800 Entonces
      descuento ← sueldoBase * 0.10
  Sino
      descuento ← sueldoBase * 0.15
  FinSi

  sueldoFinal ← sueldoBase - descuento
  Escribir sueldoFinal

Fin
```

---

## **Parte E. Resultado esperado (Punto extra)**

**Datos:**
Horas trabajadas = 45

**Cálculo:**

* Horas normales: 40 × 45 = 1800
* Horas extra: 5 × 22 = 110
* Sueldo base: 1910
* Retención (15%): 286.50
* Sueldo final: **$1623.50**

---

## **Resultado final esperado:**

✅ **$1623.50**

---

### **Sugerencia de evaluación**

* Lógica correcta aunque falte sintaxis exacta: ✔ válido
* Error en porcentaje o cálculo final: ❌ resta puntos
* Pseudocódigo incompleto: ❌

---

Si deseas, puedo:

* Unir **examen + hoja de respuestas** en un solo documento
* Exportarlo a **PDF o Word**
* Crear una **rúbrica de calificación detallada**
* Adaptarlo a **examen práctico con computadora**
