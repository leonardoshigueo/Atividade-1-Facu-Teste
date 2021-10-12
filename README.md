import java.util.Scanner;

class Main {
  public static void main(String[] args) {
    char genero;
    float altura, peso;
    Scanner leitura = new Scanner (System.in);
    System.out.print("Insira o seu gênero (M ou F): ");
    genero = leitura.nextLine().toUpperCase().charAt(0);
    System.out.print("Insira agora a sua altura: ");
    altura = leitura.nextFloat();
    if ( (genero !='m') && (genero !='M') && (genero !='f') && (genero !='F') ) System.out.print("Gênero inválido");
    else if ( genero=='M' ) {
      peso = ((float)72.7 * altura) - 58;
      System.out.printf("O seu peso ideal é de %.2f", peso);
      }
    else if ( genero=='F' ) {
      peso = ((float)62.1 * altura) - (float)44.7;
      System.out.printf("O seu peso ideal é de %.2f", peso);
      }
    }
  }
