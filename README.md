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
package ClasseVsMetodos;

public class ContaBancariaTeste {
	public static void main(String[] args) {
		
		ContaBancaria conta1 = new ContaBancaria("Gabriel Silva Moraes",21.58);
		
		conta1.mostrarSaldo();
		conta1.depositar(40.00);
		conta1.mostrarSaldo();
		conta1.sacar(15.50);
		conta1.mostrarSaldo();
	}
}
```
