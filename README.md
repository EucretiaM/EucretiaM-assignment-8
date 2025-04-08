Assignment 8 focus much on the State diagrams and the Activing diagrams relating to functional requirements in assignment 4, user stories and sprints in assignment 6
State diagrams and activity diagrams are both part of **UML (Unified Modeling Language)** and are used to model different aspects of a system's behavior, particularly in relation to **functional requirements**.

**state diagrams** and **activity diagrams**, how they relate to **functional requirements**, and what they typically show:

## 🔁 **State Diagrams** (State Machine Diagrams)

### 📌 Purpose:
State diagrams model the **dynamic behavior** of a system by showing how an object changes **states** in response to **events**. These are useful for modeling the lifecycle of an object, especially when the object’s behavior depends on its current state.

### 🔄 How They Relate to Functional Requirements:
State diagrams are tied to **specific functional requirements** that involve state-dependent behavior. For example, if a user can be in “logged out”, “logged in”, or “banned” states, a state diagram shows transitions between these based on actions like login attempts, password failures, or bans.

### ✅ Used For:
- Describing object behavior over time.
- Systems with **clearly defined states** (e.g., login/logout, order processing, user roles).

### 🧩 Components:
- **States** (e.g., Idle, Active, Logged In)
- **Transitions** (arrows between states triggered by events)
- **Events** that trigger state transitions (e.g., `loginSuccess`, `logout`)
- **Actions** (optional; executed on entry/exit or during a transition)

## 🔁 **Activity Diagrams**

### 📌 Purpose:
Activity diagrams model the **flow of control or data** from activity to activity. They are similar to flowcharts and are used to describe **workflow**, **business logic**, or **sequence of operations**.

### 🔄 How They Relate to Functional Requirements:
Activity diagrams are used to **visualize functional requirements** that involve step-by-step processes, such as how a user registers, solves a quiz, or checks progress in an app.

### ✅ Used For:
- Modeling the **workflow of a use case**
- Showing **logic** of complex operations
- Visualizing **sequential and parallel activities**

### 🧩 Components:
- **Activities** (tasks/operations)
- **Decisions/Merges** (like if/else)
- **Start and End Nodes**
- **Transitions (Control Flows)**
- **Swimlanes** (optional; show responsibility across actors/components)

## 🧠 Example: For a Math Learning App (like "Math Booster")

### 🔷 Functional Requirement:
**"A student should be able to take a quiz and view their results."**

#### 1. **Activity Diagram** (for "Taking a Quiz"):
```
[Start] → Display Quiz → Receive Answers → Validate Answers → Store Results → Display Score → [End]
```

#### 2. **State Diagram** (for "Quiz Session"):
```
[Idle]
  |
  | startQuiz
  v
[In Progress]
  |
  | submit
  v
[Submitted]
  |
  | scoreDisplayed
  v
[Completed]
```

---

If you have specific functional requirements or user stories in mind, I can help create exact **state diagrams** or **activity diagrams** based on them. Want to try that with one of your system features?
