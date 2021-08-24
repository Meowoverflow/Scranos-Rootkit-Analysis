# Scranos-Rootkit-Analysis

This was a school project as we ( (Aisha Ahmed) [[https://www.linkedin.com/in/aychaa/](https://www.linkedin.com/in/aychaa/)] and I ) wanted to learn Windows kernel rootkits analysis and Scranos was our first rootkit sample, 
also we got A+ for this project "Yaaaaaaay 🙌🙌".

Scranos rootkit component has some interesting techniques like:

- Using un-exported Windows API by NTOSKRNL.EXE "ZwCreateThread" by reaching the address of the fist following exported API then subtracts 4 bytes to get the function pointer.
- The sample maps the image to non paged pool in memory so it's not easy to delete the image while the driver is running.
- ...etc more can be found in the analysis pdf.