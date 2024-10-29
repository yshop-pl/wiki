---
icon: server
---

# Plugin yShop.pl

## Minecraft Java

### Instalacja
Pobieramy najnowszą wersję pluginu [tutaj](https://github.com/yshop-pl/yshop-plugin-v4/releases).
Następnie wrzucamy plugin do folderu ``~/plugins/`` w plikach twojego serwera Minecraft.
Po dodaniu pluginu na serwer należy **zrestartować serwer**.

### Konfiguracja
W folderze ``~/plugins/yShopPlugin`` znajdziesz plik ``config.yml``, w którym musisz uzupełnić zmienne.

```yml
# Klucz API do autoryzacji licencji
# Panel > Ustawienia > Klucz API
apiKey: 'TWÓJ KLUCZ API, ZNAJDUJE SIĘ W ZAKŁADCE Ustawienia > Klucze API'

# ID serwera z panelu Panel > Serwery > Zarządzanie
serverId: 'ID TWOJEGO SERWERA Z PANELU'

# Klucz serwera do generowania sygnatury
# Panel > Serwery > Zarządzanie
serverKey: 'KLUCZ TWOJEGO SERWERA'

# Link do serwera API
apiUrl: 'https://api.yshop.pl/v4'

# Tryb debugowania włącz tylko wtedy kiedy masz problemy z połączeniem
# UWAGA! Tryb pokaże w konsoli wrażliwe informacje
debug: false
```

Po uzupełnieniu pliku konfiguracyjnego zapisujemy plik i **restartujemy serwer**

!!!warning Restart serwera
Nie używaj komendy ``/reload`` lub innych pluginów odpowiedzialnych za przeładowywanie pluginów
!!!

### Rozszerzenia pluginu
Nasz plugin posiada możliwość pisania własnych rozszerzeń. Wszystkie rozszerzenia znajdują się w folderze ``~/plugins/yShopPlugin/extensions``, jeżeli nie widzisz tego folderu - stwórz go

Nazwa rozszerzenia   | Link do pobrania
---    | ---
Placeholders | Pobierz w panelu yshop.pl