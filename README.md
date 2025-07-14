MongoDB_UDF -- Sara Diaz
## 5. Casos Prácticos y Ejercicios

### ✅ Ejercicio 1

📌 Mostrar nombre y categoría de cada cliente:

```js
function funcion(client) {
  print("Cliente:", client.nombre);
  print("Categoria:", client.categoria);
}

db.clientes.find().forEach(function (client) {funcion(client);})
```

---

### ✅ Ejercicio 2

📌 Filtrar clientes cuya media de compras sea superior a $90.000:

```js
function clientesmedia(client) {
  var promedio = calcularPromedio(client.compras);
  if (promedio >= 900000) {
    return ("Cliente:", client.nombre);
  } 
}
db.clientes.find().forEach(function (client) {clientesmedia(client);})
```

---

### ✅ Ejercicio 3

📌 Crear una función que determine si un cliente es joven (edad < 30) y lo imprima:

```js
function clasificarCliente(client) {
  var age = calcularEdad(cliente.edad);
  if (age <= 30) {
    return "Cliente joven";
  }
}


## 6. 🛠 Taller Final

### 🎯 Reto: Crear una función que clasifique clientes en rangos

- Joven Premium: edad < 30 y promedio >= 90.000
- Adulto Frecuente: edad >= 30 y promedio entre 70.000 y 90.000
- Otro: lo demás
t
```js

[Function: clasificarCliente]
function clasificaredad(client) {
  var edad = calcularedad(client.edad);
	var compra= calcularcompra(client.compras)
  if (edad <= 30 ) {
    return "Joven";
  } else if (edad >= 30) {
    return "Adulto";
  } else {
    return "Otro";
  }
}




```


