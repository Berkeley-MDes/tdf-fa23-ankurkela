# Weekly Report #1 - Rhino, Laser Cutting, and Getting my Hands Dirty. 

## Hmm, maybe I can do this design thing?
Last week, I was introduced to Rhino (a 3D computer graphics / design software) as part of my graduate course in Technology Design Foundations. Previously, I used Blender (another 3D modelling software) but only got as far as designing half a donut in my first project. So, a lot of this learning is new to me. 

I began by watching tutorials on the basics of Rhino - understanding the interface, learning about different features and tools, and practicing to draw symmetrical lines and circles without using my cursor (thanks to the 'command' tool!). It took a few attempts to actually create something on my own. I discovered quite quickly that simply watching the tutorials would only get me so far, so I started to watch and create simultaneously. 

![rhino practice!](https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/14d2d29e48846e5bf416b9bc97571cec9b4fc5c2/weekly-reports/rhino%20practice%202.png)

## Trial by Fire
For our first assignment, we were asked to either laser cut or 3D print a computationally designed cell phone stand (for users to self-record videos). I never laser cut or 3D printed before, so I approached the project with a little nervousness (scared that I wouldn't know what to do or that I would make a mistake). I decided to just focus on executing a simple laser cut of the pre-designed 2D graphic. After rewatching a tutorial video on laser cutting and taking some diligent notes, I felt a lot more confident on what I had to do before stepping into the lab. 

While at the Lab, I set up my Adobe Illustrator file and exported it to the laser cutting software on the lab desktop. Along the way, some of my classmates pointed out that I needed to make a few adjustments, such as scaling the size of the 2D graphics to the appropriate size for my phone. After double checking all my settings and ensuring that my design would print in the appropriate place on my piece of scrap wood by using the pointing tool, I hit the green button! The process began and I was excited to see that it was being executed as expected. Once the job was done, I switched off the exhuast of the machine and pulled my piece of scrap wood out. When I pulled it out, I realized it was cut but only on one side 🥲 I wasn't sure what I did wrong, so my classmates suggested making a few more adjustments. 

![laser cutting in action](https://www.youtube.com/shorts/iMp4A9I7sUw)

The second time around, I realized that doing a test cut is super critical if you want to save time and materials. We slowed down the speed at which the laser cut through the material and increased the quality settings of the cut. I quickly created a new file on Illustrator containing a small red rectangle, exported, and sent the print job. Success! The laser cut through the wood completely. I continued by making the same adjustment settings to my cell phone stand and printed again. The laser cut slower, which I learned helps dig into the material further since it spends more time on any specific point. Took the scrap wood out once the job completed, but it didn't cut through again 😭

I did not consult in design specialist since I was running out of time but I would do so next time. My suspicion was that the laser might not have been as sharp, as my classmates used the same settings on their respecitve laser cutters and were able to get a proper cut. Anyway, I decided to just use a box cutter to get the job done. I spent a little over 30 minutes cutting through the wood to get my final product! 

![boxcutting](https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/6831e2536589d810fd132789aaa7971d0ea5262b/weekly-reports/boxcutting.jpg) 


## Hopping around in Grasshopper 
Later on, I experimented a bit on Grasshopper because I was curious to learn how to customize files. I spent some time navigating the interface and got to the stage where I discovered the control panel where you could specify dimensions like your phone width, phone length, etc and the 2D file would adjust accordingly to fit your phone perfectly. The ability to modualarize a design file without needing to recreate the whole thing is a life-saver and I hope to continue playing around in this tool to understand how this works in practice, and then how to set up structures to do this for other 2D / 3D designs in the future. 

## Observations and Speculations 

Consider: What other contextual observations would be useful to capture?

### Other Contextual Parameters to Consider
In class, we discussed some of the parameters included in the extensive grasshopper file including phone dimensions, user body characteristics, and capturing a point cloud of the users' movements / activity. In addition, I think understanding the user's self-recording experience by documenting parameters like distance from phone, depth of vision, etc could help create a very personalized experience. In addition, I can imagine a user may want to adjust the phone to different angles based on the specific activity they are performing. For example, some may require a close-in shot or a shot where the phone isn't meant to be perfectly flat. Therefore, including some flexibility in the design for the user to adjust the stand's modualirty will help them capture many different angles. 

### Adding AI to the Mix
We can leverage AI in analyzing vast amounts of self-recorded video data. If designing this product for scale, I would hope to test the product with a diverse group of creators, making sure to include a sample of people with different heights, range of motion, hobbies or activities, recording setting, and so on. Based on the data, my next step would be to leverage AI to categorize similar videos together and help define the common charactertistics of each category; in addition, to challenging the AI to build a model that helps fit the needs of every individual or the individual who requires several unique parameters. 

While the product is in the hands of users, I think it would be important to set up data capture mechanisms to understand the users' live experience. If there is a way to document when the users activity exits the frame of the video or the number of times the user needs to make an adjustment of the stand, we can document areas of improvement for further iteration. 

'Till next time. 

![phonestandinaction](https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/5d3d29f498bb146f07a518fdbaa31c6c1edfb6b6/weekly-reports/phonestandinaction.jpg)


Consider: What other evaluations of results would be useful to provide as feedback?


Consider: Are there points in the process where you think AI…
Could be used to assist?
Could be trained on input and output?
Other?





# Hello DES INV 202 Student!
Welcome to your new GitHub repository! 

If you’re new to GitHub, you can think of this as a shared file space (like a Google Drive folder, or a like a USB drive that’s hosted online.) 

This is your space to store project files, videos, PDFs, notes, images, etc., and (hopefully, neatly) organize so it's easy for viewers (and you!) to navigate. That said, it’s super easy for you to share any file or folder with us (your TDF instructional team) - just send us the link! 

The specific file that I’m typing into right now is the **README.md** for this repo. 
##### (💡 TIP: The .md indicates that we’re using [Markdown formatting.](https://www.markdownguide.org/cheat-sheet/)) #####
<h6> (💡 TIP 2: GitHub Markdown supports <a href="https://gist.github.com/seanh/13a93686bf4c2cb16e658b3cf96807f2"> <em>HTML formatting</em> too, including emojis 😄</a>, in case that helps!) </h6>

### :star: Whatever you write in your **README.md** will show up on the “front page” of your GitHub repo. This is where we’ll be looking for your [weekly progress reports](https://github.com/Berkeley-MDes/desinv-202/wiki/3.0-Weekly-Submissions). They might look something like this: ###
---
# Example Report 1 - Week of 08/21/2023 #
This week, I designed a cool phone stand made of rocks. Check out all my cool sketches and progress photos from this week below, etc., etc....

<img width="200" alt="Cool Phone Stand made of rocks" src="https://github.com/s-almeda/tdf-template-repo/assets/21287693/bc2f1864-af5a-456d-9a71-e1d80d51190c">

---

or, if you prefer, you can create separate files and link to them here, like so:

---
[Example Report 1](weekly-reports/example-report-1.md)
---

Either way, it's time to start making this space your own! If you want to save these instructions -- Don't worry, I already copied them over to another file for you [here.](welcomeREADME.md) So feel empowered to delete everything in this README.md and start documenting! 

sparkles,

your TDF TA, shm :sparkles:

PS: let me know if you have any questions!!

--- 
PPS: 
## Quick Links, compiled here for your convenience: ##

- [TDF Wiki](https://github.com/Berkeley-MDes/desinv-202/wiki) - the ultimate source for truth and information about the course and assignments
- [Google Drive Folder](https://drive.google.com/drive/folders/1OjFgu4llHn-2WayQFVWRKFyOkQ_WaQRx?usp=drive_link) - slides and other resources
- [bCourses](https://bcourses.berkeley.edu/courses/1528355) - where the grading happens


