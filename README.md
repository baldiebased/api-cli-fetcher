# api-cli-fetcher
aplikacja CLI służąca do pobierania danych z zewnętrznego API i zapisywania ich do pliku JSON. przydatna do automatyzacji pobierania danych z różnych źródeł.
## instalacja i uruchomienie

1. upewnij się, że masz zainstalowanego **Pythona 3**:

   ```bash
   python --version
   ```

2. sklonuj repozytorium:

   ```bash
   git clone https://github.com/baldiebased/api-cli-fetcher.git
   cd api-cli-fetcher
   ```

3. (opcjonalnie) stwórz środowisko wirtualne:

   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/macOS
   venv\Scripts\activate     # Windows
   ```

4. zainstaluj wymagane biblioteki:

   ```bash
   pip install -r requirements.txt
   ```

## użycie

uruchom aplikację z odpowiednimi argumentami:

```bash
python cli_fetcher.py --fetch --url https://api.example.com/data
```

lub (jeśli masz prawa do uruchamiania bezpośredniego):

```bash
./cli_fetcher --fetch --url https://api.example.com/data
```

po wykonaniu komendy dane zostaną zapisane do pliku `output.json`.

## możliwości rozbudowy

możesz łatwo dodać nowe źródła danych, modyfikując plik `cli_fetcher.py` i dodając nowe opcje URL lub logikę parsowania.

**pomysły na rozwój:**

- obsługa wielu URL-i w jednej komendzie  
- eksport do innych formatów (np. CSV)  
- harmonogram pobierania (np. z użyciem `cron`)  

---

