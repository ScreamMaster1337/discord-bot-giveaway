# Discord Giveaway Bot (discord.js v14)

Bot Discord umożliwiający organizowanie konkursów, w których użytkownicy mogą brać udział klikając przycisk, a po upływie określonego czasu bot wybiera zwycięzców. Zbudowany w **discord.js v14**, z integracją z **MongoDB**.

## Podgląd

Poniżej znajduje się zrzut ekranu prezentujący komendę:

![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291914252944150621/Zrzut_ekranu_2024-10-05_020611.png?ex=6701d468&is=670082e8&hm=036891d3b1d4b6e2b2aa517eb78f9fb6b7538d7bc78cac73c4504a77303ceb1b&)

- **/start [nagroda] [liczba_zwycięzców] [czas]**: Rozpoczyna nowy konkurs.
  - **Nagroda**: Przedmiot, który zwycięzcy otrzymają.
  - **Liczba_zwycięzców**: Ile osób wygra.
  - **Czas**: Czas trwania konkursu (np. 10s, 5m, 1h).
  
  **Przykład**: `/start test 1 10s` – rozpoczyna konkurs z nagrodą "Nagroda Testowa", 1 zwycięzcą, i czasem trwania 10 sekund.

- **Automatyczny udział**: Użytkownicy klikają przycisk pod wiadomością konkursową, aby wziąć udział, a ponowne kliknięcie anuluje ich udział.

- **Automatyczne zakończenie konkursu**: Po upływie czasu bot automatycznie zamyka konkurs i wybiera zwycięzcę(-ów).

## Podgląd

Poniżej znajduje się zrzut ekranu prezentujący komendę:

![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291914749394812958/image.png?ex=6701d4de&is=6700835e&hm=a5bf83f4fda172c5392c81289bbd846b5ef8f22ec81798b791d220fee0fdb3ff&)

- **/end [ID_wiadomości]**: Zamyka konkurs przed czasem.

  **Przykład**: `/end 123456789012345678` – kończy konkurs o danym ID wiadomości.

## Podgląd

Poniżej znajduje się zrzut ekranu prezentujący komendę:

![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291914700665258065/image.png?ex=6701d4d3&is=67008353&hm=73bb66f687f951afa1fbf5b111073619b2b3e99e9e2a1202e904b0ab071550a8&)

- **/reroll [ID_wiadomości]**: Przeprowadza losowanie nowego zwycięzcy.

  **Przykład**: `/reroll 123456789012345678` – ponownie losuje zwycięzcę konkursu o danym ID wiadomości.

- **Integracja z MongoDB**: Wszystkie dane o konkursach i uczestnikach są zapisywane w bazie danych MongoDB.

## Podgląd

Poniżej znajduje się zrzut ekranu prezentujący działanie rozpoczęcia, zakończenia oraz wzięcia i anulowania udziału:

![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291915431048908853/image.png?ex=6701d581&is=67008401&hm=8d167a7d263e36c320b4236642c95f028c76cba31aa308bfbd3f5430e4ab4a84&)
![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291916386205040690/image.png?ex=6701d665&is=670084e5&hm=13f3466087696901adce770beb508d4bb87275efd48ed8e7d9b5443ebf3c06ff&)

![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291915460257906760/image.png?ex=6701d588&is=67008408&hm=462c0233b75592630b33297ff2c68403cf991cfa6039363294e60bd8746bc4d6&)
![footer](https://cdn.discordapp.com/attachments/1102682877235310734/1291915493850218568/image.png?ex=6701d590&is=67008410&hm=13f3226319be3344bafcf1faed1d9238a2aa61505d3cd9bf03825d64db907cfa&)

## Wymagania

- **Node.js** v16.9.0 lub nowszy
- **npm**
- Konto Discord oraz utworzona aplikacja [na Discord Developer Portal](https://discord.com/developers/applications)
- MongoDB URI

**Autor:** [ScreamMaster1337](https://github.com/ScreamMaster1337)  
**Licencja:** MIT
