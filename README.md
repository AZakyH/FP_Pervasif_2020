# FP_Pervasif_2020
Penerapan AODV Teroptimasi pada WSN

ERA-AODV maximum energy residue cluster head:
1. Setup phase
  - setiap node menentukan apakah dirinya akan menjadi CH pada round tersebut dengan cara memilih angka acak dan membandingkannya dengan treshold
  - setiap node yang terpilih menjadi cluster head akan menyebarkan pesan ke tetangganya tentang ke-ch-annya
  - setiap node non-cluster head akan menghitung energy residue mereka terhadap setiap ch disekitarnya.
  - route dengan energy residue tertinggi akan dipilih dan node non-ch akan menentukan CH dengan energy residue tertinggi tersebut sebagai CHnya.
2. Steady phase
  - node non-ch akan mengirimkan data sensornya ke node cluster head pada clusternya.
  - setiap cluster head akan mengagregasi data yang diterima lalu mengirimkan hasil agregasi tersebut ke NAH

### Week-10
1. Installing ns3 and ns2.
2. Testing sample script on both.

### Until Week-14
Mengubah Cluster Head Selection menjadi bergantung pada perhitungan energy.

