¡Claro que sí! Aquí tienes el código en **Python** basado exactamente en el documento de requisitos que diseñamos. 

He mantenido el nivel **principiante**: uso listas y diccionarios para guardar los datos (sin clases complejas), funciones separadas para cada tarea y comentarios explicativos en cada paso.

> **💡 Nota importante:** Para que la función *"Imprimir Historial"* tenga sentido, agregué una opción extra en el menú llamada **"Registrar Visita"**. Sin esto, el historial estaría siempre vacío. ¡Es un ajuste lógico necesario!

---

### 🐾 Código: Sistema Veterinaria "Huellitas"

```python
import datetime  # Importamos librería para manejar fechas

# 📦 Base de datos temporal (se borra al cerrar el programa)
# Guardaremos clientes como diccionarios dentro de una lista
lista_clientes = []

# ---------------------------------------------------------
# 1. FUNCIÓN: REGISTRAR CLIENTE
# ---------------------------------------------------------
def registrar_cliente():
    print("\n--- 📝 Registrar Nuevo Cliente ---")
    nombre = input("Nombre del cliente: ")
    apellido = input("Apellido del cliente: ")
    
    # Validación simple: no permitir campos vacíos
    if nombre == "" or apellido == "":
        print("❌ Error: Debes ingresar nombre y apellido.")
        return

    # Creamos un diccionario con los datos del cliente
    nuevo_cliente = {
        "nombre": nombre,
        "apellido": apellido,
        "mascotas": []  # Lista vacía para guardar sus mascotas
    }
    
    lista_clientes.append(nuevo_cliente) # Guardamos en la lista global
    print(f"✅ Cliente {nombre} {apellido} registrado con éxito.")

# ---------------------------------------------------------
# 2. FUNCIÓN: AGREGAR MASCOTA
# ---------------------------------------------------------
def agregar_mascota():
    print("\n--- 🐶 Agregar Mascota ---")
    nombre_cliente = input("Nombre del cliente dueño: ")
    
    # Buscamos al cliente en la lista
    cliente_encontrado = None
    for cliente in lista_clientes:
        if cliente["nombre"] == nombre_cliente:
            cliente_encontrado = cliente
            break
    
    if cliente_encontrado:
        nombre_mascota = input("Nombre de la mascota: ")
        tipo_mascota = input("Tipo de animal (Perro, Gato, etc.): ")
        
        if nombre_mascota == "" or tipo_mascota == "":
            print("❌ Error: Datos de mascota incompletos.")
            return

        # Creamos la mascota con una lista vacía para sus visitas
        nueva_mascota = {
            "nombre": nombre_mascota,
            "tipo": tipo_mascota,
            "visitas": [] 
        }
        
        cliente_encontrado["mascotas"].append(nueva_mascota)
        print(f"✅ Mascota {nombre_mascota} agregada a {cliente_encontrado['nombre']}.")
    else:
        print("❌ Error: Cliente no encontrado. Regístralo primero.")

# ---------------------------------------------------------
# 3. FUNCIÓN: LISTAR CLIENTES Y MASCOTAS
# ---------------------------------------------------------
def listar_clientes_mascotas():
    print("\n--- 📋 Lista de Clientes y Mascotas ---")
    
    if len(lista_clientes) == 0:
        print("No hay clientes registrados aún.")
        return

    for cliente in lista_clientes:
        print(f"\n👤 Cliente: {cliente['nombre']} {cliente['apellido']}")
        if len(cliente["mascotas"]) > 0:
            for mascota in cliente["mascotas"]:
                print(f"   🐾 Mascota: {mascota['nombre']} ({mascota['tipo']})")
        else:
            print("   (Sin mascotas registradas)")

# ---------------------------------------------------------
# 4. FUNCIÓN EXTRA: REGISTRAR VISITA (Necesaria para el historial)
# ---------------------------------------------------------
def registrar_visita():
    print("\n--- 🏥 Registrar Visita Médica ---")
    nombre_cliente = input("Nombre del cliente: ")
    
    cliente_encontrado = None
    for cliente in lista_clientes:
        if cliente["nombre"] == nombre_cliente:
            cliente_encontrado = cliente
            break
            
    if cliente_encontrado:
        nombre_mascota = input("Nombre de la mascota atendida: ")
        mascota_encontrada = None
        for mascota in cliente_encontrado["mascotas"]:
            if mascota["nombre"] == nombre_mascota:
                mascota_encontrada = mascota
                break
        
        if mascota_encontrada:
            resumen = input("Resumen de la atención: ")
            fecha = datetime.datetime.now().strftime("%Y-%m-%d %H:%M")
            
            # Guardamos la visita en la lista de la mascota
            nueva_visita = {"fecha": fecha, "resumen": resumen}
            mascota_encontrada["visitas"].append(nueva_visita)
            print("✅ Visita registrada correctamente.")
        else:
            print("❌ Error: Mascota no encontrada en este cliente.")
    else:
        print("❌ Error: Cliente no encontrado.")

# ---------------------------------------------------------
# 5. FUNCIÓN: IMPRIMIR HISTORIAL (Genera archivo .txt)
# ---------------------------------------------------------
def imprimir_historial():
    print("\n--- 🖨️ Imprimir Historial de Visitas ---")
    nombre_cliente = input("Nombre del cliente para el reporte: ")
    
    cliente_encontrado = None
    for cliente in lista_clientes:
        if cliente["nombre"] == nombre_cliente:
            cliente_encontrado = cliente
            break
    
    if cliente_encontrado:
        # Creamos el nombre del archivo
        nombre_archivo = f"historial_{nombre_cliente}.txt"
        
        try:
            with open(nombre_archivo, "w") as archivo:
                archivo.write(f"HISTORIAL VETERINARIO - {nombre_cliente}\n")
                archivo.write("=" * 40 + "\n")
                
                tiene_visitas = False
                for mascota in cliente_encontrado["mascotas"]:
                    if len(mascota["visitas"]) > 0:
                        tiene_visitas = True
                        archivo.write(f"\nMascota: {mascota['nombre']} ({mascota['tipo']})\n")
                        for visita in mascota["visitas"]:
                            archivo.write(f"  📅 Fecha: {visita['fecha']}\n")
                            archivo.write(f"  📝 Atención: {visita['resumen']}\n")
                
                if not tiene_visitas:
                    archivo.write("No hay visitas registradas para las mascotas de este cliente.")
            
            print(f"✅ Archivo '{nombre_archivo}' generado con éxito.")
        except Exception as e:
            print(f"❌ Error al crear el archivo: {e}")
    else:
        print("❌ Error: Cliente no encontrado.")

# ---------------------------------------------------------
# 6. FUNCIÓN: SALIR
# ---------------------------------------------------------
def salir():
    print("\n👋 ¡Gracias por usar Veterinaria Huellitas! Hasta luego.")
    return False  # Esto indicará al bucle principal que debe terminar

# ---------------------------------------------------------
# 🎮 PROGRAMA PRINCIPAL (Menú)
# ---------------------------------------------------------
def main():
    ejecutando = True
    
    while ejecutando:
        print("\n=================================")
        print("   🏥 VETERINARIA HUELLITAS 🐾   ")
        print("=================================")
        print("1. Registrar Cliente")
        print("2. Agregar Mascota")
        print("3. Listar Clientes y Mascotas")
        print("4. Registrar Visita (Extra)")
        print("5. Imprimir Historial (.txt)")
        print("6. Salir")
        print("=================================")
        
        opcion = input("Seleccione una opción: ")
        
        # Llamamos a la función según la opción elegida
        if opcion == "1":
            registrar_cliente()
        elif opcion == "2":
            agregar_mascota()
        elif opcion == "3":
            listar_clientes_mascotas()
        elif opcion == "4":
            registrar_visita()
        elif opcion == "5":
            imprimir_historial()
        elif opcion == "6":
            ejecutando = salir()  # Cambia la variable a False
        else:
            print("⚠️ Opción no válida, intenta de nuevo.")

# Esto asegura que el programa inicie solo si ejecutamos este archivo
if __name__ == "__main__":
    main()
```

---

### 🧪 ¿Cómo probar tu código?

1.  **Copia y pega** el código en un archivo llamado `veterinaria.py`.
2.  **Ejecuta el programa** en tu terminal o editor.
3.  **Sigue este flujo de prueba:**
    *   Opción **1**: Registra un cliente (ej: *Ana López*).
    *   Opción **2**: Agrega una mascota a Ana (ej: *Firulais, Perro*).
    *   Opción **4**: Registra una visita para Firulais (ej: *Vacunación*).
    *   Opción **5**: Imprime el historial de Ana. ¡Ve a la carpeta de tu proyecto y busca el archivo `.txt`!
    *   Opción **3**: Lista todo para verificar que los datos están guardados.
    *   Opción **6**: Sal del programa.

### 💡 Consejos para tu tarea
*   **Comentarios:** Fíjate que cada función tiene un comentario arriba explicando qué hace. Esto es vital para que tu profesor vea que entiendes el código.
*   **Funciones Separadas:** Cumplimos el requisito de que cada acción esté en su propia función (`def`).
*   **Validación:** El código verifica si el cliente existe antes de agregarle una mascota, evitando errores.

¡Mucho éxito con tu proyecto! 🚀🐶🐱
