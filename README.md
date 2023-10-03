<?php
class CompanyNetlandInvestment {
    private $nama;
    private $cabang;
    private $tahunTerbit;

    public function __construct($nama, $cabang, $tahunTerbit) {
        $this->nama = $nama;
        $this->cabang = $cabang;
        $this->tahunTerbit = $tahunTerbit;

    }

    public function getInfocompany() {
        return "{$this->nama} mempunyai cabang {$this->cabang} dan tahun {$this->tahunTerbit}.";

   }
}
?>

<?php
// Memuat class CompanyNetlandinvestment
require_once 'Company_Netland_Investment.php';

// Membuat beberapa objek CompanyNetlandInvestment,
$company1 = new company("Company Netland Investment", "cabang ke 2", 2019);
$company2 = new company("Company Netland Investment", "cabang ke 3", 2022Company Netland Investment);

// Menampilkan informasi buku di halaman utama
?>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Halaman Utama</title>
</head>
<body>
    <h1>Selamat Datang di Halaman Utama</h1>
    <p><?php echo $company1->getInfocompany(); ?></p>
    <p><?php echo $company2->getInfocompany(); ?></p>
</body>
</html>
