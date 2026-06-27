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
                Salida "Whisky Johnnie Walker Red Label - $25"
                Salida "Whisky Chivas Regal 12 Años - $40"
                Salida "Ron Abuelo 7 Años - $22"
                Salida "Ron Zacapa 23 - $55"
                Salida "Vodka Absolut - $20"
                Salida "Vodka Smirnoff - $15"
                Salida "Tequila José Cuervo Especial - $28"
                Salida "Tequila Don Julio Blanco - $60"
                Salida "Cerveza Corona (6 pack) - $8"
                Salida "Cerveza Pilsener (6 pack) - $6"
                Salida "Vino Casillero del Diablo - $12"
                Salida "Vino Trapiche Malbec - $14"
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
            Declarar Cadena ProductoNuevo
            Declarar Real CodigoProductoNuevo

            Entrada ProductoNuevo
            Salida "Coloca el codigo del producto."
            Entrada CodigoProductoNuevo
            Salida "Se añadio al inventario: " & ProductoNuevo & " con el código:" & CodigoProductoNuevo
        Fin
        Si selección = 3
            Salida "===Actualizar un producto==="
            Salida "1. Venta"
            Salida "2. Actualizar todos los campos"
            Entrada selecciónactualizar
            Si selecciónactualizar = 1
                Declarar Entero codigodelproducto
                Declarar Entero cantidadvendida

                Salida "ingrese el codigo del producto"
                Entrada codigodelproducto
                Salida "ingrese la cantidad vendida"
                Entrada cantidadvendida

                ... Aqui sucede la operacion
                Salida "cantidad actualizada exitosamente"
            Fin
            Si selecciónactualizar = 2
                Declarar Cadena nombredelproducto

                Salida "Ingrese el nombre del producto"
                Entrada nombredelproducto
                Declarar Real preciodeventadelproducto

                Salida "Ingrese el precio de venta del producto"
                Entrada preciodeventadelproducto
                Declarar Real preciodecompradelproducto

                Salida "Ingrese el precio de compra del producto"
                Entrada preciodecompradelproducto
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
