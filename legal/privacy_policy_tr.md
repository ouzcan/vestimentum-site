---
layout: legal
title: Gizlilik Politikası
description: Vestimentum — KVKK uyumlu Gizlilik Politikası
permalink: /legal/privacy_policy_tr/
lang: tr
---
# Gizlilik Politikası

**Yürürlük tarihi:** 2026-05-25
**Son güncelleme:** 2026-05-25

Bu Gizlilik Politikası, Vestimentum mobil uygulamasının ("**Uygulama**",
"**Vestimentum**") kişisel verilerinizi nasıl topladığını, kullandığını,
paylaştığını ve koruduğunu açıklar.

Vestimentum, Oğuzcan Özüpek tarafından geliştirilmektedir ("**biz**",
"**bize**"). İleride şirketleşme durumunda bu Politika, ilgili tüzel
kişilik adına güncellenecektir.

İletişim için: **privacy@vestimentum.app**

---

## 1. Kapsam

Bu Politika; Vestimentum mobil uygulamasını kullandığınızda topladığımız
tüm kişisel verileri kapsar. Uygulama dışındaki üçüncü taraf hizmetlere
(Cloudinary, Firebase, Anthropic, Open-Meteo vb.) gönderilen veriler
için, ilgili üçüncü tarafların kendi gizlilik politikaları da geçerlidir
(bkz. Bölüm 4).

Bu Politikayı kabul etmiyorsanız Uygulamayı kullanmayınız.

---

## 2. Topladığımız Veriler

### 2.1 Hesap Verileri
- **Kimlik bilgileri:** E-posta adresi (Firebase Authentication
  aracılığıyla); Google ile giriş yaptıysanız Google hesabınızın e-posta
  ve adı; misafir girişi yaptıysanız sentetik bir tanımlayıcı.
- **Profil:** İsim (isteğe bağlı), doğum tarihi (isteğe bağlı — burç
  özelliği için), cinsiyet (isteğe bağlı), avatar fotoğrafı (isteğe
  bağlı), dil tercihi, stil tercihleri.
- **Konum:** Yaklaşık konum (enlem/boylam). GPS ile alınır VEYA
  uygulama içindeki şehir listesinden seçilir. Hava durumu sorgusu
  için kullanılır. Hassas/kesin konum **toplamıyoruz**.

### 2.2 Gardırop Verileri
- Yüklediğiniz kıyafet fotoğrafları.
- Yapay zekanın bu fotoğraflardan çıkardığı meta veriler: kategori
  (üst/alt/dış/ayakkabı/aksesuar), renk, materyal tahmini, formalite
  skoru, stil etiketleri, sezon etiketleri.
- Kıyafetlere verdiğiniz isim, notlar, giyildiği tarihler.

### 2.3 Kullanım Verileri
- Aldığınız kombin önerileri ve bu önerilerin meta verileri (hava
  durumu, ruh hali, durum, burç bağlamı).
- Kombin geçmişi: hangi kombinleri kaydettiniz, giydiniz, paylaştınız.
- Discover akışındaki paylaşımlarınız: kombin görselleri (gerçek
  fotoğraflar değil — soyut çizimler), başlıklar, beğeniler.
- Abonelik durumu (Free / Vestimentum+) ve geçmişi.

### 2.4 Teknik Veriler
- **Çökme raporları:** Sentry üzerinden anonim cihaz bilgisi, hata
  yığını (stack trace). PII içermez. Yalnızca `SENTRY_DSN`
  yapılandırıldığında aktiftir.
- **IP adresi:** Firebase Authentication doğrulama sırasında geçici
  olarak görür; biz kalıcı olarak saklamayız.
- **Cihaz bilgisi:** Uygulama sürümü, işletim sistemi sürümü (örn.
  Android 14), cihaz modeli (yalnızca çökme raporlarında).

### 2.5 Toplamadığımız Veriler
- **Davranışsal takip:** Reklam tanımlayıcıları, çapraz uygulama
  takibi, tarama geçmişi → yok.
- **Hassas veriler:** Sağlık, biyometrik, finansal hesap numaraları,
  siyasi/dini görüşler, cinsel yönelim, etnik köken → yok.
- **Hassas konum:** Sokak seviyesi GPS verisi → toplanmıyor.
- **Mesajlaşma içeriği:** Şu an yok (ilerleyen sürümlerde yorumlar
  eklendiğinde bu bölüm güncellenecek).

---

## 3. Verileri Nasıl Kullanıyoruz

Topladığımız verileri yalnızca aşağıdaki amaçlarla kullanırız:

| Amaç | Yasal Dayanak (KVKK m.5 / GDPR m.6) |
|---|---|
| Hesabınızı oluşturmak ve yönetmek | Sözleşmenin ifası |
| Yapay zeka kombin önerileri üretmek | Sözleşmenin ifası |
| Hava durumuna uygun öneri için konumunuzu sorgulamak | Sözleşmenin ifası + meşru menfaat |
| Burç temelli öneri (opt-in) | Açık rıza (sadece premium kullanıcı toggle açtıysa) |
| Discover akışında paylaşımlarınızı diğer kullanıcılara göstermek | Açık rıza (paylaş tuşuna bastığınızda) |
| Uygulama hatalarını çözmek (Sentry) | Meşru menfaat |
| Abonelik faturalandırma kaydı | Sözleşmenin ifası + yasal yükümlülük |
| KVKK/GDPR yükümlülüklerimizi yerine getirmek (silme talepleri vb.) | Yasal yükümlülük |

**Yapmadıklarımız:**
- Verilerinizi reklam amaçlı satmıyoruz.
- Davranışınızı reklam ağlarıyla paylaşmıyoruz.
- Verilerinizi profil çıkarma (profiling) amacıyla işlemiyoruz.
- E-posta ile pazarlama bültenleri göndermiyoruz (yalnızca işlemsel
  bildirimler: hesap güvenliği, abonelik durumu vb.).

---

## 4. Üçüncü Taraf Hizmetler

Vestimentum'un çalışması için bazı veriler aşağıdaki hizmet
sağlayıcılarına aktarılır. Her birinin verilerinizi kendi gizlilik
politikalarına göre işlediğini unutmayın.

### 4.1 Firebase (Google LLC) — Kimlik Doğrulama
- **Aktarılan veri:** E-posta, parola hash, oturum tokenları, IP
  (geçici).
- **Konum:** ABD veri merkezleri (Standard Contractual Clauses
  uygulanır).
- **Gizlilik politikası:** https://firebase.google.com/support/privacy

### 4.2 Cloudinary (Cloudinary Ltd.) — Görsel Barındırma
- **Aktarılan veri:** Kıyafet ve avatar fotoğraflarınız, oluşturulan
  küçük resimler.
- **Konum:** ABD/AB veri merkezleri.
- **Gizlilik politikası:** https://cloudinary.com/privacy

### 4.3 Anthropic (Anthropic PBC) — Yapay Zeka İşleme (Claude)
- **Aktarılan veri:** Kıyafet fotoğraflarınız (sınıflandırma için),
  kombin önerisi bağlamı (hava durumu, ruh hali, gardırop özetleri).
- **Konum:** ABD veri merkezleri.
- **Önemli:** Anthropic, API çağrıları üzerinden gelen verileri model
  eğitimi için kullanmaz.
- **Gizlilik politikası:** https://www.anthropic.com/legal/privacy

### 4.4 remove.bg (Kaleido AI GmbH) — Arka Plan Kaldırma
- **Aktarılan veri:** Yüklediğiniz orijinal kıyafet fotoğrafı (geçici
  işleme için).
- **Konum:** AB.
- **Saklama:** Fotoğraflar işleme sonrası remove.bg tarafından silinir
  (kendi politikaları uyarınca).
- **Gizlilik politikası:** https://www.remove.bg/privacy

### 4.5 Open-Meteo — Hava Durumu Verisi
- **Aktarılan veri:** Yalnızca enlem/boylam koordinatları. Hiçbir
  kişisel tanımlayıcı gönderilmez.
- **Konum:** Almanya.
- **Gizlilik politikası:** https://open-meteo.com/en/terms

### 4.6 Sentry (Functional Software, Inc.) — Çökme Raporlaması
- **Aktarılan veri:** Hata yığınları, cihaz türü, uygulama sürümü.
  PII gönderilmez (`sendDefaultPii=false` zorla ayarlıdır).
- **Konum:** ABD/AB.
- **Yalnızca prodüksiyon yapılandırmasında aktiftir.**
- **Gizlilik politikası:** https://sentry.io/privacy

### 4.7 Uygulama Mağazaları

#### 4.7.1 Apple App Store (Apple Inc.)
- **Aktarılan veri:** Abonelik kimlik bilgisi (anonim purchase
  token), fatura kayıtları, IP adresi, Apple ID (kullanıcı tarafı;
  biz bu kimliği görmeyiz).
- **Konum:** ABD/Avrupa veri merkezleri (Apple kendi politikası).
- **Gizlilik politikası:** https://www.apple.com/legal/privacy/

#### 4.7.2 Google Play (Google LLC)
- **Aktarılan veri:** Abonelik kimlik bilgisi (anonim purchase
  token), fatura kayıtları, IP adresi, Google Play hesabı
  (kullanıcı tarafı; biz bu kimliği görmeyiz).
- **Konum:** Küresel veri merkezleri.
- **Gizlilik politikası:** https://policies.google.com/privacy

---

## 5. Verilerin Saklanma Süresi

- **Aktif hesap verileri:** Hesabınızı silene kadar saklanır.
- **Hesap silindiğinde:** Sunucu tarafında 30 gün içinde tüm kişisel
  veriler kalıcı olarak silinir. Veritabanı tetiği "silme" tuşuna
  basıldığında anında çalışır; yedeklemelerden silme 30 günü
  bulabilir.
- **Cloudinary fotoğrafları:** Hesabınızı sildiğinizde, profil
  fotoğrafınız ve giysi görselleriniz dahil tüm Cloudinary varlıkları
  en geç 30 gün içinde silinir.
- **Loglar (Sentry / sunucu logları):** 90 gün sonra otomatik silinir.
- **Yasal saklama yükümlülüğü:** Faturalandırma kayıtları, yasal
  zorunluluk gereği 10 yıla kadar saklanabilir (Türk Vergi Usul Kanunu).

---

## 6. Verilerin Saklandığı Yer & Uluslararası Aktarım

Vestimentum prodüksiyon altyapısı henüz yayında değildir; üretim
ortamına geçildiğinde sunucular **AB veri merkezlerinde**
(Fly.io veya Railway'in AB bölgesi) barındırılacaktır. Bazı üçüncü
taraf hizmetler (Firebase, Anthropic) verileri **ABD'de** işler.
Bu aktarımlar **Standart Sözleşme Maddeleri (SCC)** kapsamında
yapılır; GDPR Bölüm 5 ve KVKK 9. madde gerekliliklerine uyulur.

---

## 7. Haklarınız

### 7.1 KVKK Kapsamında (Türkiye Vatandaşları)
KVKK 11. madde uyarınca, aşağıdaki haklara sahipsiniz:

- Kişisel verilerinizin işlenip işlenmediğini öğrenme
- İşlendiyse buna ilişkin bilgi talep etme
- İşleme amacını ve verilerin amacına uygun kullanılıp kullanılmadığını
  öğrenme
- Yurt içinde / yurt dışında verilerin aktarıldığı üçüncü kişileri bilme
- Eksik / yanlış verilerin düzeltilmesini isteme
- Verilerin silinmesini veya yok edilmesini isteme
- Düzeltme / silme işleminin verinin aktarıldığı üçüncü kişilere
  bildirilmesini isteme
- İşlenen verilerin yalnızca otomatik sistemler aracılığıyla analiz
  edilmesi sonucunda aleyhinize bir sonuca itiraz etme
- Verilerin kanuna aykırı işlenmesi sebebiyle zarara uğramanız halinde
  zararın giderilmesini talep etme
- Verilerinizin yapılandırılmış, yaygın kullanılan ve makine
  tarafından okunabilir bir formatta tarafınıza iletilmesini talep
  etme (KVKK Genelge yorumu çerçevesinde)

### 7.2 GDPR Kapsamında (AB Vatandaşları)
GDPR 15-22. maddeler kapsamında ayrıca:

- **Erişim hakkı** — verilerinizin bir kopyasını talep edebilirsiniz.
- **Düzeltme hakkı** — yanlış verileri düzeltebilirsiniz.
- **Silme ("unutulma") hakkı** — verilerinizi sildirebilirsiniz.
- **İşlemeyi kısıtlama hakkı** — belirli durumlarda işlemeyi durdurun.
- **Taşınabilirlik hakkı** — verilerinizi yapılandırılmış formatta
  alın.
- **İtiraz hakkı** — meşru menfaate dayalı işlemeye itiraz edin.
- **Rıza geri çekme hakkı** — burç toggle gibi açık rıza ile yapılan
  işlemleri her zaman durdurabilirsiniz.
- **Denetim otoritesine şikayet hakkı** — yerel veri koruma otoritesine
  başvurabilirsiniz.

### 7.3 CCPA Kapsamında (Kaliforniya Sakinleri)
CCPA kapsamında ayrıca:

- **Bilme hakkı** — hangi kategorilerde veri topladığımızı, hangi
  amaçlarla kullandığımızı.
- **Silme hakkı** — Bölüm 7.4'teki silme yöntemiyle aynı.
- **Satışa hayır deme hakkı** — Vestimentum kişisel verileri
  **satmaz**. (CCPA tanımına göre "satış" yoktur.)
- **Ayrımcılık yasağı** — haklarınızı kullandığınız için size farklı
  davranmayız.

### 7.4 Haklarınızı Nasıl Kullanırsınız

**En kolay yol — uygulama içinden:**
- Profil → "Hesabımı sil" → tüm verileriniz silinir.
- Verimi indir: privacy@vestimentum.app adresine yazarak JSON
  formatında verilerinizin bir kopyasını talep edebilirsiniz.
- Diğer değişiklikler için profil ayarlarını kullanın.

**E-posta ile:**
- privacy@vestimentum.app adresine yazın. Talebinizi kimliğinizi
  doğrulamak için kullandığınız e-postadan iletin.
- Yanıt süresi: 30 gün içinde (KVKK), 1 ay içinde uzatılabilir
  (GDPR).

---

## 8. Çocuklar ve Yaş Sınırı

Vestimentum **13 yaş altındaki kişiler tarafından kullanılamaz.**
Kayıt sırasında doğum tarihinizi girmeniz halinde sistem 13 yaş
altını otomatik reddeder; kayıt sırasında doğum tarihi girmediyseniz
bile uygulamayı kullanmanız 13+ olduğunuzu beyan ettiğiniz anlamına
gelir.

13 yaş altındaki bir çocuğa ait veri topladığımızı fark edersek
hesabı derhal sileriz. Çocuğunuzun Vestimentum kullandığını
düşünüyorsanız privacy@vestimentum.app adresine yazın.

---

## 9. Güvenlik

Verilerinizi korumak için aldığımız önlemler:

- **Aktarımda şifreleme:** Tüm istemci-sunucu iletişimi HTTPS/TLS 1.2+
  üzerinden gerçekleşir.
- **Kimlik doğrulama:** Firebase Authentication standartlarına dayalı
  oturum yönetimi; parolalar Firebase tarafından bcrypt benzeri
  algoritmalarla hashlenir, biz parolayı asla görmeyiz.
- **Erişim kontrolü:** Yalnızca işletimsel gereklilikler için sınırlı
  kişiler veri tabanına erişebilir.
- **Saklamada şifreleme:** Veritabanı seviyesinde TDE (Transparent
  Data Encryption); Cloudinary varsayılan olarak verileri AES-256
  ile şifreler.
- **İzleme:** Sentry üzerinden anormal davranışlar gözlemlenir
  (yalnızca prodüksiyon).

Hiçbir sistem %100 güvenli değildir; bir veri ihlali durumunda
KVKK Veri İhlal Bildirim yönetmeliğine ve GDPR m.33-34'e uygun
olarak ilgili otoritelere 72 saat içinde, etkilenen kullanıcılara
gecikmeksizin bildirim yaparız.

---

## 10. Çerezler ve Takip

Vestimentum **mobil uygulama**'dır; tarayıcı çerezi kullanmaz. Aşağıdaki
takip teknolojilerini kullanmaz:

- Üçüncü taraf analitik (Google Analytics, Mixpanel vb.)
- Reklam tanımlayıcıları (IDFA, AAID)
- Sosyal medya entegrasyonu için izleme pikselleri
- Çapraz uygulama davranış takibi

İlerde uygulama içi analitik eklenirse bu Politika güncellenir ve
opt-out seçeneği sunulur.

---

## 11. Bu Politikadaki Değişiklikler

Bu Politikada değişiklik yaparsak:

- **Önemli değişiklikler** (ör. yeni veri kategorileri, yeni üçüncü
  taraflar, hakların değişmesi): Uygulama içi banner ile bilgilendirir,
  yürürlük tarihini en az 14 gün önceden duyururuz.
- **Küçük değişiklikler** (ör. yazım düzeltmeleri, üçüncü taraf
  linklerinin güncellenmesi): Sessizce güncellenir; "Son güncelleme"
  tarihi yenilenir.

Politika ile aktif olarak ilgilenmek için bu sayfayı periyodik olarak
kontrol etmenizi öneririz.

---

## 12. İletişim

Bu Politika hakkında soru veya talepleriniz için:

- **E-posta:** privacy@vestimentum.app
- **Veri Sorumlusu / Data Controller:** Oğuzcan Özüpek (gerçek
  kişi / individual data controller) — İzmir, Türkiye
  (privacy@vestimentum.app — kurumsallaşma sonrası güncellenecektir)

KVKK kapsamındaki taleplerinizi yanıtlamamızdan memnun değilseniz,
Kişisel Verileri Koruma Kurulu'na (KVKK) şikayet hakkınız vardır:
https://www.kvkk.gov.tr

GDPR kapsamındaki şikayetler için yerel veri koruma otoritenize
başvurabilirsiniz (https://edpb.europa.eu/about-edpb/about-edpb/members_en).

---

*Bu Gizlilik Politikası, KVKK (6698 sayılı Kanun), GDPR (EU 2016/679),
CCPA (Cal. Civ. Code §1798.100 vd.) ve Google Play / Apple App Store
gereksinimleri dikkate alınarak hazırlanmıştır. Resmi hukuki danışmanlık
yerine geçmez; lansman öncesinde bir avukat tarafından gözden
geçirilmesi önerilir.*
