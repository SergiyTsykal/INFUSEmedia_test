Please find below a task for PHP/JS proficiency evaluation:
Create MySQL table `logs` with the next mandatory columns:
- ip_address
- user_agent
- view_date
- image_id
- view_count
Every time index.html is loaded, send a request to get a random image ID (number from 1 to 4).
On the client side generate an image file path from the received identifier '/src/{image_ID}.jpg'.
Important: you do not need to create a link on the backend and check for the existence of the
file, in this task you need to do this on the frontend side.
Try to load an image from the generated path
If the image exists and is loaded:
- Send a request to increase the number of views on this file
- Send a request to get the current number of views for this file
- Start a timer to periodically update the current view count (every 5 seconds). If there were
views on other tabs, the view counter on the current tab should be updated without reloading
the page.
If the image is not loaded (error, image does not exist):
- Set the image file path to '/src/empty.jpg'
- DON'T send a request to increase the number of views on this file
- DON'T send a request to get the current number of views for this file
- DON'T start a timer to periodically update the current view count.
Every time an incrementation of views count is requested, create/update an entry in the `logs`
table. If a user with the same IP address, user-agent, and image ID requests to increase the
views count again, the view_date column should be updated with the current date and time, as
well as views_count column should be increased by 1.
The task should be completed in PHP/JS.
Please provide a link to GitHub or BitBucket with the uploaded code and let us know how
long it took you to complete this task.
Thank you!
