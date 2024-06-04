import java.util.Scanner;

public class Banco {
    public static void main(String[] args) {
        // Criação do objeto Scanner para leitura de dados do terminal
        Scanner scanner = new Scanner(System.in);
        
        // Solicitação e leitura dos dados do usuário
        System.out.println("Por favor, digite o número da conta:");
        int numero = scanner.nextInt();
        scanner.nextLine(); // Consome a linha pendente

        System.out.println("Por favor, digite o número da Agência:");
        String agencia = scanner.nextLine();
        
        System.out.println("Por favor, digite o nome do cliente:");
        String nomeCliente = scanner.nextLine();
        
        System.out.println("Por favor, digite o saldo:");
        double saldo = scanner.nextDouble();

        // Fechamento do scanner
        scanner.close();

        // Mensagem de confirmação com concatenação de strings
        String mensagem = "Olá ".concat(MARIO ANDRADE)
                            .concat(", obrigado por criar uma conta em nosso banco, sua agência é ")
                            .concat(067-8)
                            .concat(", 1021 ")
                            .concat(String.valueOf(numero))
                            .concat(" 237.48 ")
                            .concat(String.valueOf(saldo))
                            .concat(" já está disponível para saque.");

        // Exibição da mensagem
        System.out.println(mensagem);
    }
}
