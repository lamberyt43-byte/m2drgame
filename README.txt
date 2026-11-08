M2DR — проект для сборки IPA (iOS) на GitHub, без Mac

1. Зарегистрируйся на github.com.
2. Нажми «+» → New repository → имя M2DR → Create repository.
3. Нажми «uploading an existing file» и перетащи ВСЁ содержимое этой папки
   (project.yml, README.txt и папку M2DR). Нажми Commit changes.
4. Папка .github может не загрузиться перетаскиванием (она скрытая). Тогда:
   Add file → Create new file → в имени напиши  .github/workflows/build.yml
   и вставь туда текст из файла .github/workflows/build.yml. Commit changes.
5. Открой вкладку Actions → Build IPA → Run workflow. Сборка идёт ~5–10 минут.
6. Когда появится зелёная галочка — открой сборку, внизу в Artifacts скачай M2DR-IPA.
   Внутри будет M2DR-1.0-unsigned.ipa.

IPA НЕ ПОДПИСАН. Чтобы поставить на iPhone:
 • Sideloadly (sideloadly.io) на Windows/Mac: подключи iPhone кабелем, войди своим Apple ID,
   перетащи IPA → Start. На iPhone: Настройки → Основные → VPN и управление устройством →
   доверять своему Apple ID. С бесплатным Apple ID приложение работает 7 дней, потом заново.
 • С аккаунтом Apple Developer ($99/год) — подписка на год и выкладка в App Store.

Bundle ID: com.aunxzz.m2dr  · Версия 1.0
Игра лежит в папке M2DR/web — чтобы обновить игру, замени там index.html и запусти сборку снова.
