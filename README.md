# Owen Geltz | CS-499 Capstone ePortfolio

Hello! My name is Owen. I started my time here at SNHU in July 2024 in their Computer Science program. This GitHub pages site is to showcase my capstone project. I am set to graduate with my Bachelor of Science in November 2026. After this, I plan to target junior network engineering roles. 

**Contents:**
[Professional Self-Assessment](#professional-self-assessment) ·
[Code Review](#code-review) ·
[The Artifact: CIDR Slicer](#the-artifact-cidr-slicer) ·
[Enhancement One: Software Design and Engineering](#enhancement-one-software-design-and-engineering) ·
[Enhancement Two: Algorithms and Data Structures](#enhancement-two-algorithms-and-data-structures) ·
[Enhancement Three: Databases](#enhancement-three-databases)

---

## Professional Self-Assessment

### How the program shaped my goals
When I first started my college journey, I went into it studying film production, wanting to become a film editor. Around my junior year, I realized that film was more of a hobby of mine, and not something that I wanted to pursue a career in. After a few weeks of deciding, I made the decision to switch my major to computer science at the school I was at at the time, Kutztown University of Pennsylvania. I transferred to SNHU shortly after for the flexibility that the school offers, allowing me to complete my school work while balancing a full-time job, among other responsibilities.

I originally came into the CS program wanting to become a software developer. However, as time went on and I landed a role as an IT help desk technician, I started to become more interested in the networking field. After I took IT-212 here at SNHU, Introduction to Computer Networks, that locked in my decision that I wanted to pursue a career in networking instead. Starting to go in depth into how computers communicate with each other, how to design network topologies, and how to configure networking equipment captivated me.

I did not wish to switch to an IT degree once I made this decision. I was already about 75% complete with my CS degree once I finally honed down my career goals. Coding is still something I am very much interested in, and I wanted to incorporate that alongside my goals to get into the networking field. This capstone will show how I meshed the two together.
 
### Collaborating in a team environment
Throughout my jobs in the IT field as well as this capstone, I have gained experience collaborating within a team environment. My first IT role was a help desk position for a major investment firm in the US. During my time there, I helped migrate the employees at the main headquarters (roughly 13,000) from a Windows 10 environment to Windows 11. I was involved with helping the users themselves get their new devices set up, and assisted them with any questions they may have had relating to the migration. Each migration event consisted of people from multiple teams at the company collaborating to ensure the process ran as smoothly as possible. People from the help desk team, like myself, would be the front-liners to assist users. People from the hardware team were there to swap each user's laptop, and then those from the engineering team were there to assist with specific, complicated issues that the help desk team did not have access to fix.

For this capstone specifically, I ensured that I wrote docstrings throughout the code and a comprehensive README. Doing so would allow another person who has never seen the tool before to pick up and use it with minimal issues. 

### Communicating with stakeholders
As part of the capstone, I created a code review video of my original code, before any enhancements were made to it. Throughout the video, I split it into three parts that targeted each enhancement that I was going to implement. Within these parts, I mentioned what the code did (or did not) do at the time. I explained my plan of attack as to how exactly I was going to enhance the program based upon the requirements of the capstone. I talked about current limitations of the program and how I wanted to handle those with the work I completed throughout this capstone course. 

Referencing my current job, I have to communicate technical related issues to a wide variety of people. After my first IT role, I accepted a job offer as a help desk technician in the education sector. In my day-to-day, I help teachers, students, administrators, and faculty with any technological-related issue they are facing. Typically, these users do not come from a technological background. I always ensure I can explain what exactly is going on with their system, and the steps I am taking to resolve their issue, in easy-to-understand terms that encapsulate all the necessary information. 

### Data structures and algorithms
Throughout my coursework here at SNHU, this capstone project and CS-260 have taught me a lot about data structures and algorithms, along with my own self-study into the topic. In CS-260, I completed assignments relating to creating various data structures such as linked lists, hash tables, and binary search trees. I learned about algorithms like sorting algorithms, including but not limited to quick sort, bubble sort, and others. During my work on the capstone, I realized I had a good grasp on data structures and how they function, but my algorithm knowledge was lacking. I studied and compared various types of algorithms I could use for my enhancement, and settled upon a buddy memory allocation system. Instead of allocating memory however, I wrote it to allocate different IP addresses, which I will get into further down in the Enhancement Two section.

### Software engineering and databases

#### Software engineering
I worked on multiple projects throughout my time at SNHU, like with CS-465, where I created a full-stack MEAN application with MongoDB. Each project I created taught me more than writing code that runs: it also taught me design techniques that meet industry standards, how to properly test my code with unit tests, and more. Outside of SNHU, I have worked on my own projects, including _emerscrape_, which is a Python-based web scraper that I wrote to pull data from my county's active emergency alerts website, which taught me about various Python libraries like beautifulsoup, matplotlib to visualize the data, and others. Another project I worked on was a continuation of my CS-330 work, Computational Graphics and Visualization. This course focuses on teaching OpenGL with C++, and after this course ended, I enhanced it further by adding save states, further model importing, and an ImGUI menu to manipulate the scene live. 

#### Databases
The first course I took at SNHU for the CS major was DAD-220, Introduction to Structured Database Environments. I knew _about_ databases prior and had a rough understanding of how they functioned, but this class introduced me to actually creating and manipulating real databases using SQL. After this, in conjunction with the web scraper from the software engineering section, I set up and configured a PostgreSQL database to hold the data from the web scraper. This taught me a lot not just about PostgreSQL, but concepts of designing database schemas and maintaining a database as well.

### Security
This capstone has taught me a lot about proper security techniques, mainly when it comes to utilizing a database in the program. I picked SQLite for the databases enhancement. For the security aspect, I learned how to guard against things like SQL injection attacks, and how to safeguard the program with parameterized queries, two-layer validation, schema constraints, and refusing damaged data, to prevent a bad actor from breaking the program down.

From my personal work, I have a homelab that I use for various services, like a NAS, Windows Server and Kali Linux lab, among other services. For the networking side, I learned how to segment traffic by utilizing ACLs and VLANs to ensure the services and devices I have on my network are isolated from others as needed, and to prevent traffic from bouncing between VLANs in the event it ever were to become compromised.

### How the artifacts fit together
After getting professor approval, I picked a project that was not completed throughout the CS program here at SNHU. Instead, it was a proof-of-concept script I wrote for an IPAM (IP Address Management) tool. The career I am targeting is within the IT field, specifically networking. I wanted to pick a project that does not just showcase my abilities when it comes to coding programs, but also knowledge within the networking field as well. 

I picked this artifact as the sole artifact to show a single tool growing up. It started off as a hardcoded script and then became a structured command-line tool with an allocation engine, and persistence applied through SQLite to become a real IPAM tool. I started off by refactoring the structure of the program in Enhancement One. In Enhancement Two, I applied the buddy system algorithm along with the binary tree, which depended on the updates created in Enhancement One. In Enhancement Three, I applied the SQLite persistence database, which needed the methods from the algorithm created in Enhancement Two.

---

## Code Review
[Watch the code review on YouTube](https://youtu.be/XqyGsG3CxDs)

---

## The Artifact: CIDR Slicer
CIDR Slicer is an IPAM tool that manages named IPv4 address pools from the command line. Each pool and its allocations are saved within a SQLite database. Each run rebuilds the pool's buddy allocation tree from the saved rows and saves any change made after commands are executed.

Originally, it was a proof-of-concept CLI tool that I had built outside of SNHU’s main coursework earlier in 2026. The script would run with a hardcoded master network and prefix variable and it would print out information regarding the master network, such as the network and broadcast addresses, as well as the subnet mask and total usable hosts. It would then print out subnets carved out with the hardcoded prefix, which was /26. This would show the subnet itself, the range, and the number of usable hosts, per subnet allocation. I selected this artifact after getting professor approval, as it was not originally built for a specific course here at SNHU. I chose this artifact as it directly connects the degree I’m pursuing in the Computer Science program to the career that I am working towards, which is network engineering.

| Version | What it is | Code |
|---|---|---|
| Original | Original artifact before any enhancements were done | [View original](https://github.com/hiiraeth/cidr-slicer/tree/original) |
| After Enhancement One | Refactored into a basic CLI tool | [View](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-1) |
| After Enhancement Two | Implemented the buddy system algorithm and a state kept for the session | [View](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-2) |
| After Enhancement Three (final) | Implemented permanent persistence with SQLite and subcommand CLI | [View](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-3) |

For Enhancement One, I tested the program by running edge cases by hand. For Enhancement Two, I created separate unit tests to check my work and make sure that each new addition I implemented functioned correctly, and did not fail or crash on edge cases. For Enhancement Three, I utilized the same unit tests from Enhancement Two to ensure that the core of the additions added in that enhancement still functioned correctly, and I tested edge cases by running commands against scratch databases.

---

## Enhancement One: Software Design and Engineering
**Before:** [View original code](https://github.com/hiiraeth/cidr-slicer/tree/original) · **After:** [View enhanced code](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-1)

### Why it's included
I have decided I would like to pursue a career in the networking field rather than the traditional software engineering/development path. This artifact helps showcase this goal of mine as the majority of my coursework is general-purpose programming exercises/tools, which would be useful for a software development career path, but not so much a networking path. This is a real tool that I had planned out for a real networking task, which makes it a natural piece to choose so I can demonstrate that I am able to write maintainable code, specifically for network engineering problems.

For specific components of the artifact that showcase my skills and abilities in software development, I separated the parsing of the command-line arguments from the validation, which are done in parse() and NetworkManager.__init__/main(), respectively, from the execution part of the program, which would be analyze() and carve(). I added two helper methods within the NetworkManager class, _usable_host_count() and _range_string(). I added this towards the completion of the enhancement, as I had realized the original per-subnet math I created was duplicated in two separate parts of the program, and the math did not correctly handle networks with a /31 and /32 host-count. I also added docstrings on every method that state the purpose of the method, but also what it assumes about the program and describes any errors it may throw, rather than being caught locally.

For this enhancement specifically, I refactored the tool from a 36 line script into an object-oriented CLI application. The original version of this tool relied on two hardcoded variables to run the program, and two standalone functions that each reconstructed the same IPv4Network object. With this enhancement, I updated it to center around a NetworkManager class. This class owns the network object as an instance state and exposes analyze() and carve(prefix) as its public methods. I implemented Python’s argparse library to take in user input. Each possible failure path, which could be something like a malformed subnet string or a non-integer prefix, for example, is now caught and reported back to the user using an error reporting system. In the original version, the program would simply crash and throw out an unhandled exception error, or continue to run with logic errors.

### Reflection
One of the biggest things I had learned throughout the work of this enhancement was how easy it was to fix one bug, only to introduce different bugs in the process of fixing one. As the refactored code currently stands, I take the requested_prefix argument from parse() in as a string, and then convert it to an int type in main(). Originally, I had this logic inside the carve() method. This worked, however it did not match the “validate everything up front, trust it downstream” pattern I had established in main(). It was a small change moving this validation from carve() to main(), but it helped the design become consistent rather than just functional.

Another issue I wanted to focus on was fixing the /31 and /32 host-count issue. I had introduced a bug during the enhancement progress where the method, self._usable_host_count(), was computing the host count only once, before the enumerated loop that prints each subnet, which used the master network’s prefix length instead of each subnet’s. Due to this, whenever I tested the program, the host count output was outputting the same exact number of host counts for each allocation, which was wrong. This taught me to test the program against specific edge cases, like using a network with a /31 or /32 host-count and reading through the output carefully, rather than simply assuming it was fixed as the program did not crash on me.

### Course outcomes
In my plan in Module One, I had identified this enhancement of being worthy of multiple upgrades, specifically towards refactoring it into an object-oriented application, adding CLI tools, and defensive programming with the error handling, which are tied to the outcomes around using well-founded and innovative techniques and tools, and building a collaborative environment through maintainable, documented code. This enhancement did not focus on the other course outcomes. The class structure of NetworkManager, the Pythonic argparse-based CLI implementation, and consistent validation strategy are all in place and thoroughly tested.

I did have one update to my original plan I wanted to address. While working through this enhancement, I did not realize I would have to implement a fix to handle /31 and /32 host-count and address-range edge cases. This surfaced during testing of the program. I decided to fix it during this enhancement rather than deferring it to a later point, as it directly touched the methods I was already refactoring.

---

## Enhancement Two: Algorithms and Data Structures

**Before:** [View code before this enhancement](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-1) · **After:** [View enhanced code](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-2)

### Why it's included
I selected this item as it was a good program to use to showcase my knowledge within data structures and algorithms. As the code originally stood, it would list which subnets were possible, but it did not have any idea which ones were in use or have a way to store currently allocated subnets. For this enhancement, I replaced the original enumeration technique from the original code with a buddy allocation algorithm. This algorithm is most commonly used to manage memory, but I instead applied it to IP address space. The data structure used is a binary tree, and the master network works as the root of the tree. Its nodes split into two “buddies” whenever a request needs a smaller block, and it only gets split as far down as the request requires. When the block gets released and its buddy is also in a free state, the two merge back into their parent node, which is repeated up the tree.

The data structure is a binary tree that works as a trie on the address bits. Each level further down reads one more bit of said address. Each node can have one of three states: FREE, SPLIT, and ALLOCATED, which are stored in an enum. The tree can only go as deep as 32, minus the root’s prefix length. Routers use this same kind of structure for longest-prefix-match lookups.

The artifact was improved in ways that the original script was unable to match. In the original version of the code, there was no allocation implemented. After implementing this enhancement, the state lasted for the session, and overlapping allocations are not possible. Once a block gets handed out, then nothing inside said block can be handed out again without it first being freed. Freed space now merges back into larger blocks, and invalid requests get rejected before any logic gets applied onto the tree itself. 

One piece I added to the code during this enhancement was a continuous session ability, as the binary tree got reset with every new execution of the program. Without adding this, I would not be able to easily test the code to make sure that the data structure is storing data correctly, as the code would run and immediately quit after processing the command the user had inputted. I handled this by implementing run_session() and handle_command() in subnet.py, which continuously prompts the user for command input until quit is entered, and handles the user inputted command, respectively. I also implemented a help command which showcases all current available commands, their usage, and a brief description of what they do.

### Reflection
The biggest challenge I faced while working on this enhancement was implementing recursion. I understood how the buddy algorithm worked after sketching it out, but it took some time for me to turn that into recursive code. How I ended up understanding the concept and implementing it into the program was tracing specific allocation requests by hand first. By doing so, I was able to notice that each node only ever made one decision out of a handful of decisions based on the node’s size and state. Once I understood this, and that in effect the node’s children would be answering the same questions, the recursive method became clear to me. When implementing the release logic, since the logic only moved up one level in the tree at a time, I opted for a while loop instead.

An important lesson that I have continued to learn throughout my work in the CS program and in this enhancement was that logic errors can hide in plain sight, even though the code runs without errors/without crashing. Several bugs I ran into produced wrong results without any kind of exception or raised error, which was the same issue I faced in Enhancement One. One example of this was instead of assignment with =, I accidentally had coded ==, which checks for equality between two values. Because of this, an allocated block would never change state, and the same subnet could get handed out twice.

I also learned some concepts about Python itself. The language I am most comfortable with is C++. My knowledge on Python’s file structure standards and importing modules were a bit rusty, as I have been so used to writing shorter scripts using the language. I ended up splitting the code into two separate modules/files: subnet.py, which handles the NetworkManager class, main(), and some helper methods to assist with NetworkManager, and allocator.py, which handles the buddy allocation algorithm class and holding the binary tree logic. I had to get familiar with the syntax to call classes and use their methods in other modules like subnet.py again, as I was creating errors trying to import the modules. 

### Course outcomes
During the planning phase in Module One, I noted that this enhancement should cover mainly outcome 3, which is designing and evaluating computing solutions using algorithmic principles while managing trade-offs. The main trade-off I had to consider when implementing the buddy allocation algorithm was the amount of code it took compared to the simple enumeration technique from the original code. However, by implementing this algorithm, it guaranteed no overlap between allocations, it can recover from fragmentation and keeps the operations fast.

One update from the outcome-coverage plans was that this enhancement ended up partly covering outcome 5, which is the security mindset. I had originally saved this outcome for the next enhancement, databases, but it came up naturally in this enhancement while I was working through it. If two allocations exist on the same address, this is a real network failure and can introduce unwanted effects, so ensuring that there can be no overlap is a safety property. I also made the release() method in the BuddyAllocator class reject anything that is not currently allocated, which includes releasing a block twice or releasing a block that has smaller allocations inside of it. Either of these would end up freeing space that someone else already owns. Additionally, all input is validated in a public wrapper method within the BuddyAllocator class, so bad input cannot get passed to the main logic and incorrectly manipulate the tree.

Course outcomes 1, 2, and 4 were not touched on in this enhancement.

---

## Enhancement Three: Databases

**Before:** [View code before this enhancement](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-2) · **After:** [View enhanced code](https://github.com/hiiraeth/cidr-slicer/tree/enhancement-3)

### Why it's included
In the original code before writing any enhancements, it would take in a master network and print out information related to the network and the request prefix to carve out subnets from the network. There was no persistence in between runs, which could be argued that saving allocations was the most important missing feature. Therefore, for this enhancement, I implemented a SQLite database to the program so that persistence exists between runs of the program and rebuilt my command-line interface around it.

The schema of the database holds two tables: address_pools for master networks, and allocations, for each allocated subnet along with its VLAN, its description, and creation time. The database enforces its own rules by using strict typing, using a check to ensure VLANs are between 1 and 4094 and forcing uniqueness for each subnet so no two of the same subnets can exist within the same pool. The class I created in database.py, SubnetStore, functions as the wrapper and storage mechanism for the SQLite database. I ensured that every query uses parameterized placeholders; this way input is only ever treated as data.

Within allocator.py which I created in Enhancement Two, I added an extra method to the buddy allocator class, claim(). This method allocates one exact network, so on every run of the program, the program will load a pool’s saved rows and claims each row. This way, the tree behaves the same way it did in previous executions of the program. The database functions as the source of truth for the program, and the binary tree gets rebuilt from it every time. 

I also overhauled the command-line interface. Originally, I was working with the NetworkManager class in subnet.py (now called cidr_slicer.py) to handle the bulk of the logic. With the updates to the command-line tools using Python’s argparse and talking back and forth with the database, I added subcommands such as create_pool, allocate, release and report. These commands call handlers that call methods from allocator.py and then SubnetStore to perform operations on the database.


### Reflection
The biggest challenge I had faced while enhancing and modifying this artifact was that it has been years since I last designed a database. I was extremely rusty on how to properly design one and had to go back to learning the basics about them, such as tables, columns, keys, constraints, etc. I had written multiple schemas which I tested out with deliberately bad data before touching any Python code to ensure the schema would hold up. 

Connecting the database to the program itself through the Python code brought a different set of challenges I had to face. Quite a few logic errors popped up that I had to fix, such as a bug I created where the report command passed the pool’s name it was attempting to look up, when the ID of the pool was expected instead. SQLite accepted this and returned an empty result with each call instead of an error. Another wasn’t a logic bug, but instead a bug within the allocate command in cli/commands.py, which caused the program to crash after the tree had been changed. This proved to be useful however, as I had created the write order of the program in this enhancement: the tree would update first, and then it would write to the database. With this bug, although the tree was modified, the database itself was not touched, and was able to recover with the next run of the program.

Lastly, I had learned that good design can sometimes mean refactoring previously written code. NetworkManager is a good example of this. In Enhancement One, this class was the source of truth at the time as it held the entire state. However, once the database became the source of truth and every command turned into a separate run, the responsibilities that the class had ended up fitting better elsewhere. For example, I refactored rebuilding the tree into load_pool within commands.py. I also moved methods from NetworkManager into the cli/commands.py file, such as allocate(). In the NetworkManager class, the job of allocate was to print the subnet the user asked for, and that was its whole job, as in Enhancement Two, the tree only had to last for the session. With persistence, now allocation has two halves; updating the tree, then recording the update in the database. If I kept NetworkManager’s allocate(), it would only complete the first half.

### Course outcomes
For this enhancement, I originally planned to cover outcome 4 and outcome 5, using well-founded and innovative tools and techniques, and having a security mindset, respectively. 

Referencing outcome 4, I decided to go with an SQLite implementation vs. another database implementation like PostgreSQL. I have some experience with PostgreSQL, so I naturally gravitated towards it until I thought deeper about the program. Although PostgreSQL has extra features that would be useful to the program, such as native CIDR types and the ability to prevent overlapping rows in the database itself, the major drawback was that it needed an active server connection to run. Therefore, I decided to go with SQLite as it runs anywhere that Python does, and it also does not need a server connection. There are some trade-offs I had to consider, however, which show up in the design of the program. The overlap prevention is coded into the allocator, and addresses from the database are sorted in Python rather than in SQL. The CLI also follows industry standard conventions, such as all input errors go to stderr, and the exit statuses are 0 for success, 1 for refused request, and 2 for incorrect input.

For outcome 5, I implemented several layers of security in my design. One example is the parameterized queries when inputting user data into queries that go to the database. I tested this by attempting to create a pool name with an SQL injection-style name, and it ended up being stored as plain text without ever affecting the database. Following my pattern throughout all the enhancements, I enforced validation at the command line, so that any kind of malformed input does not reach the database. I ensured that when an error occurs, the error message provides useful information to the user but does not expose information about the database like table and/or column names. Lastly, I implemented detection of damaged data so that if two saved allocations overlap, the pool fails to rebuild instead of building it with the bad data.

As for updates, I touched on outcome 2 and outcome 3. For outcome 2, I enhanced the help text and error messages for someone who is not used to the tool. For outcome 3, this came through design decisions, such as retiring the NetworkManager class in the main entry file, cidr_slicer.py, and the write order.

---

[GitHub](https://github.com/hiiraeth)
