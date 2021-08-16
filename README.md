<p align="center">
  <img src="https://i.imgur.com/sJzfZsL.jpg" width="154">
  <h1 align="center">InstaPy</h1>
  <p align="center">Tooling that <b>automates</b> your social media interactions to “farm” Likes, Comments, and Followers on Instagram
Implemented in Python using the Selenium module.<p>
  <p align="center">
    <a href="https://github.com/timgrossmann/InstaPy/blob/master/LICENSE">
      <img src="https://img.shields.io/badge/license-GPLv3-blue.svg" />
    </a>
    <a href="https://github.com/SeleniumHQ/selenium">
      <img src="https://img.shields.io/badge/built%20with-Selenium-yellow.svg" />
    </a>
    <a href="https://www.python.org/">
    	<img src="https://img.shields.io/badge/built%20with-Python3-red.svg" />
    </a>
    <a href="https://travis-ci.org/timgrossmann/InstaPy">
	<img src="https://travis-ci.org/timgrossmann/InstaPy.svg?branch=master">
    </a>
    <a href="https://www.github.com/timgrossmann/InstaPy#backer">
	<img src="https://opencollective.com/instapy/backers/badge.svg">
    </a>
    <a href="https://www.github.com/timgrossmann/InstaPy#sponsors">
	<img src="https://opencollective.com/instapy/sponsors/badge.svg">
    </a>  
    <a href="https://discord.gg/FDETsht">
	<img src="https://img.shields.io/discord/510385886869979136.svg">
    </a>
  </p>
</p>

[Twitter of InstaPy](https://twitter.com/InstaPy) | [Twitter of Tim](https://twitter.com/timigrossmann) | [Discord Channel](https://discord.gg/FDETsht) | [How it works (FreeCodingCamp)](https://www.freecodecamp.org/news/my-open-source-instagram-bot-got-me-2-500-real-followers-for-5-in-server-costs-e40491358340/) |   
[Talk about automating your Instagram](https://youtu.be/4TmKFZy-ioQ) | [Talk about doing Open-Source work](https://www.youtube.com/watch?v=A_UtST302Og&t=0s&list=PLa4P1NPX9hthXV-wko0xyxFpbhYZFkW7o) | [Listen to the "Talk Python to me"-Episode](https://talkpython.fm/episodes/show/142/automating-the-web-with-selenium-and-instapy)


**Newsletter: [Sign Up for the Newsletter here!](http://eepurl.com/cZbV_v)**   
**Official Video Guide: [Get it here!](https://www.udemy.com/instapy-guide/?couponCode=INSTAPY_OFFICIAL)**   
**Guide to Bot Creation: [Learn to Build your own Bots with the Creators of InstaPy](https://www.udemy.com/course/the-complete-guide-to-bot-creation/?referralCode=7418EBB47E11E34D86C9)**    
**Our Data Visualization Hands-On Workshop: [Learn to create insightful Visualizations from Scratch!](https://amzn.to/3gwWDNM)**   

<br />

**Learn Automation from Scratch: [The School of Automation](https://www.school-of-automation.com)**   
**Learn the Skills to build your own InstaPy: [Automating Social Media Interactions](https://www.school-of-automation.com/learn/p/automating-social-media-interactions)**.  

[<img src="https://static1.squarespace.com/static/5f71907917b093635185fc3e/t/5f9d03cec73af0034b6ffa3a/1604126514869/?format=1500w" width="250"/>](https://www.school-of-automation.com)


<br />

# Find the full documentation on [InstaPy.org](https://instapy.org)
**Table of contents**
- [How to install and run InstaPy](https://instapy.org/#installation)
  * [Installing InstaPy](https://instapy.org/#installation)
  * [Running Instapy](https://instapy.org/#installation)
  * [Updating InstaPy](https://instapy.org/#updating-instapy)
  * [Guides and tutorials](https://instapy.org/#guides)
    * [Video tutorials](https://instapy.org/#video-tutorials)
    * [Written guides](https://instapy.org/#written-guides)
- [Externals and additionals tools](https://instapy.org/#external-tools)
  * [Web Interface](https://instapy.io)
- [Running InstaPy on Docker](https://instapy.org/#docker)
- [Documentation of all Instapy's features](https://instapy.org/settings)
- [Support](https://instapy.org/#support)
- [Credits](https://instapy.org/#credits)

<br />

## Credits
### Community
An active and supportive community is what every open-source project needs to sustain. Together we reached every continent and most of the countries in the world!   
Thank you all for being part of the InstaPy community ✌️

<p align="center">
	<img src="https://i.imgur.com/XkxHcM7r.png" alt="InstaPy reach" width="500px"/>
</p>

### Contributors

This project exists thanks to all the people who contribute. [[Contribute](https://github.com/timgrossmann/InstaPy/wiki/How-to-Contribute)].

<a href="https://github.com/timgrossmann/InstaPy/graphs/contributors"><img src="https://opencollective.com/instapy/contributors.svg?width=890&button=false" /></a>

### Backers

Thank you to all our backers! 🙏 [[Become a backer](https://opencollective.com/instapy#backer)]

<a href="https://opencollective.com/instapy#backers" target="_blank"><img src="https://opencollective.com/instapy/backers.svg?width=890"></a>

---

> **Disclaimer**<a name="disclaimer" />: Please note that this is a research project. I am by no means responsible for any usage of this tool. Use it on your behalf. I'm also not responsible if your accounts get banned due to the extensive use of this tool.

### Test strategy

TODO set_quota_supervisor randomiser - activity needs to appear organic otherwise account will be penalised

```
NOTES:
- Always ask for feedback, use more than 4 words and always have emojis.
- Target active accounts, I use two unfollow methods.
  - The first will unfollow everyone who did not follow back within 12h.
  - The second one will unfollow the followers within 24h.


# login credentials
insta_username = 'xxx'
insta_password = 'xxx'

import random
from instapy import InstaPy
from instapy import smart_run

# get a session!
session = InstaPy(username=insta_username, password=insta_password, headless_browser=True)

# let's go! :>
with smart_run(session):
    hashtags = [‘oyuncu', 'bugün', 'elza', 'life', 'love', 
    'TagsForLikes', 'TFLers', 'tweegram', 'beautiful', 
    'woman', 'coffee', 'coffeetime', 'fashion', 'look', 'cool', 'me', 'stylish', 
    'swag', 'photooftheday', '20likes', 'amazing', 'smile', 'siyah', 'beyaz', 
    'follow4follow', 'like4like', 'woman', 'style ', 'todaysmood', 'animals', 
    'sundayfunday', 'acting', 'action', 'actresses', 'london', 'model', 'act', 
    'goals', 'sundayfunday', 'sundayvibes', 'sunday', 'la', 'newyork', 
    'turkey', 'beach', 'holiday', 'actors', 'loveyourself', 'bozdağfilm', 'oyuncu', 'actor', 
    'movies', 'shooting', 'elsaanna', 'loveacting', 'mandirmanjolaleddin', 'peyveste', 
    'elzaamani', 'bozdağ', 'bozdağfilm', 'millytv', 'ozbekistan', 'la', 'actor', 'actresslife', 
    'actress', 'loveacting', 'elzaamani’]
    random.shuffle(hashtags)
    my_hashtags = hashtags[:10]

    # general settings
    session.set_dont_like(['sad', 'rain', 'depression'])
    session.set_do_follow(enabled=True, percentage=80, times=1)
    session.set_do_comment(enabled=True, percentage=80)
    session.set_comments([
        u'What an amazing shot! :heart_eyes: What do '
        u'you think of my recent shot?',
        u'What an amazing shot! :heart_eyes: I think '
        u'you might also like mine. :wink:',
        u'Wonderful!! :heart_eyes: Would be awesome if '
        u'you would checkout my photos as well!',
        u'Wonderful!! :heart_eyes: I would be honored '
        u'if you would checkout my images and tell me '
        u'what you think. :wink:',
        u'This is awesome!! :heart_eyes: Any feedback '
        u'for my photos? :wink:',
        u'This is awesome!! :heart_eyes:  maybe you '
        u'like my photos, too? :wink:',
        u'I really like the way you captured this. I '
        u'bet you like my photos, too :wink:',
        u'I really like the way you captured this. If '
        u'you have time, check out my photos, too. I '
        u'bet you will like them. :wink:',
        u'Great capture!! :smiley: Any feedback for my '
        u'recent shot? :wink:',
        u'Great capture!! :smiley: :thumbsup: What do '
        u'you think of my recent photo?'],
        media='Photo')
    session.set_do_like(True, percentage=70)
    session.set_delimit_liking(enabled=True, max_likes=100, min_likes=0)
    session.set_delimit_commenting(enabled=True, max_comments=20, min_comments=0)
    session.set_relationship_bounds(enabled=True,
                                    potency_ratio=None,
                                    delimit_by_numbers=True,
                                    max_followers=3000,
                                    max_following=2000,
                                    min_followers=50,
                                    min_following=50)

    session.set_quota_supervisor(enabled=True,
                                 sleep_after=["likes", "follows"],
                                 sleepyhead=True, stochastic_flow=True,
                                 notify_me=True,
                                 peak_likes_hourly=200,
                                 peak_likes_daily=585,
                                 peak_comments_hourly=80,
                                 peak_comments_daily=182,
                                 peak_follows_hourly=48,
                                 peak_follows_daily=None,
                                 peak_unfollows_hourly=35,
                                 peak_unfollows_daily=402,
                                 peak_server_calls_hourly=None,
                                 peak_server_calls_daily=4700)

    session.set_user_interact(amount=10, randomize=True, percentage=80)

    # @bozdagfilm  @mendirman_official  @milliytvofficial 
    # TODO require all related images to post 
    # activity
    session.like_by_tags(my_hashtags, amount=90, media=None)
    session.unfollow_users(amount=500, instapy_followed_enabled=True, instapy_followed_param="nonfollowers",
                           style="FIFO",
                           unfollow_after=12 * 60 * 60, sleep_delay=501)
    session.unfollow_users(amount=500, instapy_followed_enabled=True, instapy_followed_param="all",
                           style="FIFO", unfollow_after=24 * 60 * 60,
                           sleep_delay=501)

    """ Joining Engagement Pods...
    """
    # https://blog.hubspot.com/marketing/instagram-pods
    # Not an effective engagement strategy
    # session.join_pods(topic='sports', engagement_mode='no_comments')
```