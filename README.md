package co.edu.uniquindio.poo;

import java.util.ArrayList;
import java.util.List;

public record veterinariaBasic(String nombre, String especie, String raza, String genero, String color, int edad, int peso) {

    // Enum con las propiedades

            public class EnumsAnimal {

            public enum especie {
                PERRO, GATO, TORTUGA, PEZ ;
            }
        
            public enum raza {
                PERSA, SIAMES, SIBERIANO, BULLDOG, PASTOR, LABRADOR, GOLFINA, CAGUAMA, CAREY, BETTA, GUPPY, TETRANEON ;
            }
        
            public enum genero {
                MASCULINO, FEMENINO ;
            }
        
            public enum color {
                AZUL, VERDE, CAFE, NEGRO, GRIS, BLANCO, MANCHADO, DORADO ;
            }
        
        }
        
    // Constructor
    public veterinariaBasic {
        assert nombre != null && !nombre.isBlank() : "El nombre debe ser diferente";
        assert especie != null && !especie.isBlank() : "La especie debe ser diferente";
        assert raza != null && !raza.isBlank() : "La raza debe ser diferente";
        assert genero != null && !genero.isBlank() : "El género debe ser diferente";
        assert color != null && !color.isBlank() : "El color debe ser diferente";
        assert edad > 0 : "La edad debe ser mayor a cero";
        assert peso > 0 : "El peso debe ser mayor a cero";      
    }

    public static void main(String[] args) {

        
        // Crear una lista de veterinariaBasic utilizando ArrayList
        List<veterinariaBasic> listaveterinariaBasic = new ArrayList<>();

        // Crear 60 instancias de veterinariaBasic y agregarlas a la lista

        listaveterinariaBasic.add(new veterinariaBasic("Sasha", "Perro", "Labrador", "Femenino", "Azul", 3, 25));

        listaveterinariaBasic.add(new veterinariaBasic("Simba", "Gato", "Guppy", "Masculino", "Verde", 2, 10));

        listaveterinariaBasic.add(new veterinariaBasic("Puffy", "Tortuga", "Siberiano", "Masculino", "Cafe", 5, 15));

        listaveterinariaBasic.add(new veterinariaBasic("Luna", "Pez", "Persa", "Femenino", "Gris", 4, 12));

        listaveterinariaBasic.add(new veterinariaBasic("Rocky", "Perro", "Bulldog", "Masculino", "Negro", 7, 30));

        listaveterinariaBasic.add(new veterinariaBasic("Bella", "Gato", "Siames", "Femenino", "Verde", 1, 8));

        listaveterinariaBasic.add(new veterinariaBasic("Max", "Tortuga", "Pastor", "Masculino", "Blanco", 4, 28));

        listaveterinariaBasic.add(new veterinariaBasic("Nina", "Pez", "Golfina", "Femenino", "Azul", 3, 18));

        listaveterinariaBasic.add(new veterinariaBasic("Lucky", "Perro", "Labrador", "Masculino", "Verde", 6, 22));

        listaveterinariaBasic.add(new veterinariaBasic("Daisy", "Gato", "Persa", "Femenino", "Verde", 2, 10));

        listaveterinariaBasic.add(new veterinariaBasic("Charlie", "Tortuga", "Caguama", "Masculino", "Cafe", 5, 5));

        listaveterinariaBasic.add(new veterinariaBasic("Milo", "Pez", "Guppy", "Masculino", "Dorado", 3, 14));

        listaveterinariaBasic.add(new veterinariaBasic("Coco", "Perro", "Siberiano", "Masculino", "Verde", 8, 18));

        listaveterinariaBasic.add(new veterinariaBasic("Lola", "Gato", "Carey", "Femenino", "Manchado", 4, 20));

        listaveterinariaBasic.add(new veterinariaBasic("Toby", "Tortuga", "Bulldog", "Masculino", "Negro", 5, 25));

        listaveterinariaBasic.add(new veterinariaBasic("Chloe", "Pez", "Siames", "Femenino", "Verde", 2, 8));

        listaveterinariaBasic.add(new veterinariaBasic("Teddy", "Perro", "Betta", "Masculino", "Azul", 6, 16));

        listaveterinariaBasic.add(new veterinariaBasic("Lucy", "Gato", "Golfina", "Femenino", "Gris", 5, 22));

        listaveterinariaBasic.add(new veterinariaBasic("Buddy", "Perro", "Labrador", "Masculino", "Dorado", 7, 30));

        listaveterinariaBasic.add(new veterinariaBasic("Zoe", "Gato", "Persa", "Femenino", "Verde", 1, 7));

        listaveterinariaBasic.add(new veterinariaBasic("Jack", "Perro", "Pastor", "Masculino", "Azul", 4, 26));

        listaveterinariaBasic.add(new veterinariaBasic("Mia", "Tortuga", "Golfina", "Femenino", "Verde", 3, 15));

        listaveterinariaBasic.add(new veterinariaBasic("Rocky", "Pez", "Caguama", "Masculino", "Cafe", 5, 6));

        listaveterinariaBasic.add(new veterinariaBasic("Luna", "Pez", "Carey", "Femenino", "Manchado", 2, 10));

        listaveterinariaBasic.add(new veterinariaBasic("Max", "Tortuga", "Siberiano", "Masculino", "Verde", 8, 20));

        listaveterinariaBasic.add(new veterinariaBasic("Daisy", "Tortuga", "Guppy", "Femenino", "Gris", 4, 12));

        listaveterinariaBasic.add(new veterinariaBasic("Charlie", "Gato", "Bulldog", "Masculino", "Negro", 5, 28));

        listaveterinariaBasic.add(new veterinariaBasic("Milo", "Gato", "Siames", "Masculino", "Verde", 3, 16));

        listaveterinariaBasic.add(new veterinariaBasic("Charlie", "Perro", "Bulldog", "Masculino", "Negro", 5, 28));

        listaveterinariaBasic.add(new veterinariaBasic("Milo", "Perro", "Siames", "Masculino", "Verde", 3, 16));

        listaveterinariaBasic.add(new veterinariaBasic("Sasha", "Tortuga", "Labrador", "Femenino", "Azul", 3, 25));

        listaveterinariaBasic.add(new veterinariaBasic("Simba", "Pez", "Guppy", "Masculino", "Verde", 2, 10));

        listaveterinariaBasic.add(new veterinariaBasic("Puffy", "Perro", "Siberiano", "Masculino", "Cafe", 5, 15));

        listaveterinariaBasic.add(new veterinariaBasic("Luna", "Gato", "Persa", "Femenino", "Gris", 4, 12));

        listaveterinariaBasic.add(new veterinariaBasic("Rocky", "Tortuga", "Bulldog", "Masculino", "Negro", 7, 30));

        listaveterinariaBasic.add(new veterinariaBasic("Bella", "Pez", "TetraNeon", "Femenino", "Verde", 1, 8));

        listaveterinariaBasic.add(new veterinariaBasic("Max", "Perro", "Pastor", "Masculino", "Blanco", 4, 28));

        listaveterinariaBasic.add(new veterinariaBasic("Nina", "Gato", "Golfina", "Femenino", "Azul", 3, 18));

        listaveterinariaBasic.add(new veterinariaBasic("Lucky", "Perro", "Labrador", "Masculino", "Verde", 6, 22));

        listaveterinariaBasic.add(new veterinariaBasic("Daisy", "Gato", "Persa", "Femenino", "Verde", 2, 10));

        listaveterinariaBasic.add(new veterinariaBasic("Charlie", "Tortuga", "Caguama", "Masculino", "Cafe", 5, 5));

        listaveterinariaBasic.add(new veterinariaBasic("Milo", "Pez", "Guppy", "Masculino", "Gris", 3, 14));

        listaveterinariaBasic.add(new veterinariaBasic("Coco", "Tortuga", "Siberiano", "Masculino", "Verde", 8, 18));

        listaveterinariaBasic.add(new veterinariaBasic("Lola", "Pez", "Carey", "Femenino", "Manchado", 4, 20));

        listaveterinariaBasic.add(new veterinariaBasic("Toby", "Perro", "Bulldog", "Masculino", "Negro", 5, 25));

        listaveterinariaBasic.add(new veterinariaBasic("Chloe", "Tortuga", "Siames", "Femenino", "Verde", 2, 8));

        listaveterinariaBasic.add(new veterinariaBasic("Teddy", "Perro", "Betta", "Masculino", "Azul", 6, 16));

        listaveterinariaBasic.add(new veterinariaBasic("Lucy", "Gato", "Golfina", "Femenino", "Gris", 5, 22));

        listaveterinariaBasic.add(new veterinariaBasic("Buddy", "Tortuga", "TetraNeon", "Masculino", "Blanco", 7, 30));

        listaveterinariaBasic.add(new veterinariaBasic("Zoe", "Gato", "Persa", "Femenino", "Verde", 1, 7));

        listaveterinariaBasic.add(new veterinariaBasic("Jack", "Perro", "Pastor", "Masculino", "Azul", 4, 26));

        listaveterinariaBasic.add(new veterinariaBasic("Mia", "Pez", "Golfina", "Femenino", "Verde", 3, 15));

        listaveterinariaBasic.add(new veterinariaBasic("Rocky", "Perro", "Caguama", "Masculino", "Cafe", 5, 6));

        listaveterinariaBasic.add(new veterinariaBasic("Luna", "Pez", "Carey", "Femenino", "Manchado", 2, 10));

        listaveterinariaBasic.add(new veterinariaBasic("Max", "Perro", "Siberiano", "Masculino", "Verde", 8, 20));

        listaveterinariaBasic.add(new veterinariaBasic("Daisy", "Gato", "Guppy", "Femenino", "Gris", 4, 12));

        listaveterinariaBasic.add(new veterinariaBasic("Charlie", "Perro", "Bulldog", "Masculino", "Negro", 5, 28));

        listaveterinariaBasic.add(new veterinariaBasic("Milo", "Tortuga", "Siames", "Masculino", "Verde", 3, 16));

        listaveterinariaBasic.add(new veterinariaBasic("Charlie", "Perro", "TetraNeon", "Masculino", "Negro", 5, 28));

        listaveterinariaBasic.add(new veterinariaBasic("Milo", "Pez", "Siames", "Masculino", "Verde", 3, 16));

         // Contadores para cada especie

         int contadorPerros = 0;
         int contadorGatos = 0;
         int contadorTortugas = 0;
         int contadorPeces = 0;

          // Contadores para cada raza

         int contadorPersas = 0;
         int contadorSiameses = 0;
         int contadorSiberianos = 0;
         int contadorBulldogs = 0;
         int contadorPastores = 0;
         int contadorLabradores = 0;
         int contadorGolfinas = 0;
         int contadorCaguamas = 0;
         int contadorCareys = 0;
         int contadorBettas = 0;
         int contadorGuppys = 0;
         int contadorTetraNeones = 0;

          // Contadores para cada genero

         int contadorMasculinos = 0;
         int contadorFemeninos = 0;

          // Contadores para cada color

         int contadorAzules = 0;
         int contadorVerdes = 0;
         int contadorCafes = 0;
         int contadorNegros = 0;
         int contadorGrises = 0;
         int contadorBlancos = 0;
         int contadorManchados = 0;
         int contadorDorados = 0;
 
         // Recorre la lista y cuenta cuantas especies ahi 
         for (veterinariaBasic animal : listaveterinariaBasic) {
            
             if (animal.especie().equals("Perro")) {
                 contadorPerros++;

             } else if (animal.especie().equals("Gato")) {
                 contadorGatos++;

             }else if (animal.especie().equals("Tortuga")) {
                contadorTortugas++;

            }else if (animal.especie().equals("Pez")) {
                contadorPeces++;

            }
         }

         // Recorre la lista y cuenta cuantas razas ahi 

         for (veterinariaBasic animal : listaveterinariaBasic) {
            if (animal.raza().equals("Persa")) {
                contadorPersas++;

        } else if (animal.raza().equals("Siames")) {
                contadorSiameses++;

        }else if (animal.raza().equals("Siberiano")) {
               contadorSiberianos++;

        }else if (animal.raza().equals("Bulldog")) {
               contadorBulldogs++;

        }else if (animal.raza().equals("Pastor")) {
            contadorPastores++;

        }else if (animal.raza().equals("Labrador")) {
            contadorLabradores++;

        }else if (animal.raza().equals("Golfina")) {
            contadorGolfinas++;

        }else if (animal.raza().equals("Caguama")) {
            contadorCaguamas++;

        }else if (animal.raza().equals("Carey")) {
            contadorCareys++;

        }else if (animal.raza().equals("Betta")) {
            contadorBettas++;

        }else if (animal.raza().equals("Guppy")) {
            contadorGuppys++;

        }else if (animal.raza().equals("TetraNeon")) {
            contadorTetraNeones++;

        }
        }

        // Recorre la lista y cuenta cuantos generos ahi 

        for (veterinariaBasic animal : listaveterinariaBasic) {

            if (animal.genero().equals("Masculino")) {
                contadorMasculinos++;

        } else if (animal.genero().equals("Femenino")) {
                contadorFemeninos++;

        }
    }

         // Recorre la lista y cuenta cuantos colores ahi 
          
        for (veterinariaBasic animal : listaveterinariaBasic) {
              if (animal.color().equals("Azul")) {
                contadorAzules++;

        }else if (animal.color().equals("Verde")) {
                contadorVerdes++;

        }else if (animal.color().equals("Cafe")) {
               contadorCafes++;

        }else if (animal.color().equals("Negro")) {
               contadorNegros++;

        }else if (animal.color().equals("Gris")) {
            contadorGrises++;

        }else if (animal.color().equals("Blanco")) {
            contadorBlancos++;

        }else if (animal.color().equals("Manchado")) {
            contadorManchados++;

        }else if (animal.color().equals("Dorado")) {
            contadorDorados++;

        }      
    } 

        // Imprimir la información de cada veterinariaBasic en la lista

        for (veterinariaBasic veterinariaBasic : listaveterinariaBasic) {

            System.out.println("---------------------------------------------------------------------------------------");
            System.out.println("- Nombre: " + veterinariaBasic.nombre());
            System.out.println("- Especie: " + veterinariaBasic.especie());
            System.out.println("- Raza: " + veterinariaBasic.raza());
            System.out.println("- Género: " + veterinariaBasic.genero());
            System.out.println("- Color: " + veterinariaBasic.color());
            System.out.println("- Edad: " + veterinariaBasic.edad());
            System.out.println("- Peso: " + veterinariaBasic.peso());
            System.out.println("----------------------------------------------------------------------------------------");
            System.out.println();

             // Imprimir la información de cada contador de especie
        }
            System.out.println("----------------------------------------------------------------------------------------");
            System.out.println("Contador de especies:");
            System.out.println("Número de Perros: " + contadorPerros);
            System.out.println("Número de Gatos: " + contadorGatos);
            System.out.println("Número de Tortugas: " + contadorTortugas);
            System.out.println("Número de Peces: " + contadorPeces);
            System.out.println("----------------------------------------------------------------------------------------");

             // Imprimir la información de cada contador de raza
  
            System.out.println("----------------------------------------------------------------------------------------");
            System.out.println("Contador de razas:");
            System.out.println("Persas: " + contadorPersas);
            System.out.println("Siameses: " + contadorSiameses);
            System.out.println("Siberianos: " + contadorSiberianos);
            System.out.println("Bulldogs: " + contadorBulldogs);
            System.out.println("Pastores: " + contadorPastores);
            System.out.println("Labradores: " + contadorLabradores);
            System.out.println("Golfinas: " + contadorGolfinas);
            System.out.println("Caguamas: " + contadorCaguamas);
            System.out.println("Careys: " + contadorCareys);
            System.out.println("Bettas: " + contadorBettas);
            System.out.println("Guppys: " + contadorGuppys);
            System.out.println("TetraNeones: " + contadorTetraNeones);
            System.out.println("----------------------------------------------------------------------------------------");

             // Imprimir la información de cada contador de genero

            System.out.println("----------------------------------------------------------------------------------------");
            System.out.println("\nContador de géneros:");
            System.out.println("Masculinos: " + contadorMasculinos);
            System.out.println("Femeninos: " + contadorFemeninos);
            System.out.println("----------------------------------------------------------------------------------------");

             // Imprimir la información de cada contador de colores

            System.out.println("----------------------------------------------------------------------------------------");
            System.out.println("\nContador de colores:");
            System.out.println("Azules: " + contadorAzules);
            System.out.println("Verdes: " + contadorVerdes);
            System.out.println("Cafes: " + contadorCafes);
            System.out.println("Negros: " + contadorNegros);
            System.out.println("Gris: " + contadorGrises);
            System.out.println("Blancos: " + contadorBlancos);
            System.out.println("Manchados: " + contadorManchados);
            System.out.println("Dorados: " + contadorDorados);
            System.out.println("----------------------------------------------------------------------------------------");
    }
}
