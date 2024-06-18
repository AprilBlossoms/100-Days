# #100DaysOfCode - Seventh Attempt

Welcome to my seventh attempt at the #100DaysOfCode challenge! This repository will document my journey as I commit to coding for 100 days. Each day, I will update this README with my progress, challenges, and things I learned.

## Challenge Rules

1. I will code for at least one hour every day for the next 100 days.
2. I will tweet my progress using the hashtag #100DaysOfCode.
3. I will update this repository daily with my progress.

## Progress Log

| Day | Date       | Focus                | My Progress               | Challenges                | Lessons Learned               |
|-----|------------|-----------------------|---------------------------|---------------------------|---------------------------|
| 1   | 06/06/2024 | Tarot and Astrology Flask App | Got the login page to redirect to settings if the user hasn't set up their initial profile and notification settings. | Struggled for a bit, figuring out how to handle the individual notification settings, if the user has opted not to receive either in app or email notifications. Decided to just check if they have notifications enabled when handling notification creation, and then if they do we'll then check if they want that particular type of notification. That should work. I guess we'll see when we get to handling notifications | Sometimes simpler is better lol |
| 2   | 06/07/2024 | Learning Django! | Well, TERRIBLE progress in record keeping, as it is now 6/8 lol. But. well, terrible progress in Django as well. This is so much more complex than flask. Wtf is an app? Is that like a blueprint? Why don't we put the models all together? Soo many questions! So... back to the progress. I've created a project. I've decided (probably unwisely) to follow a learn django by building a blog tutorial, but instead of building a blog I'm going to create a Content Management app. I got the project set up, my first app added ('posts') and the model created. Then, when I went to run it again, I got a Page Not Found error. So, that was all the progress I made today. Not much. | So many. I' gonna watch some videos on Django and try to get a better grasp of how it works, becase I'm at a loss right now. And I installed django-ckeditor which apparently is no longer supported, so I had to uninstall it and install django-ckeditor-5, and then I couldnt migrate the updated model because the old migration had references to django-ckeditor, which was uninstalled. I got that figured out, but like I said earlier, then I got a page not found error so we're still stuck. I think I'm going to find a different tutorial. The django girls one is good, but I need a video I think. | Well, if I were responsible I'd say I learned that I should follow the tutorial, not try to build an entirely different web app with absolutely no knowledge of the framework I'm working in. But I'm not responsible. I haven't learned shit lol. Well, I learned how to create an app and a model. That's not nothing I guess. |
| 3   | 06/08/2024 | Learning Django | Figured out why my page wasn't loading.. I'd typed to extend from 'blog/base.html' but there was no blog directory. i'm not making a blog. Silly mistake lol. Watched more videos on Django and I think I have a better grasp of it, but really it's just Flask with a lot of extra steps |  | |
| 4   | 06/09/2024 | Learning Django | Got the log in and out and register functionality added and some basic styles added. It's not great looking, but I'm mainly focusing on functionality, styling comes next. I wish I'd have gotten father but I was having a lot of trouble focusing today. I'm happy with the progress I made though. | Wasn't sure the best way to set up the models so that I can have multiple attachments, that can be any type of file format, and a post can have multiple attachments, and then how to set up the forms that allow for this. Will be focusing on this more tomorrow. | |
| 5   | 06/10/2024 | Flask Project Skelton Creator and Content management app | Today was much more productive than yesterday. Got all the auth routes (login and out, register, password reset, settings, channel setings, etc) taken care of. Just need styling, but the functionality is there. Then I worked on a Flask Project Skeleton Creator, which was a bit tedious to make, but I'm really happy with the result | just some styling bs with the cms. The generator was more frustrating because I had to figure out how to handle the indenting, and how to remove the space from the blueprints so they arent importing with extra whitespace. Should be simple, but I struggled for a bit | .strip() is your friend when handling comma separated lists from user input lol |
| 6   | 06/11/2024 | Learning DearPyGui | Got a basic feel for the structure down. It's very different from like Kivy and Tkinter. Like, much more straightforward. I'm hoping that will make it easier to create a kind of complex app, but we'll see. | Trouble with a circular import with the navigation file had me scratching my head for a bit. Got a workaround by creating a screen_manager to help handle it, but it's a little clunky. Probably not the best way to handle it, but it runs so what are you gonna do | There's always another project! Especially when you're in the middle of three... lol |
| 7   | 06/12/2024 | pyStructify | I'm really feeling comfortable working with dearPyGUI. It's so straightforward and simple (in the best way). Today I set up a few screens and a screen manager for my app. I think it's coming along nicely. | Despite all that good shit I was talking, I did face a lot of issues. Number one, circular imports. Figuring out how to work around that took some time, but I think I've got a decent set up now. Number two, images. I wanted to set a logo as teh background image on the home screen and MAN was that a tale of trial and error lol. I do see some limitations with this GUI. It's actually in a lot of the things I love about it. Kivy and Pygame for example require a lot of legwork. Create the widget, give it a size, give it a position, then display it. With dearPyGui it's add_text("text!) and boom, it's on the screen. This is brilliant! And also a bit frustrating when I can't center or position things easily without knowing the exact pos I want it at. But stylings not my strong suit anyway, so I don't mind too much. | Once you start coding, the ideas really start flowing! I started with a basic flask project generator and have thought of so many additional features I'm so excited to implement! |
| 8   | 06/13/2024 | pyStructify | So much progress! Spent today working on my Preferences screen, added all the default starter code and added functionality that allows the user to update this code if desired. Also checks for a default directory upon opening and if it's not set, you're directed to the Preferences page instead of the home page. Lots of other little things. And then the styling. Went through like 5 different color schemes before I decided on one (more because I was tired of dealing with it than because it spoke to me but oh well). The themes are pretty cool, but I do find myself wishing there were more customizeable options. (Button text color for example, instead of creating a separate button theme and having to apply it to every button. Sigh.) | Not so much a coding thing but dealing with the styling was a bitch and a half. And I'm still not thrilled with it. | I AM NOT AN ARTIST |
| 9   | 06/14/2024 | pyStructify | realized I forgot several options when I created my preferences page. So I updated it to hav a tab for general settings and a tab for flask settings. | no real trouble setting this stuff up, just frustration redoing it all lol | patience is key lol |
| 10  | 06/15/2024 | pyStructify | got all my links reset and updated my restore defaults button to behave differently depending on which defaults were restored (flask or general) | more tedium. had a bit of trouble figuring out how to handle storing the updated starter code so that it could be restored without restoring everything else. But once I got it the rest came easily |  |
| 11  | 06/16/2024 | pyStructify | tested all the restore default buttons and started building the page that shows once you click 'create project' (for flask projects. will be a different page if its not a flask projects. havent decided how i'm gonna do that one yet) | no real challenges today, just lots of repetition | patience, patience, lol |
| 12  | 06/17/2024 | pyStructify | ugh, not much. I've at least got the basic page and tabs added, but getting the project name, that should be stored with the tag "project_name" has proven to be more difficult than it should be. Also, there are three input boxes showing up at the top of my page. Did I put them there? Nope. Where are they coming from?! | I'm doing something wrong, clearly. But what? | |
| 13  | 06/18/2024 |                      |                           |                           |                           |
| 14  | 06/19/2024 |                      |                           |                           |                           |
| 15  | 06/20/2024 |                      |                           |                           |                           |
| 16  | 06/21/2024 |                      |                           |                           |                           |
| 17  | 06/22/2024 |                      |                           |                           |                           |
| 18  | 06/23/2024 |                      |                           |                           |                           |
| 19  | 06/24/2024 |                      |                           |                           |                           |
| 20  | 06/25/2024 |                      |                           |                           |                           |
| 21  | 06/26/2024 |                      |                           |                           |                           |
| 22  | 06/27/2024 |                      |                           |                           |                           |
| 23  | 06/28/2024 |                      |                           |                           |                           |
| 24  | 06/29/2024 |                      |                           |                           |                           |
| 25  | 06/30/2024 |                      |                           |                           |                           |
| 26  | 07/01/2024 |                      |                           |                           |                           |
| 27  | 07/02/2024 |                      |                           |                           |                           |
| 28  | 07/03/2024 |                      |                           |                           |                           |
| 29  | 07/04/2024 |                      |                           |                           |                           |
| 30  | 07/05/2024 |                      |                           |                           |                           |
| 31  | 07/06/2024 |                      |                           |                           |                           |
| 32  | 07/07/2024 |                      |                           |                           |                           |
| 33  | 07/08/2024 |                      |                           |                           |                           |
| 34  | 07/09/2024 |                      |                           |                           |                           |
| 35  | 07/10/2024 |                      |                           |                           |                           |
| 36  | 07/11/2024 |                      |                           |                           |                           |
| 37  | 07/12/2024 |                      |                           |                           |                           |
| 38  | 07/13/2024 |                      |                           |                           |                           |
| 39  | 07/14/2024 |                      |                           |                           |                           |
| 40  | 07/15/2024 |                      |                           |                           |                           |
| 41  | 07/16/2024 |                      |                           |                           |                           |
| 42  | 07/17/2024 |                      |                           |                           |                           |
| 43  | 07/18/2024 |                      |                           |                           |                           |
| 44  | 07/19/2024 |                      |                           |                           |                           |
| 45  | 07/20/2024 |                      |                           |                           |                           |
| 46  | 07/21/2024 |                      |                           |                           |                           |
| 47  | 07/22/2024 |                      |                           |                           |                           |
| 48  | 07/23/2024 |                      |                           |                           |                           |
| 49  | 07/24/2024 |                      |                           |                           |                           |
| 50  | 07/25/2024 |                      |                           |                           |                           |
| 51  | 07/26/2024 |                      |                           |                           |                           |
| 52  | 07/27/2024 |                      |                           |                           |                           |
| 53  | 07/28/2024 |                      |                           |                           |                           |
| 54  | 07/29/2024 |                      |                           |                           |                           |
| 55  | 07/30/2024 |                      |                           |                           |                           |
| 56  | 07/31/2024 |                      |                           |                           |                           |
| 57  | 08/01/2024 |                      |                           |                           |                           |
| 58  | 08/02/2024 |                      |                           |                           |                           |
| 59  | 08/03/2024 |                      |                           |                           |                           |
| 60  | 08/04/2024 |                      |                           |                           |                           |
| 61  | 08/05/2024 |                      |                           |                           |                           |
| 62  | 08/06/2024 |                      |                           |                           |                           |
| 63  | 08/07/2024 |                      |                           |                           |                           |
| 64  | 08/08/2024 |                      |                           |                           |                           |
| 65  | 08/09/2024 |                      |                           |                           |                           |
| 66  | 08/10/2024 |                      |                           |                           |                           |
| 67  | 08/11/2024 |                      |                           |                           |                           |
| 68  | 08/12/2024 |                      |                           |                           |                           |
| 69  | 08/13/2024 |                      |                           |                           |                           |
| 70  | 08/14/2024 |                      |                           |                           |                           |
| 71  | 08/15/2024 |                      |                           |                           |                           |
| 72  | 08/16/2024 |                      |                           |                           |                           |
| 73  | 08/17/2024 |                      |                           |                           |                           |
| 74  | 08/18/2024 |                      |                           |                           |                           |
| 75  | 08/19/2024 |                      |                           |                           |                           |
| 76  | 08/20/2024 |                      |                           |                           |                           |
| 77  | 08/21/2024 |                      |                           |                           |                           |
| 78  | 08/22/2024 |                      |                           |                           |                           |
| 79  | 08/23/2024 |                      |                           |                           |                           |
| 80  | 08/24/2024 |                      |                           |                           |                           |
| 81  | 08/25/2024 |                      |                           |                           |                           |
| 82  | 08/26/2024 |                      |                           |                           |                           |
| 83  | 08/27/2024 |                      |                           |                           |                           |
| 84  | 08/28/2024 |                      |                           |                           |                           |
| 85  | 08/29/2024 |                      |                           |                           |                           |
| 86  | 08/30/2024 |                      |                           |                           |                           |
| 87  | 08/31/2024 |                      |                           |                           |                           |
| 88  | 09/01/2024 |                      |                           |                           |                           |
| 89  | 09/02/2024 |                      |                           |                           |                           |
| 90  | 09/03/2024 |                      |                           |                           |                           |
| 91  | 09/04/2024 |                      |                           |                           |                           |
| 92  | 09/05/2024 |                      |                           |                           |                           |
| 93  | 09/06/2024 |                      |                           |                           |                           |
| 94  | 09/07/2024 |                      |                           |                           |                           |
| 95  | 09/08/2024 |                      |                           |                           |                           |
| 96  | 09/09/2024 |                      |                           |                           |                           |
| 97  | 09/10/2024 |                      |                           |                           |                           |
| 98  | 09/11/2024 |                      |                           |                           |                           |
| 99  | 09/12/2024 |                      |                           |                           |                           |
| 100  | 09/13/2024 |                      |                           |                           |                           |

## Resources

- [Official #100DaysOfCode Website](http://100daysofcode.com/)
- [#100DaysOfCode on Twitter](https://twitter.com/search?q=%23100DaysOfCode)

## Acknowledgements

A big thank you to the #100DaysOfCode community for the support and inspiration!

## Contact

- [Twitter](https://twitter.com/aprilmaycodes)
- [Website](https://www.aprilmaycodes.com)

Let's code, learn, and grow together!
