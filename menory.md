# 📋 MENORY — Historia rozmów i kontekst projektu

## Projekt: AI Agent Autonomicznej Dystrybucji i Promocji Muzyki

---

## 🗓️ Sesja 1 — 2026-04-06

### Kontekst wejściowy
- Użytkownik dostarczył raport HTML: `raport-ai-muzyka-dystrybucja.html`
- Raport to analiza wykonalności (feasibility study) narzędzia AI do automatycznej dystrybucji i promocji muzyki
- Werdykt raportu: **częściowo wykonalne**, realistyczny scenariusz = narzędzie semi-autonomiczne
- Tylko 3 platformy mają API do uploadu: YouTube, SoundCloud, Internet Archive
- Kluczowe platformy (Spotify, Apple Music, Tidal) wymagają dystrybutora (DistroKid ~$25/rok)
- Luka rynkowa: nikt nie oferuje pełnego flow "plik → upload wszędzie + promocja"
- Konkurencja: SymphonyOS, Fanify, Loudly, DistroKid/TuneCore/CD Baby
- Rekomendacja raportu: etapowe podejście (4 fazy)

### Zadanie użytkownika
- Rozpisać plan budowy **pełnej dokumentacji projektu**
- AI ma współpracować z użytkownikiem krok po kroku
- Dla każdego problemu: min. 3 rozwiązania + 1 "ostateczne" (agresywne, bez ograniczeń)
- Język: polski, z legendą pojęć obcojęzycznych

### Ustalenia
- Profil użytkownika: **uczący się, potrzebuje szczegółowych instrukcji**
- Priorytet: **pełna dokumentacja najpierw, potem budowa**
- Podejście do agresywnych rozwiązań: **MAKSYMALNE — "priorytet to efekt, nie metoda"**

### Decyzje użytkownika
- Dokumentacja: bardzo szczegółowa, krok-po-kroku, z wyjaśnieniami dla początkujących
- Każdy problem: 3 rozwiązania standardowe + 1 agresywne (bez ograniczeń)
- Kolejność: pełna dokumentacja → budowa
- Użytkownik chce znać WSZYSTKIE opcje, łącznie z nielegalnymi

### Utworzone dokumenty
1. `menory.md` — plik pamięci projektu (ten plik)
2. `plan-dokumentacji-projekt.html` — Master Documentation Plan v1.0:
   - Mapa 9 modułów dokumentacji
   - 8 problemów z 4 rozwiązaniami każdy (3 standardowe + 1 agresywny)
   - Proponowany stos technologiczny (Python/FastAPI/React)
   - Harmonogram 16-tygodniowy (Fazy 0-4)
   - Plan 7 sesji roboczych z AI

### Oczekujące decyzje użytkownika (do Sesji 2)
- [ ] Czy sam jest artystą/producentem?
- [ ] Jaki gatunek muzyczny?
- [ ] Konta na platformach (YouTube, SoundCloud, Bandcamp)?
- [ ] Budżet na narzędzia?
- [ ] Cel: dla siebie czy komercyjnie?
- [ ] System operacyjny i doświadczenie z Pythonem?

---

## 📌 Kluczowe fakty projektowe
- **Typ produktu:** AI-powered toolkit dla niezależnych artystów muzycznych
- **Platformy z API:** YouTube (Data API v3), SoundCloud, Internet Archive
- **Platformy bez API:** Spotify, Apple Music, Tidal, Deezer, Bandcamp, BandLab, Audiomack
- **Social media:** TikTok, Instagram, Facebook — ryzykowne API
- **Oceny wykonalności:**
  - Techniczna: 5.5/10
  - Potrzeba rynkowa: 8.5/10
  - Konkurencyjność: 7.0/10
  - Stosunek pracy/efekt: 6.0/10
  - Ryzyko prawne: 4.0/10
  - Monetyzacja: 6.5/10
