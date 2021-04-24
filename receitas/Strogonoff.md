Strogonoff de Frango

**Negrito**

bla blab label


package pesqorientacao;


public class PqesBinariaAula {
    public static void main(String[] args) {
        System.out.println("Pesquisa Binaria");

        int[] numeros = {4,5,7,7,9,12,15,19,25};

        int inicio = 0;
        int meio = 0;
        int fim = numeros.length - 1;

        // o algotirmo da pesquisa binária começa aqui 
        while(inicio <= fim){
            meio = (fim + inicio) / 2;

            System.out.println("Inicio: " + numeros[inicio] + " - Meio: " + numeros[meio] + " - Fim: " + numeros[fim]);
            System.out.println("Inicios: " + inicio + " - Meio: " + meio + "- Fim: " + fim);

            if(numeros[meio] == 13){
                System.out.println("Encontrou o numero 13 na posição " + inicio);
                break;
            }

            if(numeros[meio] < 13){
                inicio = meio + 1;
            } else {
                fim = meio - 1;
            }
        }
        //e terminar aqui, não é necessário ter os Print

        if(inicio > fim){
            System.out.println("Não encontrou o numero 13");
        }
    }

}
