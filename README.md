# ser321-assignment-4-threads-and-serialization-solved
**TO GET THIS SOLUTION VISIT:** [SER321 Assignment 4 Threads and Serialization Solved](https://www.ankitcodinghub.com/product/ser321-assignment-4-threads-and-serialization-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;97693&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SER321 Assignment 4 Threads and Serialization Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
<h1>Prerequisites</h1>
<ol>
<li>The assigned readings in module 4 on Canvas</li>
<li>Lecture videos from Canvas (or in person)</li>
<li>Running and understanding the examples listed on the Canvas page</li>
<li>Setup of a second device (second computer, AWS EC2, Raspberry PI) – see Canvas for details (should already be done)</li>
</ol>
<strong>Learning outcomes of this assignment are:</strong>

<ol>
<li>Apply sockets in an efficient way</li>
<li>Understand how to use threads</li>
<li>Understand how to work with shared state when using threads</li>
<li>Use different protocols to serialize data</li>
</ol>
<h1>Preliminary things (10 points)</h1>
I strongly advise you to work on Git and GitHub, to version control and also to practice.

Submit your code and all documents via your GitHub Assignment 4 directory.

Please watch the videos supplied with this assignment to get some more insight.

<strong>What you definitely need:</strong>

<ol>
<li>Structure: you will have to create two programs one for each Activity. So your assignment 4 folder should have two subdirectories, you can keep them as they are in the starter code. Each project needs a README.md and a build.gradle file.</li>
<li>md for each activity
<ol>
<li>A description of your project and a detailed description of what it does</li>
<li>An explanation of how we can run the program</li>
<li>Explain how to “work” with your program, what inputs does it expect etc.</li>
<li>A short video for each activity (2-4min) showing how you run the program, showing what works and briefly show your code.</li>
<li>Design your calls and user interaction in a way that they are easy. Remember we have many assignments to grade, design it so it is easy for us. There will be some requirements later you should fulfill.</li>
<li>Name the requirements that you think you fulfilled</li>
</ol>
</li>
</ol>
<h1>1&nbsp;&nbsp;&nbsp;&nbsp; Activity: Threads (30 points)</h1>
<h2>Background</h2>
For this activity you will convert a simple single-threaded server to a multi-threaded server. You will create 2 versions, one that allows threads to grow unbounded, and one that sets the number of allowed clients at a time to a fixed number. This is just a toy example to get started this should not take crazy long.

You are given starting code of a single-threaded server. There is a Client provided, which you should use for your implementation. It also specifies a protocol which you need to implement as is.

<h2>Given Code</h2>
You are given starter code for this assignment on Canvas:

<ul>
<li>java – a main program that accepts incoming client connections</li>
<li>java – a program that does the “business logic” of what the client requests • StringList.java – a simple wrapper class for a list of strings</li>
<li>java – a client which has the main functions and user interaction part which you should implement on the Server/Performer side</li>
<li>A build.gradle file which can run the base Client and Server, see Readme</li>
</ul>
You can have any package structure you want and add new classes etc. Important, you should only have 1 Readme and 1 build.gradle file for all 3 tasks. Each task (server) can be started separately and work only with the features described. You can make any changes in the given files you like, BUT the protocol should work as described in the code and README (and Task 1).

<h2>Task 1: Make Performer more interesting (11 points)</h2>
Presently, all the Performer does is add strings to an array. Make it more interesting by implementing the following protocol (code specifies something a bit different, go by this assignment text):

<ol>
<li>add &lt;string&gt; – adds a string to the list (presently what it does by default now) and displays the list (strings will be added to the end) – already implemented</li>
<li>pop – removes the top element of the list and displays it. If the list is empty return</li>
</ol>
“null”

<ol start="3">
<li>display – displays the current list</li>
<li>count – returns the number of elements in your list and displays the number</li>
<li>switch &lt;int int&gt; – switch the elements at the given indexes. If one of the indexes is invalid return “null” (list does not change)</li>
</ol>
<h2>Task 2: Make the server multi-threaded (12 points)</h2>
You can add new classes here of course. Task 1 should still run as is!

<ol>
<li>Name this server class “ThreadedServer”</li>
<li>Allow unbounded incoming connections to the server.</li>
<li>No client should block.</li>
<li>The shared state of the string list should be properly managed.</li>
</ol>
<strong>Task 3: Make the multi-threaded server bounded (3 points) </strong>You can add new classes here of course. Task 1 and 2 should still run as is.

<ol>
<li>Name this server class “ThreadPoolServer”.</li>
<li>Only allow a set number of incoming connections at any given time. How many should be specified when calling the program through Gradle.</li>
<li>Name this server class “ThreadPoolServer”.</li>
</ol>
<h2>Gradle (5 points)</h2>
<ol>
<li>In your ONE Gradle file there should be 3 Gradle tasks to run the different servers</li>
<li>Gradle should use default values for each task, per default host=localhost, port=8000 3. We should be able to run “gradle runClient” and it should also use the default values.</li>
<li>Running your different servers:
<ol>
<li>One for running Task 1: gradle runTask1</li>
<li>One for running Task 2: gradle runTask2</li>
<li>One for running Task 3: gradle runTask3</li>
</ol>
</li>
<li>Provide a detailed Readme.md file in your project, which tells us how to run each task and a description of which parts you accomplished of the requirements.</li>
<li>Make sure you include your screencast here as well, one screencast for all 3 parts not longer than 4 minutes.</li>
</ol>
<h1>2&nbsp;&nbsp;&nbsp;&nbsp; Activity: Threads and Protobuf (60 points)</h1>
A simple multi-player game using Protobuf as protocol.

<h2>The Game</h2>
We want to implement and design a simple game, where users can play a simple Pair Guessing Game with similarities of Memory.

The server is the game host and is the only one knowing the original tiles for the game, a leader board and a log file. The server and clients communicate through a given Protobuf protocol. See protobuf files and the Readme in the given code.

<strong>YOU HAVE TO implement the given protocol as described the given proto file!!</strong>

Your code needs to work with our protocol exactly as defined in the Readme, if you change it then our client would not work with your server. Theoretically, everyone’s client should work with everyone’s server.

See the video on how the game might look like for more detailed information.

The points in the constraints section add up to more than 60 points, the extra points will be extra credit. You can basically choose which ones you fulfill. BUT it needs to be a playable game that makes sense and implements the protocol.

<h2>Constraints (60 points)</h2>
These are estimates, server and client should also not crash, it should be well implemented, readable, use good coding practices. If you do not do the above you might loose points even if the functionality is fulfilled.

<ol>
<li>The project needs to run through Gradle (nothing really to do here, just keep the Gradle file as is)</li>
<li><strong>(6 points) You need to implement the given protocol (Protobuf) see the Protobuf files, the README and the Protobuf example in the examples repo (this is NOT an optional requirement)</strong>. If you do not do this you will loose 15 points (instead of getting the 7 points) since then our client will not run your server for testing and thus basically your interface is wrong and not what the customer asked for.</li>
<li><strong>(4 points) The main menu gives the user 3 options: 1: leaderboard, 2 play game, 3 quit. After a game is done the menu should pop up again. Implement the menu on the Client side (not optional). So the client shows the menu, the Server does not send the menu options to the Client.</strong></li>
<li>(3 points) When the user chooses the option 1, a leader board will be shown (does not have to be sorted or pretty).</li>
<li>(2.5 points) The leader board is the same for all users; take care that multiple users do not corrupt it.</li>
<li>(2.5 points) The leader board persists even if the server crashes and is re-started.</li>
<li>(2 points) User chooses option 2 (play game) and the current game board is shown. 8. (5 points) Multiple users will enter the same game and will thus play the game faster. NOTE: The server will only run a single instance of the game at any given time. If a user requests a new game and a game is in progress, they will join the current game. See video for details.</li>
<li>(2 points) Users win after finding all matches, they get 1 point for winning.</li>
<li>(2 points) After winning the Client goes back to the main menu.</li>
<li>(2 points) Multiple clients can win together and each get a point for winning.</li>
<li>(3 points) A tile coordinate is a 2 character string with row first as letter followed by column as number, columns are one indexed (0 is invalid) e.g. tile = “d1”, row=d, column=1. You can assume no more than a 4×4 board size, so rows are a, b, c, d, columns 1, 2, 3, 4 – also keep in mind that row * column = even.</li>
<li>(3 points) You have a couple boards already given in the resources folder, you are allowed to change the format of these if you do not want the “|” or row column information in them to make turning tiles easier. That is up to you. When displayed on the Client the letters and column numbers should be displayed though!</li>
<li>(4 points) Client sends first tile and server evaluates if the request is valid and sends back the board with that tile unturned. Handle errors accordingly, e.g. out of bounds, tile already turned – use the “error” flag in response for errors.</li>
<li>(4 points) Client sends second tile (if first tile was success response) and server evaluates if the request is valid and sends back the board with that tile unturned. Handle errors accordingly, e.g. out of bounds, tile already turned – use the “error” flag in response for errors.</li>
<li>(2 points) Client presents the information well.</li>
<li>(2 points) After both turned tiles are shown user presses any key which will lead to the Client to just show the current board (with the two tiles if not matches turned back again).</li>
<li>(3 point) Game quits gracefully when option 3 is chosen.</li>
<li>(3 points) Server does not crash when the client just disconnect (without choosing option 3).</li>
<li>(4 points) You need to run and keep your server running on your AWS instance (or somewhere where others can reach it and test it) – if you used the protocol correctly everyone should be able to connect with their client. Keep a log of who logs onto your server (this logging is already included). You will need to post your exact Gradle command we can use (including ip and port) on the channel on Slack #servers.</li>
<li>(2 points) You test at least 3 other servers with your client. You should comment on their servers on Slack, this is how we will grade these two points. – this can be done up until 2 days after the official due date.</li>
<li>(3 points – extra) In my version the board on the client is only updated after they made a “guess”, change the implementation so that as soon as the server updates the board the client will get this information and will update the board and inform the user, e.g. client B makes a correct guess, so the board updates and all other clients will get the information about the new board right away.</li>
<li>(3 points) If user types in “exit” while in the game, the client will exit gracefully.</li>
<li>(2 points) When sending back an error DO NOT just use error codes but a descriptive message that the Client can print. Since others are supposed to be able to use your server they might not know your error codes, so print good messages.</li>
<li>Overall your server/client programs do not crash, handle errors well and are well structured. No extra points for this but you might loose up to 5% if this is not the case since your pograms should be robust at this point.</li>
</ol>
<strong>NEEDED</strong>: On your server always print the board with all tiles unturned, so we can play faster when grading. Make sure your program is robust with all possible inputs, we should not be able to break it and crash it. We will not be mean when running it but with using it to our best ability and basic “gaming” it should not crash.

<strong>Hints:</strong>

These are some tips you can take them or leave them.

<ul>
<li>Spend some time on the given code, make small changes to it, even if they are stupid. Just to get a feel of Protobuf. Especially with the repeated fields. Get the feel for protobuf before even continuing.</li>
<li>Start with the base functionality, e.g. just one task one possible answer and so on</li>
<li>Setup the thread first and not when the rest is done (I did it the other way and it was more painful to change)</li>
<li>Go little step by little step. I usually add one new request with dummy data, check if I receive it on the server. Then add the real data, check if I receive it. Then I parse it on server, check if that works. Then create response and send it to client, check if I receive it. I usually got a couple lines at a time, especially if it is new to you.</li>
</ul>
<h1>Submission</h1>
On Canvas submit your link to your Assignment 4 folder on GitHub and also submit the Assignment 4 folder on Canvas. Remember the Readmes and your screen casts.
