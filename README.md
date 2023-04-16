# dds-macowins
Ejercicio diagnóstico Macowins para la materia Diseño de Sistemas en UTN FRBA

## Pseudocódigo

```
clase Prenda
  metodo precio()
    retornar estado.precio(precioBase)

clase Nueva
  metodo precio(precioBase)
    retornar precioBase

clase Promocion
  metodo precio(precioBase)
    retornar precioBase - descuento

clase Liquidacion
  metodo precio(precioBase)
    retornar precioBase * 0.5

clase Local
  metodo gananciasPorFecha(fecha)
    retornar ventas
      .filter(v => v.fueRealizadaEn(fecha))
      .sum(v => v.importeTotal())

clase Venta
  metodo fueRealizadaEn(unaFecha)
    retornar fecha.Equals(unaFecha)

  metodo importeTotal()
    retornar items.sum(i => i.importe())

clase VentaConTarjeta
  metodo importeTotal()
    retornar cantidadCuotas * coeficiente + 0.01 * super() + super()

clase Item
  metodo importe()
    retornar prenda.precio() * cantidad

```