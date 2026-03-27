# ALU_Health_care

Here is a complete, step-by-step setup guide for your ALU Healthcare project.

---

## What You Need First

Before anything else, make sure you have these installed on your computer:

**1. A Code Editor — VS Code**
Go to https://code.visualstudio.com, click Download, and install it like any normal program. This is where you will write and manage your code.

**2. A Browser**
Google Chrome or Microsoft Edge work best. You likely already have one.

---

## Step 1 — Create Your Project Folder

1. Go to your Desktop (or anywhere you prefer)
2. Right-click → **New Folder**
3. Name it **ALU-Healthcare**

This folder is your entire project. Everything lives here.

---

## Step 2 — Put Your Files In The Folder

Take the two files you downloaded from this conversation:
- `login.html`
- `index.html`

**Move or copy both of them into your ALU-Healthcare folder.**

When you open the folder it should look exactly like this — nothing else, just these two files:

```
ALU-Healthcare/
├── login.html
└── index.html
```

---

## Step 3 — Open The Folder in VS Code

1. Open **VS Code**
2. Click **File** in the top menu
3. Click **Open Folder**
4. Find your **ALU-Healthcare** folder and click **Select Folder**

You will now see both files listed in the left panel called the Explorer. This means VS Code is aware of your whole project, not just one file.

---

## Step 4 — Install the Live Server Extension

This is the most important step. You cannot just double-click the HTML files to open them — the login system uses browser storage that only works on a proper server, not a file path. Live Server creates that server for you instantly.

1. In VS Code, look at the left sidebar and click the **Extensions icon** (it looks like 4 squares)
2. In the search box at the top, type **Live Server**
3. The first result should say **Live Server** by **Ritwick Dey**
4. Click the blue **Install** button
5. Wait for it to finish — it takes about 10 seconds

You only ever need to do this once.

---

## Step 5 — Launch the Project

1. In the VS Code Explorer panel on the left, **right-click on login.html**
2. Select **"Open with Live Server"**
3. Your browser will automatically open and you will see the ALU Healthcare login page

The address in your browser will look like this:
```
http://127.0.0.1:5500/login.html
```
That address means the project is running correctly on your own computer.

---

## Step 6 — Create an Account and Log In

You are now on the login page. You have two options:

**Option A — Use a demo account (fastest)**
Click any of the four demo buttons on the login page:
- **Amara K.** — Student account
- **James M.** — Trainer account
- **Dr. Reeves** — Clinician account
- **Admin** — Administrator account

The email and password fill in automatically. Then click **Sign In**.

**Option B — Create your own account**
1. Click the **Create Account** tab
2. Fill in your first name, last name, email and password
3. Select your role (Student, Trainer, or Clinician)
4. Click **Create Account**

Your account is saved permanently in your browser's storage. You will not lose it when you close the tab.

---

## Step 7 — Explore the Dashboard

After signing in you land on the main dashboard — `index.html`. From the left sidebar you can navigate to:

| Section | What it does |
|---|---|
| Dashboard | Overview of your health and academic stats |
| Courses | Your enrolled courses |
| Assignments | Upcoming and overdue work |
| Calendar | Monthly view of events |
| Grades | GPA and course grades |
| Discussions | Forum threads |
| Inbox | Messages |
| Files | Uploaded documents |
| Health Hub | Water tracker and sports schedule |
| **Health Request** | Submit a medical service request |
| My Profile | View and edit your account info |
| Sign Out | Logs you out and returns to login |

---

## Step 8 — Stopping and Restarting the Project

**To stop:** Go back to VS Code and click **Go Live** at the very bottom right of the screen — it toggles the server off.

**To start again:** Right-click `login.html` in the Explorer and choose **Open with Live Server** again.

**To close VS Code and come back later:** Just reopen VS Code, it will remember your folder. Then launch Live Server again from Step 5.

---

## Troubleshooting — Common Problems

**The browser opens but shows a blank page or an error**
Make sure both `login.html` and `index.html` are in the same folder. If they are in different folders the redirect between them will not work.

**I see "Cannot GET /index.html" in the browser**
You opened a single file instead of the folder. Go to File → Open Folder and select the ALU-Healthcare folder, then launch Live Server again.

**I registered but my account disappeared**
This happens if you opened the files by double-clicking them instead of using Live Server. The storage only works at the `http://127.0.0.1` address. Always use Live Server.

**Live Server is not showing in the right-click menu**
The extension did not install properly. Go to Extensions, search Live Server, uninstall it, restart VS Code, and install it again.

**The page opened but it immediately redirected me to login.html when I tried to open index.html directly**
That is correct behaviour — the auth guard is working. You must always start from `login.html` and sign in first.

---

## Quick Reference Summary

| What | How |
|---|---|
| Start the project | Right-click `login.html` → Open with Live Server |
| Demo login | Click any demo button on the login page |
| Your custom account | Use the Create Account tab |
| Where data is stored | Your browser's localStorage (stays after closing) |
| Session (login state) | Your browser's sessionStorage (clears when tab closes) |
| Stop the server | Click "Go Live" button at bottom of VS Code |

That is the complete setup. Once Live Server is installed (Step 4), starting the project every time after that is just Steps 5 and 6.
