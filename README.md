# AplikasiPenambahanDuaAngka
 


 Nama   : Zainal Abidin 


 NPM    : 2210010087


 Kelas	: 5B NonReg Banjarmasin


 Matkul : Pemrograman Berbasis Objek 2

1. saya menggunakan "JFrameForm" sebagai tampilan utama aplikasi

2. pada JFrameForm saya menambahkan komponen GUI Seperti
-"JPanel" untuk menempatkan komponen
-"JLabel" untuk 'Angka Pertama',Dan 'Angka Kedua' serta 'Hasil'
-"JTextField" untuk memasukkan 'Angka pertama','Angka Kedua',dan 'Hasil'
-"JButton Untuk Tombol 'Tambah','Hapus',dan'Keluar'.
3. Koding:

-MEMASUKKAN KODING TAMBAH

 Disini saya menambahkan tombol "Tambah" 
 Dengan kode di bawah ini:


  private void jButton1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
try {
    int angka1 = Integer.parseInt(jTextField1.getText());
    int angka2 = Integer.parseInt(jTextField2.getText());
    int hasil = angka1 + angka2;
    jTextFieldHasil.setText(Integer.toString(hasil));
} catch (NumberFormatException e) {
    JOptionPane.showMessageDialog(this, "Masukkan angka yang valid", "Error", JOptionPane.ERROR_MESSAGE);
}


-MEMASUKKAN KODING HAPUS 


Disini Saya menambahkan tombol " Hapus "
Dengan kode di bawah ini:


  private void jButton2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
jTextField1.setText("");
jTextField2.setText("");
jTextFieldHasil.setText("");
jTextField1.requestFocus();  // Mengarahkan fokus kembali ke JTextField pertama
        // TODO add your handling code here:
    }


-MEMASUKKAN KODING KELUAR


 Disini Saya menambahkan " Tombol Keluar "
 Dengan Kode Di bawah ini:

 
    private void jButton3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
System.exit(0);
        // TODO add your handling code here:
    }    
 
