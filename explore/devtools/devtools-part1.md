# DevTools Part 1: Network Tab

1. **What is the name of the new JSON file?**  
   `citylots.json`

2. **Which file initiated the download of the new file?**  
   `expose.js`

3. **What is the file size of the downloaded file?**  
   File was served from disk cache, but original transfer size is about ~2.3MB.  
   (Displayed as `(disk cache)` in this session.)

4. **How long did it take to download?**  
   Between 59 ms to 69 ms (cached).

---

5. **What was your User-Agent for the browser that made the request?**  
   `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/135.0.0.0 Safari/537.36`

6. **In the response header, what type of server did it come from?**  
   `GitHub.com`

7. **When was the file last modified?**  
   `Thu, 15 Sep 2022 22:44:30 GMT`

8. **What was the Content-Type of the file?**  
   `application/json; charset=utf-8`

9. Which function inside the initiating file made the request?  
   `fetchData()` — this function calls `fetch('./citylots.json')` when the "Fetch Data" button is clicked.
