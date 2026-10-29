For the Stardance Hackclub project I decided to build a web-based operating system called specOS. I made it in 3 separate steps.

Devlog 1: Building welcome screen and creating desktop with a clock.
  
  I first started off by creating separate files for html, css and javascript; those being index.html, style.css and script.js.
  I designed them with a dark background and red glowing accents which I thought looked really cool. I then used AI (Gemini) to
  help me debug the code as I was running into a problem. When I first made the desktop and added the top bar with the clock the 
  text was overlapping with the specOS title. After debugging I used Flexbox in my style.css file. Using display: flex; and 
  justify-content: space-between; to my .topbar, I was able to fix this issue.

Devlog 2: Building the window manager and making the window draggable, closable and openable.

  I then started building the window system so any person using the operating system could open any window in the OS. This would
  allow the OS to look quite smooth. I ran into another problem here. Everytime I would drag the windows they would stick to the 
  cursor of my mouse. They would also keep dragging even if I let go of my mouse. I fixed this by changing the mousemove and mouseup
  listeners to listen globally for the whole document while dragging was active. After the fix, the OS tracked mouse movements smoothly.

Devlog 3: Making the Task Matrix

  I started brainstoring ideas and came up with a task manager and scheduler. I thought up about this because I myself am quite the 
  procrastinator. The task manager would be able to track tasks set by the user, and I added categories based on my own usage like: 
  school, uni applications, social and personal. A due date system and notification system was also implemented into the system. 
  Upon debugging for this, I realized that everytime I refreshed the operating system all my tasks decided to vanish. I had to learn 
  how to use localStorage in JavaScript and used JSON.stringify() so that a task could be saved in the browser itself as a text string. 
  I then used JSON.parse() so that when the page is loaded back up, it shows the tasks as they were before.
  
