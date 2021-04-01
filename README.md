# Engenheiro de Qualidade de Software Pleno – Teste Prático

1 – Dado que um cliente do banco XPTO deseja realizar um saque de um determinado valor de sua conta bancária. Implemente uma função que permita que o cliente realize o saque de sua conta bancária e em seguida implemente um teste unitário para essa função de saque (Considere aplicar saques positivos e negativos no teste). Considere as classes abaixo para o desenvolvimento do programa.

### Classe cliente
 ```java
 
 public class Cliente {
	
	private String nome;
	private Conta conta;
	
	
	public void setNome(String nome) {
		this.nome = nome;
	}
	
	public String getNome() {
		return this.nome;
	}
	
	public void setConta(Conta conta) {
		this.conta = conta;
	}
	
	public Conta getConta() {
		return this.conta;
	}


}
 
 ```
 
 ### Classe conta
  ```java
 
public class Conta {
	
	
	private int saldo;
	
	public void setSaldo(int saldo) {
		this.saldo = saldo;
	}
	
	public int getSaldo() {
		return this.saldo;
	}

}
 
 ```
 

2 – Realizar a validação dos campos de retorno da api dos correios de acordo com o cep informado onde esses campos não podem estar vazios. 
Considere receber o cep de uma variável de ambiente e utilize a aba “Pre-request script” para construir o request da api. Obs: Para esse teste utilize o Postman.

Endpoint : https://apps.correios.com.br/SigepMasterJPA/AtendeClienteService/AtendeCliente

3 – Realize a automação funcional dos 4 cenários abaixo:

Cenário 1 – Validar especificações do produto
•	Acessar o site https://advantageonlineshopping.com
•	No menu, clicar na opção “Special Offer”
•	Clicar no botão “See offer”
•	Validar que as especificações do produto de acordo com as informações retornadas do banco de automação 

Cenário 2 – Validar alteração de cor do produto no carrinho
•	Acessar o site https://advantageonlineshopping.com
•	No menu, clicar na opção “Special Offer”
•	Clicar no botão “See offer”
•	Alterar a cor do produto de acordo com a cor informada no banco de automação
•	Clicar no botão “Add to cart”
•	Validar que produto foi adicionado ao carrinho com a cor selecionada

Cenário 3 – Remover produto do carrinho de compras
•	Acessar o site https://advantageonlineshopping.com
•	No menu, clicar na opção “Special Offer”
•	Clicar no botão “See offer”
•	Clicar no botão “Add to cart”
•	Clicar no carrinho de compras
•	Remover produto do carrinho de compras
•	Validar que o carrinho de compras está vazio

Cenário 4 – Validar página de checkout
•	Acessar o site https://advantageonlineshopping.com
•	Pesquisar o produto clicando no ícone de lupa (Seguir o nome do produto do banco de automação)
•	Selecionar produto pesquisado
•	Alterar a cor do produto para uma diferente da existente no banco de automação
•	Alterar a quantidade de produtos que deseja comprar
•	Clicar no botão “Add to cart”
•	Acessar a página de checkout
•	Validar que a soma dos preços corresponde ao total apresentado na página de checkout
•	Realizar um update no banco de automação alterar a cor existente no banco para a cor selecionada no teste.


Não esqueça de realizar um commit e push nesse repositório para avaliação do seu projeto.
