# EduCoAI - System Overview & User Workflows

Visual walkthrough of the platform's core features and user journeys.

---

## 🔐 Login Portal

<img width="1012" height="651" alt="login" src="https://github.com/user-attachments/assets/ce8859a1-4cfe-4b36-b95a-86ef1b02587a" />


### Unified Authentication
All users access EduCoAI through a single login portal. The system automatically directs users to their role-specific dashboard after authentication.

**Available Roles:**
- Super Admin
- School Admin
- Teacher
- Student
- Parent

**Note:** Demo accounts are provided for testing purposes with auto-fill credentials.

---

## 👨‍💼 Super Admin Dashboard

<img width="997" height="857" alt="Super-Admin" src="https://github.com/user-attachments/assets/4ea651b7-2a78-495c-aa6e-964b14792a1f" />

### Platform Management Center

The Super Admin dashboard provides a bird's-eye view of the entire platform across all schools.

**What You See:**
- **Overview Cards**: Quick snapshot of total schools, users, lessons, and AI interactions across the platform
- **Growth Trends Chart**: Visual representation of platform growth over time
- **AI Usage Analytics**: Weekly breakdown of AI feature adoption

**Schools Table:**
Lists all schools on the platform with:
- School name and contact email
- Location
- Number of students and teachers
- Active/Inactive status
- Subscription tier (Premium/Basic)

**Primary Action:**
- "Add School" button to onboard new institutions

**Use Case:**
Super Admin monitors platform health, tracks growth, manages schools, and views system-wide AI usage.

---

## 🏫 School Admin Dashboard

<img width="997" height="857" alt="School-Admin" src="https://github.com/user-attachments/assets/b9ba8a30-9fb3-4e91-92bf-3d8eb19988ff" />

### School Management Hub

School Admin sees only their school's data and operations.

**What You See:**
- **Overview Cards**: Total students, teachers, classes, and school-wide average performance
- **Subject Performance Chart**: Comparative bar chart showing performance across different subjects
- **Class Performance Table**: Detailed view of each class with student count, average scores, completion rates, and at-risk student count

**Quick Actions Panel:**
- Create Class
- Add Teacher
- Enroll Student
- Manage Terms (academic calendar)
- Run Auto-Promotion (for end-of-session student advancement)

**Use Case:**
School Admin manages their institution's structure, creates classes, assigns teachers/students, and monitors overall school performance.

---

## 👨‍🏫 Teacher Dashboard

<img width="931" height="939" alt="Teacher" src="https://github.com/user-attachments/assets/1e0ab58d-bb7d-484f-9035-a53d08538627" />

### Classroom & Content Center

Teachers see their assigned classes, students, and content creation tools.

**What You See:**
- **Overview Cards**: Number of classes, students, published lessons, and draft lessons
- **Recent Lessons List**: All created lessons with titles, descriptions, and status (published/draft). AI-generated lessons are clearly marked.
- **My Classes Panel**: Quick access to assigned classes with student counts
- **Student Performance Table**: Comprehensive view of all students showing class, scores, completion rates, AI usage, and performance status

**Primary Actions:**
- "Create Lesson" button for new content
- "View Class" to see class details
- "Full Analytics" for deeper insights

**Use Case:**
Teachers create content (manually or with AI assistance), monitor student progress, and identify students who need support.

---

## 👨‍🎓 Student Dashboard

<img width="931" height="939" alt="Student" src="https://github.com/user-attachments/assets/790cdcb1-30f0-48e1-8b29-c77397596094" />


### Personal Learning Space

Students see their own learning journey and available content.

**What You See:**
- **Overview Cards**: Lessons completed, average score, completion rate, and time spent learning
- **Continue Learning Section**: Active lessons with progress bars and "Start" buttons to resume learning
- **My Subjects Panel**: List of all subjects with available lesson counts
- **Recent Activity Feed**: History of completed lessons, started lessons, and AI assistant interactions

**Quick Actions Panel:**
- View Progress (personal analytics)
- AI Learning Assistant (access chatbot)
- Accessibility Settings (TTS, font size, STT configuration)

**Use Case:**
Students access their lessons, track their own progress, get AI help, and customize their learning experience with accessibility tools.

---

## 👨‍👩‍👧 Parent Dashboard

<img width="931" height="939" alt="Parent" src="https://github.com/user-attachments/assets/8525b4b9-8ea2-4495-825a-4683e0675060" />

### Family Monitoring Center

Parents can monitor one or multiple children from a single account.

**What You See:**
- **Overview Cards**: Number of linked children, overall performance rating, and new notifications
- **Child Performance Cards**: Individual card for each child showing:
  - Student name, ID, and class
  - Performance rating (Excellent/Good/Fair)
  - Key metrics: Average score, completion rate, AI interactions, attendance
  - Progress trend graph over multiple weeks
  - Subject-specific performance bars
  - Recent activity timeline

**Actions Per Child:**
- "View Full Report" for detailed analytics
- "Message Teacher" for direct communication

**Use Case:**
Parents monitor their children's academic progress, identify strengths/weaknesses, and communicate with teachers when needed.

---

## 🔄 User Journey Flow

### Complete Platform Flow

```
1. LOGIN
   All users → Single login portal → Role detection
   
2. DASHBOARD ROUTING
   ├─ Super Admin → Platform overview → Manage schools
   ├─ School Admin → School overview → Manage classes/users
   ├─ Teacher → Content hub → Create lessons/monitor students
   ├─ Student → Learning hub → Access lessons/track progress
   └─ Parent → Family hub → Monitor children/view reports

3. CORE ACTIONS
   Super Admin: Add schools, view analytics
   School Admin: Create classes, enroll students, run promotions
   Teacher: Create lessons, monitor performance
   Student: Complete lessons, use AI assistant
   Parent: View reports, message teachers
```

---

## 🎯 Dashboard Characteristics

### Design Principles Across All Roles

**Consistent Elements:**
- Clean, card-based layouts
- Visual data representation (charts, graphs, progress bars)
- Role-specific quick action buttons
- Notification system
- Intuitive navigation

**Role-Based Views:**
Each dashboard shows only relevant data:
- Super Admin sees everything (platform-wide)
- School Admin sees their school only
- Teacher sees their classes and students
- Student sees their own content only
- Parent sees their children only

**Visual Hierarchy:**
- Important metrics displayed as cards at the top
- Primary actions easily accessible
- Detailed tables/lists below overview
- Charts for trend analysis

---

## 📊 Information Architecture

### What Each Role Manages

| Role | Scope | Creates | Monitors | Actions |
|------|-------|---------|----------|---------|
| **Super Admin** | Platform-wide | Schools | All schools, AI usage | Add schools, set policies |
| **School Admin** | Single school | Classes, Users | School performance | Manage structure, run promotions |
| **Teacher** | Assigned classes | Lessons, Quizzes | Student progress | Create content, intervene |
| **Student** | Personal | None | Own progress | Learn, take quizzes |
| **Parent** | Children | None | Children's performance | View reports, message teachers |

---

## 🚀 System Navigation Summary

**From Login to Action:**

1. **Login** → Enter credentials → System authenticates
2. **Role Detection** → System identifies user role
3. **Dashboard Load** → Role-specific dashboard displays
4. **Overview** → User sees relevant metrics and data
5. **Action** → User performs role-specific tasks
6. **Result** → Changes reflect in respective dashboards

**Example Flow:**
- School Admin creates class → Teacher sees new class → Teacher creates lesson → Student sees new lesson → Parent sees child's progress

---

**EduCoAI** - Purpose-built dashboards for every role in the educational ecosystem.
