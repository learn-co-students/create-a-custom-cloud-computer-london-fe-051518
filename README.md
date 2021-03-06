# Create a Custom Cloud Computer

In this first lab we're going to use the power of Flatiron School's
instructional environment (Learn, the thing where you click on lessons and
submit labs) to create a computer in the cloud.

Why create a computer in the cloud? We do this so that your, our student,
doesn't have to worry about setting up a coding environment. By helping your
workspace "live in the cloud" we assure you that you can work from wherever you
want: home, grandma's house, a library terminal, at work during a
lunchbreak. Here's how to take advantage of this "cloud computer."

Whenever you open to **this** lab and open up the learn IDE by clicking
the "OPEN IDE" <span
style="display:inline"><img src="https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/open_ide.png" alt="Button to open
IDE"/></span> button, you'll be presented with an integrated development
environment (IDE) hosted, for you, in the cloud on a virtual computer.

That sounded like a lot of buzzwords, but they all mean something, we
promise you :)

This is what we mean by a "computer in the cloud:" Somewhere, somewhere
that you're not responsible for, a computer is running and is providing
you this "IDE" to run code on that computer. It is saving your work and
as long as you have a network connection and a computer, _you can access
it_.

Now the IDE might look a bit scary at first, but in time you'll come to
view it as a reliable friend. You'll be learning more about its parts in
upcoming lessons.

![The LearnIDE, labeled](http://learn-co-videos.s3.amazonaws.com/welcome/ide-components.png)

## Experiencing Your Custom Cloud Computer's "Statefulness"

What's really exciting is that this cloud computer is "stateful."
That's a fancy technologist word meaning that if you close the tab suddenly or
the computer you're using catches fire or all the Wifi in your city goes down,
**the information on your cloud computer is completely safe!**

Let's test it out!

Open up the IDE for this lesson by using the "Open IDE" button. If your IDE
is already open, then you can skip this step :).

Click in the Learn Terminal (the black part at the bottom) in the same way you
would select any window on Windows or MacOS. The white cursor should start
flashing letting you know that it's waiting for your input.

Type:

`$ date > remember_me.txt`

![Redirect date command output to textfile](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/redir_date.png)

This will put the current date and time into a file called `remember_me.txt`
You can select this file from the "File Browser" at left and see that your
file contains the date, time, timezone and year. It should look something like:
`Tue Mar 27 16:40:58 UTC 2018`.

Now, after you read this paragraph, you're going to close this tab!

Remember, because your cloud computer is _stateful_ we've
already saved that development space _for you_! You're not going to lose anything.
Accordingly, we should expect `remember_me.txt` to be present and to have your
data. You can restore a closed tab by using (⌘ + Shift + T).

Try it out now! We'll wait.

You're back! Glad to see you. Re-open the lab with the "Open IDE" button.  Take
a look at your `remember_me.txt` file and you'll see that it has the date and
time from _before you closed the tab_. This means that you can use cloud computer as a
private web development environment.  We think it's very cool and hope you will
too.

![Resurrected tab has previously stored date output](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/content_of_remember.png)

## Basic Web Server

Your Custom Cloud Computer also ships with a web server. Typically to see what
a website under development looks like you have to "deploy" the site to a
remote server with a real internet address. We'll learn more about that later
in this class, but we've included a basic web server on your Custom Cloud
Computer.

This lab ships with a basic `index.html` file &mdash; you're going to be
creating a lot more of these files and will overwrite this basic file many,
many times in this class &mdash; so don't get too attached! When you start the
basic web server, the server will look for this `index.html` file by default
and "serve" it.

Activate the server by typing `httpserver`. It should look like this

![Basic httpserver launch](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/httpserver_command.png)

The `httpserver` will tell you how to access your Custom Cloud Computer's
webserver by offering you an address and a port.

In this example the address is `192.241.157.192` and the port is `53056`. This
server is available on the internet at `192.241.157.192` and this server is
listening at port `53056`. It's sorta like telling someone to deliver a package
to "85 Broad Street, New York, New York 10006" and then specifying "27th floor."

We don't need to understand the finer points of addresses and ports yet save 
to know that in order for a browser to find your cloud computer's web server,
we need to provide the full address and port specification to our browser.

Provide this address and port combination to your browser. You may have never
typed _numbers_ in your browser's URL bar before. That's OK, there's a first
time for everything and, as you may come to learn if you continue your exploration
of web programming, the names like `flatironschool.com` or `google.com` are
actually just human-friendly names placed on those numbers!

Let's look at what our web server is serving: type in the **address**, then
a colon (`:`) and then the **port**. The screen shot below shows what it looks
like on our test instance. Try it out for your computer and its web server.

![Output of index.html page](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/basic_index_html_display.png)

If you look in the Learn terminal you can see that we logged to the screen a
"hit" or a "web site request."

![Server output for the browser lookup](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/server_output.png)

Amazing! This line means that some computer at 204.148.42.142 at a certain
datestamp said `GET` me whatever's at `/` and the server responded `200` which
means "OK!"

To stop the web server type "CTRL + C." If you try to refresh the same page
you'll no longer get anythihng back because, well, you stopped the server.

## Conclusion

While you'll work through many labs and READMEs in this course, you can always
return to this lab and pick up where you left off. You can use this as a
staging computer for your "Portfolio Projects" or for a personal website about
yourself. We don't know where your creativity will lead you, but we're excited
to see what you do!

## Moving On


We need to do some housekeeping on this lab. Most labs will handle this for
you, but in this case, this isn't a lab that's testing something and that
"finishes" we need to tell learn that we've understood the expectations
of this lessons.

The following steps **have not been taught** and **you're not expected to understand them**.
If you have trouble following these steps or get confused **don't panic!** Your
instructor will be able to help you on the first day of class!

When entering the following steps, **don't** type in the `$` – that's a
typographical convention for showing "this is a command you enter in the Terminal."

Select the LearnIDE Terminal and enter the following commands:

1. `$ git add remember_me.txt`
2. `$ git commit -m'Added my remember_me file'`

Here's are two screenshots showing what this looked like on my computer:

![Commit output](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/commit_output.png)

Next, enter:

1. `$ git push origin HEAD:remember_me`

![Pushed branch output](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/pushed_branch_output.png)

Then, at the top of this lesson, find the "Octocat" icon. Octocat is the mascot
and logo of GitHub. Clicking on this icon will open a link to your copy of this
Lab in GitHub. Here's a picture to help you find it.

![Octocat icon](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/see_octocat.png)

In the new tab, we want to create a "Pull Request" for the `remember_me`
branch. Click the "Compare &amp; pull request" green button:

![Select create a PR for remember_me](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/select_branch_for_create_pr.png)

You'll be given another screen, but you need only click on "Create pull
request."

![Confirm Create PR](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/create_pr.png)

You should now see that you've completed a "Pull Request."

![Created PR Output Page](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/completed_pr.png)

Return to the lesson page (this page) and you'll see that the lesson is now complete:

![Finished lab signal](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/submit_button.png)

Mark the lab as complete by clicking on the grayed-out "READ" icon. Confirm
that you're done!

![Commit output](https://curriculum-content.s3.amazonaws.com/skills-front-end-web-development/create-a-custom-cloud-computer/mark_lesson_complete.png)

All done! While you might not understand all the steps of using `git` and GitHub yet, this is the process used by
thousands of developers worldwide _every day_: create push branches (e.g. `remember_me`), create PRs for the branch, merge it in. Consider this a brief tour of the future you're going to be a master of in very short order!
