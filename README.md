import java.util.Scanner;

public class Banco {
    public static void main(String[] args) {
        // Criação do objeto Scanner para leitura de dados do terminal
        Scanner scanner = new Scanner(System.in);
        
        // Solicitação e leitura dos dados do usuário
        System.out.println("Por favor, digite o número da conta:1021");
        int numero = scanner.nextInt();
        scanner.nextLine(); // Consome a linha pendente

        System.out.println("Por favor, digite o número da Agência:067-8");
        String agencia = scanner.nextLine();
        
        System.out.println("Por favor, digite o nome do cliente:MARIO ANDRADE");
        String nomeCliente = scanner.nextLine();
        
        System.out.println("Por favor, digite o saldo:237.48");
        double saldo = scanner.nextDouble();

        // Fechamento do scanner
        scanner.close();

        // Mensagem de confirmação com concatenação de strings
        String mensagem = "Olá ".concat(nomeCliente)
                            .concat(", obrigado por criar uma conta em nosso banco, sua agência é ")
                            .concat(agencia)
                            .concat(", conta ")
                            .concat(String.valueOf(numero))
                            .concat(" e seu saldo ")
                            .concat(String.valueOf(saldo))
                            .concat(" já está disponível para saque.");

        // Exibição da mensagem
        System.out.println(mensagem);
    }
}
