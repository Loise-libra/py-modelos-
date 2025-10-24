tareas = []

def mostrar_menu():
    """Imprime el menú de opciones."""
    print("\n--- Lista de Tareas de Consola ---")
    print("1. Agregar tarea")
    print("2. Ver todas las tareas")
    print("3. Eliminar tarea")
    print("4. Salir")
    print("----------------------------------")

def agregar_tarea():
    """Pide al usuario una tarea y la agrega a la lista."""
    tarea = input("Escribe la nueva tarea: ")
    if tarea:
        tareas.append(tarea)
        print(f"✅ ¡Tarea '{tarea}' agregada!")
    else:
        print("❌ No puedes agregar una tarea vacía intenta de nuevo.")

def ver_tareas():
    """Muestra todas las tareas en la lista, con numeración."""
    if not tareas:
        print("\n>> No hay tareas pendientes Ingresa . <<")
    else:
        print("\n--- Tus Tareas ---")
     
        for i, tarea in enumerate(tareas, 1):
            print(f"{i}. {tarea}")

def eliminar_tarea():
    """Muestra las tareas y pide al usuario el número de la que desea eliminar."""
    ver_tareas() 
    
    if not tareas:
        return 

    try:
        num_tarea = int(input("Ingresa el número de la tarea que deseas eliminar: "))
        
      
        indice = num_tarea - 1
        
        if 0 <= indice < len(tareas):
            tarea_eliminada = tareas.pop(indice)
            print(f"✅ ¡Tarea '{tarea_eliminada}' eliminada!")
        else:
            print("❌ Número de tarea no válido.")
            
    except ValueError:
    
        print("❌ Entrada no válida. Debes ingresar un número.")

def main():
    """Función principal que ejecuta el bucle de la aplicación."""
    while True:
        mostrar_menu()
        opcion = input("Elige una opción (1-4): ")
        
        if opcion == '1':
            agregar_tarea()
        elif opcion == '2':
            ver_tareas()
        elif opcion == '3':
            eliminar_tarea()
        elif opcion == '4':
            print("¡Hasta luego! 👋")
            break
        else:
            print("❌ Opción no válida. Por favor, elige un número del 1 al 4.")


if __name__ == "__main__":
    main()
