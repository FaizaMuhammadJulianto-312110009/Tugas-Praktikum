public class Main {
    public static void main(String[] args) {
        Manager m = new Manager();
        m.setNama("Faiza");
        m.setGajiPokok(5000000);
        m.setTunjangan(2500000);
        m.cetakInfo();
        System.out.println("--------------------------------");
        Programmer p = new Programmer();
        p.setNama("Fahri");
        p.setGajiPokok(6000000);
        p.setBonus(300000);
        p.cetakInfo();
    }
}
