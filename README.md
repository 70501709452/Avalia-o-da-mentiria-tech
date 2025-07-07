# Avalia-o-da-mentiria-tech

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
{
