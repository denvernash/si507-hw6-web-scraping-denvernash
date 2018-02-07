SI 507/206 
Homework 6: Web Scraping & Beautiful Soup

Homework Objectives:
Understand the basic structure of HTML documents
Be able to use BeautifulSoup to extract data from web pages without an API

Supporting Material:
Beautiful soup documentation https://www.crummy.com/software/BeautifulSoup/bs4/doc/
HTML <img> alt Attribute
https://www.w3schools.com/tags/att_img_alt.asp

Starter Files
We have provided you with the following files:
hw6_part1.py
hw6_part2.py
hw6_ec1.py
hw6_ec2.py

Please use these python files as a template to add your code. You can chose to use functions or not. If you do chose to use functions, please make sure to call all functions at the end of your code (i.e. part1()), so when we run hw6.py, all outputs should print. 


Part 1 (10 points): Print some ‘alt’ tags
There are 10 images on the page http://newmantaylor.com/gallery.html. Some of them have “alt text,” which is the text that is displayed or spoken when the image can’t be displayed (because of browser limitations, or because someone is using a screen reader). Scrape this page and print out the alt text for each image. If there is no alt text, print “No alternative text provided!”

Your input will be a webpage url (i.e. http://newmantaylor.com/gallery.html) that you will pass in when you run the file.

Sample input:
$ python hw6_part1.py http://newmantaylor.com/gallery.html

Given the current version of the page, which will remain constant until after the deadline, Your output should look like this:

*********** PART 1 ***********
Mark's page -- Alt tags

Waving Kitty 1
No alternative text provided!!
Waving Kitty 3
Waving Kitty 4
Waving Kitty 5
Waving Kitty 6
No alternative text provided!!
Waving Kitty 8
Waving Kitty 9
Waving Kitty 10


We may test your code on a different version of gallery.html (a different url) that has different alt text. For example, it may be that the 8th image is missing alt text and the 7th images has the alt text “Waving Kitty 7.” There will still be 10 images though. You will receive one point for each correct alt text output.

Part 2 (10 points): Scrape Michigan Daily

For this problem, you will need to inspect the Michigan Daily page (https://www.michigandaily.com/) to figure out how to extract the “Most Read” headlines. It’s the part of the page that looks like this (as of 3:31 pm, Feb. 6, 2018):


And it should not surprise you to learn that the output from a program that scrapes these headlines should print out (as it did at 3:31 pm, Feb. 6, 2018):

Sample input:
$ python hw6_part2.py

*********** PART 2 ***********
Michigan Daily -- MOST READ

Students call CSG Campus Affordability Guide "out of touch"
Former Michigan Medicine physician under investigation for sexual misconduct
Report: Michigan coaching staff undergoing more shakeups
Let's Bitch About It: Football is boring and overrated 
University ranks second in total number of reported sexual assaults


Your code will be graded by pulling the current Most Read headings at the time of grading and comparing them to your output. 

Extra Credit 1 (2 points): Michigan Daily Top 10 for News, Sports and Arts
Utilizing a similar approach to part 2, scrape the Michigan Daily to extract the top 10 headlines for News, Sports and Arts for that day. By top 10, we are referring to the first 10 headlines. 

Your output should look like this (as of 3:31 pm, Feb. 6, 2018):

Sample input:
$ python hw6_ec1.py


*********** EXTRA CREDIT 1 ***********
Top Headlines

Top 10 Headlines: news
Provost launches new undergraduate education taskforce
AAPD recommends Skeeps lose liquor license
Democratic gubernatorial candidates talk tax abatements, charter schools and environment
WeListen fosters cross-party dialogue on immigration
New University academic programs seek to alleviate poverty, class inequality
Students, CSG move forward with improving affordability guide
Controversy surrounds city staff and police seats on police review board
MSU students, faculty push back against Engler appointment
Former Pentagon official leads talk on future of the Middle East
Biden talks hope in post-White House life at Michigan Theater

Top 10 Headlines: sports
Wolverines prepare for second Northwestern matchup in eight days
The continuous rise of Dakota Raabe
SportsMonday Column: Hanging on 
Michigan tops Minnesota in wild finish, 76-73
Wolverines haunted by missed opportunities, fall to Wisconsin
Michigan handles the pressure in win over Ohio State
Wolverines grind out a tough win against No. 15 Nebraska
Three takeaways from the Nebraska meet
Michigan finishes fourth at Stanford Invitational
Amid penalties galore, Michigan outlasts Wisconsin, 5-3

Top 10 Headlines: arts
Electronic duo Louis the Child headlining 2018 SpringFest
The eclectic ‘Man of the Woods’
‘Faces Places’ is an impressive celebration of life
‘Babylon Berlin’ creates a complex portrait of Berlin in the 1920s
Oscar Snubs: ‘Beach Rats’
Rae Morris takes a haunting step forward with ‘Someone Out There’
‘Farewell to the Horse’ tells a detailed cultural history 
Required Listening: Pavement’s ‘Brighten the Corners’ turns 21
Brit Bennett, Jane Hirshfield and their simply stunning writing
‘8980 Book of Travelers’: A cross-country journey seeking to unite our nation

When grading, we will check the top 10 headlines for each sector (news, sports, and arts), and check if your program outputs the same headlines. 


Extra Credit 2 (2 points) Re-sort Athletes by State
Scrape the NXR Midwest Regional Championships ( https://www.athletic.net/CrossCountry/Results/Meet.aspx?Meet=135827) for the 5,000 Meters Championship Race, and re-sort the list of athletes by state for both “Men’s Results” and “Women’s Results”. Print out the top 3 finishers from Michigan for each division, Men’s and Women’s.

Sample input:
$ python hw6_ec2.py

Your output should look like this:
Top 3 Women for Michigan: 
1. Athlete1
2. Athlete2
3. Athlete3

Top 5 Men for Michigan:
1. Athlete1
2. Athlete2
3. Athlete3

What to turn in on Canvas
A screenshot of your github repository after the last push to github (as done in homework 5)

Note:
Be sure to commit everything (and push!) to your GitHub repo. At a minimum, your repo should include the following files, which you have modified:
hw6_part1.py
hw6_part2.py
(optional) hw6_ec1.py
(optional) hw6_ec2.py
README.md

