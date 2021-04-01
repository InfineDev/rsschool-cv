# The Markdown Task
## Dzmitry Dzemiashkevich
_This article is written using the Markdown markup language and devoted to **Mr. Dzmitry Dzemiashkevich**._
<br>
_I hope you would enjoy reading it!_

## My contacts
<pre style="font-family:helvetica">
Mail: <a href="mailto:appleinfinity@mail.ru">appleinfinity@mail.ru</a>
Gmail: <a href="mailto:dzmitrydzemiashkevich@gmail.com">dzmitrydzemiashkevich@gmail.com</a>
Telegram: <a href="https://t.me/dzmdzmdzmu">@dzmdzmdzm</a>
GitHub: <a href="https://github.com/InfineDev">https://github.com/InfineDev</a>
LinkedIn: <a href="https://www.linkedin.com/in/dzmitry-dzemiashkevich-9aa178200/">Dzmitry Dzemiashkevich</a>
Instagram: <a href="https://www.instagram.com/dzmitry_dzemiashkevich/">@dzmitry_dzemiashkevich</a>
</pre>
_I used a bit of HTML here because I didn't find how to compound the syntax highlighting and links using the Markdown._<br><br>


## Education
### __Secondary Education__
[Gymnasium №31](http://gymn31.minsk.edu.by/) in __Minsk__. Finished with __Gold Medal__ in June 2020.
GPA: 9.7/10.
In 2020 graduated from the [Gymnasium №31](http://gymn31.minsk.edu.by/) with a __Gold Medal__.
> _I strongly recommend you __not to visit__ the site of my Gymnasium because your PC might burn down._


### __Art Education__
In 2016 I successfully graduated from the __Children's Music School of Arts №19__ in Minsk. I play the __saxophone__, __block-flute__, and __piano__.
### __Higher Education__
>While preparing for Belarusian Central Testing I enrolled in the tutor courses __"100 баллов"__. Thanks to it and personally to __Mr. Евгений Борисович Ливянт__, I visited a few __EPAM TechTalks__ and after finishing the courses received the __recommendation letter__ for working at __EPAM__. One of the courses I visited was devoted to the basics of computer science and led by __Dmitry Samal__.<br>

* I passed Belarussian CT [central testing – Belarusian examination system] for __352 of 400__ points and entered __Belarusian State University__ for __Faculty of Applied Mathematics and Informatics__ in August 2020.<br>
* On the 13th of October 2020, I left BSU (due to political reasons) and entered __Vytautas Magnus University__ for __Informatics Systems__ in Kaunas (__Lithuania__).
* On the 19th of March 2020, I applied for the __Erasmus__ program and was accepted by __Regensburg University__ for studying there in the winter semester [August 2021 – January 2022] (__Germany__).


## Skills
I am convinced I started my IT career at school. The first important task I recall was __Computer Vision__ project with __OpenCV__ (__C++__). It was devoted to the Scientific-Practical Conference, in which I got the __3d Degree Republican Diploma__. My project was about recognizing colored objects on the image and navigating them in space.<br>

Then I learnt the basis of __C#__ and got the idea of __OOP__.<br>

The following and very important stage was the __Stanford Machine Learning__ course which I took on [coursera.org](https://www.coursera.org/). (developer: __Prof. Andrew Ng__, language: __Octave__)<br>

__Python__ is the language that I currently dedicate all my time and effort to. I have made a __Telegram bot__ and now I am testing it and work under adding AI tools. I tried myself in the following spheres of programming: __HTML "scrapers"__, __Computer Vision__, __Machine Learning__ predicting systems.<br>
I work with different modules, such as:

* NumPy
* Pandas
* Telebot
* Tkinter
* Multiprocessing
* ...

## Fresh Code example
```
import sys
sys.path.insert(0, "C:/Users/Администратор/.spyder-py3/READY/Bot/UI")
import time
import multiprocessing as mp
import SUI
import infinity

# This code starts 2 processes:
# 1. Telegram Bot API
# 2. Control window
# If the button in window pressed, the message "msg" appears in the queue "DestroyQ"
# Then the processes are closed

if __name__ == "__main__":

    # Queues
    DestroyQ = mp.Queue()
    UserQ = mp.Queue()

    # Server process
    I = mp.Process(target=infinity.E, args=(UserQ, ))
    # Window process
    U = mp.Process(target=SUI.execute, args=(DestroyQ, UserQ, ))

    # Processes start
    I.start()
    U.start()
    print("The server started working")

    # loop
    while True:
        msg = DestroyQ.get()
        # If button was pressed
        if msg == True:
            print("The processes will be destroyed.")
            I.terminate()
            U.terminate()
            if not I.is_alive():
                print("The Bot process was destroyed successfully!")
            if not U.is_alive():
                print("The Window process was destroyed successfully!")
            DestroyQ.close()
            UserQ.close()
            break
```

## Languages
* Russian: Native (C2+). 
I have a very deep knowledge of the Russian language and am able to check and edit texts for publication.

* English: C1-C2 
In order to confirm it, I took the “Business English C1-C2” subject and by the end of the semester [February 2021 – June 2021] I will have received a certificate.

* German (Deutsch): A1.
Currently, I study it at the University. Since I will go to Regensburg University the following semester, I plan to have the A2-B1 level by the end of this summer.
## Working experience
I was working as a servant at Astoria Riverside [premium Azerbaijan restaurant in Belarus] in summer 2019. The most guest I served were foreigners, so I talked to them in English and challenged my English skills in real life.

## Certificates and licenses
### School
* The Third-Degree Diploma of the Minsk Math Internet Olympiad.
* The Third-Degree Diploma of The Republican IT conference. Teamwork, together with Daniil Kulinkovich. (described above)
* The Second-Degree Diploma of The District English conference.
* Many other diplomas for team competitions among pupils. I used to be a captain of teams in Biology and History. Once I even had to memorize the voices of 20 birds and to recognize them afterwards:).
### IT
* Stanford Machine Learning Certificate on coursera.org. (described above)
* Grant from a WorkFusion company for the content “Neural Networks” which was conducted by IT-school “myfreedom”.

