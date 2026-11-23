# GameLens Eklentileri

[GameLens](../../../GameLens) için isteğe bağlı parçalar. Bunları elle indirmenize gerek yok:
GameLens'in sol menüsündeki **Eklentiler** sayfası bilgisayarınıza uygun olanı bulur, indirir ve doğrular.

## Ekran kartı hızlandırması (AMD / Vulkan)

Türkçe dublajda konuşmayı ekran kartında tanır (cümle başına ~0,3 sn yerine ~0,05–0,1 sn).
Oyun ekran kartını doldurursa iş kendiliğinden işlemciye kayar.

| Dosya | Boyut | SHA-256 |
|---|---|---|
| `GameLens_Whisper_Vulkan_b5907.zip` | 14,5 MB | `4fcffbbec0bab801e71d6a45f7d84f2c5dd64a2d939e95fcc5b6f8a2236f09c3` |

- [whisper.cpp](https://github.com/ggml-org/whisper.cpp) b5907 (MIT lisansı) resmî kaynak kodundan derlenmiştir
  (Vulkan, Visual Studio 2022, Vulkan SDK 1.4.363.0). Paketin içinde whisper.cpp lisansı ve Microsoft Visual C++
  çalışma kütüphaneleri vardır.
- NVIDIA kartlarda GameLens, whisper.cpp'nin kendi resmî CUDA paketini kullanır; o paket bu depoda değildir.
