# Matris Döndürme Hakkında

Bu projede, iki boyutlu ve üç boyutlu uzayda matris döndürme işlemleri hakkında temel bilgi verilmekte ve bunların kullanım alanları anlatılmaktadır.

## Matris Döndürme Nedir?

Matris döndürme, bir matrisi (özellikle görüntü veya vektörlerle temsil edilen veriler) belirli bir açı etrafında döndürme işlemidir. Bu işlem, görüntü işleme, bilgisayar grafikleri, robotik ve 3D modelleme gibi alanlarda sıkça kullanılır. Matris döndürme, iki boyutlu veya üç boyutlu bir vektörü ya da görüntüyü uzayda belirli bir açı etrafında çevirmek için geometrik dönüşümlerde uygulanır.

### 2D (İki Boyutlu) Matris Döndürme

İki boyutlu bir vektörü veya noktayı orijine göre döndürmek için kullanılan döndürme matrisi şu şekildedir:

R(θ) = | cos(θ) -sin(θ) | | sin(θ) cos(θ) |


Burada `θ`, döndürme açısını temsil eder. Bu matris, bir vektörü ya da görüntüdeki noktaları saat yönünde veya saat yönünün tersine döndürmek için kullanılır.

Bir noktayı `θ` açısı kadar döndürmek için yeni koordinatlar şu şekilde hesaplanır:

x' = x * cos(θ) - y * sin(θ) y' = x * sin(θ) + y * cos(θ)


### 3D (Üç Boyutlu) Matris Döndürme

Üç boyutlu uzayda döndürme işlemi daha karmaşıktır ve X, Y, Z eksenleri etrafında ayrı ayrı döndürme yapılır. Örneğin, Z ekseni etrafında döndürme şu şekildedir:

Rz(θ) = | cos(θ) -sin(θ) 0 | | sin(θ) cos(θ) 0 | | 0 0 1 |


X ve Y eksenleri etrafında da benzer döndürme matrisleri kullanılmaktadır.

## Kullanım Alanları

- **Görüntü İşleme:** Bir görüntüyü belirli bir açı etrafında döndürmek için kullanılır (örneğin, bir fotoğrafı 90 derece döndürmek).
- **Bilgisayar Grafikleri:** 3D modelleme ve animasyonlarda nesneleri döndürmek için kullanılır.
- **Robotik:** Robot kolu gibi cihazların hareketlerini modellemek için kullanılır.
- **Fizik:** Uzaydaki cisimlerin yönelimi ve hareketlerini hesaplamak için kullanılır.
