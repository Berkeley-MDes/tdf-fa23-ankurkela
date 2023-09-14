# Weekly Report #3 - Building a 3D Toiletry Holder 

FYI - check out my 3D printed stand which I forgot to share in the last update. 

<img width="800" alt="3d print phone stand" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/6a45b592ef4c01e50252c1b27ed60a8cfd6120ed/weekly-reports/IMG_8044.jpg
">

## Ideation and Sketching

Prior to this experience, I never designed something new in any 3D modeling software but I was eager to ‘learn by experimentation’ by modeling a custom 3D asset from scratch. I decided to create a toiletry holder as I recently moved to a new apartment and am struggling with an unorganized sink counter. To begin, I looked up images online for inspiration on what I could build.

I picked the design that I thought I could create parametric adjustments for in Grasshopper, and proceeded to sketch the design on paper before creating the model on the software. Sketching helps me understand the different parts or components of a 3D asset and activates my thinking process on how I can begin to design the model on Grasshopper. See the image below. 

<img width="800" alt="toiletry holder sketch" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/41888a544154b6d77e7925e4b8eca5add6f35060/weekly-reports/IMG_8045.jpg">

## Building the Model

I began with creating the outer boundary for the top and bottom “shelves” of the asset. In Rhino, I used the Curve tool to draw the outline then connected it to Grasshopper from where I could make more adjustments. In Grasshopper, I used the ‘Offset Curve’ and ‘Extrude’ tool to add thickness and height to my curve and connected both using the ‘Boundary’ tool. 

Next, I worked on creating the compartments within the rectangular part. One compartment had to be bigger than the rest and this was specifically designed to place my large tube of toothpaste, but for the rest I wanted the same size and the ability to easily configure the number of compartments in Grasshopper. To do this, I created a box, then deconstructed it to extract the individual lines that made up the length and width of the box. I calculated the distance of each line and used the ‘divide’ tool to split them into equal parts. Finally, I used the ‘Rectangular (RecGrid)’ tool to create a baseline grid that would divide my larger box into equal sized rectangles. 

Next, I created two side stands by following a similar process above of creating a curve and then using the ‘extrude’ tool to add height. I wanted to make sure the stand height and top shelf height were dependent on each other, so that you could easily adjust the height of the stand and the shelf would follow. By using the ‘solid union’ tool, I joined all the boxes involved in creating the bottom shelf and replicated that for the top shelf. Then, I used the ‘Move’ and ‘Unit Z’ tool to change the height of the top shelf. I connected the slider I used to adjust the height of the stand to the factor input for the ‘Unit Z’ tool. 

## Final Model (still aways to go!)

I could not find the time to 3D print the model before submitting the report; however, the final design is close to ready. There are still a few adjustments that need to be made to ensure the model will be printed correctly, and may require a review from a design specialist or instructor. You can find images of the inspiration design and custom model in Rhino below. 

## Personal Challenges and Speculations

Given that a lot of these software tools and methods were new to me, this project was a bit challenging and required a lot of trial by failure. I really hoped to build something that was personal and useful, and this required a lot of time spent in the Jacobs Makerspace, watching external Youtube tutorials, navigating online Grasshopper-related threads, and collaborating with my classmates. 

From the Computational Design Stack, the two challenges I took on was learning how to create equal-dimensioned grids by layering a lot of mathematical logic to deconstruct shapes into lines. This involved a few hours of figuring out the right elements to use, and some assistance from a design specialist in the Lab. In addition, I learned how to connect two different curves or elements together so that they could work synchronistically. In the example mentioned above, I was able to connect the height of the stand to the Z unit position of the top shelf in order to customize the overall holder’s height. Even though I was not able to meet my eventual goal of 3D printing the stand, I learnt a lot about how one can use parametric modeling to create interesting 2D or 3D assets to solve for more complex design problems. 

As far as next steps go, I hope to complete the printing of the toiletry holder so I can actually use it in my bathroom! I anticipate that the 3D print may not be perfect, so I hope to test to see if there were any other adjustments I could make to the model to either simplify its construction or to use less material / resources in printing the 3D stand.  

The discipline of Computational Design allows designers to tackle complexity by building exploration and flexibility into their creation process. More specifically, computational design aligns incredibly well with the human-centered notion of iterative design. By building in a set of rules and sequence of operations into your design, one can easily and quickly change their product to meet new specifications. In the context of user testing, parametric modeling can close the gap between building and testing a product as new constraints are defined; similarly, it can provide the affordance for a user to customize a product to their specific needs. This level of modularity can minimize the amount of disruption in a design process where market needs are evolving at a rapid pace and in which the design recognizes or acknowledges the diversity of experiences in their users. Pairing this discipline with inclusive design, which takes into consideration the diversity of human experiences, is something that I am interested in exploring further in subsequent projects in this class. 

I would like to thank Cody Glen, Divya Srinivasan, LingXiu, Gia Kirk for their assistance in developing the assets above which facilitated my learning of using these new tools. 




# Weekly Report #2 - Grasshopper and 3D Printing. 

## Life as a Baby Grasshopper and Youtube Tutorials at 2x speed

This week, I focused on understanding the interface of Grasshopper and learning how to make adjustments to the parametric model of the cell phone stand. 

I was quite intimiated by Grasshopper as a software. It wasn't very intuitive, at the beginning, and I was lost on all the available features and ways to navigate. So I decided it might be important to learn the basics. I watched a youtube tutorial series, recommended by the instructor team, by Parametric Camp. These were really helpful in helping me understand how Grasshopper works at a fundamental level and understanding ways to customize the software interface to make it easier to use. 

<img width="800" alt="watching gh tutorial" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/de0d88caa7c09e300ba68675c234b69d8a99c3d7/weekly-reports/GH%20Tutorial.png">

Later on, I followed along with TJ's video tutorial of the simplified cell phone stand model. I watched half the video and recreated what TJ was doing on screen. I adjusted the model parameters to fit my cell phone dimensions and preferred viewing angle, and exported the file to 3D print. 

<img width="800" alt="watching gh tutorial" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/de0d88caa7c09e300ba68675c234b69d8a99c3d7/weekly-reports/GH%20Tutorial%202.png">


## My first 3D Print! 

At the Makerspace, I installed the Cura Software and the custom Jacob profiles to print on the Prusa printers. Cody, one of the design specialists, showed and explained the different steps involved in preparing for a print. He pointed out that most of the defaults configured by the embedded Jacob profile helped save many steps, and recommended to use a 'gyroid' infill to use less material and also to include strength & flexibility into the 3D strucutre. After configuring the specific parameters, Cody explained that the file which Prusa uses as input to print the 3D asset is in the form of G-Code (which stands for Geometry code). This file includes a set of different categories of instructions, which tells the "pointers" of the 3D printers which points to make rapid movements towards in the 3D plane space (G0), and where to cut, make incisions, or add material (G1). 

<img width="800" alt="configuring prusa print using Cura software" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/de0d88caa7c09e300ba68675c234b69d8a99c3d7/weekly-reports/Prusa%20Model.png">

The print is supposed to take 8 hours long, so it is still currently in the process of being completed. I hope to see the final product tomorrow. 

[![3D Printing in Action](https://img.youtube.com/vi/c0k_OWcKVv0maxresdefault.jpg)](https://www.youtube.com/shorts/c0k_OWcKVv0)

## Reflections on Computational Design for Larger Systems 

I really find it interesting that we can design variables that make necessary adjustments to an object based on the needs or constraints of another defined object. For example, in the cell phone stand example, we can configure a computational design that can take behavioral or action-based inputs of the user into consideration and automatically adjust the dimensions of the object to meet those constraints. I think this will be super critical when designing larger systems with many "objects". For example, in a city planning situation, a change to the layout of a street or an addition of something new (such as a bike lane) will affect the experience of many other pre-designed objects. It is important to consider the consequences of any change and understand how to optimize all systems so that they co-exist or co-depend. 




# Weekly Report #1 - Rhino, Laser Cutting, and Getting my Hands Dirty. 

## Hmm, maybe I can do this design thing?
Last week, I was introduced to Rhino (a 3D computer graphics / design software) as part of my graduate course in Technology Design Foundations. Previously, I used Blender (another 3D modelling software) but only got as far as designing half a donut in my first project. So, a lot of this learning is new to me. 

I began by watching tutorials on the basics of Rhino - understanding the interface, learning about different features and tools, and practicing to draw symmetrical lines and circles without using my cursor (thanks to the 'command' tool!). It took a few attempts to actually create something on my own. I discovered quite quickly that simply watching the tutorials would only get me so far, so I started to watch and create simultaneously. 

<img width="800" alt="watching and creating with rhino" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/14d2d29e48846e5bf416b9bc97571cec9b4fc5c2/weekly-reports/rhino%20practice%202.png">

## Trial by Fire 

<img width="400" alt="dog in fire" src="https://media.giphy.com/media/QMHoU66sBXqqLqYvGO/giphy.gif">

For our first assignment, we were asked to either laser cut or 3D print a computationally designed cell phone stand (for users to self-record videos). I never laser cut or 3D printed before, so I approached the project with a little nervousness (scared that I wouldn't know what to do or that I would make a mistake). I decided to just focus on executing a simple laser cut of the pre-designed 2D graphic. After rewatching a tutorial video on laser cutting and taking some diligent notes, I felt a lot more confident on what I had to do before stepping into the Lab. 

While at the Lab, I set up the Adobe Illustrator file and exported it to the laser cutting software on the Lab desktop. Along the way, some of my classmates pointed out that I needed to make a few adjustments, such as scaling the size of the 2D graphics to the appropriate size for my phone. After double checking all my settings and ensuring that my design would print in the appropriate place on my piece of scrap wood, I hit the green button! The process began and I was excited to see that it was being executed as expected (check out the video below!). Once the job was done, I switched off the exhuast of the machine and pulled my piece of scrap wood out. When I pulled it out, I realized it was cut but only on one side 🥲 I wasn't sure what I did wrong, so my classmates suggested making a few more adjustments. 

[![Laser Cutting in action](https://img.youtube.com/vi/iMp4A9I7sUwmaxresdefault.jpg)](https://www.youtube.com/shorts/iMp4A9I7sUw)


The second time around, I realized that doing a test cut is super critical if you want to save time and materials. We slowed down the speed at which the laser cut through the material and increased the quality settings of the cut. I quickly created a new file on Illustrator containing a small red rectangle, exported, and sent the print job. Success! The laser cut through the wood completely. I continued by making the same adjustment settings to my cell phone stand and printed again. The laser cut slower, which I learned helps dig into the material further since it spends more time on any specific point. I took the scrap wood out once the job completed, but it didn't cut through again 😭

I did not consult a design specialist since I was running out of time but I would do so next time. My suspicion was that the laser might not have been as sharp, as my classmates used the same settings on their respecitve laser cutters and were able to get a proper cut. Anyway, I decided to just use a box cutter to get the job done. I spent a little over 30 minutes cutting through the wood to get my final product and some wood-stained hands on the side.  

<img width="400" alt="resorting to box cutting" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/6831e2536589d810fd132789aaa7971d0ea5262b/weekly-reports/boxcutting.jpg">

## Hopping around in Grasshopper 🪲

Later on, I experimented a bit on Grasshopper because I was curious to learn how to customize files. I spent some time navigating the interface and got to the stage where I discovered the control panel where you could specify dimensions like your phone width, phone length, etc and the 2D file would adjust accordingly to fit your phone perfectly. The ability to modualarize a design file without needing to recreate the whole thing is a life-saver and I hope to continue playing around in this tool to understand how this works in practice, and then how to set up structures to do this for other 2D / 3D designs in the future. 

## Observations and Speculations 

### Other Contextual Parameters to Consider
In class, we discussed some of the parameters included in the extensive grasshopper file including phone dimensions, user body characteristics, and capturing a point cloud of the users' movements / activity. In addition, I think understanding the user's self-recording experience by documenting parameters like distance from phone, depth of vision, etc could help create a very personalized experience. In addition, I can imagine a user may want to adjust the phone to different angles while recording the same video. For example, some may require to do a close-in shot for a specific part of their video or a shot where the phone isn't meant to be perfectly flat. Therefore, including some flexibility in the design for the user to adjust the stand's modualirty will help them capture many different angles. 

### Adding AI to the Mix
We can leverage AI in analyzing vast amounts of self-recorded video data. If designing this product for scale, I would hope to test the product with a diverse group of creators, making sure to include a sample of people with different heights, range of motion, hobbies or activities, recording setting, and so on. Based on the data, my next step would be to leverage AI to categorize similar videos together and help define the common charactertistics of each category; in addition, challenging the AI to build a model that helps fit the needs of every individual or the individual who requires several unique parameters. 

While the product is in the hands of users, I think it would be important to set up data capture mechanisms to understand the users' live experience. If there is a way to document when the users activity exits the frame of the video or the number of times the user needs to make an adjustment of the stand, we can document areas of improvement for further iteration. 

'Till next time. See my boy in action below. 

<img width="800" alt="phone stand in action" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/5d3d29f498bb146f07a518fdbaa31c6c1edfb6b6/weekly-reports/phonestandinaction.jpg">
