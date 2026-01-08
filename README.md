<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Remote Access Console</title>
<style>
    body {
        background: black;
        font-family: "Courier New", monospace;
        padding: 20px;
        overflow: hidden;
    }
    .log {
        color: #00ff00;
        font-size: 17px;
        line-height: 1.5;
        white-space: pre-line;
    }
    .cursor {
        display: inline-block;
        width: 10px;
        background: #00ff00;
        margin-left: 5px;
        animation: blink 1s infinite;
    }
    @keyframes blink {
        0%, 50%, 100% { opacity: 1; }
        25%, 75% { opacity: 0; }
    }
    .warning {
        animation: flash 0.5s infinite;
    }
    @keyframes flash {
        0% { opacity: 1; }
        50% { opacity: 0.3; }
        100% { opacity: 1; }
    }

    /* FINAL PRANK TEXT */
    .prank {
        display: none;
        text-align: center;
        font-size: 64px;
        font-weight: bold;
        color: white; /* ONLY white text */
        margin-top: 150px;
        animation: zoom 2.5s ease-in-out infinite;
    }

    @keyframes zoom {
        0%   { transform: scale(1); }
        50%  { transform: scale(1.3); }
        100% { transform: scale(1); }
    }
</style>
</head>
<body>

<div class="log" id="log"></div>
<div class="prank" id="prank">😆prank matra ho😆</div>

<script>
const log = document.getElementById("log");
const prank = document.getElementById("prank");

function addText(text, delay) {
    setTimeout(() => {
        log.innerHTML += text + "\n";
        window.scrollTo(0, document.body.scrollHeight);
    }, delay);
}

// Fake hacker sequence
addText("Booting remote exploit framework...", 1000);
addText("Loading modules [net_scan.dll, cam_access.dll]...", 2500);
addText("Establishing encrypted tunnel...", 4000);
addText("Tunnel status: SECURE ✔", 5500);
addText("Target IP detected: 192.168.0.117", 7000);
addText("Running vulnerability scan...", 8500);
addText("Vulnerabilities found: 7 CRITICAL", 10000);
addText("Bypassing firewall rules...", 11500);
addText("Firewall disabled successfully ✔", 13000);
addText("Detecting operating system...", 14500);
addText("OS detected: Android / Windows Hybrid", 16000);
addText("Camera access: GRANTED", 17500);
addText("Injecting malicious payload...", 18500);
addText("Viruses added successfully ✔", 20000);
addText("<span class='warning'>DEVICE INFECTED ⚠</span>", 21000);
addText("Opening backdoor ports: 80, 443, 8080", 22000);
addText("Tracking GPS coordinates...", 23000);
addText("Location found: Ilam, Nepal", 24000);
addText("Extracting files: contacts.db, photos.zip", 25500);
addText("Uploading data to remote server [▓▓▓▓▓▓▓░░░] 70%", 27000);
addText("Upload complete ✔", 28500);
addText("Maintaining persistent access...", 30000);
addText("Connection stabilized <span class='cursor'></span>", 31500);

// Final reveal with zoom animation
setTimeout(() => {
    log.style.display = "none";
    prank.style.display = "block";
}, 34000);
</script>

</body>
</html>
