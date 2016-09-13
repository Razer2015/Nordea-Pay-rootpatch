# Nordea Pay - Root testien poisto
<h2>1. Lue ensiksi nämä ohjeet</h2>
https://github.com/Razer2015/NordeaTunnusluvut_Patched
<br><br>
<h4>Pikaisesti komentoja</h4>
<p>Purku:</p>
```txt
apktool.bat d -r fi.nordea.mep.npay-1.1.1-16.apk -o nordea_pay_111_nores
```
<p>Pakkaus:</p>
```txt
apktool.bat b -r nordea_pay_111_nores -o Nordea_Pay_1.1.1_patched.apk
```

<h4>2. Muokkaus</h4>
<p>Polku:</p>
```txt
smali\arl.smali
```
Muokkaus 1:
```txt
Lisää rivi: move v0, v1
```
![1_add](https://cloud.githubusercontent.com/assets/10619845/18481163/ddcb9bca-79e3-11e6-9d2d-f1fc639307d1.png)

Muokkaus 2:
```txt
Vaihda: const/4 v0, 0x1 -> const/4 v0, 0x0
```
![2_change](https://cloud.githubusercontent.com/assets/10619845/18481248/3b36633a-79e4-11e6-9f18-9ef3dba7ea6d.png)

Muokkaus 3:
```txt
Vaihda: move v0, v1 -> move v0, v2
```
![3_change](https://cloud.githubusercontent.com/assets/10619845/18481459/f736b2b0-79e4-11e6-8f8c-ffc0ff02b366.png)

Muokkaus 4:
```txt
Lisää rivi: move v0, v1
```
![4_add](https://cloud.githubusercontent.com/assets/10619845/18481466/faaf5a0a-79e4-11e6-9cd6-94af967df208.png)

Muokkaus 5 ja 6:
```txt
Vaihda 5: const/4 v0, 0x1 -> const/4 v0, 0x0
Vaihda 6: const/4 v0, 0x0 -> const/4 v0, 0x1
```
![5_6_change](https://cloud.githubusercontent.com/assets/10619845/18481472/fae2762e-79e4-11e6-8465-92020aa40e9c.png)

Muokkaus 7:
```txt
Lisää rivi: move v0, v1
```
![7_add](https://cloud.githubusercontent.com/assets/10619845/18481470/fadea166-79e4-11e6-8eec-aea8d612cd32.png)

Muokkaus 8:
```txt
Vaihda: const/4 v0, 0x1 -> const/4 v0, 0x0
```
![8_change](https://cloud.githubusercontent.com/assets/10619845/18481467/fadd4032-79e4-11e6-8dbb-983de4e02220.png)
Muokkaus 9:
```txt
Vaihda: move v0, v1 -> move v0, v2
```
![9_change](https://cloud.githubusercontent.com/assets/10619845/18481468/fadd435c-79e4-11e6-93a3-50741591e377.png)

Muokkaus 4:
```txt
Lisää rivi: move v0, v1
```
![10_add](https://cloud.githubusercontent.com/assets/10619845/18481469/fadd3b0a-79e4-11e6-933a-40d4c37e450f.png)

Muokkaus 11 ja 12:
```txt
Vaihda 11: const/4 v0, 0x1 -> const/4 v0, 0x0
Vaihda 12: const/4 v0, 0x0 -> const/4 v0, 0x1
```
![11_12_change](https://cloud.githubusercontent.com/assets/10619845/18481471/fae0ff06-79e4-11e6-8b23-c2948869ecbd.png)
