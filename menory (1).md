# 🧠 Menory.md — Pamięć Projektu

> **Projekt:** AI Agent Autonomicznej Dystrybucji i Promocji Muzyki
> **Repo:** https://github.com/tomsonxxx/Dystrybucja-.git
> **Ostatnia aktualizacja:** 6 kwietnia 2026

---

## 📋 Historia sesji

### Sesja 1 — Raport wykonalności (feasibility)
**Data:** 6 kwietnia 2026
**Dokument:** `raport-ai-muzyka-dystrybucja.html`
**Status:** ✅ Gotowy

**Kluczowe ustalenia:**
- Pomysł jest **częściowo wykonalny** — nie jako pełna autonomia, ale jako narzędzie semi-autonomiczne
- Tylko 3 z ~12 platform mają API do uploadu: YouTube, SoundCloud, Internet Archive
- Spotify, Apple Music, Tidal, Deezer — wymagają dystrybutora (DistroKid ~$25/rok)
- Bandcamp API — tylko dla labeli
- Browser automation = łamanie ToS = bany kont
- Rekomendacja: etapowe podejście (4 fazy), MVP w 4-6 tygodni
- Oceny: potrzeba rynkowa 8.5/10, techniczna wykonalność 5.5/10, ryzyko prawne 4.0/10
- Luka rynkowa: nikt nie oferuje pełnego flow "plik → upload wszędzie + promocja"
- Konkurencja: SymphonyOS (marketing), Fanify (micro-targeting), Loudly (AI + dystrybucja)

**Werdykt:** Warto budować, ale w okrojonej, etapowej wersji. Zasada: automatyzuj przygotowanie, nie publikację.

---

### Sesja 2 — Plan dokumentacji
**Data:** 6 kwietnia 2026
**Dokument:** `plan-dokumentacji-projekt.html`
**Status:** ✅ Gotowy

**Kluczowe ustalenia:**
- Stworzono Master Documentation Plan v1.0
- Zdefiniowano 10 dokumentów do stworzenia (8 jeszcze do zrobienia)
- Proponowany stos: Python 3.11+ / FastAPI / React+Tailwind / SQLite→PostgreSQL / Claude API / Celery+Redis / Railway
- Opisano 8 głównych problemów z wariantami rozwiązań (A/B/C + ☠️ ostateczne)
- Harmonogram: 16 tygodni przy 10-15h/tydzień pracy hobbystycznej
- Model biznesowy: freemium ($5-15/mies.) lub pay-per-release ($2-5/release)
- Break-even: 30-50 płacących użytkowników

**Problemy zidentyfikowane:**
1. Spotify/Apple/Tidal/Deezer — brak API uploadu
2. Bandcamp — API tylko dla labeli
3. TikTok/Instagram/Facebook — ryzykowne API
4. Wybór modelu AI do metadanych
5. Generowanie okładek albumów
6. YouTube wymaga audytu Google
7. Rate-limiting i quotas
8. Weryfikacja tożsamości artysty

---

### Sesja 3 — Lista ToDo + menory.md
**Data:** 6 kwietnia 2026
**Dokumenty:** `menory.md`, `ToDo.md`
**Status:** ✅ Gotowy

**Co zrobiono:**
- Stworzono plik menory.md (ten plik) — pamięć projektu
- Stworzono szczegółową listę ToDo.md z etapami budowy od zera do wersji finalnej
- Etapy: 0 (dokumentacja) → 1 (AI metadata) → 2 (upload 3 platformy) → 3 (social media kit) → 4 (dystrybutor + beta) → 5 (produkcja)

---

### Sesja 4 — Product Vision & Scope
**Data:** 6 kwietnia 2026
**Dokument:** `product-vision-scope.html`
**Status:** ✅ Gotowy

**Dane zebrane od użytkownika:**
- **Cel:** Dla siebie + udostępni za darmo (open-source)
- **Gatunek:** Electronic / EDM
- **Istniejące konta:** YouTube ✓, SoundCloud ✓
- **Budżet:** Minimalny (preferuje darmowe narzędzia)

**Kluczowe ustalenia:**
- Nazwa robocza projektu: **SoundPush**
- Model: open-source, self-hosted, licencja MIT/GPL
- Persona: niezależny producent electronic/EDM, 18-40 lat, niski budżet
- Priorytet platform: SoundCloud > YouTube > Internet Archive (Tier 1, API)
- Bandcamp, TikTok, Reddit = Tier 2 (content kit, ręczny upload)
- Spotify, Apple, Beatport = Tier 3 (wymaga dystrybutora, przyszłość)
- Metryka sukcesu MVP: release w 5 min zamiast 1-3h, 3 platformy z jednego kliknięcia
- Zasada "złotego kliku": AI przygotowuje, artysta zatwierdza
- Koszt dla użytkownika: $0 (narzędzie) + $3-10/mies. (API LLM)
- Struktura repo zdefiniowana (src/core, src/ai, src/audio, src/uploaders itd.)

---

## 🗺️ Stan dokumentów

| # | Dokument | Format | Status |
|---|----------|--------|--------|
| 1 | Raport wykonalności | HTML | ✅ Gotowy |
| 2 | Plan dokumentacji | HTML | ✅ Gotowy |
| 3 | menory.md | MD | 🔄 Aktualizowany |
| 4 | ToDo.md | MD | ✅ Gotowy |
| 5 | Product Vision & Scope | HTML | ✅ Gotowy |
| 6 | Architektura techniczna | HTML+Mermaid | ⬜ Do zrobienia |
| 7 | Mapa integracji platform | HTML/MD | ⬜ Do zrobienia |
| 8 | AI Pipeline — prompty i modele | MD+JSON | ⬜ Do zrobienia |
| 9 | Strategia obejścia ograniczeń | HTML | ⬜ Do zrobienia |
| 10 | Plan prawny i compliance | MD/HTML | ⬜ Do zrobienia |
| 11 | Harmonogram + MVP Roadmap | HTML+Gantt | ⬜ Do zrobienia |
| 12 | Model biznesowy | HTML | ⬜ Do zrobienia |

---

## 🔧 Stos technologiczny (ustalony)

- **Backend:** Python 3.11+ / FastAPI
- **Frontend:** React + Tailwind CSS
- **Baza danych:** SQLite (start) → PostgreSQL (skala)
- **AI/LLM:** Claude API (Anthropic) / OpenAI GPT-4o
- **Kolejka zadań:** Celery + Redis
- **Hosting:** Railway / Render (darmowy tier na start)
- **Analiza audio:** librosa / Essentia
- **Grafiki:** DALL-E 3 / Stable Diffusion / Canva API
- **Wideo:** FFmpeg
- **Social scheduling:** Buffer API / Hootsuite API

---

## 🎯 Decyzje podjęte

1. **Podejście etapowe** — nie budujemy pełnej autonomii od razu
2. **Legalne API tylko** — nie używamy browser automation w MVP
3. **DistroKid jako pośrednik** — dla platform streamingowych
4. **Najpierw CLI, potem dashboard** — szybki prototyp przed UI
5. **Zasada:** automatyzuj przygotowanie, nie publikację

---

## 👤 Profil użytkownika (potwierdzony)

- **Rola:** Niezależny producent muzyczny (artysta)
- **Gatunek:** Electronic / EDM
- **Cel projektu:** Dla siebie + udostępnienie za darmo (open-source)
- **Istniejące konta:** YouTube ✓, SoundCloud ✓
- **Budżet:** Minimalny (preferuje darmowe narzędzia)
- **Nazwa robocza:** SoundPush
