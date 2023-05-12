# Scanner

import java.util.Scanner;

public class MediaAritmetica {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int quantidade;
        double soma = 0;

        System.out.print("Digite a quantidade de números a serem lidos: ");
        quantidade = sc.nextInt();

        int[] numeros = new int[quantidade];

        for (int i = 0; i < quantidade; i++) {
            System.out.print("Digite o " + (i+1) + "º número: ");
            numeros[i] = sc.nextInt();
            soma += numeros[i];
        }

        double media = soma / quantidade;

        System.out.println("A média aritmética é: " + media);
    }
}
