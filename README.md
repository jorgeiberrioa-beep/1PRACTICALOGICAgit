# 1PRACTICALOGICAgit
1ra practica de Git-DLL-IJAB_UNIQ
public class Main {
    public static void main (String[]args){
        System.ou.println("Hola Jorge, ¿Qué tal?");
    }
}

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        String pregunta = ingresarTexto(
            "Señor Jorge, ¿me puede describir cómo se encuentra el día de hoy con una sola palabra?: "
        );

        String mensaje = mensajeRespuesta(pregunta);
        mostrarMensaje(mensaje);
    }

    public static String ingresarTexto(String mensaje) {
        Scanner scanner = new Scanner(System.in);
        System.out.print(mensaje);
        String texto = scanner.nextLine();
        return texto;
    }

    public static String mensajeRespuesta(String pregunta) {
        String mensaje = "Señor Jorge, nos alegra mucho que usted se encuentre "
                + pregunta + " el día de hoy.";
        return mensaje;
    }

    public static void mostrarMensaje(String mensaje) {
        System.out.println(mensaje);
    }
}
