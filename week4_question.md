# Week 4: Shell Commands
## Navigate the Machine

### Context anchor

In Week 1 you connected to a remote server using SSH and moved files using SCP. You typed commands and things happened. You were told exactly what to type.

In Week 3 you used the terminal again — to send a reachability signal to a server and to make an HTTP request. The commands were described to you.

This week you take the training wheels off. You will open the terminal, connect to the server, and explore — not from instructions, but from observation. Your job is to understand the environment you have been connecting to every week, using the tools the shell gives you.

The shell has its own vocabulary. Developers use it daily to navigate filesystems, inspect files, and organise work — all without opening a single application window. Before this week ends, you will too.

---

### Part A: Your first look at the environment

Connect to the course server via SSH (the same way you did in Week 1).

Once connected, do not type any commands yet. Just look at the screen.

**Your Part A document must include:**
1. A screenshot of your terminal immediately after connecting — before typing anything. Describe in writing what you see: what does the prompt show? What does each part of the prompt tell you?
2. Research and find the command that tells you which user you are currently logged in as. Run it. Screenshot the output. What does it show?
3. Research and find the command that tells you which directory you are currently in. Run it. Screenshot the output. Is this directory specific to your user, or shared with all users? How do you know?

Do not ask for the commands. Research what each task requires, try it, and document what you observe.

---

### Part B: Map the filesystem

The server organises its files in a branching tree structure — directories inside directories, from a single root. Your task is to explore that structure and document it.

**Your Part B document must include:**
1. Find and run the command that lists the contents of your current directory. Screenshot the output. How can you tell which items are files and which are directories from the output alone?
2. Navigate into at least two other directories that you discover. For each one document: the full path of the directory, what it contains, and how you got there from the previous location.
3. Draw the directory structure you explored as an indented list — no code, just plain labels. Example format:
```
Home directory (your username)
  submissions/
    week1/
    week2/
    week3/
  [other contents you find]
```
Your map must come from your actual exploration of the server, not invented.
4. Research and document in your own words: what is an absolute path? What is a relative path? Find one real example of each from your exploration of the server.

---

### Part C: Read files without opening them

Developers read files directly in the terminal — without opening a text editor or any application. There are specific commands designed exactly for this.

**Your Part C document must include:**
1. Locate a text file anywhere on the server. Your own submission folders from previous weeks are a good place to start — you uploaded files there. Document the full path to the file you find.
2. Research the command that displays the complete contents of a text file in the terminal. Run it on the file you found. Screenshot the output. What exactly did you see?
3. If the file were very long, the contents would scroll past before you could read them. Research whether there is a command (or a variation of the one you just used) that shows a file one screenful at a time and lets you scroll through it. Document what you found and whether you tested it.
4. Research the commands that show only the first few lines of a file and only the last few lines of a file. Document what each does and when a developer would choose each one over reading the whole file.

---

### Part D: Observations

Write a document of minimum 150 words answering all three:

1. Before this week, when you thought about "files" on a computer, you probably pictured icons in a window. Now that you have navigated using the terminal, how has your mental model of the filesystem changed? What stayed the same? What looks different now?

2. In Part B you navigated the server filesystem. In Weeks 1 and 3, you uploaded files to a specific path on the server: `/home/submissions/weekN/[your-name]/`. Now that you understand paths — why do you think the path is structured that way? What does each part tell you?

3. Write one thing that confused you during this week's exploration. What did you do to resolve it? What do you still not understand?

---

### Deliverables

Submit exactly **3 PDFs** via SSH and SCP to the course server.

**PDF 1 — Environment**
Part A documentation with screenshots.

**PDF 2 — Filesystem**
Part B map with screenshots and the directory structure diagram.

**PDF 3 — Files and Observations**
Part C file-reading documentation + Part D written responses.

Place all three files in: `/home/submissions/week4/[your-name]/`

**Filename format:**
- `week4_environment_[yourname].pdf`
- `week4_filesystem_[yourname].pdf`
- `week4_observations_[yourname].pdf`

---

### Stuck protocol

**If you cannot connect via SSH:** Use the same connection details from Week 1. If you have lost them, ask your instructor for the server address and your credentials.

**If you do not know which command does what:** The shell has a built-in help system. Research "how to find out what a Linux command does without leaving the terminal" — there are at least two ways to get documentation from inside the shell itself.

**If a command gives you a "permission denied" error:** You are trying to access a directory or file that belongs to another user. Stay within your own home directory and the public submission folders.

**If you navigate deep and cannot find your way back:** Research "how to return to the home directory in Linux" — there is a shortcut that takes you home from anywhere, regardless of how deeply nested you are.

**If you cannot find any text file to read in Part C:** Research "how to list all files recursively in Linux" — there is a command that shows all files inside all subdirectories at once, which will help you find something readable.

Do not copy your classmates' filesystem maps. Your documentation must come from your own exploration of your own user environment on the server.

---

### What will not be accepted

- Screenshots that do not show the command you ran and its output together
- Directory maps that are invented or copied — they must match what is actually on the server
- Part D responses written in general terms without referencing specific observations from Parts A, B, and C
- Files submitted via email, WhatsApp, or any method other than SSH and SCP to the course server
- Observations that say "the command shows the directory" without documenting what was actually in the directory
