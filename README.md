# Mengecilkan File PDF
Ini adalah code command line untuk mengecilkan file PDF. Ini saya gunakan di Windows 11. 

Langkah-langkahnya

1. Buka Windows Powershell sebagai Administrator

2. Install ghostscript dengan perintah
```
choco install ghostscript 
```
3. Buka kembali window command prompt dengan menekan tombol Windows + r

4. ketik cmd kemudian enter
```
cmd
```
5. Setelah window command line terbuka. kamu bisa memasukkan perintah untuk mengecilkan file

6. Perintah Untuk mengecilkan file dengan resolusi 144
```
gswin64c -dNOPAUSE -dQUIET -dBATCH -sDEVICE=pdfwrite -dPDFSETTINGS=/ebook -dColorImageDownsampleType=/Bicubic -dColorImageResolution=144 -dGrayImageDownsampleType=/Bicubic -dGrayImageResolution=144 -dMonoImageDownsampleType=/Bicubic -dMonoImageResolution=144  -o out.pdf file.pdf
```
7. Perintah untuk mengecilkan file dengan resolusi 72. Ini adalah file yang sangat kecil
```
gswin64c -dNOPAUSE -dQUIET -dBATCH -sDEVICE=pdfwrite -dPDFSETTINGS=/ebook -dColorImageDownsampleType=/Bicubic -dColorImageResolution=72 -dGrayImageDownsampleType=/Bicubic -dGrayImageResolution=72 -dMonoImageDownsampleType=/Bicubic -dMonoImageResolution=72  -o out.pdf file.pdf
```
8. Keterangan tambahan 

out.pdf adalah hasil pdf yang TELAH DIKECILKAN
file.pdf adalah file pdf yang AKAN DIKECILKAN

untuk nama file pdf yang akan dikecilkan JANGAN ADA SPASI

