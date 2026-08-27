# jesse-eisenmann

Profile website for Jesse Eisenmann

## Getting Started 

This guide will walk you through everything you need to do to run this website.

### What You'll Need

Before we start, make sure you have:
- A code editor ([Visual Studio Code](https://code.visualstudio.com/))

### Step 1: Install Node.js and npm

**npm** is a tool that helps manage code libraries. It comes bundled with **Node.js**, so we only need to install one thing.

#### For Windows:
1. Go to [nodejs.org](https://nodejs.org/)
2. Click the large green button labeled "Download for Windows"
3. Open the downloaded file and follow the installer steps
4. When asked about npm, make sure it's checked (it should be by default)
5. Click "Install"

#### For Mac:
1. Go to [nodejs.org](https://nodejs.org/)
2. Click the large green button labeled "Download for macOS"
3. Open the downloaded file (.pkg)
4. Follow the installer steps and click "Install"

#### For Linux:
Follow the instructions on [nodejs.org](https://nodejs.org/) for your specific Linux distribution.

**To verify it installed correctly:**
1. Open your terminal or command prompt ( use the searchbar to open terminal)
2. Type into the command line: `node --version`
3. You should see a version number (like v18.0.0)

---
 4

### Step 2: Download This Project via zip

1. Click the green "Code" button at the top of this page
2. Click "Download ZIP"
3. Find the downloaded ZIP file on your computer
4. Right-click and select "Extract All" (Windows) or double-click (Mac/Linux)
5. Remember where you extracted it - you'll need this location

### Step 2.5: Download This Project via the command line

1. Click the green "Code" button at the top of this page
2. Copy the link from the HTTPS tab
3. Go to your command line and open up the folder you want to download the repository to:
  ``` cd /Users/{yourname}/Downloads/{yourfolder}```

5. type in
   ```pwd```
If the directory name is what you expect it to be, then you are in the right location.
6. Now you will 'clone' the repository to this folder:
  ```git clone https://github.com/sumukund/jesse-eisenmann.git```
7. You might have to log in to github - if you do, let me know.
---

### Step 3: Open a Terminal and Navigate to the Project

#### On Windows:
1. Open the folder you extracted from Step 2
2. Click on the address bar at the top (where it shows the folder path)
3. Type `cmd` and press Enter
4. A black window should open

#### On Mac:
1. Open Terminal (search for "Terminal" in Spotlight)
2. Type: `cd ` (with a space at the end)
3. Drag the folder you extracted from Step 2 into the Terminal window
4. Press Enter

#### On Linux:
1. Open your terminal
2. Type: `cd /path/to/jesse-eisenmann` (replace with your actual path)

---

### Step 4: Navigate to the App Directory

The actual website code is inside a subfolder called `my-svelte-app`. Type this in your terminal:

```
cd my-svelte-app
```

Press Enter.

---

### Step 5: Install Project Dependencies

Now you're in the app folder. We need to install some code libraries that make this website work.

1. In your terminal, type:
   ```
   npm install
   ```
2. Press Enter
3. You'll see a bunch of text appearing - this is normal! It's downloading and installing files
4. Wait until you see a prompt again (this might take 2-5 minutes)

---

### Step 6: Run the Website Locally

Now that everything is installed, let's see the website!

1. In your terminal, type:
   ```
   \. '$HOME/.nvm/nvm.sh'
   nvm use --lts
   npm run dev
   
   ```

 
2. Press Enter
3. You should see some text mentioning a local address (usually something like `http://localhost:5173`)
4. Hold down Control (Windows/Linux) or Command (Mac) and click that link, OR
5. Copy [the link](http://localhost:5173) and paste it into your web browser

**Congratulations!** You should now see the website running locally on your computer!

---

### Step 7: Stopping the website

To stop the website, go back to your terminal and press Ctrl-C.

---

## Need Help?

If something isn't working:

1. **Make sure Node.js installed correctly** - run `node --version` in your terminal
2. **Try running `npm install` again** - sometimes files need to be re-downloaded
3. **Make sure you're in the `my-svelte-app` directory** - your terminal should show that path
4. **Restart your terminal** - close it and open a new one
5. **Restart your computer** - this fixes many issues!

If you're still stuck, email me!

