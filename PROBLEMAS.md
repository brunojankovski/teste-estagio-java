public class Imc {
	public static void main(String[] args) {

		Float peso;
		Float altura;
		Float imc;
		
		//tirei o objeto e chamei a classe console direto para ler os dados
		
		

        // Ler a entrada dos dados
		String nome = Console.readString("Informe seu nome: ");
		peso = Console.readFloat("Informe o seu peso: ");  
		altura = Console.readFloat("Informe a sua altura: ");
        // Realizar o cálculo do IMC
		 imc = peso / (altura * altura); // realizei o calculo como deve ser feito

        // Exibir IMC
	      System.out.printf("\n------------------------------"); // exibi a tabela como dito no problema 3
	      System.out.printf("\nAbaixo de 17 - Muito abaixo do peso");
	      System.out.printf("\nEntre 17 e 18,49 -  Abaixo do peso");
	      System.out.printf("\nEntre 18,5 e 24,99 -  Peso Normal");
	      System.out.printf("\nEntre 25 e 29,99 -  Acima do peso");
	      System.out.printf("\nEntre 30 e 34,99 -  Obesidade I");
	      System.out.printf("\nEntre 35 e 39,99 -  Obesidade II (Severa)");
	      System.out.printf("\nAcima de 40 -  Obesidade III (Mórbita)");
	      System.out.printf("\n------------------------------");
	      System.out.printf("\nIMC = %.2f", imc);
	      // mostrei ao usuário o IMC dele somente com 2 casas decimais 
	      System.out.println("\n\n");
        // Exibir situação do usuário
	      // testei a variável IMC em forma de if else e coloquei a situção do usuário
	      if (imc < 17 ) {
	    	  System.out.println("Muito Abaixo do peso");		
	      }else if (imc <= 18.49) {
	    	  System.out.println("Abaixo do peso");	
	      }else if (imc <= 24.99) {
	    	  System.out.println("Peso Normal");	
	      }else if (imc <= 29.99) {
	    	  System.out.println("Acima do peso");
	      }else if (imc <= 34.99) {
	    	  System.out.println("Obesidade I");
	      }else if (imc <= 39.99) {
	    	  System.out.println("Obesidade II (Severa)");
	      }else {
	    	  System.out.println("Obesidade III (Mórbita)");
	      }

	}
}