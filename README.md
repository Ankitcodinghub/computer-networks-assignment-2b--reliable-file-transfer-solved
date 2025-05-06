# computer-networks-assignment-2b--reliable-file-transfer-solved
**TO GET THIS SOLUTION VISIT:** [Computer Networks Assignment # 2b- Reliable File Transfer Solved](https://www.ankitcodinghub.com/product/computer-networks-assignment-2b-reliable-file-transfer-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96395&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Computer Networks Assignment # 2b- Reliable File Transfer Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
In this assignment, your goal is to write modify your already-developed file transfer server and client to communicate using the Pipelined-RDT protocol instead of UDP sockets. As you know the Go-Back-N (GBN) and Selective Repeat (SR) are the two protocols that are enhanced versions of the simple Stop-and-Wait protocol, your objective will be to write transport layer programs that implement GBN and SR protocols to upload the file reliably over unreliable medium. Please note that the client must be able to transfer any kind of files (e.g., text, pdf, or media file) to the server.

Disclaimer: This is a group assignment. Each group should have a max of two members. Therefore, it is up to you to find your teammate, but you need to divide the tasks equally among yourselves. You need to reach out to me quickly if you cannot find a partner or would like to do this assignment alone. There are no extra points given if you wish to do the assignment alone.

Task Details:

In the previous assignment (2a), you learned how to create a TCP socket and send data blocks (of 1000 bytes) to the client. However, in this assignment, you will be developing your own pipelined reliable transport protocol using GBN and SR that will deliver the packets reliably. Follow the below architecture to implement your programs.

</div>
</div>
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
Client

</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
rdt_send(data) udt_send(pkt) GBN or SR-Sender

</div>
</div>
<div class="layoutArea">
<div class="column">
RFT_Server App

</div>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
Server

</div>
</div>
<div class="layoutArea">
<div class="column">
RFT_Client App

</div>
</div>
<div class="layoutArea">
<div class="column">
deliver(data)

</div>
</div>
<div class="layoutArea">
<div class="column">
GBN or SR-Receiver

</div>
<div class="column">
rdt_rcv(pkt)

</div>
</div>
<div class="layoutArea">
<div class="column">
Task-1 (File Transfer from Server to Client using GBN and SR)

Specifically, you should modify the server program to do the following,

<ol>
<li>When started, the server should ask for a port number and the protocol to use (GBN/SR). Then the server will wait for client’s message starting with sequence# 0.</li>
<li>The first packet that it should receive is the command &lt;RETR file_name&gt;. With this, the server can create a file with this name and wait for the next packets to append into it.</li>
<li>Here, the server is going to play the role of receiver as per our GBN and SR protocol’s point-of-view. So, you will write programs/functions to ensure server behaves like a</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
GBN or SR Sender (based on the protocol chosen) that can handle sending packets in pipeline (with Window Size = N, you should try with N=4, 8, 12, 16, 24) and ensure sliding of window as acknowledgements are received. In addition, you need to make sure the segment size is 1024 bytes at maximum.

4. When the file’s data is completely transferred, you can use your own END-OF-FILE signal to identify this situation.

Note: You would need to leverage concurrent programming concepts like multi-threading, locks/semaphores to build your GBN/SR sender functions.

Next, you need to modify the client program to do the following:

<ol>
<li>The client should ask the server’s IP, port, and protocol to use as transport layer.</li>
<li>As per the protocol chosen, you need to include the GBN and SR receiver function in
your client program.
</li>
<li>As the first packet, the client should send the file name to retrieve from the server with a
command “RETR file_name”.
</li>
<li>As the client program receives the packets, it needs to extract the content of correctly
ordered packets and append to a new file. It must continue this process until the whole content of the file is
</li>
</ol>
Task-2 (Measurements)

As you have implemented the GBN and SR sender, you would need to count the following attributes to understand how this protocol is performing (conduct separately for transfer of both files). You need to send a large file for the sake of better visualization with N=4, 8, 12, 16, 24. For each protocol (GBN and SR), you need to measure following attributes.

<ol>
<li>Total number of packets sent (Both freshly transmitted and retransmissions)</li>
<li>Number of retransmitted packets (only when time expires, packet gets
retransmitted)
</li>
<li>Number of timeout events occurred</li>
<li>Time taken to complete the file transfer</li>
</ol>
Then, use a spreadsheet or python’s Matplotlib module to plot the following comparison figures

<ol>
<li>Window size (N) vs. time taken to complete file transfer</li>
<li>Window size (N) vs. # of retransmissions</li>
<li>Window size (N) vs. # of timeout</li>
</ol>
Sample Helper Module (Must be used)

No special python modules related to file transfer is allowed to be used, except the sample helper modules given to you.

You are given with 3-auxiliary helper modules: timer, packet, udt. You must examine the helper modules to get acquainted on how and when to use them.

<ul>
<li>Timer module: Provides start(), stop(), timeout(), running() functions</li>
<li>Packet module: Provides make(seqNo, data), extract(packet), make_empty()</li>
<li>udt module: Provides send(packet, sock, addr), rcv(sock) to send/recv from unreliable
channel
</li>
</ul>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Environment to Execute the Programs

<ul>
<li>Ø &nbsp;Install a UBUNTU 18+ VM on your VirtualBox and then you would have to install the CORE emulator on that machine. Please follow the instructions from https://github.com/coreemu/core.</li>
<li>Ø &nbsp;You can create a tree topology on your own as we have seen in the class and define your client node as well as server node.</li>
<li>Ø &nbsp;In the Ubuntu home folder, you can create two subfolders named “Server” and “Client”, which are the home folders for your server and client programs respectively.</li>
<li>Ø &nbsp;In the server terminal, you would need to navigate to Server subfolder and execute your program using “python3 rftServer2.py”. Similarly, in the client terminal you have to navigate to the Client subfolder to run the client program using “python3 rftClient2.py”.
If for some reason, you cannot install CORE, you can simply use the same machine (localhost) with two separate terminals for executing your client and server programs. Please contact me ASAP, if you are confused on how to run your programs.

After the client receives the file, it terminates. Then, you should test the correctness of the files by using the DIFF command – diff -s recvdFile sentFile

Submission:

As outcomes of this assignment, you would need to submit the following:
</li>
</ul>
<ol>
<li>Python programs/modules that could produce required outputs with proper code
documentation. Lack of code documentation will cost 5% of the grade.
</li>
<li>Report containing your strategy to solve the problem, evidence, and multiple execution samples (i.e., sending different kinds of files), instructions for running the submitted programs, and references used. Comprehensive report with no grammatical error is
expected and it carries 10% of this assignment’s total grade.
</li>
</ol>
Group Activity:

<ul>
<li>The students must work in group of 2. If you decide to work alone, you will have to complete both parts, there is no bonus for working alone.</li>
<li>Each student’s contribution should also be reported with a comparative chart as shown below and should be reported through the report.
Task lists Student-1’s contribution Student-2’s contribution ………

References:

[1] Socket programming in python: https://realpython.com/python-sockets/

[2] Python multi-threading: https://realpython.com/intro-to-python-threading/

[3] GBN and SR Animation: https://www2.tkn.tu-berlin.de/teaching/rn/animations/gbn_sr/ [4] GBN and SR Tutorial: https://www.javatpoint.com/sliding-window-protocol
</li>
</ul>
</div>
</div>
</div>
