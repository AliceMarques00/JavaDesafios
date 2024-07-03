package Basico;import java.util.Scanner;

public class OperadorExercicio7 {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);

        System.out.println("Farei algumas perguntas, responda APENAS com sim ou não");

        // Fazendo as perguntas
        
        System.out.print("Telefonou para a vítima? ");
        String resp = in.nextLine();

        System.out.print("Esteve no local do crime? ");
        String resp1 = in.nextLine();

        System.out.print("Mora perto da vítima? ");
        String resp2 = in.nextLine();

        System.out.print("Devia para a vítima? ");
        String resp3 = in.nextLine();

        System.out.print("Já trabalhou com a vítima? ");
        String resp4 = in.nextLine();

        // Contagem das respostas positivas
        int respostasPositivas = 0;

        if (resp.equalsIgnoreCase("sim")) {
            respostasPositivas++;
        }
        if (resp1.equalsIgnoreCase("sim")) {
            respostasPositivas++;
        }
        if (resp2.equalsIgnoreCase("sim")) {
            respostasPositivas++;
        }
        if (resp3.equalsIgnoreCase("sim")) {
            respostasPositivas++;
        }
        if (resp4.equalsIgnoreCase("sim")) {
            respostasPositivas++;
        }

 
        
        if (respostasPositivas == 2) {
            System.out.println("Suspeito(a)!");
        } else if (respostasPositivas == 3 || respostasPositivas == 4) {
            System.out.println("Cúmplice!");
        } else if (respostasPositivas == 5) {
            System.out.println("Assassino(a)!");
        } else {
            System.out.println("Inocente!");
        }

    
    }
}
