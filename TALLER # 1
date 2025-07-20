TALLER#1(PRIMERA PARTE)


###  **EJERCICIOS EN C#**

---

####  **1. Recorra una matriz nxm y reemplace los valores negativos por un número positivo**

```csharp
int[,] matriz = {
    {-1, -2, -3},
    {-6, -8, 9},
    {-3, -4, -5}
};

for (int i = 0; i < matriz.GetLength(0); i++) {
    for (int j = 0; j < matriz.GetLength(1); j++) {
        if (matriz[i, j] < 0) {
            matriz[i, j] = Math.Abs(matriz[i, j]);
        }
    }
}

// Imprimir la matriz
for (int i = 0; i < matriz.GetLength(0); i++) {
    for (int j = 0; j < matriz.GetLength(1); j++) {
        Console.Write(matriz[i, j] + "\t");
    }
    Console.WriteLine();
}
```

---

####  **2. Calcule el promedio de los números positivos de un array de números flotantes**

```csharp
float[] numeros = {-2.5f, 3.0f, 4.5f, -1.1f, 6.2f};
float suma = 0;
int contador = 0;

foreach (float num in numeros) {
    if (num > 0) {
        suma += num;
        contador++;
    }
}

float promedio = (contador > 0) ? suma / contador : 0;
Console.WriteLine("Promedio de positivos: " + promedio);
```

---

####  **3. Dada una matriz de cadenas, cree una cadena concatenando sus celdas de izquierda a derecha y de arriba hacia abajo**

```csharp
string[,] matriz = {
    {"Hola", "a"},
    {"todos", "!"}
};

string resultado = "";
for (int i = 0; i < matriz.GetLength(0); i++) {
    for (int j = 0; j < matriz.GetLength(1); j++) {
        resultado += matriz[i, j] + " ";
    }
}

Console.WriteLine("Cadena resultante: " + resultado.Trim());
```

---

####  **4. Lea una matriz nxn de chars e imprima la matriz original y la matriz con filas invertidas**

```csharp
char[,] matriz = {
    {'o', 's', 'o'},
    {'a', 'n', 'a'},
    {'p', 'o', 'p'}
};

int n = matriz.GetLength(0);

// Original
Console.WriteLine("Matriz original:");
for (int i = 0; i < n; i++) {
    for (int j = 0; j < n; j++) {
        Console.Write(matriz[i, j] + " ");
    }
    Console.WriteLine();
}

// Filas invertidas
Console.WriteLine("Filas invertidas:");
for (int i = n - 1; i >= 0; i--) {
    for (int j = 0; j < n; j++) {
        Console.Write(matriz[i, j] + " ");
    }
    Console.WriteLine();
}
```

---

####  **5. Lea una matriz cuadrada y calcule suma de fila/columna de la mitad**

```csharp
int[,] matriz = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};

int n = matriz.GetLength(0);
int mitad = n / 2;

int sumaFila = 0;
int sumaCol = 0;

for (int i = 0; i < n; i++) {
    sumaFila += matriz[mitad, i];
    sumaCol += matriz[i, mitad];
}

Console.WriteLine($"Suma de fila central: {sumaFila}");
Console.WriteLine($"Suma de columna central: {sumaCol}");
```

---

###  **PREGUNTAS DE TEORÍA**

#### 1. ¿Qué es una función en programación?

Una **función** es un bloque de código reutilizable que realiza una tarea específica. En C#, una función se define con un tipo de retorno, un nombre y puede tener parámetros. Permite dividir un programa en partes lógicas más manejables, evitando la repetición de código.

Ejemplo:

```csharp
int Sumar(int a, int b) {
    return a + b;
}
```

---

#### 2. ¿Cuál es la diferencia entre un ciclo `for` y un ciclo `while`?

* `for`: se usa cuando **se conoce** de antemano el número de iteraciones.
* `while`: se usa cuando **no se sabe** cuántas veces se repetirá, pero se tiene una condición.

Ejemplo `for`:

```csharp
for (int i = 0; i < 5; i++) {
    Console.WriteLine(i);
}
```

Ejemplo `while`:

```csharp
int i = 0;
while (i < 5) {
    Console.WriteLine(i);
    i++;
}
```

---


