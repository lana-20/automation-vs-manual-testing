# Automation vs Manual Testing

*What's the difference between automated and manual testing? What is 'automation' to begin with? Why do we care about automation? And what is the place of manual testing in an automated world?*

I can assume you already buy into the idea that automation is a valuable skill or concept. But let's take a few minutes to examine why this is in clear and concrete ways!

### What is automation?

<img width="400" src="https://user-images.githubusercontent.com/70295997/225440847-988c10a2-8cde-4dac-a6de-9ed4a195e883.png">

First, let's talk about what automation even is. I know that we all have an idea of this, however vague. Automation is robots, or software, doing things over and over again so that humans don't have to. Indeed, the word "automatic" comes from two Greek words that together mean something which can will, drive, or act by itself. This doesn't imply of course that anything which is automatic is somehow intelligent, just that, given the right setup, instruction, and context, it can perform actions on its own without human intervention, or with minimal human intervention.

Humans have been trying to get out of doing things by hand for a very long time. There are some quite old examples of **mechanical automation**, from a clock powered by the flow of water, to a weaving loom which can put together a piece of cloth on its own, using a set of punch cards as input to say what sort of pattern should be woven.

<img width="600" src="https://user-images.githubusercontent.com/70295997/225441307-43014bbe-bd07-4a8f-9b23-5f795de7c263.png">

But with the advent of the **industrial revolution**, simple mechanical techniques became a lot more powerful with the addition of steam and electricity which could be used as a power source. Now, 'automation' was more than just a thing for wild inventors and hobbyists. It became the backbone of social production. It was, of course, still very much intertwined with human work, and required an awful lot of intervention. Eventually, all of this innovation paved the way for a totally different type of automation---the electrical computer, built on top of hundreds and hundreds of electrical circuits. Now, mathematical calculations could be performed perfectly, correctly, and almost instantaneously.

<img width="600" src="https://user-images.githubusercontent.com/70295997/225442117-0840ab9e-a456-48f9-a958-79eddbd2666d.png">


This jump from the world of trains and horseless carriages to the world of information was really, really important for us. At one particular point in this history of automation, an MIT grad student named Claude Shannon took ideas that had existed for a long time, from philosophers and mathematicians like Leibniz and George Boole, and applied them to electrical circuits. With this insight, the idea of a binary digit, or a bit, was put to work in concrete ways, and all kinds of logical calculations could all of a sudden be performed at the speed of electricity. This brought the possibility of automation to information, which is the world we now inhabit. Everything we do on computers nowadays is fundamentally built off of these very basic insights, which is why it's really interesting and important to review them.

All software is therefore a kind of automation. As long as software has existed, software has needed testing, so it makes a lot of sense that when it comes to testing software, we would turn to the same kind of automation we used when writing that software. In fact, automated software testing is not a new thing. At first, testing software was more like writing mathematical proofs that the software did the right thing. Nowadays, software is too complex and open-ended to be proved correct in this mathematical kind of way. But even many of the patterns we find in regular old automated software testing today have their roots as far back as the 1970s. You could say that automated testing went "mainstream" in the 1980s and 1990s, and some of the tools we cover in this course, like Selenium, were invented in the early years of the 2000s! In taking this course, you are joining quite a long stream of people who have decided that one very useful way of testing software involves writing software.

When you stop and think about it, it is quite incredible that we can use the very same techniques for testing software as for writing it. This is all due to the immensely powerful framework summed up in the idea of the binary digit, which allows us to encode any information we want as a set of tiny electrical charges, and to decide that some of that information is not just data, but actually instructions for operating on other information. It's really quite amazing!

### The usefulness of automation

So that's all about what automation is. But what is the promise of it for us? Like the many people who have turned to automation before us, automation is always there to solve a specific problem, usually one that we have already figured out how to solve by hand. Software testing is a good example. It's usually pretty straightforward for us as human beings to be given some software and to figure out how to test it. I say usually because there are actually lots and lots of ways that make this much more difficult than we might otherwise think. But, in the normal case, since we are users of software, we can just go about using software and seeing what happens, as a way of testing it.

But at this point, we can run into various kinds of problems.

1. First, we could start to get bored, or tired. We could lose interest, and make mistakes, ultimately making our testing itself poor quality (which is an ironic thing, because testing is supposed to be helping to determine the quality of something else! So how can it do that if it itself is not of the highest quality?)
2. Second, we could realize that we could never in a million years test a given piece of software. There might be too many variables to test. Too many scenarios. Or the software itself might be so slow that we can only run through a certain number of testcases before we grow old and perish.
3. Third, we could have difficulty setting up an appropriate test environment. What if we want to test the software that powers an airplane? Do we need to become pilots ourselves in order to test it adequately? Or if we're not pilots, how do we set up a context where we can test the software?
4. Fourth, we could realize that we don't understand the software well enough to test it. Airplane software is another good example. If I'm not a pilot, and in fact if I'm not an aerospace engineer, how would I be able to determine if the software is even working correctly?
5. There are all kinds of problems like these that we could run into. Automation can't help us with all of them. But it can help us with problems like the 1st problem, where we get bored and tired. If the steps we take to test a given piece of software or a given scenario are repetitive and simple enough for us to get bored, then maybe can find a way to make a computer do those things instead of us! After all, software is just the flow of information, specified as code or data, and so there should be a way to write other software to provoke and observe the app that we want to test, for the purpose of testing it.

Automation can also help us with situations like the second problem we mentioned, where there are just too many scenarios to test, or they take too long to test. Using automation, we can speed up the process of testing, as long as the techniques we use work faster than a human. We can also usually scale up the number of automated testers much more easily than we can scale up the number of human testers, since the automated testers are just pieces of software.

So these are the main benefits of automation over manual testing:

1. Automation can reduce repetition or boredom by encoding the repetitive steps in software so that they don't need to be taken by humans anymore.
2. Automation can unlock a new level of speed or scale in testing.

Obviously, all of this changes the fundamental role of humans in the testing process. Are they still necessary anymore? Does automation make testing so cheap and easy that we don't need human testers? Not exactly.

### The place of manual testing

There are two ways in which humans are still very important even in a world of automated testing. The first is that the whole business of automated testing still needs to be run by humans. At least for the time being, testcases are not automatically generating themselves, nor automated test scripts written by themselves. This is being challenged, however, by work in the field of AI for testing. It's worth paying attention to developments in this field, because there are approaches being explored right now that attempt to discover some elements of app quality in a completely "hands-off" way, by using artificially intelligent testing bots. At the moment, these bots have somewhat limited scope and utility. All this to say, for some time to come, human authoring of automated test cases is an important role, just as is human development of application software.

The other way humans are important in testing is handling all the thinking that software cannot do for us. At the end of the day, software is written for humans, and humans must have some kind of input when it comes to judging quality, even if that input is minimal. There are also all kinds of cases that are difficult or non-obvious to consider, whether from a manual or an automated perspective. Choosing which scenarios to include in testing, for example, can be accomplished in conjunction with data and automation, but at the end of the day it is an app team that has to make the call.

All this to say, manual testing is not a practice which will ever completely disappear. It is one, however, which will adjust, and probably narrow considerably. There is currently no reason, and in the future there will be even less reason, for loads of humans to sit mindlessly tapping through the same scenarios just to test an app before launch. Ultimately, this is a good thing, because it frees up humans to do other kinds of work that is more creative. There will always be a place for humans in the process of developing tests, and in the process of figuring out what to test and how to test it.

In this course I'm teaching you some of the most useful automation skills for app testing, because I think these skills are currently useful, and will be useful for some time yet. But remember that, as with any skill, it's important to keep it sharp, and to keep an eye on developments in the field, so that you can be a part of shaping the future of the industry.

