# Weekly Report #11 - The Beginning of the End 

After wrapping our project on fine tuning large language models, we are moving on to the final project of the semester. This project involves either continuing to build on any of the other projects in the semester or using the skills we've learned to start a new project. I decided to do something new. I will be exploring creating a recording device for self-reflection. My primary motivation for this project is based on my own personal challenges with self reflecting on a consistent basis, especially as it relates to my well-being and awareness of the different emotions and feelings I experience in a day. 

I began by exploring my concept and talking to some peers to gather their feedback to help build on the idea. So far, I've put together a high-level concept exploration including a short summary, the experiments I need to run (including testing of hardware, software, and data management), a list of materials, and a timeline with milestones. I hope to get some feedback from the instructor team on the feasability of my idea and refine the concept poster. 

An interesting article I came across in my research was a project conducted my MIT Media Lab on developing a piece of intelligent head glasses that could detect a lack of attention. The goal of the project was to provide haptic feedback through the form of sound and vibration in response to a detected drop in attention using EEG sensors that detect neural activity in the brain. I enjoyed the project's exploration into non-visual feedback, and that's inspired me to incorporate something similar in my own project as digital screens can take away from your immediate experience. 

This week in class we were visited by a hardware specialist and designer, Mohit Bhoite, who shared some fascinating prototypes he developed with electronics and microcontrollers. I really enjoyed how his prototypes were very intuitive and incorporated a sense of play, like the example below. I reached out to him to schedule a brief conversation to get feedback on my project. I'm hoping he can help me explore potential sensors and interactions to explore in accomplishing my goal. 

<img width="800" alt="hardware demo" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/1bb69f62def953f5cb1f44a677126bd929aac090/weekly-reports/IMG_8460.jpg">

[![Playful Hardware Demo](https://youtube.com/shorts/Vqrujy3l5jA?feature=share.jpg)](https://youtube.com/shorts/Vqrujy3l5jA?feature=share)

See my first draft of my concpet poster below: 

<img width="800" alt="concept poster" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/f0965588fe42884fee004b38612366d40c897c71/weekly-reports/A4%20-%201.png">




# Weekly Report #10 - My boy needs some tunin' 🛠️

Okkkkkk, what did we get upto this week? 

Well, I spent some time tinkering with my LLM and changed a few parameters to get it to perform how I hoped. I played around with the retrieval method and temperature. I decided to use an agentic method, which tasks another LLM to review the conversation and identify better search strings, to produce more contextual responses. And, utilized a low temperature which fit my specific use case where I didn’t want the model to run freely with creative expression but so to speak “stick to the script”.  

In addition, I noticed that I did not like the tone in which the model was speaking so I simplified the instructions to talk in a "straightforward and casual" tone. Before, I was providing keywords and emojis to use, but I felt that it used those excessively and the tone sounded a little too artificial. Even when I instructed the model to use keywords and emojis sparingly, it would still continue to overcompensate. 

After tinkering and testing my model, it was time to create a video for my final presentation. I sought inspiration from Peter's (co-founder of ZeroWidth) video on his homepage and had some fun recreating his nonchalant casual presentation of his business. I had to get creative and was able to get something pretty close to what I hoped. See some B-roll below. 

<img width="800" alt="b footage recording video" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/ae1c1681e80fa6146a5d446305d2f2a7c12eafac/weekly-reports/IMG_8427.jpg">


## Speculations and Ethical Considerations

With more time, I would train the model to assess my credentials through conversation, replacing the need for someone to check my resume or Linkedin. It would be cool to integrate APIs too for easy scheduling of meetings through Google Calendar or Calendly. 

This technology could automate mundane tasks, and integrate with code and APIs to improve efficiency and user friendliness. However, there’s a risk of misinformation with poorly trained models and a lack of transparency with complex systems (where multiple LLMs are involved). Ethical and intentional design is crucial for LLMs to effectively aid users while preserving their user autonomy. ‘Till next time.



# Weekly Report #9 - My new hype man 😤

This week, we moved on to another project that focuses on fine-tuning large language models. We got access to an AI platform called ZeroWidth that connects to foundational models like GPT and Google Bard, and allows to configure the model by adding specific instructions and knowledge chunks so that the model can respond to questions relevant to your specific use case. The power of fine-tuning models is to develop LLMs for specific use cases. For example, if you are a company that is looking to develop a customer service AI, you can fine tune an LLM to be trained on the customer service manual and instruct it to only provide advice or answer questions related to that content sphere. This reduces the risk of hallucinations and improves the specificity at how the LLM should be interacting with a specific audience. 

## Building a Mini Me 👨🏾

After following along a live demo of the ZeroWidth platform, I began to build the necessary components for training my model to answer questions related to my work in this class. In ZeroWidth, you can train your model using Instructions and Knowledge Chunks. Instructions are where you provide large-sweeping summaries on what you want your conversational AI to do, how you want it to talk, and where to pull detailed information from. In Knowledge chunks, you can host most of your content. Initially, I copied over my entire GitHub report to an Instruction but learned that this can lead to issues due to token limits. To prevent the model from running out of content to reference, it is smarter to host specific content in Knowledge chunks where a chunk is only called when it is relevant to the question. It performs this method through the process of identifying similar vectors, that is identifying matching key words in similar contexts. 

<img width="800" alt="knowledge chunks" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/74c41180025e0d1acb122ea460ad9808fe60cb4b/weekly-reports/Screen%20Shot%202023-10-26%20at%202.16.30%20PM.png">

After adding all the content from the Github and providing a simple instruction, I tested the conversational AI. It provided formal responses and captured most of my work, but it felt like it was just copy / pasting from my report and was not making its own connections or conclusions. I also did not love the tone as it felt a little presentational, and less conversational. 

<img width="800" alt="conversationalAI1" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/74c41180025e0d1acb122ea460ad9808fe60cb4b/weekly-reports/conversationalAI1.png">

I decided to add an instruction to have the model talk like me, including tone, common words I use, and even emojis! The result was hilarious and a little too on the nose. I became a little self-consious of the fact that I sound like a frat boy and decided to scale it back a bit. 

<img width="800" alt="conversationalAI2" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/73612a901411d6676f1f5aa72b28cfe5c2ed2ccf/weekly-reports/conversationalAI4.png">

I realized the model was not doing a great job of summarizing my project responses, and I realized that it could be due to the fact that there wasn't one specific knowledge chunk that included an overall summary of the projects I worked on in this class. Since I felt like that could be relevant to any question, I decided to add short summaries to my main instruction so that it could always reference my main work in the class. This turned out to be a great addition as I felt the responses were much more comprehensive. 

<img width="800" alt="conversationalAI3" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/74c41180025e0d1acb122ea460ad9808fe60cb4b/weekly-reports/conversationalAI3.png">

## Next Steps

Building on this model, my goal is to use this as a potential portfolio piece for anyone who is interested in learning more about my projects, deliverables, thinking process, and speculations. Thus, in addition to including information on TDF, I hope to also equip the model with an understanding of who I am and what my interests are. I'm thinking to include information like my previous work experience, my other projects, and my aspirations in terms of domains of work I'm interested in. I can pull this information from LinkedIn and my portfolio. That way, anyone can ask any questions to learn a little more about me.  



 # Weekly Report #8 - Mamma Mia, what a week :') 

I worked my butt off this week. 

<img width="800" alt="no sleep" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/be3cad72c87bb035ac8d8ec8705bcdc1aa216cde/weekly-reports/working.jpg">

## Not Enuf POWA!

Since the last entry, our group came together to refine, debug, and resolve many features to complete our prototype for the final presentation. Our first major challenge was to run many servos simulatenously. For our ghost robot, we needed multiple servos in order for it to have enough motor power and balance for the structure to move across space. We attempted to connect multiple servos to the same power source, but noticed that things were going more wrong. Once we added the second wheel, the photoresistor began giving alternating values in a way that didn’t make sense with the level of light in the room. The second motor also didn’t move at all. And, The original motor would spin, then stop, then spin again. Our diagnosis was that it had something to do with the diverted power to the second motor. 

How to get more power? We spoke with Jeff and Sudhu, and they recommended to add a Servo Featherwing Shield to our breadboard. The FeatherWing allows you to connect multiple servos that all will receive the same amount of power. In order to add the FeatherWing, we needed to learn how to sodder. After some demonstrations, I spent the next day in the makerspace soddering away and configuring our breadboard to its new setup to support multiple servos. In addition to a Servo FeatherWing, we also added a 5V Step-Up Voltage Regulator to convert the power from the USB / Battery and feed it directly to the FeatherWing's outlets.

<img width="800" alt="servo featherwing setup" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/be3cad72c87bb035ac8d8ec8705bcdc1aa216cde/weekly-reports/featherwing2.jpg">

## Coding Woes 

Once we got the hardware sorted, we had to revisit the software. Given the new hardware, the original code we wrote to move one servo would not work anymmore. I looked up template code from the Adafruit website and got help from Matthew to review the community library page on Particle - https://docs.particle.io/reference/device-os/libraries/a/Adafruit_PWMServoDriver/. After a few mind-numbing hours of running the code but not knowing what exactly to edit to make it work for our situation, I got help from Shm during our TDF class who literally changed one line of code and hooray both the servos started working. I learned that the call function for the FeatherWing looked slightly different and it also had a different syntax for how the servo rotated. Once the Servos were successfully rotating, I added the photo resistor sensor and updated the code to control the movement in response to lightness and darkness. 

See my edited code here - https://build.particle.io/build/652dd69301c674014a9a11b9

See the video of both servos running in response to light sensor input - 
[![Servo Simulation](https://youtube.com/shorts/oDPWbqIADOY?feature=share.jpg)](https://youtube.com/shorts/oDPWbqIADOY?feature=share)

Simulatenously, Christine from my team was working on constructing the prototype for the ghost - identifying the body and the wheels that the servos would be connected to. She also did some research into OLED for us to use as part of the 'Hunter' object. Originally, we wanted to communicate distance coordinates between the two devices to create a 'HOT' and 'COLD' interaction when the hunter was either close or far from the ghost. In talking to Vidit and a design specialist, we learned location finding was not possible without hardware extensive processes. So we pivoted to prototype a communication interaction between the two devices. 

In order to get two photon devices to talk to each other, we needed to first add both to the same team on Particle. Then, we reviewed online templates for the publish / subscribe feature on Particle and played around a few hours in code to try to get it to work. With help from LingXiu, we were able to successfully get the ghost to publish when it was moving or not moving, and the hunter would display the appropriate message, either "Ghost Detected" when moving or "Ghost Contained" when not moving. Using this new interaction, we pivoted our game to be one where your goal is to trap the ghost by placing a dark object over it to stop the movement. 

<img width="800" alt="OLED display" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/d7801bfa3176cafaa2631f419229150db8722a84/weekly-reports/ghost%20detected.png">


## Speculations - How Can We Make Coding Easier? 

In this process, I learned that things take time and a lot of trial and error. I never worked with microcontrollers before. I barely had any coding experience. I also had minimal prototyping experience with physical objects. Along the way, I learned that the best help you can get in those moments is to talk to other people and rely on their expertise to guide you on how to do something. Towards the end of the project, I became quite familiar with how the electronics worked on the breadboard and was able to help several other teams in configuring their breadboards in the right way if their code was not working; however, I was not able to get as far as I thought with coding. Although I worked on most of the coding elements in our team, the syntax for Particle still baffled me and I felt very uncomfortable writing code from scratch. Here is where I relied on ChatGPT, Youtube Tutorials, and available code on Particle. I wish we got the opportunity in class to learn the basic syntax of Particle so that we could be more independent in writing our code and understand how exactly the logic worked. 

Speculating on the future of these interface, I still believe this space is highly technical and can discourage many from learning more. The most difficult part is the lack of absence of feedback from hardware components and the cryptic error message when the code cannot compile or flash. I think there is an opportunity for improving these programs to be much more user friendly in the way they either educate users about how to write in specific syntax or describing in clear ways what part of the system is not working. I almost wonder if there can be a conversational interface at the beginning of running a new experiment where a user can describe thier goals of what they are hoping to accomplish, so that the program can intuit what parts of the code may be causing issues if the system does not work as expected. I also learned from Shm that when it comes to testing software, it is important to break apart a solution and test one thing at a time. For example, when we tried to publish / subscribe our interaction, we were testing the publish feature, the subscribe feature, and the OLED reliabily turning on, and it displaying the right message. So when it didn't work, we didn't know what the problem was. It's important to start with testing the first problem and iteratively understand when something is breaking down. 

I had a lot of fun with this and felt like a cute nerd when things went well. The moments of delight were precious. 

# Weekly Report #7 - BOO!

Our idea made a full pivot this week. We thought we were going to build a small robot that would help clean contertops, and now we are building a hide and seek game with a mini ghost robot. Based on feedback from class in TDF, we learned that our original idea might have been too complex given that it required many unique functional capabilities. We were encouraged to simplify and start by experimenting with what the different sensors could do as we formed a new project idea. 

## Experimenting with Sensors

We started with the Servo, which is a small motor that can rotate in different directions. Following one of the tutorials on GitHub, we learned how to use an accelerometer to control the servo motor. An accelerometer is a device that measures the vibration, or acceleration of motion, of a structure. We placed the accelerometer on our Photon and then oriented it in different directions to cause the motor to rotate simulatenously. 

After following the tutorial, we sought to rotate the Servo continuously in response to a light sensor. We found another tutorial seperately online to setup continuous Servo rotation, and used a photo resistor light sensor to control the movement. Using code from a previous tutorial in class around lighting LEDs when the light sensor detected lightness or darkness, we manipulated the code such that the Servo motor moved when it detected lightness and stopped when detecting darkness. 

<img width="800" alt="servo motor" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/971c8cc5c8fa22696222c9c10a7871a7a3fc65bb/weekly-reports/IMG_8237.jpg">

In the spirit of Halooween, this functionality gave us the idea of creating a game with a mini ghost. Esentially, the ghost would have wheels (attached to a servo motor) and would also be holding a light sensor. When the ghost detected light, it would trigger the motor and the wheels would move until it arrived in a dark area. Effectively, the ghost would be "hiding in darkness". To bring in the user to this game, we brainstormed the idea of creating another device called a 'hunter' which would provide feedback to the user whether they were near or far from the ghost. 

In order to do this, we started experimenting with distance sensors. The first one we started with was a 3V Ultrasonic Sensor which uses ultrasound to detect objects around its environment. The demo we built involved turning a LED light on or off based on whether the sensor detected some physical object within 10cm of its vicinity. We hope to expand this idea to get two specific objects to communicate their distance between each other and provide feedback to the hunter whether it is 'HOT' or 'COLD'. 

<img width="800" alt="ultrasonic sensor" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/971c8cc5c8fa22696222c9c10a7871a7a3fc65bb/weekly-reports/IMG_8248.jpg">

[![Ultrasonic Sensor Test](https://youtube.com/shorts/4bLjTI8PFow?feature=share.jpg)](https://youtube.com/shorts/4bLjTI8PFow?feature=share)

We are still running mini experiments with understanding how each of these sensors work, but we hope to begin integrating these systems soon to simulate functional experiences. It's been fun and delightful to see feedback when something you design works as expected, and I am curious how we can continue to have fun with these ideas in the project. 



# Weekly Report #6 - The Origin Story of Wipey

This week, we were assigned to groups for Project 2. Our group is working in the space of 'Clean Tech' with the goal to improve, simplify, or automate house cleaning chores. Our group decided that we wanted to focus on elevated surfaces, such as kitchen or bathroom counters, desks, etc. We met a few times to brainstorm potential ideas and technologies that we were interested in exploring. We decided to go forward with a "soft robotic"- like solution that could be flexible, maneuravable, and lightweight in order to adapt to different environments. 

I do not know a lot about soft robotics, so I conducted some preliminary research and documented notes on the key characterisics. First, I discovered this Ted Talk called "The incredible potential of flexible, soft robotics" by a biomedical engineer Giada Gerboni (https://www.youtube.com/watch?v=AI7M-JTC6_w). 

In her talk, Gerboni describes the existing problem with hard robots. Although they are designed to be highly precise and can perform specific tasks at scale, they are vulnerable to randomness and uncertainty in their environment. When deployed in the real world, hard robots often fail due to their rigidity and can pose safety concerns. The missing ingredient in hard robot design is that they do not posess 'embodied intelligence', that is the intelligence of their body and movements to adapt to any environment. Giada goes on to introduce and share examples of the growing discipline of soft robotics that aim to overcome challenges with hard robots. Often, soft robots use biomemetic principles to replicate the movements or behavior of actual organisms in the real world. Their applications have been seen in healthcare (to navigate complex surgical processes), accessing dexterous environments (for example, navigating a plumbing system, or a mining dig site). 

In addition to watching the TED video, I explored a few other channels and websites to expand my understanding. Something interesting I came across which I believe can be something useful for our project was this idea of pneumatic pressure, which uses pressurized gas like compressed air to generate pressure which can translate to something like movement. In this specific example of someone who built a worm-like soft robot, they used pneumatic pressure to enable the worm's movement. 

https://www.instructables.com/Inch-Worm-Soft-Robot/

<img width="800" alt="worm soft robot" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/e3ae02d5a25fcf97bc710d3ee8622ac6e6540f06/weekly-reports/soft%20robot.jpeg">

<img width="800" alt="pneumatic pressure robot anatomy" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/e3ae02d5a25fcf97bc710d3ee8622ac6e6540f06/weekly-reports/pneumatic.webp">


## Ideas and Constraints for Our Project 

Our group decided to build a self-cleaning soft robot called 'Wipey' that can move under and around objects on elevated surfaces and collect finer particles (like dust, small hairs, food crumbs, etc). We are looking to equip Wipey with visual or touch sensors in order to navigate its environment and a cleaning material like microber that can either naturally clean. The most challengeing constraints we will need to solve for include: 

* movement and interaction with objects (need to ensure it does not fall off the elevated surface or tip over an object)
* pressure application on surfaces in order to effectively clean
* portability and usability in order to easily remove cleaning fabric for washing and store in a safe and oragnized way

This upcoming week, we will begin experimenting by tackling each one of these constraints from top to bottom. 

<img width="800" alt="wipey" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/c325f753e3dcc1ced437314225faea1fd4965a71/weekly-reports/IMG_2056.png">

# Weekly Report #5 - The TL;dr on Microcontrollers

Mai-kro-kun-tro-lur-s. Basically, a tiny computer that can perform one task at a time. Sounds fancy but they are not too hard to wrap your head around.  

The three main parts include: 
* A CPU (central processing unit) that runs the whole operating system
* Two different types of memory: RAM (for temporary data storage) and ROM (read only memory that reads program code)
* Inputs / Outputs to connect different devices 

Microcontrollers are primarily used for applications that relate to IoT (Internet of Things). For example, a smart security system uses microcontrollers to facilitate the process of vision sensors detecting motion and responding by triggering the alarm bell. 

This week, I followed a few tutorials to perform some basic tasks on the microcontroller involving blinking lights. First, I simply set up my Photon to ensure that it securely connected to WiFi. Then, I borrowed some code from the tutorials provided online and ran a 'Hello World' code that prints Hello World a bunch of times on a Serial Debug Log. Next, I followed the blinking light tutorials to blink the internal LED (D7) on the photon device and an external LED by using a few wires and a resistor to prevent the LED from burning out.  

<img width="800" alt="hello world photon" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/ddefef85ae89704411f71e65e9b9a509652dcb1f/weekly-reports/hello%20world.png">

<img width="800" alt="blinking LED" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/ddefef85ae89704411f71e65e9b9a509652dcb1f/weekly-reports/blinking_LED.jpg">

## Identifying Project Topics 

In class this week, we divided into groups to brainstorm potential concepts or solutions for the next project. Our group was asked to brainstorm solutions for 'Environment'. I led the facilitation and we begun by first identifying problems to explore. After individually jotting down ideas on sticky notes, we grouped the ideas into common themes and voted for three to move forward to the next stage. Then, we performed the same tasks for potential solutions and discussed further how they could involve a larger digital ecosystem. 

Our final ideas: 
* A personal head covering that could limit exposure to pollution when bad air quality was detected in the atmosphere
* A smart survival kit to help faciliate the provision of basic necesseities in the case of an apocalyptic event
* A feature on food packaging that could allow a user to discover the supply chain journey of an item as part of their purchasing consideration (aimed at increasing awareness around the food cycle and unsustainable processes).

<img width="800" alt="brainstorming problems" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/ddefef85ae89704411f71e65e9b9a509652dcb1f/weekly-reports/white_board_brainstorm.jpg">

## Speculations 

I am looking forward to applying this technology toolkit to create an ecosystem or process targeted at performing a specific task. When designing such a system, I believe it is very important to consider how you can create feedback interactions for the user to understand what the system is doing. For example, for any sensor that is built into a system, what types of indication can we provide to the user that 'sensing is happening' or 'something has been detected' that is intuitive and appropriate for the context and environment. This is why it is critical to design these solutions based on research from user pain points and to involve the user in the prototype process. 

# Weekly Report #4 - Wrapping Project 1 

## That's a Wrap!

This week, I wrapped up Project 1. Last week, I showcased my final video to the class and recieved feedback on my design process and presentation. Overall, many classmates enjoyed the presentation and highlighted that I did well in communicating my entire process from inspiration to final concept. Primarily, my classmates hoped I could print the 3D model and compare the physical product to the outlined design specifications as there is a lot to learn when handing off from digital design to physical print. 

I spent time over the weekend compiling my final report and adding a few speculations on how computational design could be relevant to industry with fast-changing customer needs. One example I mentioned was how it can be applied to the automotive industry. For example, consumers are growing to expect a responsive driving experience. It would be interesting to see cars thats physical components are more dynamic wherein they can optimize their position depending on the speed or mode of the car. 

## Next on the Menu...

For the second project, we are exploring 'The Digital Ecosystem'. This is an opportunity to use microcontrollers to manipulate or functionalize a physical product or experience. This will involve a back-and-forth process of setting up the hardware components and programming specific instructions in software. I am excited to explore this space as it is very new but seems to have a lot of interesting applications. Specifically, I would love to explore the IoT space and explore ways to add intelligence to ordinary physical products that can be responsive to human communication via voice, touch, or vision. 

To begin, I set up my photon device by connecting it to my laptop. I followed the instructions provided to update the device and connect it to my home network. Next, I will look to get it connected to the Berkeley IoT ecosystem in order to work on the device on campus. See a few images of my process below. 

<img width="800" alt="photon microntroller update" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/aac54315bf02843b6cc03fa38ce6886d9b75c28d/weekly-reports/IMG_8086.jpg">

<img width="800" alt="digital ecosystem toolbox" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/aac54315bf02843b6cc03fa38ce6886d9b75c28d/weekly-reports/IMG_8087.jpg">



# Weekly Report #3 - Building a 3D Toiletry Holder 

FYI - check out my 3D printed stand which I forgot to share in the last update. 

<img width="800" alt="3d print phone stand" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/6a45b592ef4c01e50252c1b27ed60a8cfd6120ed/weekly-reports/IMG_8044.jpg">

## Going Rogue on Rhino

I would like to place a disclaimer that a lot of the information shared below is already included in my final report submission. I felt that both captured a recap of my progress and observations this week. 

Prior to this experience, I never designed something new in any 3D modeling software but I was eager to ‘learn by experimentation’ by modeling a custom 3D asset from scratch. I decided to create a toiletry holder as I recently moved to a new apartment and am struggling with an unorganized sink counter. To begin, I looked up images online for inspiration on what I could build.

I picked the design that I thought I could create parametric adjustments for in Grasshopper, and proceeded to sketch the design on paper before creating the model on the software. Sketching helps me understand the different parts or components of a 3D asset and activates my thinking process on how I can begin to design the model on Grasshopper. See the image below. 

<img width="800" alt="toiletry holder sketch" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/41888a544154b6d77e7925e4b8eca5add6f35060/weekly-reports/IMG_8045.jpg">

## Building the Model

I began with creating the outer boundary for the top and bottom “shelves” of the asset. In Rhino, I used the Curve tool to draw the outline then connected it to Grasshopper from where I could make more adjustments. In Grasshopper, I used the ‘Offset Curve’ and ‘Extrude’ tool to add thickness and height to my curve and connected both using the ‘Boundary’ tool. 

Next, I worked on creating the compartments within the rectangular part. One compartment had to be bigger than the rest and this was specifically designed to place my large tube of toothpaste, but for the rest I wanted the same size and the ability to easily configure the number of compartments in Grasshopper. To do this, I created a box, then deconstructed it to extract the individual lines that made up the length and width of the box. I calculated the distance of each line and used the ‘divide’ tool to split them into equal parts. Finally, I used the ‘Rectangular (RecGrid)’ tool to create a baseline grid that would divide my larger box into equal sized rectangles. 

<img width="800" alt="grasshopper visual programming" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/0ee8ab8b138e3709d3f5d9c9e730ebe4a971a604/weekly-reports/Screen%20Shot%202023-09-14%20at%2010.32.23%20AM.png">

Next, I created two side stands by following a similar process above of creating a curve and then using the ‘extrude’ tool to add height. I wanted to make sure the stand height and top shelf height were dependent on each other, so that you could easily adjust the height of the stand and the shelf would follow. By using the ‘solid union’ tool, I joined all the boxes involved in creating the bottom shelf and replicated that for the top shelf. Then, I used the ‘Move’ and ‘Unit Z’ tool to change the height of the top shelf. I connected the slider I used to adjust the height of the stand to the factor input for the ‘Unit Z’ tool. 

<img width="800" alt="3D toiletry stand" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/0ee8ab8b138e3709d3f5d9c9e730ebe4a971a604/weekly-reports/Screen%20Shot%202023-09-14%20at%2011.19.56%20AM.png">

## Final Model (still aways to go!)

I could not find the time to 3D print the model before submitting the report; however, the final design is close to ready. There are still a few adjustments that need to be made to ensure the model will be printed correctly, and may require a review from a design specialist or instructor. You can find images of the inspiration design and custom model in Rhino below. 

<img width="800" alt="3D toiletry holder" src="https://github.com/Berkeley-MDes/tdf-fa23-ankurkela/blob/0ee8ab8b138e3709d3f5d9c9e730ebe4a971a604/weekly-reports/Screen%20Shot%202023-09-14%20at%2011.31.04%20AM.png">

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
