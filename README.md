# comp90015-assignment-1--multi-threaded-dictionary-server-solved
**TO GET THIS SOLUTION VISIT:** [COMP90015  Assignment 1-  Multi-threaded Dictionary Server Solved](https://mantutor.com/product/comp90015-assignment-1-multi-threaded-dictionary-server-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115905&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP90015&nbsp; Assignment 1-&nbsp; Multi-threaded Dictionary Server Solved&nbsp;&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
&nbsp;

<strong>&nbsp;</strong>

<h1>Problem Description</h1>
Using a client-server architecture, design and implement a multi-threaded server that allows concurrent clients to search the meaning(s) of a word, add a new word, and remove an existing word.

This assignment has been designed to demonstrate the use of two fundamental technologies that have been discussed during the lectures:

<ul>
<li><em>Sockets </em></li>
<li><em>Threads</em></li>
</ul>
Hence, the assignment must make an <strong>EXPLICIT</strong> use of the two above. By explicit, we mean that in your application, sockets and threads must be the lowest level of abstraction for network communication and concurrency.

<h1>Architecture</h1>
<ul>
<li>The system will follow a client-server architecture in which multiple clients can connect to a (single) multi-threaded server and perform operations concurrently.</li>
<li>The multi-threaded server may implement a thread-per-request, thread-per-connection, or worker pool architecture. This is a design decision for you to make.</li>
</ul>
<h1>Interaction</h1>
<ul>
<li>All communication will take place via sockets. These sockets can be either TCP or UDP, however, keep in mind that all communication between clients and server is required to be reliable.</li>
<li>You are responsible for designing your own message exchange protocol. Some data formats that you may use include XML, JSON, Java Object Serialization, or you may choose to design your own.<strong>&nbsp;</strong></li>
</ul>
<h1>Failure Model</h1>
<ul>
<li>All communication between components has to be reliable. If you are using TCP, then the reliability guarantees offered by the protocol are sufficient. If you decide to use UDP, then you have to implement an infrastructure that offers reliable communication over UDP. For those of you with previous experience using TCP, using UDP may be a rewarding challenge.</li>
<li>It is expected that, on both the server and the client side, errors (by means of exception handling) are properly managed. The errors include the following:</li>
<li>Input from the console for what concerns the parameters passed as command line.</li>
<li>Network communication (address not reachable, bad data…).</li>
<li>I/O to and from disk (cannot find the dictionary file, error reading the file, etc…).  Other errors you might come up with.</li>
</ul>
&nbsp;

The application will be tested and validated against all these errors.

<strong>&nbsp;</strong>

<h1>Functional Requirements</h1>
<strong>&nbsp;</strong>

<ul>
<li><strong>Query the meaning(s) of a given word</strong></li>
</ul>
&nbsp;

The client should implement a function that is used to query the dictionary with the following minimum (additional input/output parameters can be used as required) input and output:

&nbsp;

<u>Input:</u> Word to search

&nbsp;

<u>Output:</u> Meaning(s) of the word

&nbsp;

<u>Error:</u> The client should clearly indicate if the word was not found or if an error occurred.&nbsp; In case of an error, a suitable description of the error should be given to the user.

<strong>&nbsp;</strong>

<ul>
<li><strong>Add a new word</strong></li>
</ul>
&nbsp;

Add a new word and one or more of its meanings to the dictionary. For the word to be added successfully it should not exist already in the dictionary. Also, attempting to add a word without an associated meaning should result in an error. A new word added by one client should be visible to all other clients of the dictionary server. The minimum input and output parameters are as follows:

&nbsp;

<u>Input:</u> Word to add, meaning(s)

&nbsp;

<u>Output:</u> Status of the operation (e.g., success, duplicate)

&nbsp;

<u>Error:</u> The user should be informed if any errors occurred while performing the operation.

&nbsp;

<ul>
<li><strong>Remove an existing word</strong></li>
</ul>
&nbsp;

Remove a word and all of its associated meanings from the dictionary. A word deleted by one client should not be visible to any of the clients of the dictionary server.&nbsp; If the word does not exist in the dictionary then no action should be taken. The minimum input and output parameters are as follows:

&nbsp;

<u>Input:</u> Word to remove

&nbsp;

<u>Output:</u> Status of the operation (e.g., success, not found)

&nbsp;

<u>Error:</u> The user should be informed if any errors occurred while performing the operation.

&nbsp;

<ul>
<li><strong>Update meaning of an existing word</strong></li>
</ul>
&nbsp;

Update associated meanings of a word from the dictionary. If multiple meanings exist, all of them should be replaced by new meaning(s) provided by user. Update made by one client should be visible to any of the clients of the dictionary server.&nbsp; If the word does not exist in the dictionary, then no action should be taken. The minimum input and output parameters are as follows:

&nbsp;

<u>Input:</u> Word to update, meaning(s)

&nbsp;

<u>Output:</u> Status of the operation (e.g., success, not found)

&nbsp;

<u>Error:</u> The user should be informed if any errors occurred while performing the operation.

<strong>&nbsp;</strong>

<h1>User Interface</h1>
A Graphical User Interface (GUI) is required for this project. You are free to design it and to use any existing tools and libraries for this purpose.

<h1>Implementation Guidelines</h1>
<strong>&nbsp;</strong>

These are guidelines only, you are allowed and encouraged to come up with your own design and interfaces.

<ul>
<li>When the server is launched, it loads the dictionary data from a file containing the initial list of words and their meanings. These data is maintained in memory in a structure that enables an efficient word search. When words are added or removed, the data structure is updated to reflect the changes.</li>
</ul>
&nbsp;

<ul>
<li>sample command to start the server is:</li>
</ul>
&nbsp;

&gt; java –jar DictionaryServer.jar &lt;port&gt; &lt;dictionary-file&gt;

&nbsp;

Where &lt;port&gt; is the port number where the server will listen for incoming client connections and &lt;dictionary-file&gt; is the path to the file containing the initial dictionary data.

&nbsp;

<ul>
<li>When the client is launched, it creates a TCP socket bound to the server address and port number. This socket remains open for the duration of the client-server interaction. All messages are sent/received through this socket.</li>
</ul>
&nbsp;

<ul>
<li>sample command to start the client is:</li>
</ul>
&nbsp;

&gt; java –jar DictionaryClient.jar &lt;server-address&gt; &lt;server-port&gt;

&nbsp;

<h1>Implementation Language</h1>
&nbsp;

The assignment should be implemented in <strong>Java</strong>. Utilization of technologies such as RMI and JMS are <strong>not allowed</strong>.

<strong>&nbsp;</strong>

<h1>Report</h1>
&nbsp;

You should write a report describing your system and discussing your design choices. Your report should include:

&nbsp;

<ul>
<li>The problem context in which the assignment has been given.</li>
<li>A brief description of the components of the system.</li>
<li>An overall class design and an interaction diagram.</li>
<li>A critical analysis of the work done followed by the conclusions.</li>
</ul>
&nbsp;

Please mind that the report is a <strong>WRITTEN</strong> document, do not put only graphs. A report without any descriptive text addressing the problem, architecture, protocols, and the analysis of the work done will not be considered valid.

&nbsp;

The length of the report is not fixed. A good report is auto-consistent and contains all the required information for understanding and evaluating the work done. Given the level of complexity of the assignment, a report in the range of 4 to 6 pages is reasonable. Please mind that the length of the report is simply a guideline to help you in avoiding writing an extremely long or incomplete report.

&nbsp;

It is important to put your details (name, surname, student id) in:

&nbsp;

<ul>
<li>The head page of the report.</li>
<li>As a header in each of the files of the software project.</li>
</ul>
&nbsp;

This will help to avoid any mistakes in locating the assignment and its components on both sides.

&nbsp;

<h1>Submission</h1>
&nbsp;

You need to submit the following via LMS:

&nbsp;

<ul>
<li>Your report in PDF format <em>only</em>.</li>
<li>Two <em>executable jar</em> files (DictionaryClient.jar and DictionaryServer.jar) that will be used to run your system on the day of the demo.</li>
<li>Your source files in a .ZIP or .TAR archive <em>only</em>.</li>
</ul>
&nbsp;

Submissions will be due on: <strong>Monday 19 of April (5 pm). </strong>

<strong>&nbsp;</strong>

<h1>Marking</h1>
&nbsp;

The marking process will be structured by first evaluating whether the assignment (application + report) is compliant with the specification given. This implies the following:

&nbsp;

<ul>
<li>Use of TCP/UDP sockets and threads for the application;</li>
<li>proper use of concurrency in the server;</li>
<li>proper handling of the errors;</li>
<li>a report with the requested content and format (PDF);</li>
<li>timeliness in submitting the assignment in the proper format (names, directory structure, etc.).</li>
</ul>
&nbsp;

All of the above elements will earn you a maximum of 10 (out of 15) marks. The rest of the marks are assigned to two elements:

&nbsp;

<ul>
<li><em>Excellence (3 marks – 2 for implementation, 1 for report)</em>. The assignment has not only been implemented by meeting the minimum requirements but the design has been well thought and a proper interaction with the user has been provided (notification of errors, which really help to understand what went wrong). For what concerns the report excellence, the report is complete and well written with the <strong>proper graphs</strong> and a discussion and <strong>analysis of the system implemented</strong> including <strong>advantages and disadvantages of your design choices</strong>. You need to explicitly write in the Report all <strong>Excellence elements</strong> <em>(point-by-point listing with brief illustration/discussion included) in a separate section.</em></li>
</ul>
&nbsp;

<ul>
<li><em>Creativity (2 marks)</em>. Any additional implementation such as a GUI for managing the server or other enhancements to the code introducing advanced features (such as processing of user requests within a server in scalable, reliable, and efficient manner) will be considered a plus. <strong>For example, using your own implementation of a thread pool (not Java’s) would earn you these marks</strong>. You need to explicitly write in the Report all <strong><em>Creativity elements</em></strong><em> (point-by-point listing with brief illustration/discussion included) in a separate section.</em></li>
</ul>
<strong>&nbsp;</strong>

<strong><u>NOTE 1 (EXTREMELY IMPORTANT):</u></strong> The excellence and the creativity marks (5 marks) cannot compensate any lack in the first part (the one that scores up to 10 marks). Please concentrate your efforts in getting the first 10 marks done and then proceed with the rest.

<strong>&nbsp;</strong>

<strong>Note 2:</strong> Don’t document anything you haven’t implemented in the report. This is misconduct and will result in severe penalties.

<h1>Demonstration Schedule and Venue</h1>
&nbsp;

You are required to provide a demonstration of the working application and will have the opportunity to discuss with the tutors the design and implementation choices made during the demo.

&nbsp;

You are free to develop your system where you are more comfortable (at home, on one pc, on your laptop, in the labs…) but keep in mind that the assignment is meant to be a distributed system that works on at least two different machines in order to separate the client from the server. <strong>&nbsp;</strong>

&nbsp;

<strong>We will announce the demo date, time, and venue closer to the due date</strong>. Each tutor will hold 2-3 demo sessions and you will be required to showcase your system in one of the sessions held by the tutor of the workshop in which you are enrolled.

&nbsp;

If you need any clarification on the assignment, kindly ask questions during the tutorials or in the LMS forum, so that all students benefit from it.
