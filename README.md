# C ile Uçak Kalkış Zamanlama Simülasyonu
*(Airplane Takeoff Scheduling Simulation in C)*

---

### Açıklama / Description

**🇹🇷 Türkçe:**
Bu proje, iki pisti olan bir havaalanındaki uçak kalkış operasyonlarını simüle eden bir C konsol uygulamasıdır. Program, kullanıcıdan aldığı uçak listesini ve minimum kalkış aralığı süresini kullanarak, uçakları en verimli şekilde iki pistten birine atar. Bir uçağın kalkışı minimum süreyi ihlal ediyorsa, program otomatik olarak bir gecikme uygular ve her pist için ortalama gecikme süresini hesaplayarak raporlar.

**🇬🇧 English:**
This project is a C console application that simulates airplane takeoff operations at an airport with two runways. Using a list of planes and a minimum separation time provided by the user, the program assigns planes to one of the two runways in the most efficient manner. If a plane's takeoff violates the minimum time rule, the program automatically applies a delay and reports the average delay time for each runway.

---

### Önemli Not / Important Note
**🇹🇷 Türkçe:** Bu algoritma, kullanıcı tarafından girilen uçakların **talep edilen kalkış saatlerine göre küçükten büyüğe sıralı olduğu** varsayımına dayanmaktadır. Lütfen verileri bu şekilde giriniz.

**🇬🇧 English:** This algorithm assumes that the planes entered by the user are **sorted in ascending order based on their requested takeoff times**. Please ensure the data is entered accordingly.

---

### Kullanılan Teknolojiler / Technologies Used

*   **C** (Programlama Dili)
*   `stdio.h` (C Standart Girdi/Çıktı Kütüphanesi)

---

### Kurulum ve Çalıştırma / Installation and Usage

Projeyi yerel makinenizde derlemek ve çalıştırmak için aşağıdaki adımları izleyin.

1.  **Depoyu klonlayın:**
    ```bash
    git clone https://github.com/kullanici-adiniz/c-airport-takeoff-scheduler.git
    ```

2.  **Proje dizinine gidin:**
    ```bash
    cd c-airport-takeoff-scheduler
    ```

3.  **Kodu derleyin (GCC veya uyumlu bir C derleyicisi ile):**
    ```bash
    gcc main.c -o takeoff_scheduler
    ```

4.  **Programı çalıştırın:**
    ```bash
    ./takeoff_scheduler
    ```

5.  **Program sizden gerekli bilgileri isteyecektir. Örnek bir çalışma:**
    ```
    Ucak sayisini giriniz: 5
    Ucaklarin minimum kac dakika ara ile kalkacagini giriniz: 10
    1. ucagin numarasini giriniz: 101
    1. ucagin talep edilen kalkis saatini giriniz: 1000
    2. ucagin numarasini giriniz: 102
    2. ucagin talep edilen kalkis saatini giriniz: 1002
    3. ucagin numarasini giriniz: 103
    3. ucagin talep edilen kalkis saatini giriniz: 1008
    4. ucagin numarasini giriniz: 104
    4. ucagin talep edilen kalkis saatini giriniz: 1011
    5. ucagin numarasini giriniz: 105
    5. ucagin talep edilen kalkis saatini giriniz: 1015
    ```
    *(Bu girdilere göre program ilgili pist atamalarını ve gecikme hesaplamalarını yapıp sonucu yazdıracaktır.)*

---

### Öğrenilenler & Amaç / What I Learned & Purpose

Bu proje, temel C programlama yeteneklerini kullanarak daha karmaşık bir simülasyon ve optimizasyon problemini çözmeyi amaçlamaktadır. Projenin ana öğrenme hedefleri:

*   Gerçek dünya problem senaryosunu (zamanlama/scheduling) algoritmik düşünceyle koda aktarma.
*   "Açgözlü Algoritma" (Greedy Algorithm) mantığını anlama ve basit bir seviyede uygulama.
*   Paralel diziler (uçak numarası ve zamanı gibi birbiriyle ilişkili verileri ayrı dizilerde tutma) kullanarak veri yönetimi.
*   Karmaşık `if-else if-else` yapıları ile çoklu koşullara dayalı karar mekanizmaları oluşturma.
*   Simülasyon sonuçlarını (toplam gecikme, ortalama gecikme) takip etmek ve raporlamak için sayaç ve toplayıcı değişkenler kullanma.