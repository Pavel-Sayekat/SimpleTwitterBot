## Abstract

This bot runs in the following ways.

1. Search tweets using `search_term` in Twitter.

2. Re-tweet the tweets.

In this example, `search_term` is `Cafe Miyama`,
and you can see how it behaves by checking the following account.

http://twitter.com/cafemiyamabot


## How to setup

1. Register your OAuth client on Twitter
      URL: http://twitter.com/oauth_clients
      NOTE: You MUST change permission settings to `Read & Write` if you wanna update via API. The default is `Read Only`.

2. Run `python register_pin.py` and use `CONSUMER_KEY` and `CONSUMER_SECRET` you got from the registeration.
      NOTE: Make sure you are now signing in Twitter as your Bot account when visiting a given URL.

3. Change setting variables (`CONSUMER_KEY` and `CONSUMER_SECRET`) in `main.py` to the given ones.

4. Run Google App Engine dev_server and visit the following URL
      URL: http://localhost:8080/cron/update
      * If you finish all of your setting, set `debug_flag` in `main.py` off.

5. Done!

Enjoy developing your own twitter bot!

YasuLab
yohei@yasulab.jp
