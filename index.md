---
layout: page
title: Відсутній Семестр у Вашій CS-освіті
nositetitle: true
---

Під час навчання в університеті ви дізнаєтеся все про найсучасніші теми в CS, від операційних систем 
до машинного навчання. Проте одна важлива тема рідко висвітлюється 
і залишається на розсуд студентів: володіння 
інструментами. Ми навчимо вас опановувати командний рядок, користуватися потужним 
текстовим редактором, використовувати хитромудрі можливості систем контролю версій та багато іншого!

Студенти проводять сотні годин, використовуючи ці інструменти протягом своєї
освіти (і тисячі за їх кар'єру), тому має сенс зробити
досвід максимально гладким і безтурботним. Заволодіння цими інструментами не
тільки дозволяє вам витрачати менше часу розібратися, як змусити свої інструменти слухатись
вас, але й дозволяє розв'язувати проблеми, які раніше здавалися
неможливо складними.

Прочитайте про [мотивацію цього курсу](/about/).

{% comment %}
# Registration

Sign up for the IAP 2020 class by filling out this [registration form](https://forms.gle/TD1KnwCSV52qexVt9).
{% endcomment %}

# Розклад курсу

{% comment %}
**Lecture**: 35-225, 2pm--3pm<br>
**Office hours**: 32-G9 lounge, 3pm--4pm (every day, right after lecture)
{% endcomment %}

<ul>
{% assign lectures = site['2020'] | sort: 'date' %}
{% for lecture in lectures %}
    {% if lecture.phony != true %}
        <li>
        <strong>{{ lecture.date | date: '%-m/%d/%y' }}</strong>:
        {% if lecture.ready %}
            <a href="{{ lecture.url }}">{{ lecture.title }}</a>
        {% else %}
            {{ lecture.title }} {% if lecture.noclass %}[no class]{% endif %}
        {% endif %}
        </li>
    {% endif %}
{% endfor %}
</ul>

Відеозаписи лекцій доступні [на
YouTube](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J).

# Про курс

**Викладачі**: [Anish](https://www.anishathalye.com/), [Jon](https://thesquareplanet.com/), [Jose](http://josejg.com/).<br>

# Крім MIT

Сподіваючись, що ці матеріали будуть корисними не лише студентам MIT, 
автори поділилися курсом на наступних платформах:

 - [Hacker News](https://news.ycombinator.com/item?id=22226380)
 - [Lobsters](https://lobste.rs/s/ti1k98/missing_semester_your_cs_education_mit)
 - [/r/learnprogramming](https://www.reddit.com/r/learnprogramming/comments/eyagda/the_missing_semester_of_your_cs_education_mit/)
 - [/r/programming](https://www.reddit.com/r/programming/comments/eyagcd/the_missing_semester_of_your_cs_education_mit/)
 - [Twitter](https://twitter.com/jonhoo/status/1224383452591509507)
 - [YouTube](https://www.youtube.com/playlist?list=PLyzOVJj3bHQuloKGG59rS43e29ro7I57J)

{% comment %}
Some more URLs:

- https://news.ycombinator.com/item?id=27154577
- https://news.ycombinator.com/item?id=34934216
- https://www.reddit.com/r/learnprogramming/comments/nca1v3/mit_the_missing_semester_of_your_cs_education/
- https://www.reddit.com/r/compsci/comments/eyywv8/the_missing_semester_of_your_cs_education_from_mit/
- https://www.reddit.com/r/programming/comments/io7nq3/the_missing_semester_of_your_cs_education_mit/
- https://twitter.com/MIT_CSAIL/status/1349766980413263873
- https://twitter.com/MIT_CSAIL/status/1481676163491659780
- https://twitter.com/MIT_CSAIL/status/1581313961093484545
{% endcomment %}

# Подяки

Автори курсу дякують Elaine Mello, Jim Cain та [MIT Open 
Learning](https://openlearning.mit.edu/) за можливість 
запису відеозаписів лекцій; Anthony Zolnik та [MIT 
AeroAstro](https://aeroastro.mit.edu/) за аудіо та відеообладнання; Brandi Adams и 
[MIT EECS](https://www.eecs.mit.edu/) за підтримку цього курсу.

---

<div class="small center">
<p><a href="https://github.com/ua-missing-semester/ua-missing-semester.github.io">Source code</a>.</p>
<p>Licensed under CC BY-NC-SA.</p>
<p>See <a href="/license/">here</a> for contribution &amp; translation guidelines.</p>
</div>
