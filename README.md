# 📸 Instagram Clone  

An Instagram-like social media application built to practice system design, backend development, and database schema design. This project follows a structured SDLC approach, covering **Requirement Analysis**, **System Design**, **Implementation**, **Testing**, **Deployment**, and **Maintenance**.  

---

## 📌 Features  
- User authentication with OTP verification & email validation  
- Create, like, and comment on posts  
- Follow/unfollow system with request statuses  
- Private and public profiles  
- Replies on comments  
- Block/unblock functionality  
- Media uploads and profile management  

---

## 🗂️ Database Design  

### **User Schema**  
- `firstName`, `lastName`, `userName`, `email`, `password`  
- `dob`, `gender`, `bio`, `profilePic`  
- `posts`, `followers`, `following`, `blocked`  
- `isPrivate`  

### **Post Schema**  
- `caption`, `location`, `comments`, `likes`, `media`, `author`  

### **Comments Schema**  
- `author`, `text`, `likes`, `replies`  

### **Replies Schema**  
- `author`, `liked`, `text`  

### **Follow Request Schema**  
- `from`, `to`, `status` (Accepted, Rejected, Pending)  

### **OTP Schema**  
- `otp`, `mail`, `isVerified` (expires in 2 min)  

---

## ⚙️ Tech Stack  
- **Backend**: Node.js, Express.js  
- **Database**: MongoDB (Mongoose ORM)  
- **Authentication**: JWT & OTP-based  
- **Frontend**: React
