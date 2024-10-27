# praktikum4
# bangundatar.java
        public abstract class BangunDatar {
    public abstract float luas();
    public abstract float keliling();
    }

  ![bangundatar](https://github.com/user-attachments/assets/879868de-cd9d-4c57-ba0a-ccab91278788)

# lingkaran.java
    public class Lingkaran extends BangunDatar {
    private int r;

    public Lingkaran(int r) {
        this.r = r;
    }

    @Override
    public float luas() {
        return (float) (Math.PI * r * r);
    }

    @Override
    public float keliling() {
        return (float) (2 * Math.PI * r);
    }
    }

 ![lingkaran](https://github.com/user-attachments/assets/3c1a8c0d-b50e-4ed5-bc50-63d24352de48)

# segitiga.java
    public class Segitiga extends BangunDatar {
    private int alas;
    private int tinggi;

    public Segitiga(int alas, int tinggi) {
        this.alas = alas;
        this.tinggi = tinggi;
    }

    @Override
    public float luas() {
        return (float) (0.5 * alas * tinggi);
    }

    @Override
    public float keliling() {
        // Asumsikan ini adalah segitiga sama sisi untuk memudahkan
        return 3 * alas;
    }
    }
![segitiga](https://github.com/user-attachments/assets/cb432ca7-6341-41da-bb7e-3e1cdac31178)

    
# persegi.java
    public class Persegi extends BangunDatar {
    private int sisi;

    public Persegi(int sisi) {
        this.sisi = sisi;
    }

    @Override
    public float luas() {
        return sisi * sisi;
    }

    @Override
    public float keliling() {
        return 4 * sisi;
    }
    }

![persegi](https://github.com/user-attachments/assets/8d4b1fbd-7ec6-4fd8-955f-688fef1e17ae)

# utama.java
    public class Utama {
    public static void main(String[] args) {
        Lingkaran lingkaran = new Lingkaran(7);
        Segitiga segitiga = new Segitiga(5, 10);
        Persegi persegi = new Persegi(4);

        System.out.println("Luas Lingkaran: " + lingkaran.luas());
        System.out.println("Keliling Lingkaran: " + lingkaran.keliling());

        System.out.println("Luas Segitiga: " + segitiga.luas());
        System.out.println("Keliling Segitiga: " + segitiga.keliling());

        System.out.println("Luas Persegi: " + persegi.luas());
        System.out.println("Keliling Persegi: " + persegi.keliling());
    }
    }
![utama](https://github.com/user-attachments/assets/7917a38e-f96c-402c-bcba-121f93b2d985)

# output
![image](https://github.com/user-attachments/assets/b99697bd-c683-4e39-93ed-6a832ae0cb9b)


