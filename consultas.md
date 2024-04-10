# Práctica Agregaciones en MongoDB

##  Cuenta los productos de tipo “medio”, usando un método básico 
**db.getCollection('productos').find({
  tipo: 'medio'
});**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd88"),
      codigo: 1,
      nombre: 'Rustic Concrete Pants',
      unidades: 66,
      precio: 279,
      fabricante: 'Mercury General',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd89"),
      codigo: 2,
      nombre: 'Small Soft Fish',
      unidades: 96,
      precio: 189,
      fabricante: 'Primoris Services',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      codigo: 4,
      nombre: 'Ergonomic Metal Ball',
      unidades: 5,
      precio: 246,
      fabricante: 'Seaboard',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8e"),
      codigo: 7,
      nombre: 'Handmade Steel Chair',
      unidades: 16,
      precio: 337,
      fabricante: 'CIT Group',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      codigo: 10,
      nombre: 'Handmade Plastic Hat',
      unidades: 7,
      precio: 253,
      fabricante: "Dick's Sporting Goods",
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd95"),
      codigo: 14,
      nombre: 'Small Concrete Fish',
      unidades: 40,
      precio: 126,
      fabricante: 'Precision Castparts',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9a"),
      codigo: 19,
      nombre: 'Handcrafted Steel Chicken',
      unidades: 55,
      precio: 113,
      fabricante: 'State Street Corp.',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9e"),
      codigo: 23,
      nombre: 'Handcrafted Metal Tuna',
      unidades: 63,
      precio: 320,
      fabricante: 'Williams-Sonoma',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda1"),
      codigo: 26,
      nombre: 'Intelligent Plastic Bike',
      unidades: 39,
      precio: 241,
      fabricante: 'Tractor Supply',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda3"),
      codigo: 28,
      nombre: 'Handcrafted Granite Cheese',
      unidades: 27,
      precio: 304,
      fabricante: 'Lennar',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda4"),
      codigo: 29,
      nombre: 'Unbranded Soft Computer',
      unidades: 33,
      precio: 69,
      fabricante: 'Delta Tucker Holdings',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda6"),
      codigo: 31,
      nombre: 'Generic Fresh Keyboard',
      unidades: 69,
      precio: 16,
      fabricante: 'WestRock',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda7"),
      codigo: 32,
      nombre: 'Sleek Soft Towels',
      unidades: 68,
      precio: 68,
      fabricante: 'Alere',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda9"),
      codigo: 34,
      nombre: 'Practical Cotton Keyboard',
      unidades: 43,
      precio: 25,
      fabricante: 'AutoNation',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdab"),
      codigo: 36,
      nombre: 'Rustic Soft Table',
      unidades: 73,
      precio: 331,
      fabricante: 'Werner Enterprises',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdae"),
      codigo: 39,
      nombre: 'Handmade Soft Chips',
      unidades: 56,
      precio: 208,
      fabricante: 'State Farm Insurance Cos.',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdaf"),
      codigo: 40,
      nombre: 'Handmade Frozen Salad',
      unidades: 13,
      precio: 85,
      fabricante: 'Nordstrom',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb1"),
      codigo: 42,
      nombre: 'Licensed Granite Ball',
      unidades: 74,
      precio: 92,
      fabricante: 'SunPower',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb6"),
      codigo: 47,
      nombre: 'Practical Frozen Chips',
      unidades: 0,
      precio: 305,
      fabricante: 'Delta Air Lines',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb9"),
      codigo: 50,
      nombre: 'Awesome Frozen Shoes',
      unidades: 33,
      precio: 125,
      fabricante: 'Comerica',
      tipo: 'medio'
    }
  ]
```
---
## Indicar con un distinct, las empresas (fabricantes) que hay en la colección  
**db.productos.distinct("fabricante");**
```
[
    'A.O. Smith',
    'Alere',
    'American Tire Distributors Holdings',
    'Anthem',
    'Archrock',
    'Ascena Retail Group',
    'AutoNation',
    'Best Buy',
    'CIT Group',
    'Cabot',
    'Comcast',
    'Comerica',
    'Core-Mark Holding',
    'DST Systems',
    'Darling Ingredients',
    'Delta Air Lines',
    'Delta Tucker Holdings',
    "Dick's Sporting Goods",
    'First Solar',
    'HCA Holdings',
    'Hanesbrands',
    'Hartford Financial Services Group',
    'Hawaiian Holdings',
    'HealthSouth',
    'Hyatt Hotels',
    'Kar Auction Services',
    'Kelly Services',
    'Kemper',
    'Kimberly-Clark',
    'Lennar',
    'Mercury General',
    'Mondelez International',
    'Motorola Solutions',
    'Nasdaq OMX Group',
    'National Oilwell Varco',
    'Nordstrom',
    'OneMain Holdings',
    'Oneok',
    'Orbital ATK',
    'Pep Boys-Mann',
    'Pool',
    'Precision Castparts',
    'Primoris Services',
    'Raymond James Financial',
    'Seaboard',
    'Securian Financial Group',
    'Simon Property Group',
    'State Farm Insurance Cos.',
    'State Street Corp.',
    'SunPower',
    'TEGNA',
    'Telephone & Data Systems',
    'Total System Services',
    'Tractor Supply',
    'TransDigm Group',
    'Trinity Industries',
    'TrueBlue',
    'Universal American',
    'Universal Health Services',
    'WGL Holdings',
    "Wendy's",
    'Werner Enterprises',
    'WestRock',
    'Williams-Sonoma'
  ]
```
---
## Usando aggregate, visualizar los productos que tengan más de 80 unidades  
**db.getCollection('productos').find({
  unidades: { $gt: 80 }
});**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd87"),
      codigo: 0,
      nombre: 'Fantastic Wooden Fish',
      unidades: 95,
      precio: 291,
      fabricante: 'Kimberly-Clark',
      tipo: 'avanzado'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd89"),
      codigo: 2,
      nombre: 'Small Soft Fish',
      unidades: 96,
      precio: 189,
      fabricante: 'Primoris Services',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd93"),
      codigo: 12,
      nombre: 'Refined Concrete Salad',
      unidades: 90,
      precio: 129,
      fabricante: 'Universal Health Services',
      tipo: 'avanzado'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda5"),
      codigo: 30,
      nombre: 'Small Rubber Pants',
      unidades: 89,
      precio: 16,
      fabricante: 'Hanesbrands',
      tipo: 'basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fda8"),
      codigo: 33,
      nombre: 'Generic Concrete Hat',
      unidades: 82,
      precio: 70,
      fabricante: 'American Tire Distributors Holdings',
      tipo: 'basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbc"),
      codigo: 53,
      nombre: 'Licensed Plastic Hat',
      unidades: 96,
      precio: 38,
      fabricante: 'Best Buy',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbd"),
      codigo: 54,
      nombre: 'Generic Metal Sausages',
      unidades: 84,
      precio: 77,
      fabricante: 'DST Systems',
      tipo: 'medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc4"),
      codigo: 61,
      nombre: 'Sleek Rubber Keyboard',
      unidades: 82,
      precio: 33,
      fabricante: 'Alere',
      tipo: 'basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc9"),
      codigo: 66,
      nombre: 'Incredible Concrete Fish',
      unidades: 96,
      precio: 336,
      fabricante: 'Darling Ingredients',
      tipo: 'medio'
    }
  ]
```
---
## Con $project visualizar solo el nombre, unidades y precio de los productos que  tengan menos de 10 unidades

**db.getCollection('productos').aggregate(
   [
     {
       $project: {
         nombre: 1,
         unidades: 1,
         precio: 1
       }
     },
     { $match: { unidades: { $lt: 10 } } }
   ]
 );**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      nombre: 'Ergonomic Metal Ball',
      unidades: 5,
      precio: 246
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      nombre: 'Handmade Plastic Hat',
      unidades: 7,
      precio: 253
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9b"),
      nombre: 'Ergonomic Metal Table',
      unidades: 0,
      precio: 94
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb6"),
      nombre: 'Practical Frozen Chips',
      unidades: 0,
      precio: 305
    },
    {
      _id: ObjectId("66158f33b51434e90848fdba"),
      nombre: 'Fantastic Metal Pants',
      unidades: 5,
      precio: 129
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbf"),
      nombre: 'Intelligent Frozen Sausages',
      unidades: 3,
      precio: 111
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc6"),
      nombre: 'Rustic Plastic Mouse',
      unidades: 5,
      precio: 24
    }
  ]
```
---
## Con $project ponemos el fabricante, pero le cambiamos el nombre por “empresa”.  Usamos el mismo comando anterior 
**db.getCollection('productos').aggregate(
  [
    {
      $project: {
        nombre: 1,
        unidades: 1,
        precio: 1
      }
    },
    { $match: { unidades: { $lt: 10 } } }
  ]
);**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      nombre: 'Ergonomic Metal Ball',
      unidades: 5,
      precio: 246,
      empresa: 'Seaboard'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      nombre: 'Handmade Plastic Hat',
      unidades: 7,
      precio: 253,
      empresa: "Dick's Sporting Goods"
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9b"),
      nombre: 'Ergonomic Metal Table',
      unidades: 0,
      precio: 94,
      empresa: 'Kelly Services'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb6"),
      nombre: 'Practical Frozen Chips',
      unidades: 0,
      precio: 305,
      empresa: 'Delta Air Lines'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdba"),
      nombre: 'Fantastic Metal Pants',
      unidades: 5,
      precio: 129,
      empresa: 'OneMain Holdings'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbf"),
      nombre: 'Intelligent Frozen Sausages',
      unidades: 3,
      precio: 111,
      empresa: 'A.O. Smith'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc6"),
      nombre: 'Rustic Plastic Mouse',
      unidades: 5,
      precio: 24,
      empresa: 'Orbital ATK'
    }
  ]
```

---
## Añadir a la consulta anterior un campo calculado que se llame total y que multiplique  precio por unidades. 
**db.getCollection('productos').aggregate(
  [
    {
      $project: {
        nombre: 1,
        unidades: 1,
        precio: 1,
        empresa: '$fabricante',
         total: {
           $multiply: ['$precio', '$unidades']
        }
      }
    },
    { $match: { unidades: { $lt: 10 } } }
  ]
);**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      nombre: 'Ergonomic Metal Ball',
      unidades: 5,
      precio: 246,
      empresa: 'Seaboard',
      total: 1230
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      nombre: 'Handmade Plastic Hat',
      unidades: 7,
      precio: 253,
      empresa: "Dick's Sporting Goods",
      total: 1771
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9b"),
      nombre: 'Ergonomic Metal Table',
      unidades: 0,
      precio: 94,
      empresa: 'Kelly Services',
      total: 0
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb6"),
      nombre: 'Practical Frozen Chips',
      unidades: 0,
      precio: 305,
      empresa: 'Delta Air Lines',
      total: 0
    },
    {
      _id: ObjectId("66158f33b51434e90848fdba"),
      nombre: 'Fantastic Metal Pants',
      unidades: 5,
      precio: 129,
      empresa: 'OneMain Holdings',
      total: 645
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbf"),
      nombre: 'Intelligent Frozen Sausages',
      unidades: 3,
      precio: 111,
      empresa: 'A.O. Smith',
      total: 333
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc6"),
      nombre: 'Rustic Plastic Mouse',
      unidades: 5,
      precio: 24,
      empresa: 'Orbital ATK',
      total: 120
    }
  ]
```

---
## Hacer que el nombre salga en mayúsculas con el operador $toUpper 
**db.getCollection('productos').aggregate(
  [
    {
      $project: {
        nombre: { $toUpper: '$nombre' }
      }
    }
  ]
);**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd87"),
      nombre: 'FANTASTIC WOODEN FISH'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd88"),
      nombre: 'RUSTIC CONCRETE PANTS'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd89"),
      nombre: 'SMALL SOFT FISH'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8a"),
      nombre: 'PRACTICAL SOFT PANTS'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      nombre: 'ERGONOMIC METAL BALL'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8c"),
      nombre: 'SMALL STEEL GLOVES'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8d"),
      nombre: 'ERGONOMIC WOODEN SHIRT'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8e"),
      nombre: 'HANDMADE STEEL CHAIR'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8f"),
      nombre: 'HANDCRAFTED SOFT GLOVES'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd90"),
      nombre: 'FANTASTIC CONCRETE SALAD'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      nombre: 'HANDMADE PLASTIC HAT'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd92"),
      nombre: 'REFINED WOODEN TUNA'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd93"),
      nombre: 'REFINED CONCRETE SALAD'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd94"),
      nombre: 'UNBRANDED SOFT FISH'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd95"),
      nombre: 'SMALL CONCRETE FISH'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd96"),
      nombre: 'REFINED CONCRETE BIKE'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd97"),
      nombre: 'TASTY COTTON PANTS'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd98"),
      nombre: 'INCREDIBLE GRANITE GLOVES'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd99"),
      nombre: 'PRACTICAL METAL MOUSE'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9a"),
      nombre: 'HANDCRAFTED STEEL CHICKEN'
    }
  ]
```

---
## Añadir un campo calculado que ponga el nombre del producto y el tipo concatenado  con el operador $concat. Le llamamos al campo “completo” 
**db.getCollection('productos').aggregate(
  [
    {
      $project: {
        nombre: { $toUpper: '$nombre' },
        unidades: 1,
        precio: 1,
        empresa: '$fabricante',
        total: {
          $multiply: ['$precio', '$unidades']
        },
        completo: {
          $concat: ['$nombre', ' - ', '$tipo']
        }
      }
    },
    { $match: { unidades: { $lt: 10 } } }
  ]
);**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      unidades: 5,
      precio: 246,
      nombre: 'ERGONOMIC METAL BALL',
      empresa: 'Seaboard',
      total: 1230,
      completo: 'Ergonomic Metal Ball - medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      unidades: 7,
      precio: 253,
      nombre: 'HANDMADE PLASTIC HAT',
      empresa: "Dick's Sporting Goods",
      total: 1771,
      completo: 'Handmade Plastic Hat - medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9b"),
      unidades: 0,
      precio: 94,
      nombre: 'ERGONOMIC METAL TABLE',
      empresa: 'Kelly Services',
      total: 0,
      completo: 'Ergonomic Metal Table - avanzado'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb6"),
      unidades: 0,
      precio: 305,
      nombre: 'PRACTICAL FROZEN CHIPS',
      empresa: 'Delta Air Lines',
      total: 0,
      completo: 'Practical Frozen Chips - medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdba"),
      unidades: 5,
      precio: 129,
      nombre: 'FANTASTIC METAL PANTS',
      empresa: 'OneMain Holdings',
      total: 645,
      completo: 'Fantastic Metal Pants - basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbf"),
      unidades: 3,
      precio: 111,
      nombre: 'INTELLIGENT FROZEN SAUSAGES',
      empresa: 'A.O. Smith',
      total: 333,
      completo: 'Intelligent Frozen Sausages - basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc6"),
      unidades: 5,
      precio: 24,
      nombre: 'RUSTIC PLASTIC MOUSE',
      empresa: 'Orbital ATK',
      total: 120,
      completo: 'Rustic Plastic Mouse - avanzado'
    }
  ]
```

---
## Ordena el resultado por el campo “total”  
**db.getCollection('productos').aggregate(
  [
    {
      $project: {
        nombre: { $toUpper: '$nombre' },
        unidades: 1,
        precio: 1,
        empresa: '$fabricante',
        total: {
          $multiply: ['$precio', '$unidades']
        },
        completo: {
          $concat: ['$nombre', ' - ', '$tipo']
        }
      }
    },
    { $match: { unidades: { $lt: 10 } } },
    { $sort: { total: 1 } }
  ]
);**

```
[
    {
      _id: ObjectId("66158f33b51434e90848fd9b"),
      unidades: 0,
      precio: 94,
      nombre: 'ERGONOMIC METAL TABLE',
      empresa: 'Kelly Services',
      total: 0,
      completo: 'Ergonomic Metal Table - avanzado'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdb6"),
      unidades: 0,
      precio: 305,
      nombre: 'PRACTICAL FROZEN CHIPS',
      empresa: 'Delta Air Lines',
      total: 0,
      completo: 'Practical Frozen Chips - medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdc6"),
      unidades: 5,
      precio: 24,
      nombre: 'RUSTIC PLASTIC MOUSE',
      empresa: 'Orbital ATK',
      total: 120,
      completo: 'Rustic Plastic Mouse - avanzado'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdbf"),
      unidades: 3,
      precio: 111,
      nombre: 'INTELLIGENT FROZEN SAUSAGES',
      empresa: 'A.O. Smith',
      total: 333,
      completo: 'Intelligent Frozen Sausages - basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fdba"),
      unidades: 5,
      precio: 129,
      nombre: 'FANTASTIC METAL PANTS',
      empresa: 'OneMain Holdings',
      total: 645,
      completo: 'Fantastic Metal Pants - basico'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      unidades: 5,
      precio: 246,
      nombre: 'ERGONOMIC METAL BALL',
      empresa: 'Seaboard',
      total: 1230,
      completo: 'Ergonomic Metal Ball - medio'
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      unidades: 7,
      precio: 253,
      nombre: 'HANDMADE PLASTIC HAT',
      empresa: "Dick's Sporting Goods",
      total: 1771,
      completo: 'Handmade Plastic Hat - medio'
    }
  ]
```

---
## Haciendo una nueva consulta, averiguar el numero de productos por tipo de producto  
**db.getCollection('productos').aggregate(
  [
    {
      $group: {
        _id: { tipo: '$tipo' },
        'Numero de Productos': { $count: {} }
      }
    }
  ]
);**

```
[
    { _id: { tipo: 'medio' }, 'Numero de Productos': 25 },
    { _id: { tipo: 'basico' }, 'Numero de Productos': 24 },
    { _id: { tipo: 'avanzado' }, 'Numero de Productos': 18 }
  ]
```
---
## Añadir el valor mayor y el menor  
**db.getCollection('productos').aggregate(
  [
    {
      $group: {
        _id: { tipo: '$tipo' },
        'Numero de Productos': { $count: {} },
        Minimo: { $min: '$precio' },
        Maximo: { $max: '$precio' }
      }
    }
  ]
);**

```
[
    {
      _id: { tipo: 'medio' },
      'Numero de Productos': 25,
      Minimo: 16,
      Maximo: 337
    },
    {
      _id: { tipo: 'basico' },
      'Numero de Productos': 24,
      Minimo: 16,
      Maximo: 285
    },
    {
      _id: { tipo: 'avanzado' },
      'Numero de Productos': 18,
      Minimo: 18,
      Maximo: 331
    }
  ]
```

---
## Añade el total de unidades por cada tipo  
**db.getCollection('productos').aggregate(
  [
    {
      $group: {
        _id: { tipo: '$tipo' },
        'Numero de Productos': { $count: {} },
        Minimo: { $min: '$precio' },
        Maximo: { $max: '$precio' },
        'Total de unidades': { $sum: '$unidades' }
      }
    }
  ]
);**

```
[
    {
      _id: { tipo: 'medio' },
      'Numero de Productos': 25,
      Minimo: 16,
      Maximo: 337,
      'Total de unidades': 1224
    },
    {
      _id: { tipo: 'basico' },
      'Numero de Productos': 24,
      Minimo: 16,
      Maximo: 285,
      'Total de unidades': 1067
    },
    {
      _id: { tipo: 'avanzado' },
      'Numero de Productos': 18,
      Minimo: 18,
      Maximo: 331,
      'Total de unidades': 773
    }
  ]
```

---
## Con el operador $set y el operador “$substr” visualiza todos los datos del producto  "Small Metal Tuna" y los primeros 5 caracteres del nombre
**db.getCollection('productos').aggregate(
  [
    { $match: { nombre: 'Small Metal Tuna' } },
    {
      $set: {
        nombre: { $substr: ['$nombre', 0, 5] }
      }
    }
  ]
);**

```

  [
    {
      _id: ObjectId("66158f33b51434e90848fdbe"),
      codigo: 55,
      nombre: 'Small',
      unidades: 46,
      precio: 43,
      fabricante: 'Raymond James Financial',
      tipo: 'medio'
    }
  ]
```

---
## Creamos una salida que tenga el nombre del articulo y el total (precio por unidades) y  lo guardamos en una colección denominada productos2 
**db.getCollection('productos').aggregate(
  [
    {
      $project: {
        'Nombre del articulo': '$nombre',
        Total: {
          $multiply: ['$unidades', '$precio']
        }
      }
    },
    { $out : "productos2" }
  ]
);**

```
```

---

## Comprobamos que se ha creado 
**show collections**

```
productos
productos2
```

---
## Hacemos un find para comprobar el resultado 

 **db.getCollection('productos2').find()**

```
 [
    {
      _id: ObjectId("66158f33b51434e90848fd87"),
      'Nombre del articulo': 'Fantastic Wooden Fish',
      Total: 27645
    },
    {
      _id: ObjectId("66158f33b51434e90848fd88"),
      'Nombre del articulo': 'Rustic Concrete Pants',
      Total: 18414
    },
    {
      _id: ObjectId("66158f33b51434e90848fd89"),
      'Nombre del articulo': 'Small Soft Fish',
      Total: 18144
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8a"),
      'Nombre del articulo': 'Practical Soft Pants',
      Total: 2747
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8b"),
      'Nombre del articulo': 'Ergonomic Metal Ball',
      Total: 1230
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8c"),
      'Nombre del articulo': 'Small Steel Gloves',
      Total: 1665
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8d"),
      'Nombre del articulo': 'Ergonomic Wooden Shirt',
      Total: 14994
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8e"),
      'Nombre del articulo': 'Handmade Steel Chair',
      Total: 5392
    },
    {
      _id: ObjectId("66158f33b51434e90848fd8f"),
      'Nombre del articulo': 'Handcrafted Soft Gloves',
      Total: 4512
    },
    {
      _id: ObjectId("66158f33b51434e90848fd90"),
      'Nombre del articulo': 'Fantastic Concrete Salad',
      Total: 12985
    },
    {
      _id: ObjectId("66158f33b51434e90848fd91"),
      'Nombre del articulo': 'Handmade Plastic Hat',
      Total: 1771
    },
    {
      _id: ObjectId("66158f33b51434e90848fd92"),
      'Nombre del articulo': 'Refined Wooden Tuna',
      Total: 8480
    },
    {
      _id: ObjectId("66158f33b51434e90848fd93"),
      'Nombre del articulo': 'Refined Concrete Salad',
      Total: 11610
    },
    {
      _id: ObjectId("66158f33b51434e90848fd94"),
      'Nombre del articulo': 'Unbranded Soft Fish',
      Total: 9434
    },
    {
      _id: ObjectId("66158f33b51434e90848fd95"),
      'Nombre del articulo': 'Small Concrete Fish',
      Total: 5040
    },
    {
      _id: ObjectId("66158f33b51434e90848fd96"),
      'Nombre del articulo': 'Refined Concrete Bike',
      Total: 2700
    },
    {
      _id: ObjectId("66158f33b51434e90848fd97"),
      'Nombre del articulo': 'Tasty Cotton Pants',
      Total: 3536
    },
    {
      _id: ObjectId("66158f33b51434e90848fd98"),
      'Nombre del articulo': 'Incredible Granite Gloves',
      Total: 20590
    },
    {
      _id: ObjectId("66158f33b51434e90848fd99"),
      'Nombre del articulo': 'Practical Metal Mouse',
      Total: 6650
    },
    {
      _id: ObjectId("66158f33b51434e90848fd9a"),
      'Nombre del articulo': 'Handcrafted Steel Chicken',
      Total: 6215
    }
  ]
  ```