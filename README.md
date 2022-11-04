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

public class Pegawai {
    private String nama;
    private double gajiPokok;

    public void setNama(String n) {
        nama = n;
    }

    public String getNama() {
        return nama;
    }

    public void setGajiPokok(double g) {
        gajiPokok = g;
    }

    public double getGajiPokok() {
        return gajiPokok;
    }

    public void cetakInfo() {
        System.out.println("Nama Pegawai : "+nama);
        System.out.println("Gaji Pokok : "+gajiPokok);
    }
}

public class Manager extends Pegawai {
    private double tunjangan;

    public void setTunjangan(double t) {
        tunjangan = t;
    }

    public double getTunjangan() {
        return tunjangan;
    }

    public void cetakInfo() {
        super.cetakInfo();
        System.out.println("Tunjangan : "+tunjangan);
    }

    public void cetakTunjangan() {
        System.out.println("Tunjangan : "+tunjangan);
    }
}

class Programmer extends Pegawai {
    private double bonus;

    public void setBonus(double b) {
        bonus = b;
    }

    public double getBonus() {
        return bonus;
    }

    public void cetakInfo() {
        super.cetakInfo();
        System.out.println("Bonus : "+bonus);
    }

    public void cetakBonus() {
        System.out.println("Bonus : "+bonus);
    }
}
