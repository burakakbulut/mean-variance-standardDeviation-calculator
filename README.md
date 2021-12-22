## Mean-Variance-Standard Deviation Calculator

3x3 boyutlarında bir matrisin elemanlarının ortalamasını, varyansını, standart sapmasını, minimum ve maksimum elemanlarını ve  toplamlarını hesaplayan hesapla() adında Numpy dizisi döndüren bir fonksiyon oluşturma.

Fonksiyonun inputu(girdisi) 9 elemanı olan bir dizi olmalıdır. Fonksiyon diziyi 3x3’lük Numpy dizisine çevirmeli ve matrisin ortalamasını, varyansını, standart sapmasını, minimum ve maksimum elemanlarını ve toplamını dictionary olarak return etmelidir.

Fonksiyonun return edeceği dictionary şu şekilde olmalıdır:
```
{
  'mean': [axis1, axis2, flattened],
  'variance': [axis1, axis2, flattened],
  'standard deviation': [axis1, axis2, flattened],
  'max': [axis1, axis2, flattened],
  'min': [axis1, axis2, flattened],
  'sum': [axis1, axis2, flattened]
}
```
Eğer fonksiyonun input dizisinin boyutu 9’dan küçük ise “Dizinin 9 elemanı olmak zorundadır.”  ValueError mesajıyla exception oluşturulmalıdır.
Örneğin hesapla([0,1,2,3,4,5,6,7,8])fonksiyonunun return edeceği dictionary:
```
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  'standard deviation': [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```
