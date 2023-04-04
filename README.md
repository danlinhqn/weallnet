2.83Z"></path></svg></a>Linux System Fundamentals</h1>
<p dir="auto"> Nowadays, Linux (an operating system distributed under an open-source license) is becoming popular for providing a platform which developers could intervention to a system, a network server. Almost IT professionals with or no Linux experience they can be approached to. Linux provides a role better than other OS like Organizing, Managing and Operating a server, also services in Information Systems, secure for environment, solutions, ... for personal, organization and enterprise, ... Here is my report for basic and fundamentals in Linux.
</p>
<hr>
<h2 dir="auto"><a id="user-content-outline" class="anchor" aria-hidden="true" href="#outline"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>Outline</h2>
<p dir="auto"><a href="#Section1">I. Linux Session</a></p>
<ol dir="auto">
    <li><a href="#Section1.1">Whecking Information of a Linux system</a>
    </li><li><a href="#Section1.2">Users and access permission of users</a>
	</li><li><a href="#Section1.3">Checking current Disk usage "df command"</a>
	</li><li><a href="#Section1.4">Checking summarize disk usage of the set of FILEs "du command"</a>
	</li><li><a href="#Section1.5">Checking Disk Partition</a>
</li></ol>
<p dir="auto"><a href="#Section2">II. Process Control</a></p>
<ol dir="auto">
    <li><a href="#Section2.1">Overview</a>
    </li><li><a href="#Section2.2">Viewing process status "top"</a>
    </li><li><a href="#Section2.3">Kill a process</a>
</li></ol>
<p dir="auto"><a href="#Section3">III. Basic Command line with Linux</a></p>
<ol dir="auto">
    <li><a href="#Section3.1">Working with Directories</a>
    </li><li><a href="#Section3.2">Working with Files</a>
    </li><li><a href="#Section3.3">Working with file content</a>
</li></ol>
<p dir="auto"><a href="#Section4">IV. Text Editing Tools</a></p>
<p dir="auto"><a href="#Section5">V. I/O Redirection</a></p>
<p dir="auto"><a href="#Section6">VI. Filters</a></p>
<p dir="auto"><a href="#Section7">VII. File Links</a></p>
<p dir="auto"><a href="#Section8">VIII. Basic Tool for Network</a></p>
<hr>
<div id="user-content-section1" dir="auto"></div>
<h4 dir="auto"><a id="user-content-i-linux-session" class="anchor" aria-hidden="true" href="#i-linux-session"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>I. Linux Session</h4>
<div id="user-content-section1.1" dir="auto"></div>
<ol dir="auto">
<li>
<p dir="auto"><strong>Checking Information of a Linux system</strong></p>
<ul dir="auto">
<li>Checking information of a system is a important thing you have to know, specially when you are working with server. More information you know, more success you work for your project.</li>
</ul>
<p dir="auto">a. Checking CPU: By default in Linux OS, you can check CPU Information by <code>lscpu</code> command.
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/lscpu.png"><img src="/tebby455/My-Report/raw/main/images/Information/lscpu.png" alt="lscpu" style="max-width: 100%;"></a></p>
<p dir="auto">b. Checking RAM: to check memory for easy working, running suitable program, avoid unecessary program, for developers, they have to consider for coding.</p>
<ul dir="auto">
<li>
<ol dir="auto">
<li>Using <code>free [OPTION]</code></li>
</ol>
<ul dir="auto">
<li>
<p dir="auto">Ex: use <code>free</code> for normally checking RAM</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/free.png"><img src="/tebby455/My-Report/raw/main/images/Information/free.png" alt="free" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">[OPTION]: In this common command [OPTION] are used is defind output in specific unit (<code>-k</code> kilobytes, <code>--mega</code> megabytes, ...)</p>
</li>
<li>
<p dir="auto">Other, there is command <code>free -t</code> to show all memory(RAM) and swap.</p>
</li>
</ul>
</li>
<li>
<ol start="2" dir="auto">
<li>Using <code>cat /proc/meminfo</code>: This is command to show full detail of Memory information.</li>
</ol>
</li>
</ul>
<p dir="auto">c. Checking network: to check network interface, also IP, subnet mask, gateway, broadcast, ...</p>
<ul dir="auto">
<li>
<p dir="auto">Basically checking network by <code>ifconfig</code> if you installed <strong>net-tools</strong>, if not use <code>ip a</code> means <strong>ip address</strong></p>
<ul dir="auto">
<li><code>ip a</code></li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/ipa.png"><img src="/tebby455/My-Report/raw/main/images/Information/ipa.png" alt="ipa" style="max-width: 100%;"></a></p>
<ul dir="auto">
<li><code>ifconfig</code></li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/ifconfig.png"><img src="/tebby455/My-Report/raw/main/images/Information/ifconfig.png" alt="ifconfig" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><code>netstat [OPTIONS] &lt;socket&gt;</code></p>
<ul dir="auto">
<li>
<p dir="auto">Tool for follow all of network connection output and input in system. It is useful for solving problem in network.</p>
</li>
<li>
<p dir="auto">Common [OPTIONs]:</p>
<ul dir="auto">
<li>-r: show routing table</li>
<li>-i: show interface table</li>
<li>-o: display timers</li>
<li>-a: show all sockets</li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/netstat.png"><img src="/tebby455/My-Report/raw/main/images/Information/netstat.png" alt="netstat" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><code>traceroute [IP]</code></p>
<ul dir="auto">
<li>
<p dir="auto">Print the route packets trace to network host</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/traceroute.png"><img src="/tebby455/My-Report/raw/main/images/Information/traceroute.png" alt="traceroute" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><code>ping [IP]</code></p>
<ul dir="auto">
<li>
<p dir="auto"><code>ping</code> sned ICMP ECHO_REQUEST to network host, it uses to check the network, or connection from source to dest.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/ping.png"><img src="/tebby455/My-Report/raw/main/images/Information/ping.png" alt="ping" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><code>vnstat</code></p>
<ul dir="auto">
<li>
<p dir="auto"><code>vnstat</code> use to check bandwidth and packet rate of network card.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Information/vnstat.png"><img src="/tebby455/My-Report/raw/main/images/Information/vnstat.png" alt="vnstat" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">command <em>-l</em> to show in real time, <em>-i</em> to choose interface, you can check in <em>ifconfig</em></p>
</blockquote>
</li>
</ul>
</li>
</ul>
</li>
</ol>
<div id="user-content-section1.2" dir="auto"></div>
<ol start="2" dir="auto">
<li>
<p dir="auto"><strong>Users and access permission of users</strong></p>
<ul dir="auto">
<li>
<p dir="auto"><em><strong>Users</strong></em>: There are accounts that you create in Linux, it relates to use <em><strong><em>username</em></strong></em> and <em><strong><em>userID</em></strong></em></p>
<ul dir="auto">
<li>
<p dir="auto"><em><strong>Username</strong></em>: It often uses to login, provide permission, ... but in Linux, system works in <em><strong>UserID</strong></em></p>
</li>
<li>
<p dir="auto"><em><strong>UserID</strong></em>(User identifier): A number go with <em><strong>username</strong></em>, OS uses this number to manage.If two users have different name but have the same UID, these are still in one user. In Linux, to check UID, it stores in <em><strong>/etc/passwd</strong></em>, use <code>cat /etc/passwd</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/User/uid.jpg"><img src="/tebby455/My-Report/raw/main/images/User/uid.jpg" alt="Output of UID" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><em><strong>Access Permission</strong></em>: In Linux, permission of users divide into 2 permission:</p>
<ul dir="auto">
<li><em><strong>root</strong></em>: If users have <em><strong>root</strong></em> permission, those users can be accessed anything in system. These are called <em><strong>superuser</strong></em>, have an userUID=0.</li>
<li><em><strong>normal</strong></em>: It means that users have userUID#0, oftenly users that clients create a new user in system. These are work in permission of <em><strong>user with root permission</strong></em>.</li>
</ul>
</li>
</ul>
</li>
</ol>
<div id="user-content-section1.3" dir="auto"></div>
<ol start="3" dir="auto">
<li>
<p dir="auto"><em><strong>Checking current Disk usage <em>df command</em></strong></em>
a. <em><strong>df</strong></em> command</p>
<ul dir="auto">
<li>Showing the amount of disk space used and size available on Linux file System.</li>
</ul>
<p dir="auto">b. <em><strong>Syntax</strong></em>: df [OPTION] ... [FILE] ...</p>
<ul dir="auto">
<li><em><strong>Example</strong></em>:
<ul dir="auto">
<li>Show all of current disk in System: <code>df [Enter]</code></li>
<li>Show a specific file/folders: <code>df -a /dev/sdb1</code>: there is will show | Filesystem | 1K-blocks | Used | Available | Use% | Mounted on.</li>
</ul>
</li>
<li>[FILE]: Like in Example, my file is <em><strong>/dev/sdb1</strong></em></li>
<li><em><strong>Common</strong></em> [OPTION]:
<ul dir="auto">
<li>-a, --all: show all file systems, include hidden files.</li>
<li>-h: show block Size in power of 1024 (ex: 1024M)</li>
<li>-H: show block Size in power of 1000 (ex: 1.1G)</li>
<li>--total: show a sum of all of disk (ex: I have 2 disk 100G of each, there is will show a line total is 200G)</li>
<li>-T: show a file Type (ex: I partition disk to store data is /dev/sda4, it is <em><strong>a ext4 type</strong></em></li>
</ul>
</li>
</ul>
</li>
</ol>
<div id="user-content-section1.4" dir="auto"></div>
<ol start="4" dir="auto">
<li>
<p dir="auto"><em><strong>Checking summarize disk usage of the set of FILEs <em>du command</em></strong></em>
a. <em><strong>du command</strong></em>
- Showing disk usage then estimate for space usage. For example: I have disk A with size is 100GB, I use command, it shows that my Disk A used 2GB, for that I               could estimate space usage of Disk A.<br>
b. <em><strong>Syntax</strong></em>: du [OPTION] ... [FILE] ... (recommended to use)
or: du [OPTION] ... --file0-from=F</p>
<ul dir="auto">
<li>
<p dir="auto"><em><strong>Example</strong></em>:</p>
<ul dir="auto">
<li>When you are in specific folder, ex., you are in <em><strong><em>/home/name/Downloads</em></strong></em></li>
<li>Use: <code>du [ENTER]</code>, there will show all of file that folder contains and their size</li>
<li><code>du -a _/home/name/Downloads_</code>: show all of file and size that you choose, in here I choose check in _/home/name/Downloads</li>
<li><code>du -a _--file-from=/dev/sdb1_</code>: summarize disk usage of the Disk, in here I check in disk <em>/dev/sdb1</em>.</li>
</ul>
</li>
<li>
<p dir="auto"><em><strong>Common</strong></em> [OPTION]:</p>
</li>
</ul>
<ul dir="auto">
<li>-a, -all: show all file in directory</li>
<li>-h: show size of files that human readable format (ex: 1K, 1M, 1G,...)</li>
<li>-c: show total size file in directoryrecursively</li>
<li>-d + [number]: show the total level for a directory (ex: my [number] is 1, I am in <em><strong>/home/name</strong></em>, it will show <em><strong>/home/name/Downloads</strong></em>, if number is 2 it shows <em><strong>/home/name/Downloads</strong></em> and <em><strong>/home/name/Downloads/Telegram</strong></em>)</li>
<li>-s: show only total of directory</li>
</ul>
</li>
</ol>
<div id="user-content-section1.5" dir="auto"></div>
<ol start="5" dir="auto">
<li>
<p dir="auto"><strong>Checking Disk Partition</strong></p>
<p dir="auto">a. <em><strong>fdisk</strong></em> command</p>
<ul dir="auto">
<li>
<p dir="auto"><strong>fdisk</strong> is the most common used command to check the partitions on the disk. It displays the partition and details like file system type, but it does not report size in unit of each partitions. Other, <strong>fdisk</strong> can be used in partition disk or change many thing on disk.</p>
</li>
<li>
<p dir="auto"><strong>Syntax</strong></p>
<ul dir="auto">
<li><code>fdisk [OPTION] &lt;disk&gt;</code> change, edit partition disk</li>
<li><code>fdisk [OPTION] -l &lt;disk&gt;</code> list partition table of disk
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Disk/fdisk.png"><img src="/tebby455/My-Report/raw/main/images/Disk/fdisk.png" alt="fdisk" style="max-width: 100%;"></a>
<blockquote>
<p dir="auto">This is command for show all of partition of disk that are in your computer</p>
</blockquote>
</li>
<li>If you want to show specific of disk, ex: <code>fdisk -l /dev/sda1</code></li>
</ul>
</li>
</ul>
<p dir="auto">b. <strong><code>df command</code></strong> this command can be used to check partition
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Disk/df.png"><img src="/tebby455/My-Report/raw/main/images/Disk/df.png" alt="df command" style="max-width: 100%;"></a></p>
<p dir="auto">c. Mount and Umount</p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Mount:</strong> Allow computer access to I/O storage device like USB and hard drive.</p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Syntax</strong>: <code>mount [OPTIONS] device dir</code> or <code>mount [OPTIONS] device|dir</code></p>
</li>
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-l: List all the file systems mounted file</li>
<li>-h: help, display full options</li>
<li>-V: show version of <code>mount</code></li>
<li>-a: mount all filesystems mentioned in fstab</li>
<li>-t: type of filesystem device uses</li>
<li>-r: set read-only to file mounted</li>
</ul>
</li>
<li>
<p dir="auto">Example: <code>mount -l -t ext4</code> to list all mounted file that are using type <strong>ext4</strong></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Disk/mount.png"><img src="/tebby455/My-Report/raw/main/images/Disk/mount.png" alt="mount" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Umount:</strong> When you finish working with any divice that you mounted, you have to umount it to avoid data missing.</p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Syntax</strong>: <code>umount [OPTIONS] &lt;source&gt; | &lt;directory&gt;</code></p>
</li>
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-a: unmount all filesystems</li>
<li>-r: if unmounting fail, that disk will be remount in read-only</li>
<li>-t: tyoe of filesystem device uses</li>
<li>-f: force to unmount</li>
</ul>
</li>
<li>
<p dir="auto">Example: <code>mount /media/dirname</code>, if output does not appear anything, it success.
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/Disk/umount.png"><img src="/tebby455/My-Report/raw/main/images/Disk/umount.png" alt="umount" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ul>
</li>
</ol>
<hr>
<div id="user-content-section2" dir="auto"></div>
<h3 dir="auto"><a id="user-content-ii-process-control" class="anchor" aria-hidden="true" href="#ii-process-control"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>II. Process Control</h3>
<div id="user-content-section2.1" dir="auto"></div>
<ol dir="auto">
<li>
<p dir="auto"><strong>Overview</strong></p>
<ul dir="auto">
<li>
<p dir="auto">Process control is a technical to follow time by time the process activities. Managing and resolving problems in operation of process. In each processes, these are have Process ID(PID). There are two type of process: <strong>Foreground Process</strong> and <strong>Background Process</strong></p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Foreground Process:</strong> Every processes that you run interactively in your shell are Foreground Process. If a process have a while to run, you have to wait and cannot do anything until it finishs or you interupt it by <code>CTRL Z</code>. Example: I <code>ping 8.8.8.8</code>, it will run after 5 times ping <em>icmp_seq</em> for Windows, for Linux it will continue until you <code>CTRL Z</code>, in while it is running you cannot do anything.</p>
</li>
<li>
<p dir="auto"><strong>Background Process:</strong> Every processes that you run, it does not interact with your shell directly. You can run other process while Background Processes are running. Example: I run <code>sudo</code>, it will run in system, to stop it <code>exit</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/process/example.png"><img src="/tebby455/My-Report/raw/main/images/process/example.png" alt="example" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ul>
</li>
</ol>
<div id="user-content-section2.2" dir="auto"></div>
<ol start="2" dir="auto">
<li>
<p dir="auto"><strong>Viewing process status <strong><code>top</code></strong></strong></p>
<ul dir="auto">
<li>
<p dir="auto">In Linux, to display all process in real-time view of a running system, use <code>top</code>. It could be display system summary information as well as list of processes or threads.</p>
</li>
<li>
<p dir="auto"><strong>Syntax:</strong> <code>top [OPTIONS]</code></p>
<ul dir="auto">
<li>
<p dir="auto">Common [OPTIONS]:</p>
<ul dir="auto">
<li>-e: k(kilobytes) | m(megabytes) | g(gigabytes) | t(terabytes) | p(pebibytes): Enfoce task memory scaling</li>
<li>-E: k(kilobytes) | m(megabytes) | g(gigabytes) | t(terabytes) | p(pebibytes): Enfoce sumary memory scaling</li>
<li>-s: use in secure mode</li>
</ul>
</li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/process/top.png"><img src="/tebby455/My-Report/raw/main/images/process/top.png" alt="top" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">PID: process id
PR: priority of the task
NI: Nice Value of task, positive NI means lower priority, negative means higher priority
VIRT: virutal memory used
SHR: shared memory size</p>
</blockquote>
</li>
</ul>
</li>
</ol>
<div id="user-content-section2.3" dir="auto"></div>
<ol start="3" dir="auto">
<li>
<p dir="auto"><strong>Kill a process</strong></p>
<ul dir="auto">
<li><code>kill &lt;PID&gt;</code> when you install a tool, but it has conflict with PID(ex: PID=111), so you have to kill it if it does not affect with running system.</li>
<li>Example: kill a process with PID is 10, <code>kill -9 10</code>, <em>-9</em> is shutdown immediately.</li>
</ul>
</li>
</ol>
<hr>
<div id="user-content-section3" dir="auto"></div>
<h3 dir="auto"><a id="user-content-iii-basic-command-line-with-linux" class="anchor" aria-hidden="true" href="#iii-basic-command-line-with-linux"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>III. Basic command line with Linux</h3>
<div id="user-content-section3.1" dir="auto"></div>
<ol dir="auto">
<li>
<p dir="auto"><strong>Working with directories</strong></p>
<p dir="auto">a. <strong><code>pwd</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>pwd</code> print name of current/working directory. For the old Linux OS, this command was helpful for people who working in Linux.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/directory/pwd.png"><img src="/tebby455/My-Report/raw/main/images/command/directory/pwd.png" alt="pwd" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">Common used in <em>pwd</em></p>
</blockquote>
</li>
</ul>
<p dir="auto">b. <strong><code>cd</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>cd</code> change your current direcotry to <em>/root</em> directory</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/directory/cd.png"><img src="/tebby455/My-Report/raw/main/images/command/directory/cd.png" alt="cd" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">More options in cd:</p>
<ul dir="auto">
<li><strong>Syntax:</strong> <code>cd &lt;path dir&gt;</code></li>
<li><code>cd ..</code> go to the parent directory</li>
<li><code>cd -</code> go to previous directory</li>
</ul>
</li>
</ul>
<p dir="auto">c. <strong><code>ls</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>ls</code> list the content of a directory</p>
</li>
<li>
<p dir="auto"><strong>Syntax:</strong> <code>ls [OPTIONS] &lt;path dir&gt;</code></p>
<ul dir="auto">
<li>
<p dir="auto">By default, use <em>ls</em> for current directory, if you want to list other directory, you can use <code>ls [OPTION] &lt;path dir&gt;</code>, ex: <code>ls -a /home/huynx/Desktop</code>
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/directory/ex-ls.png"><img src="/tebby455/My-Report/raw/main/images/command/directory/ex-ls.png" alt="ex-ls" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-a: to show all hidden files</li>
<li>-l: to display the content in different format</li>
<li>-h: to show the number of size in human readable format</li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/directory/compare.png"><img src="/tebby455/My-Report/raw/main/images/command/directory/compare.png" alt="compare without options and with option -l" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">Different between <em>ls</em> and <em>ls -l</em></p>
</blockquote>
</li>
</ul>
</li>
</ul>
<p dir="auto">d. <strong><code>mkdir</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>mkdir</code> to create a new directory. Common used to create <code>mkdir mydir</code></p>
</li>
<li>
<p dir="auto"><strong>Syntax:</strong> <code>mkdir [OPTIONS] dirname</code></p>
</li>
<li>
<p dir="auto">Common [OPTIONS]:</p>
<ul dir="auto">
<li>
<p dir="auto">-p: to create a parent directory, for example: <code>mkdir -p mydir1/mydir2/mydir3</code> it will be created <em>mydir1</em> then <em>mydir2</em> in <em>mydir1</em>, ...</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/directory/mkdir-p.png"><img src="/tebby455/My-Report/raw/main/images/command/directory/mkdir-p.png" alt="mkdir -p" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ul>
<p dir="auto">e. <strong><code>rmdir</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>rmdir</code> to delete direcoties if they are empty</p>
</li>
<li>
<p dir="auto">Example: I used <code>rmdir</code> to delete <em><strong>mydir</strong></em> that I created before</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/directory/rmdir.png"><img src="/tebby455/My-Report/raw/main/images/command/directory/rmdir.png" alt="rmdir" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">I can not delete because in <em>mydir</em> it has other directories</p>
</blockquote>
</li>
<li>
<p dir="auto">In order to delete by <code>rmdir</code>, also use <code>rm (remove dir)</code> it can deleted directories that have content inside and common [OPTIONS] is <code>-rf</code></p>
</li>
</ul>
</li>
</ol>
<div id="user-content-section3.2" dir="auto"></div>
<ol start="2" dir="auto">
<li><strong>Working with files</strong></li>
</ol>
<ul dir="auto">
<li>
<p dir="auto">Directories is a special kind of file.
a. <strong><code>locate</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>locate</code> to search a file, or search by file type</p>
</li>
<li>
<p dir="auto">Basically, search a file without any options <code>locate task.txt</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/locate.png"><img src="/tebby455/My-Report/raw/main/images/command/file/locate.png" alt="locate" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">If you do not remember name of file, just know file type, use <code>locate *.txt</code>, this command show all file with type is <em>.txt</em></p>
</li>
</ul>
<p dir="auto">b. <strong><code>cp</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>cp</code> to copy file(s)</p>
</li>
<li>
<p dir="auto"><strong>Syntax:</strong> <code>cp [OPTIONS] SOURCE DEST </code>, copy SOURCE to DEST or multiple SOURCE to DEST</p>
<ul dir="auto">
<li>
<p dir="auto">In current directory, I copy a file into two, <code>cp hello.txt hello1.txt</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/cp.png"><img src="/tebby455/My-Report/raw/main/images/command/file/cp.png" alt="copy" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">Copy a file forward to another directory, <code>cp hello.txt /home/name/Desktop/hello.txt</code></p>
</li>
<li>
<p dir="auto">To copy multiple SOURCE to DEST, <code>cp task1 task2 task3 /home/name/Desktop/</code>, last argument must be a dricetory</p>
</li>
<li>
<p dir="auto">-i: if you want to overwrite file that existing</p>
</li>
</ul>
</li>
<li>
<p dir="auto">Do the same with directories</p>
</li>
</ul>
<p dir="auto">c. <strong><code>mv</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>mv</code> to move file(s)</p>
</li>
<li>
<p dir="auto"><strong>Syntax:</strong> <code>mv [OPTIONS] SOURCE DEST/DIR </code>, rename SOURCE to DEST or move SOURCE to DIR</p>
<ul dir="auto">
<li>
<p dir="auto">Can rename with <code>mv</code>, <code>mv hello.txt aloha.txt</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/mv-rename.png"><img src="/tebby455/My-Report/raw/main/images/command/file/mv-rename.png" alt="mv-rename" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">To move a file `mv aloha.txt
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/mv-move.png"><img src="/tebby455/My-Report/raw/main/images/command/file/mv-move.png" alt="mv-move" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>zip and unzip</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>zip</code> is used to pack files into 1 file with smaller size. In Linux, there are many type of zip, <strong>tar, gzip, zip, bz, 7z, ...</strong></p>
<ol dir="auto">
<li>
<p dir="auto"><code>tar</code></p>
<ul dir="auto">
<li>
<p dir="auto"><code>tar</code> a tool zip popular in Linux, last of files have <code>.tar</code></p>
</li>
<li>
<p dir="auto"><strong>Syntax</strong> <code>tar [OPTIONS] file</code></p>
<ul dir="auto">
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-cvf: to create a storage file, locate to it then pack, show working on screen</li>
<li>-cvzf: the same but work with only <code>.gz</code>, common use in file has <code>.tar.gz</code></li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><code>gzip</code></p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Syntax</strong> <code>gzip [OPTIONS] filename</code></p>
<ul dir="auto">
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-1~9: level for zip</li>
<li>-l: check attribute file zip</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
</ol>
</li>
<li>
<p dir="auto"><code>unzip</code> to unpack file zipped</p>
<ol dir="auto">
<li>
<p dir="auto"><code>tar</code></p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Syntax</strong></p>
<ul dir="auto">
<li>-xvf: create a storage then unpack in there.</li>
<li>-xvzf: the same but in <code>.gz</code></li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><code>gzip</code></p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Syntax</strong> <code>gzip [OPTIONS] filename</code></p>
<ul dir="auto">
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-1~9: level for zip</li>
<li>-l: check attribute file zip</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
</ol>
</li>
</ul>
</li>
</ul>
</li>
</ul>
<div id="user-content-section3.3" dir="auto"></div>
<ol start="3" dir="auto">
<li>
<p dir="auto"><strong>Working with file contents</strong></p>
<p dir="auto">a. <strong><code>head</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>head</code> to display first ten lines of a file</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/head.png"><img src="/tebby455/My-Report/raw/main/images/command/file/head.png" alt="head" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">If you add <em>-[number line]</em> <code>head -4 task.txt</code> there will show first 4 lines.</p>
</li>
</ul>
<p dir="auto">b. <strong><code>tail</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>tail</code> to display last ten lines of a file</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/tail.png"><img src="/tebby455/My-Report/raw/main/images/command/file/tail.png" alt="tail" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">If you add <em>-[number line]</em> <code>head -4 task.txt</code> there will show last 4 lines.</p>
</li>
</ul>
<p dir="auto">c. <strong><code>cat</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>cat</code> command is one of the most universal tools. It uses display a file on the screen without editor.
<a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/cat.png"><img src="/tebby455/My-Report/raw/main/images/command/file/cat.png" alt="cat" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><code>cat</code> also to use create files, <code>cat &gt; hello.txt</code></p>
</li>
</ul>
<p dir="auto">d. <strong><code>more and less</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>more and less</code> used to display file that take up more than one screen like your screen not enough to contain all of content. Users use space bar to see the next page, <strong>q</strong> to quit. <code>more and less</code> are the same uses but lightly different format.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/command/file/more.png"><img src="/tebby455/My-Report/raw/main/images/command/file/more.png" alt="more" style="max-width: 100%;"></a></p>
</li>
</ul>
<hr>
</li>
</ol>
<h3 dir="auto"><a id="user-content-iv-text-editing-tools-" class="anchor" aria-hidden="true" href="#iv-text-editing-tools-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>IV. Text Editing Tools <div id="user-content-Section4" dir="auto"></div></h3>
<ul dir="auto">
<li>In Linux, almost Text Editor can be used for developer, coding with better efficiency than compiler.</li>
</ul>
<ol dir="auto">
<li>
<p dir="auto"><strong>Vim Editor</strong>(best for Ubuntu)</p>
<ul dir="auto">
<li><strong>Vim editor</strong> a tools famous in text editor with many shortcut keys, running fast, but not easy to use for beginers.</li>
<li>To run <strong>vim</strong>, <code>vim</code>, run it with create a file <code>vim hello.txt</code></li>
</ul>
</li>
<li>
<p dir="auto"><strong>Vi Editor</strong>(most primitive editors in Linux)</p>
<ul dir="auto">
<li>
<p dir="auto">To run <em>vi editor</em>, <code>vi</code>, or create a file <code>vi hello.txt</code></p>
</li>
<li>
<p dir="auto"><em>vi</em> have 2 basics mode: <em>insert</em>(allow user can write), <em>command</em>(user only use commands in this mode)</p>
</li>
<li>
<p dir="auto">There is some commands that useful for use <em>vi</em>:</p>
<ul dir="auto">
<li>:w	Write this file out</li>
<li>:q	Quit <em>vi</em> w/o writing</li>
<li>:q!	Force quit <em>vi</em> w/o writing</li>
<li>:w!	Force write</li>
<li>:wq	Write then quit</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Nano GNU Editor</strong></p>
<ul dir="auto">
<li>
<p dir="auto">This is a text editor which for users easy to use, also popular in Unix and Linux.</p>
</li>
<li>
<p dir="auto">To run <em>nano</em>, <code>nano</code>, to create a file <code>nano hello.txt</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/text-editor/nano.png"><img src="/tebby455/My-Report/raw/main/images/text-editor/nano.png" alt="nano" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ol>
<hr>
<h3 dir="auto"><a id="user-content-v-io-redirection-" class="anchor" aria-hidden="true" href="#v-io-redirection-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>V. I/O Redirection <div id="user-content-Section5" dir="auto"></div></h3>
<ul dir="auto">
<li>
<p dir="auto">In the bash shell has three standard stream: <strong>stdin(standard input)</strong>, <strong>stdout(standard output)</strong>, <strong>stderr(standard error)</strong></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/model.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/model.png" alt="topology" style="max-width: 100%;"></a></p>
</li>
</ul>
<ol dir="auto">
<li>
<p dir="auto"><strong><code>dev/null</code></strong></p>
<ul dir="auto">
<li><code>dev/null</code> is a virtual file. Everything you stored in <code>dev/null</code> is useless, it will be removed. A null device, it received anything you redirect to</li>
</ul>
</li>
<li>
<p dir="auto"><em><strong>Standard Input(stdin)</strong></em></p>
<ul dir="auto">
<li>
<p dir="auto">Standard Input is a stream which a program <em>read</em> its input data, default stream = 0. It is request data by use of the <em>read</em> operation.</p>
</li>
<li>
<p dir="auto">Example: <code>cat /etc/passwd</code>, if you use <code>cat</code> without any parameter or option, it will slient execute with any input from keyboard until <strong>CTRL D(Character EOF)</strong></p>
</li>
<li>
<p dir="auto">For redirection, standard input is inherited from the parent process.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/stdin.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/stdin.png" alt="stdin" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">Redirect Standard Input <code>&lt;</code></p>
<ul dir="auto">
<li>
<p dir="auto">Using to read data from a file, then use it to input from another file.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/redirectinput.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/redirectinput.png" alt="redirect standard input" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Standard Output(stdout)</strong></p>
<ul dir="auto">
<li>
<p dir="auto">Standard Output is a stream which a program <em>writes</em> its output data, default stream = 1. It is request data by use of the <em>write</em> operation, example <code>cat hello.txt</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/stdout.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/stdout.png" alt="stdout" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">Redirect Standard Output</p>
<ul dir="auto">
<li>
<p dir="auto"><code>1 &gt; file</code>: redirect output to file, overwrite to file</p>
</li>
<li>
<p dir="auto">Example: <code>echo hello &gt; hello.txt</code></p>
</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Standard Error(stderr)</strong></p>
<ul dir="auto">
<li>
<p dir="auto">Standard error is another output stream, used by program to output <em>error messsages</em>. It is a stream independent of standard output can be redirected separately. Default stream = 2.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/error.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/error.png" alt="error" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">Redirect Standard Error</p>
<ul dir="auto">
<li>
<p dir="auto"><code>2 &gt; file</code>: use to prevent error messages from cuttering your screen</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/redirecterror.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/redirecterror.png" alt="redirect standard error" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>&gt;&gt; append to file</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>&gt;&gt;</code> is a operator which is adding content into the last content of file.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/append.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/append.png" alt="append" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>pipe</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto">Basically, <code>pipe</code> is a type of redirecting, use output of program  then redirect to input of another program.</p>
</li>
<li>
<p dir="auto">Signal: <code>|</code></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/IOredirect/pipe.png"><img src="/tebby455/My-Report/raw/main/images/IOredirect/pipe.png" alt="pipe" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ol>
<hr>
<div id="user-content-section6" dir="auto"></div>
<h3 dir="auto"><a id="user-content-vi-filters" class="anchor" aria-hidden="true" href="#vi-filters"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>VI. Filters</h3>
<ol dir="auto">
<li>
<p dir="auto"><strong><code>tee</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>tee</code> put <strong>stdin</strong> and <strong>stdout</strong> into a file. Function <code>tee</code> is same <code>cat</code>. Sometime, we can use <code>-a</code> append to file.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/tee.png"><img src="/tebby455/My-Report/raw/main/images/filter/tee.png" alt="tee" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>grep</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>grep</code>, common use is to filter lines of text containing. There are many [OPTIONS] of <code>grep</code> for regular expressions.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/grep.png"><img src="/tebby455/My-Report/raw/main/images/filter/grep.png" alt="grep" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">Instead of I use <em>grep copy</em>, I can use <em>grep -i copy</em> means ignore case</p>
</blockquote>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>cut</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>cut</code> can select columns from files.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/cut.png"><img src="/tebby455/My-Report/raw/main/images/filter/cut.png" alt="cut" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>tr</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>tr</code> can translate character.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/tr.png"><img src="/tebby455/My-Report/raw/main/images/filter/tr.png" alt="tr" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>wc</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>wc</code>, counting words from a file.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/wc.png"><img src="/tebby455/My-Report/raw/main/images/filter/wc.png" alt="wc" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>sort</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>sort</code> will filter file by default to an alphabetical sort.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/sort.png"><img src="/tebby455/My-Report/raw/main/images/filter/sort.png" alt="sort" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>uniq</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>uniq</code> remove duplicates from a sorted list</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/filter/uniq.png"><img src="/tebby455/My-Report/raw/main/images/filter/uniq.png" alt="uniq" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>sed</code></strong></p>
<ul dir="auto">
<li><code>sed</code> basic workflow is Read, Execute, Display, it often uses to filter by use regular expression.</li>
</ul>
</li>
</ol>
<hr>
<div id="user-content-section7" dir="auto"></div>
<h3 dir="auto"><a id="user-content-vii-file-links" class="anchor" aria-hidden="true" href="#vii-file-links"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>VII. File Links</h3>
<ol dir="auto">
<li>
<p dir="auto"><strong>Hard Links</strong></p>
<ul dir="auto">
<li>
<p dir="auto">When you create a <strong>hard link</strong> to a file win <code>ln</code>, an extra entry is added in the directory.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/file_link/hardlink.png"><img src="/tebby455/My-Report/raw/main/images/file_link/hardlink.png" alt="hardlink" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><code>ln</code> is a tool for create a files system to only an app with diferrent structure for efficient.</p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Symbolic Links</strong></p>
<ul dir="auto">
<li>
<p dir="auto"><strong>Symbolic links</strong> is a special file point to another directory, it called <strong>target</strong>. When its created, it can be replaced instead <strong>target</strong>. It is unique and can be placed anywhere you want. 1 target can be pointed to many symbolic links.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/file_link/symlink.png"><img src="/tebby455/My-Report/raw/main/images/file_link/symlink.png" alt="symbolic links" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ol>
<hr>
<div id="user-content-section8" dir="auto"></div>
<h3 dir="auto"><a id="user-content-viii-basic-linux-tools-" class="anchor" aria-hidden="true" href="#viii-basic-linux-tools-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>VIII. Basic Linux Tools <div id="user-content-Section8" dir="auto"></div></h3>
<ol dir="auto">
<li>
<p dir="auto"><em><strong>nmap tool</strong></em></p>
<ul dir="auto">
<li>
<p dir="auto"><code>nmap</code> is a open-source port scanner for UNIX and Windows. It supports a wide variety of scan types. Providing to assist users of nmap in scaning own network, or network has been given permission, also to determine the security of network. It also a Network exploration tool and security/ port scanner.</p>
</li>
<li>
<p dir="auto"><strong>Syntax</strong> `nmap [Scan types] [OPTIONS] </p>
<ul dir="auto">
<li>
<p dir="auto">Common [Scantype] [OPTION]:</p>
<ul dir="auto">
<li>-sn: ping scan withour port</li>
<li>Scan techniques: -sS/sT/sA/sW/sM: TCP SYN/Connect()/ACK/Window/Mainmon scan</li>
<li>-sU: UDP scan</li>
<li>-sV: probe open ports to determone serivce/version</li>
<li>-sC: script scan</li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/nmap/scan.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/nmap/scan.png" alt="scan" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>git</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto">Git is a version-control system for tracking changes in computer files and coordinating work on those files among multiple people. Gis is a <em><strong>Distributed Version Control System</strong></em>.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/git/workflow.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/git/workflow.png" alt="workflow" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto">Common Command Line in GIT:</p>
<ul dir="auto">
<li><code>git add</code>: to add file that is in the working directory</li>
<li><code>git commit</code>: to add all files that are staged to the local repository</li>
<li><code>git push</code>: add all file in the local repository to GitHub.</li>
<li><code>git clone</code>: to Download a repository of someone in GitHub.</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Telnet</strong></p>
<ul dir="auto">
<li>
<p dir="auto">A protocol to remote access to another PC, Router,... Telnet protocol, is used popular in local, because it does not have security, so that it connects fast.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/telnet.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/telnet.png" alt="telnet" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong>Secure Shell(SSH)</strong></p>
<ul dir="auto">
<li>
<p dir="auto">A protocol allow user can remote access to another computer in Internet. It has security, encode passwd, so that connect lower than Telnet</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/ssh.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/ssh.png" alt="ssh" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="auto"><strong>generate ssh-key</strong>*</p>
<ul dir="auto">
<li>
<p dir="auto">use the <em>ssh-keygen</em> to generate a public/private authenication key pair, allow users connect withour supplying password, but keys must be generated for each users.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/ssh-key.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/ssh-key.png" alt="ssh-key" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">Importing a key to ssh</p>
</blockquote>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/key.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/key.png" alt="key" style="max-width: 100%;"></a></p>
<blockquote>
<p dir="auto">my ssh-keygen</p>
</blockquote>
</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="auto"><strong><code>rsync</code></strong></p>
<ul dir="auto">
<li>
<p dir="auto"><code>rsync</code> is a tool for copy, sync data between host and server in Linux</p>
</li>
<li>
<p dir="auto"><strong>Syntax</strong> <code>rsync [OPTPIONS] [USER@]HOST:SRC [DEST]</code></p>
<ul dir="auto">
<li>
<p dir="auto">Common [OPTIONS]</p>
<ul dir="auto">
<li>-r: copy data recursive</li>
<li>-a: archive mode</li>
<li>-z: pack a data</li>
</ul>
</li>
</ul>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/tebby455/My-Report/blob/main/images/basic_tool/rsync.png"><img src="/tebby455/My-Report/raw/main/images/basic_tool/rsync.png" alt="rsync" style="max-width: 100%;"></a></p>
</li>
</ul>
</li>
</ol>
<hr>
<h2 dir="auto"><a id="user-content-the-end" class="anchor" aria-hidden="true" href="#the-end"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><div dir="auto">The End</div></h2>
&lt;style&gt;div.a {text-align:center}&lt;/style&gt;
<hr>
 <h3 dir="auto"><a id="user-content-references" class="anchor" aria-hidden="true" href="#references"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a>References</h3>
<p dir="auto"><a href="http://people.cs.uchicago.edu/~kaharris/cspp51081/Links/unix-resources/linux-fund.pdf" rel="nofollow">Overview Linux</a></p>
<p dir="auto"><a href="https://linux-training.be/linuxfun.pdf" rel="nofollow">Linux Fundamentals</a></p>

<hr>
<p dir="auto"><a href="https://github.com/tebby455/My-Report/blob/main/README.md">Come Back</a></p>
</article>
  </div>

    </div>

  </readme-toc>

  

  <details class="details-reset details-overlay details-overlay-dark" id="jumpto-line-details-dialog">
    <summary data-hotkey="l" aria-label="Jump to line" role="button"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump overflow-hidden" aria-label="Jump to line" role="dialog" aria-modal="true">
      <!-- '"` --><!-- </textarea></xmp> --><form class="js-jump-to-line-form Box-body d-flex" data-turbo="false" action="" accept-charset="UTF-8" method="get">
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line…" aria-label="Jump to line" autofocus="">
          <button data-close-dialog="" type="submit" data-view-component="true" class="btn">    Go
</button>
</form>    </details-dialog>
  </details>



    <div class="pt-3">
      <details class="details-reset details-overlay details-overlay-dark ">
                <summary data-view-component="true" class="btn-link" role="button">    Give feedback
</summary>

  <details-dialog class="Box d-flex flex-column anim-fade-in fast Box--overlay overflow-visible" aria-label="Provide feedback" src="/tebby455/My-Report/repos/code_nav_survey" role="dialog" aria-modal="true">
    <div class="Box-header">
      <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog="">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path d="M3.72 3.72a.75.75 0 0 1 1.06 0L8 6.94l3.22-3.22a.749.749 0 0 1 1.275.326.749.749 0 0 1-.215.734L9.06 8l3.22 3.22a.749.749 0 0 1-.326 1.275.749.749 0 0 1-.734-.215L8 9.06l-3.22 3.22a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042L6.94 8 3.72 4.78a.75.75 0 0 1 0-1.06Z"></path>
</svg>
      </button>
        <h1 class="Box-title">Provide feedback</h1>
    </div>
      <div class="Box-body overflow-auto">
                  <include-fragment>
            <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="my-3 mx-auto d-block anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke"></circle>
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke"></path>
</svg>
          </include-fragment>

      </div>
  </details-dialog>
</details>
    </div>
</div>

  </div>


