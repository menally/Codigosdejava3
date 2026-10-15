import java.util.Scanner;
public class Main {
public static void main (String[] args){
        int contador = 1;
        while (contador <= 5) {
            System.out.println("Numero actual:" + contador);
            contador++;
        }

        System.out.println("--------------------");

        Scanner scanner = new Scanner(System.in);
        int numero = -1;

        while (numero != 0) {
            System.out.println("Ingresa un numero, (ingresa 0 para salir):");
            numero = scanner.nextInt();

            if (numero != 0) {
                System.out.println("Registrado:" + numero);
            }


            System.out.println("----------------");

            System.out.println("DO-WHILE del 1 al 5");
            int i = 1;
            do {
                System.out.println("Numero do-while:" + i);
                i++;
            } while (i <= 5);

            System.out.println("--------------------");

            System.out.println("Validacion de contraseña");
            int passwordCorrecta = 1234;
            int passwordIngresada;
            do {
                System.out.println("Ingresa la contraseña numerica:");
                passwordIngresada = scanner.nextInt();

                if (passwordIngresada != passwordCorrecta) {
                    System.out.println("Contraseña incorreta, Intentalo de nuevo");
                }
            } while (passwordIngresada != passwordCorrecta);
            System.out.println("Acceso concedido");
        }

        System.out.println("--------------------");

        System.out.println("Numeros pares del 2 al 10");
        for (int i = 2; i <= 10; i += 2) {
            System.out.println("Numero par:" + i);
        }

        System.out.println("-------------------");

        System.out.println("Tabla de multiplicar");
        System.out.println("Ingresa un numero entero positivo para ver su tabla:");
        int numeroTabla = scanner.nextInt();

        for (int j = 1; j <= 10; j++) {
            int resultado = numeroTabla * j;
            System.out.println(numeroTabla + "x" + j + "=" + resultado);

        }
        System.out.println("----------------------------------");

        System.out.println("Suma de elementos");
        int[] numeros = {10, 20, 30, 40, 50};
        int sumaTotal = 0;
        for (int num : numeros) {
            sumaTotal += num;
        }

        System.out.println("El resultado total de la suma es:" + sumaTotal);
        System.out.println("-------------------------");

        System.out.println("Saludos personalizados");
        String[] nombres = {"Sofia", "Maria", "Perla", "Vanessa",};
        for (String nombrePersona : nombres) {
            System.out.println("Hola," + nombrePersona + ",Bienvenida");
        }
        System.out.println("---------------------------");
        System.out.println("Ejemplo break");
        for (int i = 1; i <= 10; i++) {
            if (i == 7) {
                break;
            }
            System.out.println("i =" + i);
        }
        System.out.println("Ejemplo continue");
        for (int j = 1; j <= 5; j++) {
            if (j == 3) {
                continue;
            }
            System.out.println("j=" + j);
        }
        System.out.println("--------------------------");
        System.out.println("Tabla de coordenadas");
        for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= 3; j++) {
                System.out.println("(" + i + " , " + j + " )");
            }
            System.out.println();
        }

            System.out.println("------------------------");
            System.out.println("Triangulo asteriscos");

            for (int i = 1; i <= 3 ; i++) {
                for (int j = 1; j <= i; j++) {
                    System.out.print("*");
                }
                System.out.println();
            }

            scanner.close();
        }
    }