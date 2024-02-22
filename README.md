# quadradoperfeito

package verificaquadradoperfeito;

import java.util.Scanner;

public class VerificaQuadradoPerfeito {

    
    
    public static void main(String[] args) {
       
    Scanner Scanner = new Scanner (System.in);
//solicita ao usuario que insira um número

        System.out.println("DIGITE UM NÚMERO INTEIRO POSITIVO:");
        int numero=Scanner.nextInt();
        //verifica se o número é um quadrado perfeito
        
        boolean ehquadradoperfeito= false;
        if(numero >=0){
            int raiz = (int) Math.sqrt(numero);
            ehquadradoperfeito = raiz*raiz== numero;
        }
        // exibe o resultado
        
        if (ehquadradoperfeito){
            System.out.println(numero + " é um quadrado perfeito.");
        }else{
            System.out.println(numero + "não é um quadrado perfeito.");
            }
        //fecha o Scanner
        Scanner.close();
        
        
    }
    
}
