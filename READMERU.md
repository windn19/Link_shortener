# Link shortener
The resulting link is shortened through the website Byt.ly. When you receive an already short link, it gives statistics by day (number of clicks)
###About Installation
The program is written in python3 and it is believed that it is already installed.
Then use pip (pip3 if there is a conflict with python2):
```
pip install -r requirements.txt
```
###Using:
The program is a console application. The command to run has the format:
```
python3 main.py [-h] [-l {CRITICAL,ERROR,WARNING,INFO,DEBUG,NOTSET}] link

positional arguments:
  link                  Enter link to verify

optional arguments:
  -h, --help            show this help message and exit
  -l {CRITICAL,ERROR,WARNING,INFO,DEBUG,NOTSET}, --logINFO {CRITICAL,ERROR,WARNING,INFO,DEBUG,NOTSET}
                        message level entry LOG(default: WARNING)

```
If you enter a long address, it displays a shortened link:
```
>>>python3 main.py http://ifserial.club/serials/drama/khoroshij_doktor_90/6-1-0-283

http://bit.ly/2JUrR1I

```
when entering a shortened link - displays statistics on it:
```
>>>python3 main.py https://bit.ly/2HwXQF9
Общее количество кликов: 2
17/06/2019 года по ней было 1 переходов
23/05/2019 года по ней было 1 переходов
```
### Project Goals

The code is written for educational purposes on online-course for web-developers [dvmn.org](https://dvmn.org/).
