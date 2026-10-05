+++

title = "Automating HTML5 Canvas Games"

draft = false

tags = ["igaming", "ocr", "websocket", "automation"]

+++



\*\*Problem:\*\* iGaming slot games render on an HTML5 canvas, so there are no DOM elements to locate. Standard Playwright or Selenium locators don't work.



\*\*My role:\*\* Designed the approach and rebuilt the framework architecture after the first DOM-based attempt failed.



\*\*Approach\*\*

\- OCR (Tesseract.js) with image preprocessing (Sharp) to read on-screen values such as balance and win amounts.

\- Coordinate-based interaction for spin and bet controls.

\- WebSocket interception to validate game-server messages independently of what the screen shows.



\*\*Tools:\*\* Node.js, Tesseract.js, Sharp, WebSocket interception



\*\*Lessons learned:\*\* Combining visual checks with network-level validation is far more reliable than OCR alone.

\*\*Code:\*\* [GitHub repo link](https://github.com/Shashikant/playwright-igamingautomation)

\*\*Note:\*\* Demonstrated on \[a public demo game, not an operator's production title].

