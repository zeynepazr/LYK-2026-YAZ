# LYK-2026-YAZ

[Türkçe](#türkçe) · [English](#english)

---

## Türkçe

Sınıfta işlediğimiz derslerin ortak arşivi. **Ders notları, slaytlar, ödevler,
simülasyonlar, örnek kodlar ve e-kitaplar** burada toplanır.

Bu repoyu öğrenciler birlikte yürütür — bir "öğretmen" ya da teslim sistemi
yoktur. Herkes elindeki materyali yükler, herkes ihtiyacı olanı buradan alır.

### 30 saniyede kural

> **Materyalin hangi konuya ait?** → `topics/<konu>/`
> **Ne tür bir dosya?** → o konunun içindeki alt klasör
> **Hiçbir konuya ait değil mi, emin değil misin?** → [`resources/`](resources/)

### Ne nereye koyulur?

| Elimde bu var | Buraya koy |
|---|---|
| Ders notu (`.md`, `.pdf`) | `topics/<konu>/notes/` |
| Sunum / slayt | `topics/<konu>/slides/` |
| Ödev ya da ödev çözümü | `topics/<konu>/assignments/` |
| Simülasyon, notebook | `topics/<konu>/simulations/` |
| Örnek kod | `topics/<konu>/examples/` |
| **E-kitap, makale, cheat sheet** | `topics/<konu>/books/` |
| Hiçbir konuya ait olmayan her şey | [`resources/`](resources/) — aşağıya bak |

### Klasör iskeleti

```
LYK-2026-YAZ/
├── README.md                   # bu dosya
├── .gitignore
├── resources/                  # hiçbir konuya ait olmayan kaynaklar
│   ├── README.md
│   ├── books/                  # konu bağımsız e-kitaplar
│   ├── guides/                 # kurulum ve araç rehberleri (Git, Python…)
│   ├── cheatsheets/            # kısa başvuru kağıtları
│   ├── slides/                 # konu dışı sunumlar, seminerler
│   ├── videos/                 # video kayıtları / bağlantı listeleri
│   └── misc/                   # yeri belli olmayan her şey
└── topics/                     # her konu kendi klasöründe
    ├── _TEMPLATE/              # yeni konu açarken kopyalanacak şablon
    │   ├── README.md
    │   ├── notes/              # ders notları
    │   ├── slides/             # sunum ve slaytlar
    │   ├── assignments/        # ödevler ve çözümleri
    │   ├── simulations/        # simülasyonlar, notebook'lar
    │   ├── examples/           # örnek kodlar
    │   └── books/              # e-kitaplar, makaleler
    ├── cryptography/            # aynı alt klasörler
    ├── blockchain/              # aynı alt klasörler
    ├── astronomy/               # aynı alt klasörler
    └── ai/                      # aynı alt klasörler
```

Her konu klasörü **aynı altı alt klasörü** içerir — bir konuda nasıl
çalıştığını öğrenirsen hepsinde aynıdır.

### Konuya bağlanamayan kaynaklar

Bir materyal tek bir derse ait değilse — genel bir e-kitap, Git kurulum
rehberi, bir seminer sunumu, faydalı bir video listesi — [`resources/`](resources/)
altına gider. Oradaki alt klasörler: `books/`, `guides/`, `cheatsheets/`,
`slides/`, `videos/`, `misc/`.

**Emin değilsen `resources/misc/` klasörüne koy.** Yanlış konunun altına
gömülmesindense burada durması iyidir; sonradan yeri belli olursa taşırız.

### Konular

| Konu | Klasör |
|---|---|
| Kriptografi | [`topics/cryptography/`](topics/cryptography/) |
| Blockchain | [`topics/blockchain/`](topics/blockchain/) |
| Astronomi | [`topics/astronomy/`](topics/astronomy/) |
| Yapay Zeka | [`topics/ai/`](topics/ai/) |

### Nasıl yüklerim?

1. Yukarıdaki tablodan dosyanın gideceği yeri bul.
2. Dosya adı: küçük harf, kelimeler arası tire, Türkçe karakter yok.
   Örnek: `caesar-sifreleme.md`, `odev-1-cozum.ipynb`
3. Aynı isimde dosya varsa üzerine yazma; sonuna kısa bir ek koy
   (`odev-1-cozum-alternatif.ipynb`).
4. Commit at ve gönder (ya da pull request aç).

**E-kitaplar için:** serbestçe paylaşılabilen ve 25 MB'tan küçük dosyaları
doğrudan `books/` klasörüne koy. Dosya büyükse ya da telifliyse **yükleme** —
ilgili `README.md` dosyasındaki kaynak tablosuna bağlantı ekle.

### Yeni konu nasıl açılır?

1. `topics/_TEMPLATE/` klasörünü kopyala ve konu adıyla yeniden adlandır
   (küçük harf, tireli): `topics/lineer-cebir/`
2. İçindeki `README.md` dosyasındaki `<...>` yerlerini doldur, en üstteki
   açıklama satırlarını sil.
3. Yukarıdaki **Konular** tablosuna bir satır ekle.

---

## English

A shared archive for the courses we cover in class: **lecture notes, slides,
assignments, simulations, example code and e-books** all live here.

This repo is run by the students together — there is no "teacher" and no
submission system. Everyone uploads what they have, everyone takes what they need.

### The rule in 30 seconds

> **Which topic is it about?** → `topics/<topic>/`
> **What kind of file is it?** → the matching subfolder inside that topic
> **Not tied to any topic, or unsure?** → [`resources/`](resources/)

### Where does it go?

| What you have | Put it here |
|---|---|
| Lecture notes (`.md`, `.pdf`) | `topics/<topic>/notes/` |
| Presentation / slides | `topics/<topic>/slides/` |
| Assignment or its solution | `topics/<topic>/assignments/` |
| Simulation, notebook | `topics/<topic>/simulations/` |
| Example code | `topics/<topic>/examples/` |
| **E-book, paper, cheat sheet** | `topics/<topic>/books/` |
| Anything not tied to a topic | [`resources/`](resources/) — see below |

### Folder structure

```
LYK-2026-YAZ/
├── README.md                   # this file
├── .gitignore
├── resources/                  # material not tied to any topic
│   ├── README.md
│   ├── books/                  # topic-independent e-books
│   ├── guides/                 # setup and tool guides (Git, Python…)
│   ├── cheatsheets/            # quick reference sheets
│   ├── slides/                 # off-topic talks, seminars
│   ├── videos/                 # recordings / link lists
│   └── misc/                   # anything that fits nowhere else
└── topics/                     # one folder per topic
    ├── _TEMPLATE/              # skeleton to copy when adding a new topic
    │   ├── README.md
    │   ├── notes/              # lecture notes
    │   ├── slides/             # presentations and slides
    │   ├── assignments/        # assignments and solutions
    │   ├── simulations/        # simulations, notebooks
    │   ├── examples/           # example code
    │   └── books/              # e-books, papers
    ├── cryptography/            # same subfolders
    ├── blockchain/              # same subfolders
    ├── astronomy/               # same subfolders
    └── ai/                      # same subfolders
```

Every topic folder has **the same six subfolders** — learn one topic and you
know your way around all of them.

### Material that fits no topic

If something isn't tied to a single course — a general e-book, a Git setup
guide, a seminar deck, a useful video list — it goes under
[`resources/`](resources/), which holds `books/`, `guides/`, `cheatsheets/`,
`slides/`, `videos/` and `misc/`.

**When in doubt, drop it in `resources/misc/`.** Better there than buried under
the wrong topic; we can move it once its place is clear.

### Topics

| Topic | Folder |
|---|---|
| Cryptography | [`topics/cryptography/`](topics/cryptography/) |
| Blockchain | [`topics/blockchain/`](topics/blockchain/) |
| Astronomy | [`topics/astronomy/`](topics/astronomy/) |
| Artificial Intelligence | [`topics/ai/`](topics/ai/) |

### How do I upload?

1. Find the destination in the table above.
2. File names: lowercase, hyphen-separated, ASCII only.
   Example: `caesar-sifreleme.md`, `odev-1-cozum.ipynb`
3. Don't overwrite an existing file with the same name; add a short suffix
   instead (`odev-1-cozum-alternatif.ipynb`).
4. Commit and push (or open a pull request).

**For e-books:** put freely shareable files under 25 MB directly into `books/`.
If a file is larger or copyrighted, **don't upload it** — add a link to the
resource table in the relevant `README.md` instead.

### How do I add a new topic?

1. Copy `topics/_TEMPLATE/` and rename it after the topic
   (lowercase, hyphenated): `topics/lineer-cebir/`
2. Fill in the `<...>` placeholders in its `README.md` and delete the note
   at the top.
3. Add a row to the **Topics** table above.
