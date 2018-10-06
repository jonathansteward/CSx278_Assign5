# Weekly Schedule Text/Email Messaging

With this project, I plan to add a text messaging application that will be able to pull from either one or multiple classes on Brightspace in order to display the entire weekly schedule of assignments/exams/homeworks in either a text message format. In addition to this, I would also like to add email functionality to this where an accessible link would be sent to the users phone that would allow them to open up a document on their computer with the information in a more readable format. Text messaging functionality exists for Brightspace already so I believe that I can leverage that existing functionality to extend it.

I chose to attack this specific problem because I find it tedious to check Brightspace frequently for assignment dates every week. It would be much easier if it could pull all due assignments for the week at once. In my interviewing of my target group, I found that a few of them did not even know that Brightspace had texting functionality at all. This is why I am choosing to extend this existing functionality in order to improve upon what is already there. The candidates that I interviewed were very receptive to the idea of extending the functionality. This is due to the fact that currently Brightspace only sends out emails a few days in advance for a given due date instead of allowing you to receive this information in text message or email form with all due dates for the week.  

All in all, I believe that I will spend around 5 to 6 days to complete this project. I plan to begin with the design phase, breaking down each individual part of the project in order to make sure that I am using best practices within each part. I plan to spend the most time on the design phase in order to make sure that I am doing exactly what is needed to drive my project to completion. Next, I plan to begin the development phase which I assume will be the shortest time that I spend on the project. At each phase of the application's development, I will test the specific part that I am working on in order to ensure that it is working properly before moving on to the next phase of the process. Overall, I believe that this project is feasible and will provide immense value to my clients (Vanderbilt students) by making it easier to become even more organized than they currently are. 

# Questions:
  1. Why do Vanderbilt students currently have to navigate to bright space to see what assignments are due this current week?
  2. How helpful do you think that having a text messaging application to solve this problem would be?
  3. How often do you need to check the due dates of assignments for the week?
  4. What other related problems do you believe that this application would need to solve?
  5. How often would you use this application?
  6. Would it be more helpful for the application to send you the URL of the bright space classroom page to log into or for you to send   the class that you wanted to see dates for and it sends you the dates in a text message with the assignment URLs?
  7. Do you think email functionality for this application would work?
  8. How soon would you want to see this application done?
  9. Should we include office hour checking as well in this application?
  10. Would it be useful to have the option to get a URL sent to your phone where it would pull up multiple classes at once with their due dates laid out?

# Answers:

## Question 1: 
  Because we don't have notifications sent to our emails automatically
  Because most teachers use it as a platform to post assignments so there’s no other option.
  I’m not sure why this is the only option. It forces students to have to either maintain their own schedules or constantly open Brightspace, both of which can be a bit time-consuming
  
## Question 2:
  - I think a text messaging application would be extremely helpful in order to solve the problem. It would allow students to be easily reminded of assignments that are on the horizon, without having to manually check. Furthermore, students tend to use their phones frequently, so it would also be very practical.
  - Pretty useful. I know a lot of people hate logging onto brightspace on their computers. However, I don’t mind it. 
  - It would be easier than using the bright space website because even though it has a mobile site, most people carry around their phones. Having texts would be a good way to get updates since it's fast and easy to access.

## Question 3:
  - check for due dates about 3-5 times a week.
  - Every day
  - Frequently because only major assignments have the due dates up on bright space's main page for my course

## Question 4:
  - I think it would be helpful if application could also provide the ability to notify when new grades have been posted or important class announcements.
  - Ideally every class’s interface would need to be the same. For example, some professors place assignments under “content” while others put it under “assignments” and it gets confusing. 
  - There should be like a countdown saying how many days left until it's due 

## Question 5:
  - I would use this application multiple times per week.
  - Maybe a few times a week. I like having a bigger screen to view assignments on as opposed to using my phone.
  - I would use it a lot since I have a lot of work

## Question 6:
  - I think it would be more helpful for the user to end the class he or she wants to see date for and then be returned the dates in a text message with assignment URLs.
  - I like the latter option. 
  - Send the class option

## Question 7:
  - I believe the email functionality for this application would work as Brightspace and VU Gmail has interconnectedness through YES.
  - Yes!
  - Yes

## Question 8:
  - I would like for this application to be created by next semester.
  - I don’t have too much of an issue with brightspace as of now, so there’s no rush for me. Ideally before I graduate in May.
  - By the end of the year

## Question 9:
  - Office hour checking would be very helpful for this application, but I would not force the user to receive information about it if they do not want to.
  - Oh I definitely think that would be a bonus.
  - Yes

## Question 10:
  - Yes, it would be useful to be able to pull up multiple classes at once with due dates listed out via a URL as it would consolidate information and be very efficient.
  - Absolutely. That way you could have a better idea of what your days are going to look like.
  - That would be very convenient
  
## Requirements
- Text messaging implementation (Finished)
- Students can join classroom through text message using a code (2 days)
- Instructor can update assignment schedule for week (2 days)
- Students can ping classroom to get full class schedule for the week in a text (3 days)

## Development Approach
I am choosing to use the agile methodology of software development style of development process because it will allow each piece of the application to be tested fully before moving onto another piece of the application. This will make it easier to make sure that all pieces of the application work well together without waiting until the end of the development process to test everything. 

In order to ensure that I am building something of value to the users, I asked a group of three students a list of ten questions that focused on the need to receive their weekly assignments in a form that would benefit their ability to design their weekly schedule at the beginning of the week. With this in mind and the requirement that we use the text messaging functionality, I came up with the idea of creating a classroom like tophat where the students use a join code in a text to join the classroom where the professor can add and remove the assignments due that week to receive the assignment updates. In addition to this, I will also make sure that the I am providing value to the users by updating the initial group of interviewees on any changes to the application. In addition to this, I brainstormed ideas and came to the conclusion that the one that I chose was the best one. After I interviewed my target group of students, I was sure that this would be the best idea to choose.

The phases of my project will consist of brainstorming, design, implementation, testing, and deployment. I covered the brainstorming phase above, but I will cover the other phases here. The design pattern that I plan to use in this instance to allow users to export their schedules is the Visitor pattern. I believe that the visitor design pattern will be best for this implementation because I plan to allow the classroom page to accept and authenticate a new user each time that they ping the server. The implementation will go as follows. Since the test messaging functionality has been created, it will be necessary to design the functionality of the classroom next. I will have a server send the students a join code when they reach out to the site. After they receive the join code, they will log in with it and this will trigger a text message to be sent back to the user with their weekly schedule. Lastly, I will design the ability for instructors to log into the classroom with simple SSO functionality. They will manually add assignments to the site with dates for that week so that students will be able to get them. In order to test the functionality, I will use the number that I created using Twilio to ping the server and expect a response. I will test the log in and add assignment functionality by logging into the page and attempting to add an assignment. Lastly, I will deploy the application after using the agile methodology at each development phase to make sure that all of the functionality is working properly. This will mitigate the risks of the application failing to work when being deployed.

I estimate that the entire application will take a week to finish completely. As listed in the requirements section of this document, I estimate that each of the individual parts will take 2 and 3 days to finish. I do not plan to make changes to my design process, but if necessary, I will overestimate that the entire process may take an extra day.
