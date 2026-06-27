Función Principal
    Declarar Booleano sistemaencendido

    Asignar sistemaencendido = true
    Mientras  sistemaencendido = true
        Declarar Entero selección, selecciónlistaproductos, selecciónactualizar

        Salida "====Menú===="
        Salida "1. Mostrar lista de productos"
        Salida "2. Añadir un producto"
        Salida "3. Actualizar un producto"
        Salida "4. Salir"
        Entrada selección
        Si selección = 1
            Salida "==Mostrar lista de productos=="
            Salida "1. Ver todos los productos"
            Salida "2. Buscar producto específico"
            Entrada selecciónlistaproductos
            Si selecciónlistaproductos = 1
                Salida "Aquí va el código para mostrar todos los productos"
            Fin
            Si selecciónlistaproductos = 2
                Salida "Aquí va el código para buscar un producto en específico"
            Fin
            Si selecciónlistaproductos <> 1 AND selecciónlistaproductos <> 2
                Salida "Opción inválida"
            Fin
        Fin
        Si selección = 2
            Salida "==Añadir un producto=="
            Salida "Aquí va el código para ingresar un producto"
        Fin
        Si selección = 3
            Salida "===Actualizar un producto==="
            Salida "1. Venta"
            Salida "2. Actualizar todos los campos"
            Entrada selecciónactualizar
            Si selecciónactualizar = 1
                Salida "Aquí va el código para la venta"
            Fin
            Si selecciónactualizar = 2
                Salida "Aquí va el código para actualizar todo un producto"
            Fin
            Si selecciónactualizar <> 1 AND selecciónactualizar <> 2
                Salida "Opción inválida"
            Fin
        Fin
        Si selección = 4
            Asignar sistemaencendido = false
            Salida "El programa ha finalizado"
        Fin
        Si selección <> 1 AND selección <> 2 AND selección <> 3 AND selección <> 4
            Salida "Opción inválida"
        Fin
    Fin
Fin
