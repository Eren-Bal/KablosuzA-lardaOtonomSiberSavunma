# 🛡️ Kablosuz Algılayıcı Ağlarda (WSN) Otonom Siber Savunma

Bu proje, WSN'lerin (Wireless Sensor Networks) en büyük zafiyeti olan Fiziksel Katman Sinyal Kesici (Jammer) saldırılarına karşı ağın otonom olarak hayatta kalmasını (Survivability) sağlayan bir simülasyonudur. Dışarıdan hazır bir ağ simülatörü kullanılmamış, tüm fiziksel ve yönlendirme katmanları Python kullanılarak sıfırdan geliştirilmiştir.

---

## 📺 Otonom Savunma Simülasyonu (Canlı Demo)

Aşağıdaki demo videosunda sırasıyla şu iki otonom senaryonun sistem tarafından nasıl yönetildiğini izleyebilirsiniz:
1. **Self-Healing (Öz İyileşme):** Jammer altında pili biten ve ölen düğümlerin tespit edilerek, ağın yeni bir iletişim rotası çizmesi.
2. **Auto-FHSS (Dinamik Frekans Atlama):** PDR (Başarı Oranı) %65'in altına düştüğünde, yapay zeka karar mekanizmasının tüm ağı temiz bir frekansa anında taşıması.

[*(BURAYA TEK VİDEONU SÜRÜKLE BIRAK)*](https://github.com/user-attachments/assets/8402ae0f-f7ee-42d9-bdbd-2e577436032e)

---

## 📸 Simülasyon Arayüzü ve Sistem Durumları

<table align="center">
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ee7c71bd-e358-4e3b-aece-8652bd2106ce" width="100%"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/8f8e6507-1e40-4bbf-b0fd-0c547453dacf" width="100%"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/bb333644-176d-4ad9-b08c-7a2be20b0bad" width="100%"/>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/57c07e0b-0948-42f7-86e8-ab8c41ad0785" width="100%"/>
    </td>
  </tr>
</table>

---

## 🚀 Projenin Temel Metrikleri ve Özellikleri
* **Canlı PDR Grafiği:** Paket başarı oranını matematiksel olarak kanıtlayan canlı radar arayüzü.
* **Canlı Sistem Telemetrisi:** Ağ üzerindeki tüm pil ölümleri, yönlendirmeler ve frekans geçişleri anlık olarak Sistem Terminali (Log) üzerinden takip edilir.
* **Enerji Tüketim Modellemesi:** Jammer altındaki düğümlerin retransmission (tekrar gönderim) çırpınışı sebebiyle pillerini 30 kat daha hızlı tüketmesi matematiksel olarak koda işlenmiştir.

## 🛠️ Kullanılan Teknolojiler
* **Dil:** Python 3
* **Motor:** Pygame (Ağ trafiği ve dinamik görselleştirme)
* **Topoloji:** 16 Düğümlü Çoklu Sıçramalı Örgü (Multi-hop Mesh)
