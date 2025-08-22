# ContaBancariaJava
Montei esse código no intuito de parecer com um sistema de gestão em uma conta bancária utilizando Java.
package ClasseVsMetodos;

```java
public class ContaBancaria {
	
	String titular;
	double saldo;
	
	ContaBancaria(String nomeTitular, double saldoUsuario){
		titular = nomeTitular;
		saldo = saldoUsuario;	
	}
	
	double depositar(double valorDeposito) {
		return saldo += valorDeposito;
	}
	
	double sacar(double valorSaque) {
		return saldo -= valorSaque;
	}
	
	void mostrarSaldo() {
		System.out.printf("Titular: %s%nSaldo: %.2f%n%n", titular, saldo);
	}
}
```java
