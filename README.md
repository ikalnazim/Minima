### Tutorial Minima di VPS
   Menggarap Minima Node via VPS bertujuan agar baterai HP lebih awet.
   Terserah kalian mau garap via VPS atau HP.

   Recommended Ubuntu 20.04

### Open Port
   ufw allow 22 && ufw allow 8080/tcp &&
   ufw allow 9001 && ufw allow 9002 && ufw
   allow 9003 && ufw allow 9004 && ufw
   allow 9005
   ufw enable

### Install Docker
   sudo curl -fsSL https://get.docker.com/ -o get-docker.sh sudo chmod +x 
./get-docker.sh && ./get-docker.sh

### Run Docker
   docker run -d -e minima_mdspassword=123 -e minima_server=true -v 
   ~/minimadocker9001:/home/minima/data -p 9001-9004:9001-9004 --restart 
   unless-stopped --name minima9001 minimaglobal/minima:latest

  Note : 123 Ganti menjadi password kalian (bebas)

### Run Service
   sudo systemctl enable docker.service
   sudo systemctl enable containerd.service

### Buka IP VPS Anda di Browser
   https://YourServerIP:9003/
  
  Pastikan gunakan https:// 
  Jika muncul di Web nya " Your Connection is Not Private " Klik
  Turn on enhanced protection.

### Masukkan Kata Sandi Anda
   Kata Sandi yang dibuat pada command Run Docker yaaaaa

### Klik Incentivized Program

### Paste Incentiv ID yang klean punya yang ada di Akun klean

    Link : https://s.id/1tnxV

### Klik Update

### Done


### Cek Logs
    docker logs minima9001


NOTE : INI AKAN BERAKHIR PADA AKHIR DESEMBER.
