- 👋 Hi, I’m [@bhuvanesh-m-dev](https://github.com/bhuvanesh-m-dev)  
- 👀 Passionate about programming and problem-solving  
- 🌱 Currently upskilling and improving my core development skills  
- 💡 Open to collaborating on open-source projects and innovative coding challenges  
- 📢 Reach me at: **bhuvaneshm.developer@gmail.com**  
  
## Explore CosmoTalker: Your Gateway to Space Tech with Python 🪐

<p align="center">
  <a href="https://bhuvaneshm.in/cosmotalker/" target="_blank" rel="noopener noreferrer">
    <img src="https://bhuvaneshm.in/cosmotalker/image/cosmotalker-github.png" alt="CosmoTalker Project Preview" width="600">
  </a>
</p>


## 🛠️ Project – Setbian {For Debian 😉}

[Setbian](https://github.com/bhuvanesh-m-dev/setbian) is a lightweight Debian post-installation GUI app built with Python Language.

It offers a simple checkbox-style interface to install essential tools like Git, Curl, Firefox, VLC, VS Code, Telegram, and more — perfect for freshly installed Debian systems.

![Setbian Screenshot](https://raw.githubusercontent.com/bhuvanesh-m-dev/setbian/refs/heads/main/setbian/screenshot1.png)

**Key Features:**
- 🐍 Built with native Python (Tkinter)
- ✅ One-click Applications installer
- 🔐 Built-in sudo password prompt
- 🎯 Designed for clean Debian setups

> 📦 Try it now:  
> <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Download SetBian for Debian</title>
</head>
<body style="font-family: sans-serif; display: flex; justify-content: center; align-items: center; min-height: 100vh; background-color: #f0f0f0; margin: 0; flex-direction: column; gap: 20px;">

    <h1 style="color: #333;">Download SetBian for Debian</h1>

    <!-- Changed from <a> to <div> tag, all CSS is now inline -->
    <div id="downloadBtn"
        style="display: inline-flex; align-items: center; justify-content: center; padding: 15px 30px; background-color: #007bff; color: white; border: none; border-radius: 30px; font-size: 1.2em; cursor: pointer; text-decoration: none; box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); position: relative; overflow: hidden; transition: background-color 0.3s ease, transform 0.2s ease, box-shadow 0.3s ease;">
        <span id="downloadIcon" style="margin-right: 10px; font-size: 1.5em; line-height: 1;">&#x2B07;</span> Download
    </div>

    <div id="thankYouMessage"
        style="margin-top: 20px; font-size: 1.5em; color: #333; opacity: 0; transform: translateY(20px); transition: opacity 0.5s ease-out, transform 0.5s ease-out;">
        Thank you for downloading SetBian for Debian!
    </div>

    <script>
        const downloadBtn = document.getElementById('downloadBtn');
        const downloadIcon = document.getElementById('downloadIcon');
        const thankYouMessage = document.getElementById('thankYouMessage');

        // Store default styles for dynamic application
        const defaultButtonStyles = {
            backgroundColor: '#007bff',
            transform: 'translateY(0px)',
            boxShadow: '0 4px 8px rgba(0, 0, 0, 0.2)'
        };

        const hoverButtonStyles = {
            backgroundColor: '#0056b3',
            transform: 'translateY(-2px)',
            boxShadow: '0 6px 12px rgba(0, 0, 0, 0.3)'
        };

        const activeButtonStyles = {
            backgroundColor: '#004085',
            transform: 'translateY(0px)', // Keep transform at 0 for active state
            boxShadow: '0 2px 4px rgba(0, 0, 0, 0.2)'
        };

        // Apply styles helper function
        function applyStyles(element, styles) {
            for (const prop in styles) {
                element.style[prop] = styles[prop];
            }
        }

        // Hover effects using JavaScript
        downloadBtn.addEventListener('mouseover', function() {
            applyStyles(this, hoverButtonStyles);
        });

        downloadBtn.addEventListener('mouseout', function() {
            // Revert to default unless active
            if (!this.classList.contains('active-state')) { // Use a class to track active state if needed
                applyStyles(this, defaultButtonStyles);
            }
        });

        // Active (click down) effects using JavaScript
        downloadBtn.addEventListener('mousedown', function() {
            applyStyles(this, activeButtonStyles);
            this.classList.add('active-state'); // Add a class to indicate active
        });

        downloadBtn.addEventListener('mouseup', function() {
            this.classList.remove('active-state');
            // Revert to hover state if mouse is still over, otherwise default
            if (this.matches(':hover')) {
                applyStyles(this, hoverButtonStyles);
            } else {
                applyStyles(this, defaultButtonStyles);
            }
        });

        // Icon spin animation using JavaScript (since @keyframes is not allowed inline)
        let spinInterval = null;
        const spinDuration = 600; // milliseconds
        const intervalTime = 10; // milliseconds for each step

        function startSpinAnimation() {
            let currentRotation = 0;
            const totalSteps = spinDuration / intervalTime;
            const rotationPerStep = 360 / totalSteps;

            // Clear any existing interval to prevent multiple animations
            if (spinInterval) {
                clearInterval(spinInterval);
            }

            spinInterval = setInterval(() => {
                currentRotation += rotationPerStep;
                if (currentRotation >= 360) {
                    currentRotation = 360; // Ensure it ends exactly at 360
                    clearInterval(spinInterval);
                    spinInterval = null;
                }
                downloadIcon.style.transform = `rotate(${currentRotation}deg)`;
            }, intervalTime);
        }

        function stopSpinAnimation() {
            if (spinInterval) {
                clearInterval(spinInterval);
                spinInterval = null;
            }
            downloadIcon.style.transform = `rotate(0deg)`; // Reset icon rotation
        }


        downloadBtn.addEventListener('click', function(event) {
            event.preventDefault(); // Prevent default link behavior (even though it's a div, good practice)

            // Start the spin animation
            startSpinAnimation();

            // Simulate a download process (e.g., after a short delay)
            setTimeout(() => {
                // Stop the spin animation and reset icon
                stopSpinAnimation();

                // Show the thank you message
                thankYouMessage.style.opacity = '1';
                thankYouMessage.style.transform = 'translateY(0px)';

                // Optionally, hide the thank you message after some time
                setTimeout(() => {
                    thankYouMessage.style.opacity = '0';
                    thankYouMessage.style.transform = 'translateY(20px)';
                }, 5000); // Hide after 5 seconds

                // In a real scenario, you would trigger the actual file download here
                // Example: window.location.href = 'path/to/your/setbian-debian.deb';
            }, 800); // Adjust this delay to match your desired animation time
        });
    </script>

</body>
</html>


---


## 🧪 Try Cosmo4U: CosmoTalker for Debian-based Systems 🐧

<p align="center">
  <a href="https://bhuvaneshm.in/cosmo4u/" target="_blank" rel="noopener noreferrer">
    <img src="https://bhuvaneshm.in/cosmo4u/image/cosmo4u.png" alt="Cosmo4U Preview" width="400">
  </a>
</p>


### I code in
<img height="50" width="50" src="https://img.icons8.com/color/48/000000/python.png" /> <img height="50" width="50" src="https://img.icons8.com/color/48/000000/c-programming.png" />  <img height="50" width="50" src="https://img.icons8.com/color/48/000000/html-5.png" /> <img height="50" width="50" src="https://img.icons8.com/color/48/000000/css3.png" /> <img height="50" width="50" src="https://img.icons8.com/color/48/000000/google-firebase-console.png"/> <img height="50" width="50" src="https://img.icons8.com/color/48/000000/mysql-logo.png"/>
### IDE I Use
<img height="50" width="50" src="https://img.icons8.com/color/48/000000/visual-studio-code-2019.png"/><img width="48" height="48" src="https://img.icons8.com/color/48/google-colab.png" alt="google-colab"/><img height="50" width="50" src="https://img.icons8.com/color/48/000000/pycharm.png"/> <img height="50" width="50" src="https://img.icons8.com/color/50/000000/git.png"/> <img height="50" width="50" src="https://img.icons8.com/dusk/64/000000/anaconda.png"/> 
### Tools I Use 
<img width="48" height="48" src="https://img.icons8.com/fluency/48/linux-terminal.png" alt="linux-terminal"/><img width="48" height="48" src="https://img.icons8.com/material-rounded/24/pypi.png" alt="pypi"/><img height="50" src="https://img.icons8.com/color/480/null/notion--v1.png" />
