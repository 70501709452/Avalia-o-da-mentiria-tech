# Avalia-o-da-mentiria-tech

Claro! Abaixo está um algoritmo em Java que simula um sistema escolar. Ele recebe as 8 notas do aluno (2 por bimestre, totalizando 4 bimestres), calcula:

As médias bimestrais (2 notas por bimestre);

As médias semestrais (2 bimestres por semestre);

E a média final (2 semestres).



---

✅ CÓDIGO EM JAVA

import java.util.Scanner;

public class SistemaEscolar {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        double[] notas = new double[8];
        double[] mediasBimestrais = new double[4];
        double[] mediasSemestrais = new double[2];

        // Entrada das 8 notas
        System.out.println("Digite as 8 notas do aluno (duas por bimestre):");
        for (int i = 0; i < 8; i++) {
            System.out.print("Nota " + (i + 1) + ": ");
            notas[i] = scanner.nextDouble();
        }

        // Cálculo das médias bimestrais
        for (int i = 0; i < 4; i++) {
            mediasBimestrais[i] = (notas[i * 2] + notas[i * 2 + 1]) / 2;
        }

        // Cálculo das médias semestrais
        mediasSemestrais[0] = (mediasBimestrais[0] + mediasBimestrais[1]) / 2;
        mediasSemestrais[1] = (mediasBimestrais[2] + mediasBimestrais[3]) / 2;

        // Cálculo da média final
        double mediaFinal = (mediasSemestrais[0] + mediasSemestrais[1]) / 2;

        // Saída dos resultados
        System.out.println("\n--- RESULTADOS ---");
        for (int i = 0; i < 4; i++) {
            System.out.printf("Média do %dº bimestre: %.2f%n", i + 1, mediasBimestrais[i]);
        }

        System.out.printf("Média do 1º semestre: %.2f%n", mediasSemestrais[0]);
        System.out.printf("Média do 2º semestre: %.2f%n", mediasSemestrais[1]);
        System.out.printf("MÉDIA FINAL: %.2f%n", mediaFinal);

        scanner.close

Claro! Vamos criar um algoritmo em Java que:

1. Recebe uma temperatura em graus Celsius do usuário;


2. Converte essa temperatura para:

Kelvin: K = C + 273.15

"Fel-Wet" (parece ser fictício; como não há fórmula oficial, vou considerar F = C * 1.8 + 50 como uma fórmula genérica para exemplo);



3. Exibe os resultados com mensagens claras.




---

🧠 Suposição:

A escala "Fel-Wet" parece ser fictícia ou um erro de digitação. Se você tiver uma fórmula correta ou desejada, posso corrigir. Aqui vou usar uma fórmula genérica para ilustração.


---

✅ Código Java:

import java.util.Scanner;

public class ConversorTemperatura {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Entrada do usuário
        System.out.print("Digite a temperatura em graus Celsius: ");
        double celsius = scanner.nextDouble();

        // Conversões
        double kelvin = celsius + 273.15;
        double felWet = celsius * 1.8 + 50; // Suposição para "Fel-Wet"

        // Saída dos resultados
        System.out.println("\n--- Conversão de Temperatura ---");
        System.out.printf("Temperatura original: %.2f °C\n", celsius);
        System.out.printf("Temperatura em Kelvin: %.2f K\n", kelvin);
        System.out.printf("Temperatura em Fel-Wet: %.2f FW\n", felWet);

        scanner.close();
    }
}


---

💡 Exemplo de Saída:

Se o usuário digitar 25:

--- Conversão de Temperatura ---
Temperatura original: 25.00 °C
Temperatura em Kelvin: 298.15 K
Temperatura em Fel-Wet: 95.00 FW


---

Se você tiver uma fórmula específica para a escala "Fel-Wet", posso atualizar o algoritmo. Deseja isso?
Claro! Vamos criar um algoritmo em Java que:

1. Recebe uma temperatura em graus Celsius do usuário;


2. Converte essa temperatura para:

Kelvin: K = C + 273.15

"Fel-Wet" (parece ser fictício; como não há fórmula oficial, vou considerar F = C * 1.8 + 50 como uma fórmula genérica para exemplo);



3. Exibe os resultados com mensagens claras.




---

🧠 Suposição:

A escala "Fel-Wet" parece ser fictícia ou um erro de digitação. Se você tiver uma fórmula correta ou desejada, posso corrigir. Aqui vou usar uma fórmula genérica para ilustração.


---

✅ Código Java:

import java.util.Scanner;

public class ConversorTemperatura {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Entrada do usuário
        System.out.print("Digite a temperatura em graus Celsius: ");
        double celsius = scanner.nextDouble();

        // Conversões
        double kelvin = celsius + 273.15;
        double felWet = celsius * 1.8 + 50; // Suposição para "Fel-Wet"

        // Saída dos resultados
        System.out.println("\n--- Conversão de Temperatura ---");
        System.out.printf("Temperatura original: %.2f °C\n", celsius);
        System.out.printf("Temperatura em Kelvin: %.2f K\n", kelvin);
        System.out.printf("Temperatura em Fel-Wet: %.2f FW\n", felWet);

        scanner.close();
    }
}


---


