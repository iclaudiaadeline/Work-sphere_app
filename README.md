# Job Finder

## Overview
Job Finder is a web application that helps users search for job opportunities based on job title and location. The application fetches real-time job listings from an external API and displays the results in an interactive and user-friendly interface.

This project is divided into two parts:
1. **Local Implementation** - Running the application on a local machine.
2. **Deployment** - Deploying the application on provided web servers with a load balancer.

## Features
- Search for jobs by title and location.
- Fetch job listings from an external API.
- Display job results in a structured format.
- Responsive and user-friendly design.
- Error handling for API failures and invalid user inputs.

---

## Technologies Used
- **Frontend:** HTML, CSS, JavaScript
- **API Integration:** External job listing API
- **Deployment:** Web01 & Web02 servers with a load balancer (Lb01)

---

## Setup & Installation
### **Running Locally**
1. Clone the repository:
   ```sh
   git clone https://github.com/iclaudiaadeline/Work-sphere_app
   cd job-finder
   ```
2. Open the `index.html` file in a browser or use **Live Server** in VS Code.
3. Enter a job title and location to search for jobs.

### **API Configuration**
- The application fetches job listings from an external API.
- Ensure you obtain an API key (if required) and update `script.js` accordingly.

---

## Deployment Instructions
### **Deploying to Web Servers**
1. **Upload Application Files:**
   - Place `index.html`, `style.css`, and `script.js` on both Web01 and Web02 servers.
   
2. **Configure Load Balancer (Lb01):**
   - Ensure it distributes traffic between Web01 and Web02.
   - Verify accessibility via the load balancer's URL.

### **Accessing the Deployed Application**
Once deployed, access the application through the load balancer URL:
```
https://www.theadeline.tech/
```

---

## API Usage
- **API Provider:** adzuna api
- **Endpoint Used:** `/search-jobs`
- **Authentication:** API Key (if required)
- **Example API Call:**
  ```js
  fetch(`https://api.example.com/jobs?title=developer&location=NY`, {
    headers: { 'Authorization': 'Bearer YOUR_API_KEY' }
  })
  .then(response => response.json())
  .then(data => console.log(data));
  ```

---

## Error Handling
- Handles API failures and invalid user inputs with alerts.
- Displays error messages when the API is unreachable.

---

## Challenges & Solutions
### **Challenges Faced:**
1. API rate limits affecting response times.
2. CORS policy issues while fetching data.
3. Load balancer configuration for even traffic distribution.

### **Solutions Implemented:**
- Implemented caching to reduce API calls.
- Used a proxy server to handle CORS restrictions.
- Verified load balancer functionality with test requests.

---

## Credits & Attribution
- API provided by [API Name] ([API Documentation Link])
- Project developed as part of a university assignment.

---

## Demo Video
Watch the full demo on YouTube:
https://www.youtube.com/watch?v=pJNq4rOXla

---



---

## Contact
For any inquiries, reach out via GitHub Issues or email at your-a.iradukund3@alustudent.com

