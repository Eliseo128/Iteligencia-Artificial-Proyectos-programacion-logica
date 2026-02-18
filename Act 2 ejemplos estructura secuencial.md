A continuación se presentan **2 ejemplos prácticos en Python** usando **estructura secuencial** (sin condicionales ni ciclos), adecuados para **nivel básico / preparatoria**.
Cada ejemplo incluye: **redacción del problema, variables, pseudocódigo y código en Python**.

---

## 🧮 Ejemplo 1: Cálculo del total a pagar en una tienda

### ✏️ Redacción del problema

Una tienda desea calcular el **total a pagar** por un producto.
El usuario debe ingresar el **precio unitario** del producto y la **cantidad comprada**.
El programa debe mostrar el **total a pagar**.

---

### 📥 Identificación de variables

| Variable | Tipo   | Descripción                   |
| -------- | ------ | ----------------------------- |
| precio   | Real   | Precio de un producto         |
| cantidad | Entero | Número de productos comprados |
| total    | Real   | Importe total a pagar         |

---

### 🧩 Pseudocódigo

```
Inicio
  Leer precio
  Leer cantidad
  total ← precio * cantidad
  Mostrar total
Fin
```

---

### 🐍 Código en Python

```python
precio = float(input("Ingrese el precio del producto: "))
cantidad = int(input("Ingrese la cantidad comprada: "))

total = precio * cantidad

print("El total a pagar es: $", total)
```

---

## ⏱️ Ejemplo 2: Cálculo del salario semanal

### ✏️ Redacción del problema

Una empresa necesita calcular el **salario semanal** de un trabajador.
El usuario debe ingresar el **número de horas trabajadas** y el **pago por hora**.
El programa debe calcular y mostrar el **salario total**.

---

### 📥 Identificación de variables

| Variable  | Tipo   | Descripción                   |
| --------- | ------ | ----------------------------- |
| horas     | Entero | Horas trabajadas en la semana |
| pago_hora | Real   | Pago por cada hora            |
| salario   | Real   | Salario semanal               |

---

### 🧩 Pseudocódigo

```
Inicio
  Leer horas
  Leer pago_hora
  salario ← horas * pago_hora
  Mostrar salario
Fin
```

---

### 🐍 Código en Python

```python
horas = int(input("Ingrese las horas trabajadas: "))
pago_hora = float(input("Ingrese el pago por hora: "))

salario = horas * pago_hora

print("El salario semanal es: $", salario)
```

---

## 📌 Nota didáctica

Estos ejemplos utilizan **estructura secuencial**, lo que significa que:

* Las instrucciones se ejecutan **en orden**
* No hay decisiones (`if`) ni repeticiones (`for`, `while`)

---

Si deseas, puedo:

* Convertir estos ejemplos a **formato de examen**
* Agregar **tabla de resultados**
* Integrarlos en un **documento Word**
* Crear ejercicios similares con **porcentajes o promedios**

Solo indícalo.
