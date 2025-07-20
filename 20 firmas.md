using System;
using System.Collections.Generic;

class Persona {

    public string Nombre;
    public int Edad;
}

class Program
{


    static void Main() {
        Saludar();
        MostrarNumero();
        MostrarMensaje("Hola, mundo!");
        int resultado = Sumar(3, 4);
        Console.WriteLine("Resultado suma: " + resultado);
        Console.WriteLine("Es par 6: " + EsPar(6));
        MostrarMultiplicacion(2, 5);
        string saludo = ObtenerSaludo("Ana");
        Console.WriteLine(saludo);
        double promedio = CalcularPromedio(new int[] { 3, 4, 5 });
        Console.WriteLine("Promedio: " + promedio);
        ImprimirArreglo(new string[] { "uno", "dos", "tres" });
        MostrarMatriz(new int[,] { {1,2}, {3,4} });
        Console.WriteLine("Mayor: " + Mayor(10, 15, 8));
        Persona p = CrearPersona("Luis", 20);
        Console.WriteLine($"Persona: {p.Nombre}, Edad: {p.Edad}");
        List<string> lista = CrearLista("a", "b", "c");
        MostrarLista(lista);
        MostrarBooleano(true);
        Console.WriteLine("Área: " + CalcularAreaRectangulo(4, 5));
        ImprimirFechaActual();
        MostrarCaracteres("Hola");
        int[] cuadrados = ElevarAlCuadrado(new int[] {1, 2, 3});
        foreach (int x in cuadrados) Console.Write(x + " ");
        Console.WriteLine();
        MostrarObjeto(p);
    }

    // 1
    static void Saludar() {
        Console.WriteLine("¡Hola!");
    }

    // 2
    static void MostrarNumero() {
        int numero = 10;
        Console.WriteLine("Número: " + numero);
    }

    // 3
    static void MostrarMensaje(string mensaje) {
        Console.WriteLine("Mensaje: " + mensaje);
    }

    // 4
    static int Sumar(int a, int b) {
        return a + b;
    }

    // 5
    static bool EsPar(int numero) {
        return numero % 2 == 0;
    }

    // 6
    static void MostrarMultiplicacion(int a, int b) {
        Console.WriteLine("Multiplicación: " + (a * b));
    }

    // 7
    static string ObtenerSaludo(string nombre) {
        return "Hola, " + nombre;
    }

    // 8
    static double CalcularPromedio(int[] numeros) {
        double suma = 0;
        foreach (int n in numeros) suma += n;
        return suma / numeros.Length;
    }

    // 9
    static void ImprimirArreglo(string[] palabras) {
        foreach (string palabra in palabras) Console.WriteLine(palabra);
    }

    // 10
    static void MostrarMatriz(int[,] matriz) {
        for (int i = 0; i < matriz.GetLength(0); i++) {
            for (int j = 0; j < matriz.GetLength(1); j++) {
                Console.Write(matriz[i,j] + " ");
            }
            Console.WriteLine();
        }
    }

    // 11
    static int Mayor(int a, int b, int c) {
        return Math.Max(a, Math.Max(b, c));
    }

    // 12
    static Persona CrearPersona(string nombre, int edad) {
        return new Persona { Nombre = nombre, Edad = edad };
    }

    // 13
    static List<string> CrearLista(string a, string b, string c) {
        return new List<string> { a, b, c };
    }

    // 14
    static void MostrarLista(List<string> lista) {
        lista.ForEach(Console.WriteLine);
    }

    // 15
    static void MostrarBooleano(bool valor) {
        Console.WriteLine("Valor: " + valor);
    }

    // 16
    static double CalcularAreaRectangulo(double baseR, double altura) {
        return baseR * altura;
    }

    // 17
    static void ImprimirFechaActual() {
        Console.WriteLine("Fecha actual: " + DateTime.Now.ToShortDateString());
    }

    // 18
    static void MostrarCaracteres(string texto) {
        foreach (char c in texto) Console.Write(c + "-");
        Console.WriteLine();
    }

    // 19
    static int[] ElevarAlCuadrado(int[] nums) {
        int[] result = new int[nums.Length];
        for (int i = 0; i < nums.Length; i++) {
            result[i] = nums[i] * nums[i];
        }
        return result;
    }

    // 20
    static void MostrarObjeto(object obj) {
        Console.WriteLine("Objeto: " + obj.ToString());
    }
}
