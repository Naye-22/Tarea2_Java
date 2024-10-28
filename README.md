# Tarea2_Java
/*Realice un programa que pida 3 numeros y realice la siguiente operacion:
 * (((n1 - n2)^2)/(n3)) + raiz cubica n2 */
package tarea2;
import java.util.Scanner;
public class Tarea_Operaciones {
	public static void main(String[] arg) {
		Scanner teclado = new Scanner (System.in);
		
		double n1, n2, n3, resultado;
		
		System.out.println("Este es un programa que realiza la operacion: ");
		System.out.println("(((n1 - n2)^2)/(n3)) + raiz cubica n2");
		System.out.print("Ingrese el primer numero: ");
		n1 = teclado.nextDouble ();
		System.out.print("Ingrese el segundo numero: ");
		n2 = teclado.nextDouble ();
		System.out.print("Ingrese el tercer numero: ");
		n3 = teclado.nextDouble ();
		
		resultado = ((Math.pow((n1-n2), 2))/n3) + Math.cbrt(n2);
		
		System.out.print("El resultado de esta operacion es: "+resultado);
	}
}
