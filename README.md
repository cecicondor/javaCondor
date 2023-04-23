// no primeiro pacote criei a Conta

package modelos;
// o método void é quando não queremos que retorne valor algum
public class Conta {
	
	float saldo;
	String conta; // essa variável servirá para o programa inteiro
	
	public Conta (String conta) {
		saldo = 0;
		this.conta = conta;
	}
	public void depositar (float depositar) {
		saldo += depositar;
	}
	
	public void sacar (float sacar) {
		if (sacar > saldo){
			System.out.println("erro");
		}
		else {
			saldo -= sacar;	
		}
	}
	
	public String toString () {
		return "saldo:" +saldo;
	}
}



