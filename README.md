# HUB Barbershop — strona internetowa

Statyczna strona wizytówka barbershopu **HUB** we Wrocławiu.
Jeden plik `index.html` + zdjęcia, hostowany na Netlify (auto‑deploy z GitHub).

---

## 🔑 Konta i dostęp

Wszystko jest podpięte pod **jeden główny adres e‑mail**:

| Co | Wartość |
|----|---------|
| Główny e‑mail (logowanie do wszystkiego) | **hubbarbershopwro@gmail.com** |
| Konto GitHub | zarejestrowane na powyższy e‑mail (`hubbarbershopwro`) |
| Konto Netlify | zarejestrowane na powyższy e‑mail |

> Logując się do GitHub i Netlify, używaj **hubbarbershopwro@gmail.com**.

---

## 🔗 Najważniejsze linki

| Zasób | Link |
|-------|------|
| **Strona na żywo (domena)** | **https://hubbarbershop.com** |
| Repozytorium GitHub | https://github.com/hubbarbershopwro/hubbarbershopwro |
| Panel Netlify (projekt) | https://app.netlify.com/projects/coruscating-brigadeiros-236c7f/overview |
| Adres testowy Netlify | https://coruscating-brigadeiros-236c7f.netlify.app |
| Rezerwacja (Booksy) | https://booksy.com/pl-pl/219728_hub-barbershop_barber-shop_13750_wroclaw |
| Instagram | https://www.instagram.com/hubwro/ |
| Lokalizacja (Mapy Google) | https://www.google.com/maps/search/?api=1&query=Mieszcza%C5%84ska+10a+Wroc%C5%82aw |

---

## 🌐 Domena

- Domena: **hubbarbershop.com**
- Została **kupiona przez Netlify**.
- Koszt: **16,99** (rocznie).
- **Termin odnowienia: 25.06.2027** — opłać przed tą datą, żeby strona nie przestała działać.
- Zarządzanie domeną: panel Netlify → **Domain management** (w projekcie powyżej).

> ⚠️ Pilnuj odnowienia. Jeśli płatność karty się nie powiedzie, domena może wygasnąć.
> Faktura i metoda płatności są w Netlify → *Billing*.

---

## 🚀 Jak działa publikacja (deploy)

Strona wdraża się **automatycznie**: każdy `git push` na gałąź `main`
uruchamia nowy deploy w Netlify (zwykle gotowe w ~30 sekund).

Nie ma kroku budowania — Netlify po prostu serwuje pliki z katalogu głównego
(konfiguracja w `netlify.toml`).

### Wprowadzenie zmiany — krok po kroku

```bash
# 1. wejdź do katalogu projektu
cd hubbarbershopwro

# 2. pobierz najnowszą wersję
git pull

# 3. edytuj index.html lub podmień zdjęcia
# 4. zapisz zmiany w git
git add -A
git commit -m "opis zmiany"

# 5. wyślij na GitHub -> Netlify zrobi resztę
git push origin main
```

### Bez Gita (najszybciej)

Można też wrzucić cały folder metodą *drag & drop* na
**https://app.netlify.com/drop** — ale wtedy zmiany nie trafią do GitHub.
Zalecana jest droga przez `git push`.

---

## 📁 Struktura plików

```
index.html        — cała strona (HTML + CSS + odrobina JS w jednym pliku)
netlify.toml      — konfiguracja hostingu (publish = katalog główny, cache zdjęć)
README.md         — ten plik

background.webp   — tło sekcji hero (wnętrze całego salonu)
interior.webp     — detal ściany (popiersia, trójząb) — sekcja "Wnętrze"
lounge.webp       — strefa oczekiwania (sofy) — sekcja "Wnętrze"

cut-01.jpeg       — Crop
cut-02.jpeg       — Skin fade
cut-03.jpeg       — Mullet
cut-04.jpeg       — Taper
cut-05.jpeg       — Buzz & broda
```

Sekcje na stronie (kolejność): **Hero → Z fotela (galeria fryzur) → Wnętrze → Stopka**.

---

## ✏️ Najczęstsze edycje

- **Zmiana zdjęć fryzur** — podmień pliki `cut-01.jpeg` … `cut-05.jpeg`
  (zachowaj te same nazwy) lub zmień `src="..."` w sekcji *galeria* w `index.html`.
- **Zmiana tła / wnętrza** — podmień `background.webp`, `interior.webp`, `lounge.webp`.
- **Godziny otwarcia** — w `index.html` znajdź sekcję `Godziny` (komentarz
  `EDYTUJ GODZINY`) i wpisz realne godziny. ⚠️ Obecnie jest placeholder
  „Pon–Sob / sprawdź dostępność w Booksy".
- **Adres / parking / dane** — sekcja `<div class="facts">` w `index.html`.
- **Linki (Booksy, Instagram, Mapy)** — szukaj `booksy.com`, `instagram.com`,
  `google.com/maps` w `index.html`.

---

## ℹ️ Dane salonu

- **Adres:** Mieszczańska 10a, 50‑201 Wrocław (Śródmieście)
- **Rezerwacja:** online przez Booksy, płatność na miejscu
- **Instagram:** @hubwro
