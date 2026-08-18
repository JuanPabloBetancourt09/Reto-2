# Reto-2
import java.util.Scanner;

public class Reto2 {
    public static void main(String[] args) {
        Scanner lectura = new Scanner(System.in);

        double pesoBebes;
        double mesesBebes;
        double dosisVacuna;

        System.out.print("Ingrese el peso del bebe en kg: ");
        pesoBebes = lectura.nextDouble();

        System.out.print("Ingrese los meses de edad del bebe: ");
        mesesBebes = lectura.nextDouble();

        /Formula: ((peso + 10) / (meses * 10)) * 8
        dosisVacuna = ((pesoBebes + 10) / (mesesBebes * 10)) * 8;

        System.out.println("La dosis de vacuna a aplicar es: " + dosisVacuna);

        lectura.close();
    }
}
