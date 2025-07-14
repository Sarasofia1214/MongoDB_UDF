MongoDB_UDF -- Sara Diaz
## 5. Casos Prácticos y Ejercicios

### ✅ Ejercicio 1

📌 Mostrar nombre y categoría de cada cliente:

```js
function mostrarResumen(cliente) {
  var promedio = calcularPromedio(cliente.compras);
  print("Cliente:", cliente.nombre);
  print("Ciudad:", cliente.categoria);
  print("-----------------------------");
}
```

---

### ✅ Ejercicio 2

📌 Filtrar clientes cuya media de compras sea superior a $90.000:

```js

```

---

### ✅ Ejercicio 3

📌 Crear una función que determine si un cliente es joven (edad < 30) y lo imprima:

```js

```



---

## 6. 🛠 Taller Final

### 🎯 Reto: Crear una función que clasifique clientes en rangos

- Joven Premium: edad < 30 y promedio >= 90.000
- Adulto Frecuente: edad >= 30 y promedio entre 70.000 y 90.000
- Otro: lo demás

```js

```

