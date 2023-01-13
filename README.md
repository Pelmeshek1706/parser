# parser
first version of parser, for [NewsState](https://github.com/A3azel/microservices-project)

author - Nikita Basenko, from IO-05




- <b>google_search</b> parser - parse your own query.

    output be like: 
 <code>[{'title': 'Отключение света в Киеве: ситуация на 29 декабря 2022',
 'link': 'https://fakty.com.ua/ru/ukraine/suspilstvo/20221228-tymchasovi-obmezhennya-tryvayut-u-kyyevi-onovyly-grafik-vidklyuchennya-svitla/',
 'text': '1 день тому — Какая ситуация с отключением света в Киеве 29 декабря 2022 года - смотрите в материале Фактов ICTV.',
 'bold': 'света'}] </code >


- <b>twitter parser</b> like google_search, but in twitter(omg).

    output be like:
<code>{'query': 'python', 'flags': ['created_at', 'lang', 'text', 'public_metrics'], 'tweets': [{'username': 'Мольфар', 'tag': 'mkbodanu4', 'text': '@rzazhukovmaxim програма Home Assistant, збирає дані з мого інвертора. точніше ...', 'date': datetime.datetime(2022, 12, 29, 22, 19, 44, tzinfo=datetime.timezone.utc), 'lang': 'uk', 'retweets': 0, 'replies': 1, 'likes': 0}]</code>


- <b>parse_tg</b> parse tg from list in func or from DB(in future)

    output be like:
    <code>{'query': 'python', 'content': [{'channel_link': 'https://t.me/UAonlii', 'message': [{'text': '\u200bNIX MultiConf #4. MultiTool для каждого в мире ITГотовьте любимые снеки, напитки и усаживайтесь поуд...', 'views': '59.0K', 'timestamp': '09:00'}]}</code>


- <b>parse_actual_news</b> parse actual news in specific region. 

    output be like:
<code> [{'title': 'У Севастополі пролунали вибухи: що відомо - РБК-Украина', 'text': 'У Севастополі пролунали вибухи: що відомо  РБК-УкраинаВ окупованому Севас...', 'date': 'Fri, 30 Dec 2022 08:24:27 GMT', 'link': 'https://www.rbc.ua/rus/news/sevastopoli-prolunali-vibuhi-shcho-vidomo-1672388667.html', 'author': 'РБК-Украина', 'image': ['https://www.rbc.ua/static/img/_/g/_gettyimages_1399173402__1__13_650x410.jpg']}]</code>