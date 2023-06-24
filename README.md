# Systemy operacyjne
## System operacyjny
To program lub zbiór programów zarządzających zasobami komputera oraz umożliwiających interakcje między sprzętem a użytkownikiem lub aplikacjami. Obejmuje funkcje takie jak zarządzanie zasobami, procesami, pamięcią, systemem plików, urządzeniami i/o, interfejs użytkownika.

## Proces
W systemie operacyjnym to działający program lub zadanie, które jest pod kontrolą systemu operacyjnego i posiada własną przestrzań adresową oraz stan, a także jest zarządzany i nadzorowany przez system operacyjny w zakresie alokacji zasobów i planowania wykonania.

## Mapa pamięci
To struktura lub schemat przedstawiający sposób, w jaki pamięć komputera jest podzielona i wykorzystywana przez system oraz aplikacje. Przedstawia ona rozkład pamięci fizycznej i wirtualnej. Mapa pamięci informuje o tym, które obszary pamięci są zajęte przez system operacyjny, które są zarezerwowane dla aplikacji i jakie są ograniczenia oraz dostępne zasoby pamięciowe.
| Przykładowa mapa |
|:--:|
| Registers |
| Cache | 
| Main memory |
| Magnetic disk |
| Magnetic tape |

## Wątki
To częściowe jednostki wykonywania w ramach procesu
Podobieństwa:
- wykonują instrukcje
- korzystają z zasobów systemowych
- są planowane przez system

Różnice:
- wątki są częścią procesu
- dzielą zasoby i przestrzeń adresową
- tworzenie i zarządzanie nimi jest szybsze
- mogą komunikować się bezpośrednio

## Stany procesów
- Gotowy - gotowy do wykonania, czeka na przydzielenie
- Wykonywany - aktualnie wykonuje swoje instrukcje na procesorze
- Oczekujący - został zawieszony i oczekuje na zdarzenie lub zasób, które jest mu niezbędne do kontynuowania wykonania. Może być to oczekiwanie na dane z urządzenia i/o, zdarzenie systemowe lub zasób systemowy
- Zakończony - zakończył swoje działanie i nie jest już aktywny. Może czekać na zwolnienie zasobów lub być oczekującym na zakończenie przez rodzica (jeśli istnieje hierarchia procesów)
- Sierota
- Zombie
- Zawieszony - został tymczasowo zawieszony lub zatrzymany przez system, zwykle w celu zwolnienia zasobów. Może być przywrócony do stanu gotowości w odpowiednim momencie.

## Implementacja wątków w przestrzeni użytkownika
To tworzenie i zarządzanie wątkami bezpośrednio przez aplikacje, bez udziału systemu. Jest szybsza i bardziej elastyczna, ale nie korzysta z zalet współdzielenia zasobów między procesami.

## Wątki w jądrze
Są zarządzane przez system, umożliwiają równoległe wykonanie na wielu procesorach i współdzielenie zasobów.
Przełączanie kontekstu między nimi jest kosztowne, ale zapewnia większą wydajność i skalowalność aplikacji.

## Komunikacja procesów
Procesy w systemie komunikują się za pomocą mechanizmów IPC, takich jak kolejki komunikatów, potoki, gniazda sieciowe, pamięć współdzielona i semafory. Dzięki nim mogą wymieniać dane i synchronizować swoje działania.

## Muteksy
Zwane również jako blokady, są mechanizmem synchronizacji używanym w systemach i programowaniu wielowątkowym. Służą do zapewnienia, że tylko jeden wątek może równocześnie korzystać z chronionego zasobu.

## Szeregowanie
Występuje w systemie i dotyczy wyboru i przydziału zasobów, takich jak procesor, pamięć lub urządzenia dla różnych zadań. Obejmuje zarówno procesów jak i wątków i ma na celu efektywne wykorzystanie zasobów, minimalizacje czasu oczekiwania i równomierne rozłożenie obciążenia.

