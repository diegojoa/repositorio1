# repositorio1

 float medida = 0;
 double longitudMax = 25;
 double LongitudMin = 15;
 int contador = 1;
 int piezasAceptadas = 0;
 int piezasNoAceptadas = 0;
 Console.WriteLine("**PIEZAS DE METAL APTAS**");

 while (contador < 10)
 {
     Console.WriteLine($"Digite la Longitud de la pieza {contador}");
     medida = int.Parse(Console.ReadLine());
     contador++;

     if (medida <= longitudMax && medida >= LongitudMin)
     {
         piezasAceptadas++;
     }
     else
     {
         piezasNoAceptadas++;
     }


 }
 Console.WriteLine();
 Console.WriteLine("Las piezas aptas para el lote son: " + piezasAceptadas);
 Console.WriteLine();
 Console.WriteLine("Las piezas no aptas para el lote son: " + piezasNoAceptadas);
