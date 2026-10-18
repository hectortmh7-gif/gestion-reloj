# gestion-reloj
Reloj en JAVa
// Aquí quisé hacer una Clase que representa un reloj.
// Contiene su marca, color y tiempo acumulado.

class Reloj {
    private String marca;
    private String color;
    private int Tiempo;

    // Aquí lo Construí el reloj
    public Reloj(String marca, String color, int Tiempo) {
        this.marca = marca;
        this.color = color;
        this.Tiempo = 0;
    }

    // Agrega segundos al tiempo del reloj
    public void marcar_el_Tiempo(int segundos) {
        Tiempo += segundos;
    }

    // Devuelve el tiempo acumulado
    public int getTiempo() {
        return Tiempo;
    }
}

// Con esto pruebo el reloj
 
public class Main {
    public static void main(String[] args) {

        // Crear un objeto de tipo Reloj
        Reloj miReloj = new Reloj("Casio", "Negro", 0);

        // Utilizar los métodos del objeto
        miReloj.marcar_el_Tiempo(10);
        miReloj.marcar_el_Tiempo(5);

        // Mostrar el resultado
        System.out.println("Tiempo del reloj: "
                           + miReloj.getTiempo()
                           + " segundos");
    }
}
