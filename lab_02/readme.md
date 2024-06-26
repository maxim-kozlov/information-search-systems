Лабораторная № 2

Преамбула: 
Чтобы понять сущность именованных сущностей, вы можете обратиться к статье на Хабре (https://habr.com/en/company/contentai/blog/449514/)
и классической статье из донейросетевой эпохи
(https://publications.hse.ru/mirror/pubs/share/folder/z5xm4d2iuh8/direct/118232483).


Если такие длинные тексты навевают на вас тоску, вот короткое определение:

Именованные сущности - общий термин, который используют для обозначения какого-то множества слов (словосочетаний, последовательностей символов), которые представляют какой-то особый интерес в контексте решаемой практической задачи и которые нужно отделить от остальных слов. Это могут быть стандартные вещи: имена, фамилии, названия организаций, локации, денежные суммы, даты, номера телефонов, а могут быть и более специфичные: статьи кодексов, белки, симптомы, товары. На основе извлечения именованых сущностей строятся онтологии, краткие пересказы, распознавание документов, etc, etc.

Понятно, что что-то можно выделить регулярками, но это неинтересно. При помощи библиотеки "Наташа" на Питоне можно выделять любые именованные сущности правилами. Здесь - вся документация к "Наташе": https://github.com/natasha/yargy
а здесь - тетрадка с примерами
https://github.com/mannefedov/compling_nlp_hse_course/blob/master/notebooks/rnn_ner/natasha.ipynb
Наташа хороша тем, что у не сравнительно неплохое распознавание кириллицы.
Есть и другие библиотеки:
https://spacy.io/ (MIT)
https://github.com/stanfordnlp/stanza (Стэнфорд)
Предполагалось, что вы будете работать с русским, поэтому я предлагаю для этой лабораторной использовать Наташу или Stanza, но не ограничиваю вас в выборе.

Задание:
1. Откройте Википедию.
2. Выберите статью, которая вам наиболее симпатична и достаточно длинна (желательно - не менее 3000 слов).
3. Определите именованные сущности, которые фигурируют в тексте.
4. Определите, какие границы этих сущностей вы хотите задать.
5. Откройте то, в чем вы кодите.
6. Поставьте "Наташу".
7. Попробуйте извлечь как можно больше именованных сущностей (исходя из п.3 - вы хотите извлекать локации, персон, даты, названия, etc) готовыми правилами.
8. Напишите минимум три новых правила, которые позволят извлекать именованые сущности более точно: персоны с должностями, локации с типом и именованием, модели с серийными номерами и т.д.

Как сдавать задание:
1. Исходный текст, код и список именованных сущностей в любом виде должны лежать на Яндекс.диске. Лучше не видео, видео не влезет.
1.2. Можно прислать ссылку на личный гит с отдельной папкой "Поисковые системы/Лабораторная № 2".
2. Каждое правило должно быть откомментировано - зачем оно нужно, какой вид сущностей оно извлекает. 
3. Вторую лабораторную начинаю принимать сегодня.
