Aquí tienes 60 problemas de decisión (lógica *if/else*) aplicados a situaciones cotidianas, diseñados para estudiantes de preparatoria. Cada problema incluye el planteamiento, 3 preguntas específicas y las variables/fórmulas necesarias.

---

### **Bloque 1: Alimentos y Bebidas (1-10)**

**1. Panadería "El Trigo"**
*   **Planteamiento:** El pan cuesta $5 c/u. Si compras más de 20 piezas, tienes 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 15 panes? 2) ¿Costo de 25 panes? 3) Si compras 50, ¿cuánto ahorras vs. precio normal?
*   **Variables/Fórmulas:** $P=5, Q=\{15, 25, 50\}, T=20, D=0.10$. $Total = P \times Q$. $Desc = Total \times D$. $Final = Total - Desc$.

**2. Frutería "La Frescura"**
*   **Planteamiento:** Las manzanas valen $12 el kg. Si llevas más de 5 kg, el kg sale a $10.
*   **Preguntas:** 1) ¿Costo de 3 kg? 2) ¿Costo de 6 kg? 3) Si llevas 10 kg, ¿cuánto ahorras comparado con el precio unitario?
*   **Variables/Fórmulas:** $P1=12, P2=10, T=5$. $Total = P \times Q$. $Ahorro = (P1 \times Q) - (P2 \times Q)$.

**3. Cafetería "Aroma"**
*   **Planteamiento:** Café a $30. Si la cuenta supera $150, hay 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 4 cafés? 2) ¿Costo de 6 cafés? 3) Si pides 10, ¿cuánto dinero te ahorras?
*   **Variables/Fórmulas:** $P=30, T=150, D=0.15$. $Subtotal = P \times Q$. $Si Subtotal > T \to Final = Subtotal - (Subtotal \times D)$.

**4. Pizzería "Rápida"**
*   **Planteamiento:** Pizza individual $80. Si compras más de 3, la 4ta es gratis (efecto 25% desc en 4).
*   **Preguntas:** 1) ¿Costo de 2 pizzas? 2) ¿Costo de 4 pizzas? 3) Si compras 8, ¿cuánto ahorras vs. pagar todas completas?
*   **Variables/Fórmulas:** $P=80, T=3$. $Total = P \times Q$. $Descuento = P \times (Q / 4)$. $Final = Total - Descuento$.

**5. Tienda de Abarrotes**
*   **Planteamiento:** Arroz $25. Si compras más de 10 bolsas, 5% de descuento.
*   **Preguntas:** 1) ¿Costo de 5 bolsas? 2) ¿Costo de 12 bolsas? 3) Si compras 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=25, T=10, D=0.05$. $Total = P \times Q$. $Ahorro = (P \times Q) \times D$ (si $Q>T$).

**6. Heladería "Frío"**
*   **Planteamiento:** Helado $40. Si compras más de 5, el descuento es del 20%.
*   **Preguntas:** 1) ¿Costo de 3 helados? 2) ¿Costo de 6 helados? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=40, T=5, D=0.20$. $Total = P \times Q$. $Final = Total \times (1-D)$ (si $Q>T$).

**7. Taquería "El Sol"**
*   **Planteamiento:** Taco $15. Si la cuenta es mayor a $200, se regalan 2 tacos.
*   **Preguntas:** 1) ¿Costo de 10 tacos? 2) ¿Costo de 15 tacos (pagando 13)? 3) Si pides 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=15, T=200$. $Total = P \times Q$. $Si Total > T \to Q_{pagar} = Q - 2$.

**8. Juguería "Vital"**
*   **Planteamiento:** Jugo $20. Si compras más de 10, el precio baja a $18.
*   **Preguntas:** 1) ¿Costo de 8 jugos? 2) ¿Costo de 12 jugos? 3) Si compras 30, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=20, P2=18, T=10$. $Ahorro = (P1 - P2) \times Q$ (si $Q>T$).

**9. Pastelería "Dulce"**
*   **Planteamiento:** Pastel $300. Si compras más de 1, 10% de descuento en el total.
*   **Preguntas:** 1) ¿Costo de 1 pastel? 2) ¿Costo de 2 pasteles? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=300, T=1, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$ (si $Q>T$).

**10. Carnicería "El Corte"**
*   **Planteamiento:** Carne $150 el kg. Si compras más de 3 kg, 12% de descuento.
*   **Preguntas:** 1) ¿Costo de 2 kg? 2) ¿Costo de 4 kg? 3) Si compras 10 kg, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=150, T=3, D=0.12$. $Total = P \times Q$. $Final = Total - (Total \times D)$.

---

### **Bloque 2: Ropa y Accesorios (11-20)**

**11. Zapatería "Camino"**
*   **Planteamiento:** Zapatos $500. Si compras 2 pares, el segundo tiene 50% de descuento.
*   **Preguntas:** 1) ¿Costo de 1 par? 2) ¿Costo de 2 pares? 3) Si compras 4 pares, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=500$. $Total = P + (P \times 0.5)$ (si $Q=2$). $Ahorro = P \times 0.5 \times (Q/2)$.

**12. Tienda de Camisas**
*   **Planteamiento:** Camisa $250. Si compras más de 5, descuento del 15%.
*   **Preguntas:** 1) ¿Costo de 3 camisas? 2) ¿Costo de 6 camisas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=250, T=5, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

**13. Boutique de Jeans**
*   **Planteamiento:** Jeans $600. Si gastas más de $1000, tienes 20% de descuento.
*   **Preguntas:** 1) ¿Costo de 1 jeans? 2) ¿Costo de 2 jeans? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=600, T=1000, D=0.20$. $Subtotal = P \times Q$. $Si Subtotal > T \to Ahorro = Subtotal \times D$.

**14. Tienda de Gorras**
*   **Planteamiento:** Gorra $100. Si compras más de 10, precio especial $80.
*   **Preguntas:** 1) ¿Costo de 5 gorras? 2) ¿Costo de 12 gorras? 3) Si compras 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=100, P2=80, T=10$. $Ahorro = (P1 - P2) \times Q$.

**15. Venta de Calcetines**
*   **Planteamiento:** Par de calcetines $50. Si compras más de 6 pares, 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 4 pares? 2) ¿Costo de 8 pares? 3) Si compras 12, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=50, T=6, D=0.10$. $Total = P \times Q$. $Final = Total \times (1-D)$.

**16. Tienda de Chaquetas**
*   **Planteamiento:** Chaqueta $800. Si compras más de 1, 5% de descuento adicional.
*   **Preguntas:** 1) ¿Costo de 1 chaqueta? 2) ¿Costo de 2 chaquetas? 3) Si compras 3, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=800, T=1, D=0.05$. $Ahorro = (P \times Q) \times D$.

**17. Venta de Vestidos**
*   **Planteamiento:** Vestido $450. Si la compra supera $2000, descuento del 25%.
*   **Preguntas:** 1) ¿Costo de 3 vestidos? 2) ¿Costo de 5 vestidos? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=450, T=2000, D=0.25$. $Subtotal = P \times Q$. $Si Subtotal > T \to Ahorro = Subtotal \times D$.

**18. Tienda de Cinturones**
*   **Planteamiento:** Cinturón $150. Si compras más de 4, el 5to es gratis.
*   **Preguntas:** 1) ¿Costo de 3 cinturones? 2) ¿Costo de 5 cinturones? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=150, T=4$. $Ahorro = P \times (Q / 5)$.

**19. Relojería "Tiempo"**
*   **Planteamiento:** Reloj $1200. Si compras más de 2, 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 1 reloj? 2) ¿Costo de 3 relojes? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=1200, T=2, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

**20. Tienda de Lentes**
*   **Planteamiento:** Lentes de sol $300. Si compras más de 1, 2x1 (50% descuento total).
*   **Preguntas:** 1) ¿Costo de 1 lente? 2) ¿Costo de 2 lentes? 3) Si compras 4, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=300$. $Total = P \times (Q / 2 + Q \% 2)$. $Ahorro = P \times (Q / 2)$.

---

### **Bloque 3: Electrónica y Tecnología (21-30)**

**21. Tienda de USB**
*   **Planteamiento:** USB $100. Si compras más de 20, precio $85.
*   **Preguntas:** 1) ¿Costo de 10 USB? 2) ¿Costo de 25 USB? 3) Si compras 50, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=100, P2=85, T=20$. $Ahorro = (P1 - P2) \times Q$.

**22. Venta de Audífonos**
*   **Planteamiento:** Audífonos $400. Si compras más de 5, 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 3 audífonos? 2) ¿Costo de 6 audífonos? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=400, T=5, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**23. Cargadores de Celular**
*   **Planteamiento:** Cargador $200. Si la cuenta > $1000, descuento 15%.
*   **Preguntas:** 1) ¿Costo de 4 cargadores? 2) ¿Costo de 6 cargadores? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=200, T=1000, D=0.15$. $Subtotal = P \times Q$. $Si Subtotal > T \to Ahorro = Subtotal \times D$.

**24. Mouse para PC**
*   **Planteamiento:** Mouse $150. Si compras más de 10, 5% de descuento.
*   **Preguntas:** 1) ¿Costo de 5 mouse? 2) ¿Costo de 12 mouse? 3) Si compras 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=150, T=10, D=0.05$. $Total = P \times Q$. $Ahorro = Total \times D$.

**25. Teclados**
*   **Planteamiento:** Teclado $500. Si compras más de 3, el 4to es gratis.
*   **Preguntas:** 1) ¿Costo de 2 teclados? 2) ¿Costo de 4 teclados? 3) Si compras 8, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=500, T=3$. $Ahorro = P \times (Q / 4)$.

**26. Monitores**
*   **Planteamiento:** Monitor $2000. Si compras más de 1, 12% de descuento.
*   **Preguntas:** 1) ¿Costo de 1 monitor? 2) ¿Costo de 2 monitores? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=2000, T=1, D=0.12$. $Total = P \times Q$. $Ahorro = Total \times D$.

**27. Tablets**
*   **Planteamiento:** Tablet $3000. Si gastas > $5000, descuento 20%.
*   **Preguntas:** 1) ¿Costo de 1 tablet? 2) ¿Costo de 2 tablets? 3) Si compras 4, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=3000, T=5000, D=0.20$. $Subtotal = P \times Q$. $Si Subtotal > T \to Ahorro = Subtotal \times D$.

**28. Cámaras Web**
*   **Planteamiento:** Cámara $600. Si compras más de 15, precio $500.
*   **Preguntas:** 1) ¿Costo de 10 cámaras? 2) ¿Costo de 16 cámaras? 3) Si compras 30, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=600, P2=500, T=15$. $Ahorro = (P1 - P2) \times Q$.

**29. Bocinas**
*   **Planteamiento:** Bocina $800. Si compras más de 2, 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 1 bocina? 2) ¿Costo de 3 bocinas? 3) Si compras 6, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=800, T=2, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**30. Discos Duros**
*   **Planteamiento:** Disco $1000. Si compras más de 5, 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 4 discos? 2) ¿Costo de 6 discos? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=1000, T=5, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

---

### **Bloque 4: Hogar y Ferretería (31-40)**

**31. Tienda de Pintura**
*   **Planteamiento:** Cubeta $400. Si compras más de 4, 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 3 cubetas? 2) ¿Costo de 5 cubetas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=400, T=4, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**32. Herramientas**
*   **Planteamiento:** Martillo $150. Si compras más de 10, precio $120.
*   **Preguntas:** 1) ¿Costo de 5 martillos? 2) ¿Costo de 12 martillos? 3) Si compras 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=150, P2=120, T=10$. $Ahorro = (P1 - P2) \times Q$.

**33. Focos LED**
*   **Planteamiento:** Foco $50. Si compras más de 20, 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 10 focos? 2) ¿Costo de 25 focos? 3) Si compras 50, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=50, T=20, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

**34. Plantas de Interior**
*   **Planteamiento:** Planta $200. Si compras más de 3, la 4ta es gratis.
*   **Preguntas:** 1) ¿Costo de 2 plantas? 2) ¿Costo de 4 plantas? 3) Si compras 8, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=200, T=3$. $Ahorro = P \times (Q / 4)$.

**35. Macetas**
*   **Planteamiento:** Maceta $80. Si la cuenta > $500, descuento 10%.
*   **Preguntas:** 1) ¿Costo de 5 macetas? 2) ¿Costo de 7 macetas? 3) Si compras 15, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=80, T=500, D=0.10$. $Subtotal = P \times Q$. $Si Subtotal > T \to Ahorro = Subtotal \times D$.

**36. Limpiadores**
*   **Planteamiento:** Limpiador $60. Si compras más de 12, precio $50.
*   **Preguntas:** 1) ¿Costo de 10 limpiadores? 2) ¿Costo de 15 limpiadores? 3) Si compras 30, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=60, P2=50, T=12$. $Ahorro = (P1 - P2) \times Q$.

**37. Toallas**
*   **Planteamiento:** Toalla $100. Si compras más de 5, 20% de descuento.
*   **Preguntas:** 1) ¿Costo de 4 toallas? 2) ¿Costo de 6 toallas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=100, T=5, D=0.20$. $Total = P \times Q$. $Ahorro = Total \times D$.

**38. Sábanas**
*   **Planteamiento:** Juego de sábanas $500. Si compras más de 2, 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 1 juego? 2) ¿Costo de 3 juegos? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=500, T=2, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

**39. Almohadas**
*   **Planteamiento:** Almohada $250. Si compras más de 4, precio $200.
*   **Preguntas:** 1) ¿Costo de 3 almohadas? 2) ¿Costo de 5 almohadas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=250, P2=200, T=4$. $Ahorro = (P1 - P2) \times Q$.

**40. Cortinas**
*   **Planteamiento:** Cortina $800. Si gastas > $2000, descuento 25%.
*   **Preguntas:** 1) ¿Costo de 2 cortinas? 2) ¿Costo de 3 cortinas? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=800, T=2000, D=0.25$. $Subtotal = P \times Q$. $Si Subtotal > T \to Ahorro = Subtotal \times D$.

---

### **Bloque 5: Servicios y Eventos (41-50)**

**41. Cine "Estelar"**
*   **Planteamiento:** Entrada $80. Si compras más de 5, 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 3 entradas? 2) ¿Costo de 6 entradas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=80, T=5, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**42. Gimnasio "Fit"**
*   **Planteamiento:** Mensualidad $500. Si pagas 6 meses, 1 mes gratis.
*   **Preguntas:** 1) ¿Costo de 3 meses? 2) ¿Costo de 6 meses (pagando 5)? 3) Si pagas 12, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=500, T=6$. $Ahorro = P \times (Q / 6)$.

**43. Autobús Turístico**
*   **Planteamiento:** Boleto $100. Si grupo > 10 personas, precio $80.
*   **Preguntas:** 1) ¿Costo para 8 personas? 2) ¿Costo para 12 personas? 3) Si son 30, ¿cuánto ahorran?
*   **Variables/Fórmulas:** $P1=100, P2=80, T=10$. $Ahorro = (P1 - P2) \times Q$.

**44. Taxi Ejecutivo**
*   **Planteamiento:** Viaje $150. Si viajas > 5 veces al mes, 15% descuento en el total.
*   **Preguntas:** 1) ¿Costo de 3 viajes? 2) ¿Costo de 6 viajes? 3) Si son 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=150, T=5, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

**45. Hotel "Descanso"**
*   **Planteamiento:** Noche $1000. Si reservas más de 3 noches, 20% descuento.
*   **Preguntas:** 1) ¿Costo de 2 noches? 2) ¿Costo de 4 noches? 3) Si son 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=1000, T=3, D=0.20$. $Total = P \times Q$. $Ahorro = Total \times D$.

**46. Concierto**
*   **Planteamiento:** Entrada $500. Si compras > 4, 5% descuento.
*   **Preguntas:** 1) ¿Costo de 2 entradas? 2) ¿Costo de 5 entradas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=500, T=4, D=0.05$. $Total = P \times Q$. $Ahorro = Total \times D$.

**47. Museo**
*   **Planteamiento:** Entrada $50. Si grupo > 20, entrada gratis para 2 personas.
*   **Preguntas:** 1) ¿Costo para 10 personas? 2) ¿Costo para 22 personas? 3) Si son 40, ¿cuánto ahorran?
*   **Variables/Fórmulas:** $P=50, T=20$. $Ahorro = P \times 2 \times (Q / 20)$.

**48. Parque de Diversiones**
*   **Planteamiento:** Pase $300. Si compras > 5, precio $250.
*   **Preguntas:** 1) ¿Costo de 4 pases? 2) ¿Costo de 6 pases? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=300, P2=250, T=5$. $Ahorro = (P1 - P2) \times Q$.

**49. Taller de Cocina**
*   **Planteamiento:** Curso $1500. Si inscribes > 2 personas, 10% descuento.
*   **Preguntas:** 1) ¿Costo de 1 persona? 2) ¿Costo de 3 personas? 3) Si son 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=1500, T=2, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**50. Curso de Idiomas**
*   **Planteamiento:** Nivel $2000. Si pagas 3 niveles, el 3ro tiene 50% descuento.
*   **Preguntas:** 1) ¿Costo de 1 nivel? 2) ¿Costo de 3 niveles? 3) Si pagas 6, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=2000$. $Ahorro = (P \times 0.5) \times (Q / 3)$.

---

### **Bloque 6: Escuela y Oficina (51-60)**

**51. Cuadernos**
*   **Planteamiento:** Cuaderno $40. Si compras > 20, precio $35.
*   **Preguntas:** 1) ¿Costo de 10 cuadernos? 2) ¿Costo de 25 cuadernos? 3) Si compras 50, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=40, P2=35, T=20$. $Ahorro = (P1 - P2) \times Q$.

**52. Bolígrafos**
*   **Planteamiento:** Bolígrafo $10. Si compras > 50, 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 30 bolígrafos? 2) ¿Costo de 60 bolígrafos? 3) Si compras 100, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=10, T=50, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.

**53. Lápices**
*   **Planteamiento:** Lápiz $5. Si compras > 100, precio $4.
*   **Preguntas:** 1) ¿Costo de 50 lápices? 2) ¿Costo de 120 lápices? 3) Si compras 200, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=5, P2=4, T=100$. $Ahorro = (P1 - P2) \times Q$.

**54. Carpetas**
*   **Planteamiento:** Carpeta $30. Si compras > 10, 10% de descuento.
*   **Preguntas:** 1) ¿Costo de 5 carpetas? 2) ¿Costo de 12 carpetas? 3) Si compras 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=30, T=10, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**55. Resmas de Papel**
*   **Planteamiento:** Resma $100. Si compras > 5, la 6ta es gratis.
*   **Preguntas:** 1) ¿Costo de 4 resmas? 2) ¿Costo de 6 resmas? 3) Si compras 12, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=100, T=5$. $Ahorro = P \times (Q / 6)$.

**56. Tinta de Impresora**
*   **Planteamiento:** Cartucho $500. Si compras > 2, 20% descuento.
*   **Preguntas:** 1) ¿Costo de 1 cartucho? 2) ¿Costo de 3 cartuchos? 3) Si compras 5, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=500, T=2, D=0.20$. $Total = P \times Q$. $Ahorro = Total \times D$.

**57. Engrapadoras**
*   **Planteamiento:** Engrapadora $150. Si compras > 10, precio $120.
*   **Preguntas:** 1) ¿Costo de 5 engrapadoras? 2) ¿Costo de 12 engrapadoras? 3) Si compras 20, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=150, P2=120, T=10$. $Ahorro = (P1 - P2) \times Q$.

**58. Tijeras**
*   **Planteamiento:** Tijera $80. Si compras > 20, 10% descuento.
*   **Preguntas:** 1) ¿Costo de 10 tijeras? 2) ¿Costo de 25 tijeras? 3) Si compras 50, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=80, T=20, D=0.10$. $Total = P \times Q$. $Ahorro = Total \times D$.

**59. Reglas**
*   **Planteamiento:** Regla $20. Si compras > 50, precio $15.
*   **Preguntas:** 1) ¿Costo de 30 reglas? 2) ¿Costo de 60 reglas? 3) Si compras 100, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P1=20, P2=15, T=50$. $Ahorro = (P1 - P2) \times Q$.

**60. Mochilas**
*   **Planteamiento:** Mochila $400. Si compras > 5, 15% de descuento.
*   **Preguntas:** 1) ¿Costo de 3 mochilas? 2) ¿Costo de 6 mochilas? 3) Si compras 10, ¿cuánto ahorras?
*   **Variables/Fórmulas:** $P=400, T=5, D=0.15$. $Total = P \times Q$. $Ahorro = Total \times D$.
