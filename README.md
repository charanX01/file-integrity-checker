File Integrity Checker
A simple browser-based tool that compares two files using their SHA-256 fingerprint to confirm whether they are byte-for-byte identical.

What it does
Drop two files into the tool. Each one is hashed with SHA-256 — a unique 64-character code generated from the file's exact contents. If the codes match, the files are identical. If they differ, at least one byte has changed.

Why it's useful
Verify that a downloaded file is genuine and hasn't been tampered with
Detect corruption after a file transfer or backup
Confirm two copies of a file are truly the same
Understand how hashing is used in digital forensics and malware analysis
How to use
Open index.html in any modern browser
Drag a file into File A and another into File B
Read the verdict — green means identical, red means different
How it works
You drop two files
The browser runs SHA-256 on each file, turning it into a unique 64-character code
Matching codes mean the files are identical; different codes mean one has changed
Tech
Plain HTML, CSS, and JavaScript. No libraries, no build step. Uses the browser's built-in Web Crypto API (crypto.subtle).

Privacy
All processing happens locally in your browser. Your files are never uploaded anywhere.
