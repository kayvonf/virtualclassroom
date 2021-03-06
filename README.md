# virtualclassroom

"Kayvon's Virtual Classroom" is an always-on, [ohyay-based](https://ohyay.co) virtual classroom kit that supports synchronous live lecture to up to 500 students (with recording), small student working groups (e.g., for breakouts or flipped classroom settings), and office hours.  The classroom experience is completely customizable, so you can modify the appearance of the UI or extend its functionality to meet your class' needs.  I have used this classroom to teach a number of courses at Stanford since Fall 2020. Please contact me (Kayvon Fatahalian) if you have additional questions.  

__If you want to receive communication about any updates to this tool in the future, please sign up [here](https://forms.gle/A8S8xJNQBtXeFaTZ9).__


## A quick example video of using the lecture hall

Read this [blog post](https://graphics.stanford.edu/~kayvonf/notes/virtualteachingkit/) explaining the basic components, or watch this eight-minute crash course video.

<p align="center">
<iframe width="720" height="405" src="https://www.youtube.com/embed/t7uTLH9DON8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>
  
## Getting Started

__Step 1.__ Create yourself a copy of the ohyay classroom, go the [project page](https://ohyay.co/space_gallery?itemId=ws_VQopSi1J) in the ohyay workspace gallery and press the "Explore" button.

<img src="images/setup/explore_screen.jpg" width="700" />

__Step 2.__ The classroom is now live! If you enter the site, you'll be on the main page, which links to a number of other rooms, such as your virtual lecture hall.

__Step 3. Go to the class configuration panel.__ If you look in the top left corner of the main menu, you'll see a red button labeled "Class Config" that will take you to the site's configuation pages.  Enter basic information about your course (the course's name, provide a vanity url that you can provide your students and course staff, etc.).  

For example here's me setting up a course called "Introduction to Computer Graphics" and giving the space the URL `https://ohyay.co/s/my-great-course`.  This is the link you will distribute to students and staff.

<img src="images/setup/screen_1_basics.jpg" width="700" />

__Step 4: Create yourself an office.__. Click the "Office Hours" tab in the configuration panel.  Give your office a name, and choose a template for what you'd like your office to look like. Below, I decided to have my office hours in Paris.  Click "Create New Office", and now you have a virtual office!  

<img src="images/setup/screen_2_office.jpg" width="700" />

__Step 5: Now explore your new virtual classroom.__. That's it! Your classroom is now live!  Notice that links to key rooms, like the main menu, the lecture hall, and now your office appear in the left navigation bar.  Those links will be there for easy navigation at all times.  Now head back to the main menu. Your main menu should look something like this.

<img src="images/setup/screen_3_mainmenu.jpg" width="700" />

## Giving Lectures: Using the Main Lecture Hall

Here's a video demonstrating the basic functionality of the lecture hall.

<p align="left">
<iframe width="720" height="405" src="https://www.youtube.com/embed/t7uTLH9DON8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

## Holding Office Hours: How to Use Your Office 

Here's a video demonstrating the basic functionality of your virtual office, and how you can use the office to conduct virtual office hours. In my courses I typically have each instructor and TA has create their own office.  This allows TAs to customize the look and feel of their office to their personality, and allows multiple virtual office hours to be going on at the same time. 

Watch the tutorial video below for a quick demo:

<p align="left">
<iframe width="720" height="405" src="https://www.youtube.com/embed/HoCbsnVO_f4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>
  
## Securing Your Classroom Space

By default, when you create a new classroom space, access control is off.  Anyone with the URL of the space will be able to access it.  

You can secure your classroom space in a number of ways: 
 * Password-protect the space (like a Zoom call)
 * Use SSO-based sign on from your university (This is how I operate at Stanford)
 * Explicitly provide a "allow list" of email addresses that can access the space. 

Unfortunately, I haven't implemented easy to use configuration panels for this.  You'll have to step into ohyay's workspace editor mode and change the security settings for the workspace yourself. (It only takes a few clicks, but please see ohyay's documentation of [security settings here](https://docs.ohyay.co/docs/password) for details of how to do it.

## FAQ

### Is it free?

Yes. This virtual classroom was created by me (Kayvon Fatahalian) and it is built on a platform called [ohyay](https://ohyay.co/).  The virtual classroom itself is "open source" in that anyone that creates a copy for their use has full access to edit the implementation of the space using the ohyay workspace editor.  Ohyay itself is a proprietary platform that is currently free for use.  At this time, ohyay states that it will remain free for educational use indefinitely.  Please contact ohyay directly if you have further questions about the ohyay platform.  (When you sign up for ohyay you'll be given access to their Discord channels, and the ohyay team is very responsive!)

You can also see ohyay's data privacy policy [here](https://ohyay.co/privacy_policy.html).

### Can I record lectures? How do I obtain a copy of the recorded video for students to view offline?

Yes. You can record *any room* in the virtual classroom space, and even multiple rooms at once if you want.  Ohyay provides the recorded video as a 1080p MP4 that you can download and then upload to regular courseware sites like Canvas or Panopto.  

However, there is no support for direct transfer of the video data to these third party sites. (For example, many instructors might be used to their Zoom recordings being automatically made available in Panopto via Zoom-Panopto integration.  You (or one of your TAs) will need to download the video file from your ohyay virtual classroom, and then upload it to the site that you will use to share the video for offline viewing with your students.

### What mechanisms does the virtual classroom provide for avoiding inappropriate behavior?

There are a number of mechanisms:
 * First, you should secure your space using a password or SSO authorization to limit access to only individuals in your organization.
 * At any time you can ban users from the workspace.  Just right click on their video (if they are on screen), or right click name in the left menu bar and select "ban user" from the pop up menu.
 * Clearing the lecture hall chat and question board is available via a single click in the "presenter tools" menu in the lecture hall.
 * Emoji reactions are displayed on screen anonymously (without attribution) to get students the ability to provide feedback without embarrassment.  But the configuration panel ("Advanced" tab) you can turn on logging of all emojis.  This option is OFF by default, but turning it on lets an instructor inspect the logs in case of inappropriate use of reaction emojis during class.  If you turn this option on, I recommend that you explicitly inform students that reactions are logged and could be attributed to them in the event someone audits the logs, since the rendering of reaction emoji's provides the sense that they are completely anonymous.
 * You can configure the space to limit reactions to a specific set of reaction emojis or, if you want to let students to be able to choose custom emojis (high recommended!) you can prevent posting of certain emojis.
  
### I'll probably stick with Zoom for lectures for simplicity, but can I use this space for office hours and group work? 

__By all means go for it!  These aspects of the space are arguably the biggest differentiators.__  I know a lot of folks that have mentioned that for various reasons (already have a teaching flow that they don't have time to adjust on short notice, school limitations on what software can be used in classroom settings, convenience of Zoom-Panopto integration, mobile support, etc.) they want to keep giving their lectures in Zoom.  But they really want the 24-7 class space for office hours and/or student working sessions. No problem at all... it's yours to do what you want with.
  
### What are the main gotcha's I should be aware of when considering whether to use this?

There are two warnings I'd like to give instructors thinking about using this virtual classroom space.
  
__Kayvon's advice #1: Check your screenshare setup as the first thing you do.__

My advice for prospective users is that the first thing you should do is go to the "lecture hall" and share your screen and see if the experience meets your needs.  Unlike Zoom or other native video conference apps, you won't see the ohyay browser window overlayed on top of your presentation mode slides.  To see your slides and also see the ohyay window at the same time, you'll to:
  * Set yourself up to present with multiple monitors
  * On a single monitor setup, use "present in window" so that both the ohyay browser window and your presentation are on screen at once. In these situations I like to use my iPhone or iPad to advance my slides. Even in a single monitor case, I personally love this setup and prefer it to Zoom, but it may take some getting used to for non-Zoom users
  * Instructors that are used to drawing on an ipad and screencasting to Zoom (e.g, whiteboard-centric math lectures), you'll make sure you can share this additional screen.

If you play videos in your slides that contain audio, you will need to take steps to make sure your audio is correctly shared.
  * On all platforms, Ohyay can share the presenter's screenshare audio if they screen share a browser tab (e.g., playing a youtube video, or using Google slides)
  * On Windows ohyay cna screenshare with audio if the presenter shares their full screen.
  * __ohyay cannot directly screenshare native app audio on OSX due to OSX security rules.__  On OSX it is possible to share native app audio by installing virtual audio devices like [Loopback](https://rogueamoeba.com/loopback/), but you will need to set this up in advance.  Alternative paths include 

__Kayvon's advice #2: Be aware that ohyay does not work great on mobile devices.__

One limitation of ohyay in Jan 2022 is that support for mobile devices is not great. Students should expect to attend class/office hours etc on a laptop/desktop computer. If accessibility via mobile phone is necessary for your class, my virtual classroom space is probably not a good solution for you at this time. 

### How many students can be in the classroom space at once?

Each instance of an ohyay workspace should be able to support 400-500 active users.

### How robust is this thing?

I personally have used variants of this classroom space during my teaching at Stanford for over four quarters now (100+ lectures), and have not seen a significant failure that prevented lecture from carrying on. Most problems that have occured (such as a students mic/camera not working) are related to students or staff using unsupported browsers. Ohyay also has convenient mechanisms in the app for anyone to "call for help" at any time, and during the work day the ohyay team is quite responsive in helping users resolve issues. In general, the ohyay platform itself has been used for many mission-critical virtual events well beyond educational/classroom use cases.

However, this virtual classroom template is created by me, and instructors should treat this as open source courseware that they choose to use at their down discretion.  I'll do my best to fix bugs and answer questions by folks that are trying to use it in their classes.


