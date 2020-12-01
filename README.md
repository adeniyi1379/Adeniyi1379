### Hi there 👋

<!--
**adeniyi1379/Adeniyi1379** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

Skip to content
Search...
120


68

19

120

Cover image for Easiest way to set up your Github profile page
Easiest way to set up your Github profile page
#portfolio #programming #webdev #tutorial
alekswritescode profile image
Aleks Popovic
Nov 27 Originally published at aleksandarpopovic.com ・10 min read
If you are a developer you probably have a GitHub account, and if you're like me your profile page is probably empty. I would even say barren. Utterly uninteresting? If that's true then you are at the right place, because in this tutorial I am going to show you some quick and easy tips to make your GitHub profile at least somewhat presentable.

If you prefer a video version you can watch me set up my GitHub profile page on YouTube and you can follow along:


Setting up the repo
To start off - you need to have a GitHub account, which I assume you do. You will also need to create a super-secret type of repo, which is just a repo with the exact same name as your GitHub account name. You need to initialize it as a public repo with a ReadMe file, because that is where all the magic happens.

We need to edit the readme file with some markdown and it will all show up on our profile page once we commit the changes. You can do all of these edits straight from the GitHub's file editor, or you can do it from your preferred text editor and upload the changes to your repo after you are finished. If you are unfamiliar with markup or need a quick refresher you can always reference this Markdown Cheatsheet on GitHub.

Using images
You can use images in your ReadMe file, just as you would in regular markdown/HTML. For ease of access you can opt to upload your images into the same repo as your profile ReadMe, and then you can access them like this:
![logo](BannerTransparent.png "banner")

// Logo is the image alt text
// BannerTransparent.png is the image we are showing (it needs to be on the same level as the ReadMe file)
// banner is the popup text you get on hover. Feel free to change these to fit your image.
or like this:
<img src="/BannerTransparent.png" alt="banner" />

// Regular HTML works in markdown
You can also align your images, as well as your other page elements, to left, right, or center, by using the "align" property (works only with HTML syntax):
<img src="/BannerTransparent.png" alt="banner" align="center" />

// Instead of "center" you can use "left" or "right"
Headings and text in markdown
To create headings you need to use the hashtag symbol - #. The number of symbols determines the heading level.
# Hi there and welcome to my GitHub page 👋 - level 1

## Hi there and welcome to my GitHub page 👋 - level 2

### Hi there and welcome to my GitHub page 👋 - level 3

#### Hi there and welcome to my GitHub page 👋 - level 4

##### Hi there and welcome to my GitHub page 👋 - level 5

###### Hi there and welcome to my GitHub page 👋 - level 6
For the main part of your profile you can write any sort of text without specific markdown syntax and GitHub will even give you some prompts, like "I am currently working on...", "My interests are..." and similar. You can customize that however you like, but I want to focus on some very useful tools that you can use to showcase your skills, tools, programming languages and other GitHub stats.

Set up custom tech badges
Most of us will want to display the technologies we use in our day to day work and there are two awesome tools you can use to create very nice and shiny badges for pretty much any tech you use. They are Shields.io and SimpleIcons.org and here is an example of what you can create with them.

Style: For the Badge

React
Angular
JavaScript
Sass
Gatsby
GraphQl

Style: Flat

React
Angular
JavaScript
Sass
Gatsby
GraphQl

Style: Flat Square

React
Angular
JavaScript
Sass
Gatsby
GraphQl

Style: Plastic

React
Angular
JavaScript
Sass
Gatsby
GraphQl

The syntax is really simple, and like I said, you can create a custom badge for any technology, language or tool you can think of. Here is what it looks like:
<img src="https://img.shields.io/badge/BadgeText-HexColor?logo=SimpleIconName&logoColor=ColorName&style=ShieldStyle" />
Let's break down all of the properties from that Url.

The BadgeText is your label or badge text. In my examples above those would be React, Angular, Gatsby etc.

HexColor is hex value of the color you want for your badge. If you want to stick with the official logo color for the tech/tool you are putting on the badge - you can find that on SimpleIcons.org. Just enter your tech in the search bar and you will get the logo image, logo name and it's hex color value. It's pretty sweet. While you are there make sure to grab the logo name as well, since that is what you need to use instead of the SimpleIconName in my example Url above.

Replace ColorName to a desired logo color. You can find the list of available color names on Shields.io.

Lastly, you need to switch ShieldStyle with one of the four values I mentioned above: plastic, flat, flat-square or for-the-badge. This will change the shape and look of your badge and you can see the examples above.

There are additional properties that you can change which I didn't use here, and you can find them on the official website.

Once you are done creating you badges you will probably want to put them in a single line in your GitHub ReadMe. To do this you need to wrap all image tags into a paragraph tag and it will work like a charm.

Here is the code example for what I used in my profile ReadMe:
<p>
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=white&style=for-the-badge" />
  <img alt="Angular" src="https://img.shields.io/badge/Angular-DD0031?logo=angular&logoColor=white&style=for-the-badge" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=white&style=for-the-badge" />
  <img alt="HTML" src="https://img.shields.io/badge/HTML-E34F26?logo=html5&logoColor=white&style=for-the-badge" />
  <img alt="Css" src="https://img.shields.io/badge/CSS-1572B6?logo=css3&logoColor=white&style=for-the-badge" />
  <img alt="Sass" src="https://img.shields.io/badge/Sass-CC6699?logo=sass&logoColor=white&style=for-the-badge" />
  <img alt="Gatsby" src="https://img.shields.io/badge/Gatsby-663399?logo=gatsby&logoColor=white&style=for-the-badge" />
  <img alt="GraphQl" src="https://img.shields.io/badge/GraphQL-E10098?logo=graphql&logoColor=white&style=for-the-badge" />
  <img alt="C Sharp" src="https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white&style=for-the-badge" />
  <img alt="Unity" src="https://img.shields.io/badge/Unity-000000?logo=unity&logoColor=white&style=for-the-badge" />
</p>
If you want to create contact cards/badges you can make them the same way. Like I said, you are not limited to just programming language logos. If you want them to link to your email or social media you will have to wrap them inside of a url tag, like this:
<a href="https://www.youtube.com/channel/UCu3RVedqyL5o776xyQlbyAw">
  <img
    alt="Youtube"
    src="https://img.shields.io/badge/youtube-FF0000?logo=youtube&logoColor=white&style=for-the-badge"
  />
</a>
<a href="https://twitter.com/alekswritescode">
  <img
    alt="Twitter"
    src="https://img.shields.io/badge/Twitter-1DA1F2?logo=twitter&logoColor=white&style=for-the-badge"
  />
</a>
<a href="https://www.instagram.com/aleks.popovic/">
  <img
    alt="Instagram"
    src="https://img.shields.io/badge/Instagram-E4405F?logo=instagram&logoColor=white&style=for-the-badge"
  />
</a>
<a href="https://www.linkedin.com/in/alekspopovic/">
  <img
    alt="Linkedin"
    src="https://img.shields.io/badge/linkedin-0077B5?logo=linkedin&logoColor=white&style=for-the-badge"
  />
</a>
GitHub Stats
If you are interested into setting up all sorts of different stats on your GitHub profile you should definitely check out this awesome repo. I will show you how to use a couple of cool widgets from there, namely - GitHub Stats Card and Top Languages Card.

Github Stats Card
There is an easy way to display all of your GitHub stats using this simple widget. You just need to take this line of code in markdown or HTML, enter your GitHub username and paste it into your ReadMe file:
![github stats](https://github-readme-stats.vercel.app/api?username=YourUsername)
<img src="https://github-readme-stats.vercel.app/api?username=YourUsername" />
Apart from entering your username, which is mandatory to see the stats, you can also enter other parameters to customize the display card. One of them is theme, which you can use to set up one of existing color themes. You can find the full list of them in the repo, but you can also customize all of the colors on your own, or even submit a new theme.

Here is an example of how you can customize the card to display stats for private repos, use a custom card title, show icons for each stat and use a custom color for text, title and icons:
<img
  src="https://github-readme-stats.vercel.app/api?username=alekspopovic&count_private=true&title_color=FD9047&icon_color=FD9047&text_color=0C2233&custom_title=Aleks+Popovic's+GitHub+Stats&show_icons=true"
/>
You can find the list of all parameters in the repo, as well as their potential values.

Top Languages Card
If you want to show your visitors what programming languages you mostly use in your repos there is an easy way to do that as well. Here is the code you need to enter into your ReadMe and don't forget to enter your own username:
![Top languages](https://github-readme-stats.vercel.app/api/top-langs/?username=alekspopovic)
or
<img
  src="https://github-readme-stats.vercel.app/api/top-langs/?username=alekspopovic"
/>
As far as additional parameters go you can use hide to block one or more languages from showing, langs_count to increase or decrease the number of languages shown (default value is 5) and layout=compact to display a one-line graphical spread with a percentage list.

Wakatime Week Stats
This one gets an honorable mention since I don't use Wakatime myself, but it looks very cool so I couldn't leave it out. If you never heard about it - Wakatime is an "open source plugin for metrics about your programming". It measures your daily productivity and tracks all sorts of stats about your programming languages and general coding habits.

To use it you will need to create an account on their official website and follow the setup instructions for your favorite IDE or text editor.

After that you can use it in a similar way to the previous two, but this time you will need to swap in your Wakatime username.
![Wakatime stats](https://github-readme-stats.vercel.app/api/wakatime?username=USERNAME)
or
<img
  src="https://github-readme-stats.vercel.app/api/wakatime?username=USERNAME"
/>
If you are using Wakatime please let me know what are your impressions and if it's helped you with your productivity. I'm really curious because I am considering to start using it myself.

Additional inspiration
Like I said in the introduction - my GitHub profile was empty just a couple of days ago. I was inspired to add stuff to it when I saw this Twitter thread by Jack Forge. I was scrolling through the multitude of responses, clicking to all the different profiles and I thought to myself - Damn, these people have really cool looking GitHub profiles. I want to make something like that.

Once I did that I wanted to share what I found and figured out with you. You can find some pretty nice profiles in there, but if you want some more examples of what can be done with just some markdown - you can check out this great repo with a list of awesome GitHub profiles.

If you want to check out my modest GitHub profile which features most of the examples I outlined in this tutorial you can find it here.

If you have any questions or comments you can reach out to me on Twitter and Instagram, where I also post interesting code tidbits and designs.

I also regularly upload React and web dev tutorials to YouTube, so if that's your cup of tea feel free to support me by subscribing to my channel.

Discussion
Subscribe
pic
Add to the discussion
 
heisdev profile image
dev
•
Nov 28

Check this out

Dynamic Animated Quote Generator


3
 
alekswritescode profile image
Aleks Popovic
•
Nov 28

Oooh, yes! I saw this one in several repos. It can give a profile a nice, poetic, touch. 😊


2
 
heisdev profile image
dev
•
Nov 28

true that


2
 
heisdev profile image
dev
•
Nov 28

This one is still under construction.. I saw they released v0.9


2
 
zoedreams profile image
☮️✝️☪️🕉☸️✡️☯️
•
Nov 27

i got some awesome widget on my profile,, feel free to fork and copy.

github.com/ZoeDreams

profile


2
 
alekswritescode profile image
Aleks Popovic
•
Nov 27

That's a neat profile page Kara. Thank you for sharing!


2
 
zoedreams profile image
☮️✝️☪️🕉☸️✡️☯️
•
Nov 27

Thank you. I love the stats counter flash back from the 90s geosites


2
Thread
alekswritescode profile image
Aleks Popovic
•
Nov 27

I considered using it on my repo, but there is currently no point as I hardly have any stars, or visitors. :)


2
 
manjunani profile image
Manjunatha Sai Uppu
•
Nov 29

Thank you so much Aleks


2
 
alekswritescode profile image
Aleks Popovic
•
Nov 29

You are welcome! I'm glad you found this useful!


2
 
memphis1983 profile image
Kieran
•
Nov 30

This is really amazing! Loved it! Thanks a lot, finally my github looks like a decent developer and not like a barren Sahara Desert LOL 🙏


2
 
alekswritescode profile image
Aleks Popovic
•
Nov 30

That is awesome Kieran! I'm really glad you liked it. 😊


1
 
chriswilkinsoncodes profile image
chris wilkinson
•
Nov 27

Time to refresh my profile! Thanks Aleks!!


2
 
alekswritescode profile image
Aleks Popovic
•
Nov 27

Thanks for the support Chris! Let me know if you make something using these tips, I'd love to see it. 😊


2
 
alekswritescode profile image
Aleks Popovic
•
Nov 27

Let me know if you make something interesting using these tips! I'd love to see your customized GitHub profiles!


2
 
gold2ragon profile image
Ming Gao
•
Nov 28

I wanted to learn about it. Thank you Aleks for the great post!👍


2
 
alekswritescode profile image
Aleks Popovic
•
Nov 28

I'm glad you liked it Ming Gao!


2
Code of Conduct • Report abuse
Read next
simonholdorf profile image
10 Awesome Github Repos Every Web Developer Should Know
Simon Holdorf - Nov 13

simonholdorf profile image
10 Things Front-End Developers Should Learn in 2021
Simon Holdorf - Nov 11

adrinlol profile image
Free React landing page template
Lasha Kakabadze - Nov 26

devsmranjan profile image
Golang for Web (Part-I): Build your first REST API with Golang & Fiber
Smruti Ranjan Rana - Nov 25

Aleks Popovic profile image
Aleks Popovic
My name is Aleks and my goal is to create interesting and practical web based projects in React and JavaScript that will help you learn and improve as a developer.
Follow
LOCATION
Belgrade, Serbia
JOINED
Jan 24, 2020
More from Aleks Popovic
Build Simple Timeline in React
#react #javascript #webdev #tutorial
How to build Instagram in React
#react #javascript #webdev #tutorial
How to build Netflix's Coming Soon page in React
#react #javascript #webdev #tutorial
<p>
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=white&style=for-the-badge" />
  <img alt="Angular" src="https://img.shields.io/badge/Angular-DD0031?logo=angular&logoColor=white&style=for-the-badge" />
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=white&style=for-the-badge" />
  <img alt="HTML" src="https://img.shields.io/badge/HTML-E34F26?logo=html5&logoColor=white&style=for-the-badge" />
  <img alt="Css" src="https://img.shields.io/badge/CSS-1572B6?logo=css3&logoColor=white&style=for-the-badge" />
  <img alt="Sass" src="https://img.shields.io/badge/Sass-CC6699?logo=sass&logoColor=white&style=for-the-badge" />
  <img alt="Gatsby" src="https://img.shields.io/badge/Gatsby-663399?logo=gatsby&logoColor=white&style=for-the-badge" />
  <img alt="GraphQl" src="https://img.shields.io/badge/GraphQL-E10098?logo=graphql&logoColor=white&style=for-the-badge" />
  <img alt="C Sharp" src="https://img.shields.io/badge/C%23-239120?logo=c-sharp&logoColor=white&style=for-the-badge" />
  <img alt="Unity" src="https://img.shields.io/badge/Unity-000000?logo=unity&logoColor=white&style=for-the-badge" />
</p>
Home Reading List Listings Podcasts Videos Tags Code of Conduct FAQ DEV Shop Sponsors About Privacy Policy Terms of use Contact Write a post
    
DEV Community – A constructive and inclusive social network. Open source and radically transparent.

Built on Forem — the open source software that powers DEV and other inclusive communities.

Made with love and Ruby on Rails. DEV Community © 2016 - 2020.
