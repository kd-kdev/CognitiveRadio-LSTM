# CognitiveRadio-LSTM
## Predviđanje stanja kanala uz pomoć LSTM (Long Short-Term Memory) modela
Uz pomoć PyTorch tehnologije, simuliramo više frekventnih kanala kao i njihovu dostupnost kroz vreme. Koristimo LSTM model koji treniramo na simulaciji jednog spektra i pravimo predviđanja o budućim stanjima spektra na osnovu njegovih prethodnih stanja.

Rad se sastoji iz sledećih delova:

- Importujemo neophodne biblioteke
- Simuliramo spektar kao i njegovo stanje kroz vreme koristeći funkciju simulate_multiple_channels
- Pripremamo/obrađujemo podatke u format pogodan za input na LSTM model
- Definišemo LSTM model
- Pripremamo DataLoader, spremamo podatke za treniranje
- Training loop - treniramo model na simuliranim podacima
- Nasumično odabiramo deo prethodno simuliranih podataka, i predviđamo buduće stanje kanala uz pomoć LSTM modela
- Proveravamo preciznost modela
- Poredimo realno stanja kanala sa predviđenim stanjem
