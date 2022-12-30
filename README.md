# parser
first version

author - Pelmeshek1706

- <b>google_search</b> parser - parse your own query.

    output be like: 
 <code>[{'title': 'Отключение света в Киеве: ситуация на 29 декабря 2022',
 'link': 'https://fakty.com.ua/ru/ukraine/suspilstvo/20221228-tymchasovi-obmezhennya-tryvayut-u-kyyevi-onovyly-grafik-vidklyuchennya-svitla/',
 'text': '1 день тому — Какая ситуация с отключением света в Киеве 29 декабря 2022 года - смотрите в материале Фактов ICTV.',
 'bold': 'света'}] </code >


- <b>twitter parser</b> like google_search, but in twitter(omg).

    output be like:
<code>{'query': 'python', 'flags': ['created_at', 'lang', 'text', 'public_metrics'], 'tweets': [{'username': 'Мольфар', 'tag': 'mkbodanu4', 'text': '@rzazhukovmaxim програма Home Assistant, збирає дані з мого інвертора. точніше зберігає і показує дані, які з інвертора збирає простенька програмка на python, яку сам написав.\nнічого додаткового для моніторингу, на жаль, нема. Хоча дуже хочу SmartShunt поставити.', 'date': datetime.datetime(2022, 12, 29, 22, 19, 44, tzinfo=datetime.timezone.utc), 'lang': 'uk', 'retweets': 0, 'replies': 1, 'likes': 0}]</code>


- <b>parse_tg</b> parse tg from list in func or from DB(in future)

    output be like:
    <code>{'query': 'python', 'content': [{'channel_link': 'https://t.me/UAonlii', 'message': [{'text': '\u200bNIX MultiConf #4. MultiTool для каждого в мире ITГотовьте любимые снеки, напитки и усаживайтесь поудобней. Мы ждали этого целый год… НИКСовая мультиконференция возвращается!24–25 октября NIX MultiConf #4 пройдет в новом онлайн-формате. Бесплатно.2 дня, 14 направлений, более 30 докладов от украинских и зарубежных экспертов мирового уровня. Готовьте вопросы спикерам из NIX, Ask Applications, Data Art, BBС, AgileLAB, Elastic и Blue Yonder GmbH. За самый креативный вопрос разыграем NIX Growth box.Уникальность конференции — в разнообразии инструментов для разработчиков, тестировщиков, дизайнеров и нетехнических специалистов в IT. Кто-то окончил ВУЗ и ищет направление по душе, кто-то хочет отвлечься от рутинных посиделок дома, а некоторые смельчаки сменили работу и пришли за новыми скиллами.Полезности ждут новичков и senior’ов. Запускаем четыре новых направления: Python, Data Science, Sales Force, HR. И не забываем о традиционных — .NET, PHP, QA, Java, Design, WordPress, Android, JavaScript, Business Analytics, Project Management.Когда: суббота и воскресенье 24–25 октября, с 10:00 до 19:00Как принять участие: регистрируйтесь на сайте и получите подробную программу.Где: на YouTube-канале', 'views': '59.0K', 'timestamp': '09:00'}]}</code>


- <b>parse_actual_news</b> parse actual news in specific region. 

    output be like:
<code> [{'title': 'У Севастополі пролунали вибухи: що відомо - РБК-Украина', 'text': 'У Севастополі пролунали вибухи: що відомо  РБК-УкраинаВ окупованому Севастополі пролунали вибухи. Що відомо?  Громадське телебаченняВ анексованому Севастополі пролунали вибухи: окупаційна влада заявляє про "роботу ППО"  ТСНВ окупованому Севастополі пролунали вибухи, повідомляється про роботу ППО  Слово і ділоУ окупантів в Криму спрацювала ППО  Українська правдаВідкрити повний огляд в додатку Google Новини', 'date': 'Fri, 30 Dec 2022 08:24:27 GMT', 'link': 'https://www.rbc.ua/rus/news/sevastopoli-prolunali-vibuhi-shcho-vidomo-1672388667.html', 'author': 'РБК-Украина', 'image': ['https://www.rbc.ua/static/img/_/g/_gettyimages_1399173402__1__13_650x410.jpg', 'https://www.rbc.ua/static/img/_/k/_kuleba_260x164.jpg', 'https://www.rbc.ua/static/img/_/v/_viyskoviy_gaybitsya_caesar__zima_gettyimages_1245851338_260x164.jpg', 'https://www.rbc.ua/static/img/_/g/_gettyimages_1399173402__1__13_1300x820.jpg']}]</code>