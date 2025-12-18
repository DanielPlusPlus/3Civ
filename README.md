
# 3Civ

## Opis / Description

**PL:**
Projekt 3Civ to gra strategiczna napisana w C++ z użyciem biblioteki SFML.

**EN:**
3Civ is a strategy game written in C++ using the SFML library.

## Wymagania / Requirements

**PL:**
- Kompilator C++ (zalecany GCC 8.1.0 MinGW-w64)
- CMake (zalecana wersja 3.15)
- SFML 2.6.2

**EN:**
- C++ compiler (recommended: GCC 8.1.0 MinGW-w64)
- CMake (recommended version: 3.15)
- SFML 2.6.2

## Instalacja bibliotek / Installing libraries

**PL:**
1. Pobierz SFML 2.6.2 ze strony: https://www.sfml-dev.org/download.php
2. Wypakuj SFML do folderu `external/SFML-2.6.2`
3. Upewnij się, że ścieżki do SFML są poprawnie ustawione w plikach CMakeLists.txt

**EN:**
1. Download SFML 2.6.2 from: https://www.sfml-dev.org/download.php
2. Extract SFML to the `external/SFML-2.6.2`
3. Make sure the SFML paths are correctly set in CMakeLists.txt

## Budowanie projektu / Building the project

**PL:**
1. Otwórz terminal w głównym katalogu projektu.
2. Utwórz katalog build (jeśli nie istnieje):
   ```sh
   mkdir build
   cd build
   ```
3. Wygeneruj pliki projektu za pomocą CMake:
   ```sh
   cmake .. 
   ```
4. Zbuduj projekt:
   ```sh
   cmake --build .
   ```
5. Uruchom program:
   - Plik wykonywalny znajdziesz w katalogu `build` lub podkatalogu zależnym od konfiguracji.

**EN:**
1. Open a terminal in the main project directory.
2. Create a build directory (if it doesn't exist):
   ```sh
   mkdir build
   cd build
   ```
3. Generate project files using CMake:
   ```sh
   cmake ..
   ```
4. Build the project:
   ```sh
   cmake --build .
   ```
5. Run the program:
   - The executable can be found in the `build` directory or a subdirectory depending on configuration.

## Uwagi / Notes

**PL:**
- Projekt korzysta z SFML 2.6.2. Inne wersje mogą nie być kompatybilne.
- Jeśli pojawią się problemy z bibliotekami, sprawdź czy ścieżki w CMakeLists.txt są poprawne.

**EN:**
- The project uses SFML 2.6.2. Other versions may not be compatible.
- If you encounter issues with libraries, check if the paths in CMakeLists.txt are correct.
