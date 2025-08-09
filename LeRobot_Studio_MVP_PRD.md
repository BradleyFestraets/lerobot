### **Product Requirements Document: LeRobot Studio (MVP)**

**Version:** 1.0
**Status:** Draft
**Author:** Product Owner

---

#### **1. Introduction & Vision**

**1.1. Vision:**
To create the most intuitive and accessible platform for anyone to teach a physical robot a new skill. We are transforming robotics from a code-driven field into a creative, hands-on pursuit.

**1.2. Problem Statement:**
Modern robotics tools are powerful but complex, requiring deep technical expertise. This locks out a vast community of students, educators, and hobbyists who want to experiment with robotics but are blocked by the steep learning curve.

**1.3. The MVP Solution:**
The LeRobot Studio MVP is a mobile application that provides a seamless, visual workflow for the core imitation learning loop: **Record, Train, Run.** It allows a user to teach their robot a simple task by demonstrating it, train an AI model based on that demonstration, and watch the robot perform the skill autonomously.

---

#### **2. Goals & Objectives**

*   **Primary Goal:** Deliver a functional, end-to-end user experience for single-task imitation learning.
*   **Secondary Goal:** Validate the core assumption that a mobile-first, visual interface can successfully abstract away the complexity of the robotics toolchain.
*   **Business Goal:** Establish a foundational user base and gather critical feedback to inform the future product roadmap.

---

#### **3. Target Audience**

*   **Primary User Persona: "The Curious Hobbyist"**
    *   **Description:** A student or electronics enthusiast who has successfully assembled a LeRobot-compatible robot (e.g., SO-101). They are excited by AI and robotics but have limited to no experience with Python scripting or command-line interfaces.
    *   **Goal:** To successfully teach their robot a simple task (e.g., "pick up the block") and feel a sense of accomplishment.

---

#### **4. User Stories & Requirements**

**4.1. Feature: Robot Connection & Control**

*   **User Story 1:** As a user, I want to easily connect the app to my robot so that I can start interacting with it.
    *   **Requirement 1.1:** The app must automatically scan the local Wi-Fi network for LeRobot-compatible devices.
    *   **Requirement 1.2:** Discovered robots shall be displayed in a list, showing their given name (e.g., "LeKiwi-LivingRoom").
    *   **Requirement 1.3:** The user must be able to select a robot from the list to establish a connection.

*   **User Story 2:** As a user, I want to manually control my robot in real-time so that I can position it for a task or perform simple actions.
    *   **Requirement 2.1:** The app must provide a "Manual Control" mode.
    *   **Requirement 2.2:** This mode must display a live, low-latency video feed from the robot's primary camera.
    *   **Requirement 2.3:** The interface must provide on-screen joysticks for 6-DOF (X, Y, Z, Roll, Pitch, Yaw) control of the robot arm.
    *   **Requirement 2.4:** The interface must provide simple buttons for opening and closing the robot's gripper.
    *   **Requirement 2.5:** Actions in this mode are for live control only and shall not be recorded.

**4.2. Feature: Imitation Learning Workflow**

*   **User Story 3:** As a user, I want to record myself performing a task so that the robot has a demonstration to learn from.
    *   **Requirement 3.1:** The app must provide a "Teach a Skill" mode.
    *   **Requirement 3.2:** Before recording, the user must be prompted to name the skill (e.g., "Push Block Left").
    *   **Requirement 3.3:** During recording, the app must capture the video feed, robot joint states, and gripper actions.
    *   **Requirement 3.4:** The user must have clear start and stop controls for recording.

*   **User Story 4:** As a user, I want to train an AI model based on my recording so that the robot has a "brain" for that skill.
    *   **Requirement 4.1:** The app must provide a "Train a Brain" screen.
    *   **Requirement 4.2:** The user shall be able to select a previously recorded skill to train on.
    *   **Requirement 4.3:** A single "Start Training" button will initiate the training process on the connected robot or host machine.
    *   **Requirement 4.4:** The app must display a clear progress indicator for the training process.
    *   **Requirement 4.5:** The underlying model will be a basic, non-language-based policy (e.g., ACT or Diffusion Policy, to be determined by the engineering team for simplicity).

*   **User Story 5:** As a user, I want to command the robot to perform the skill it learned so that I can see the result of my teaching.
    *   **Requirement 5.1:** The app must provide a "Run a Skill" screen.
    *   **Requirement 5.2:** The user shall be able to select from a list of their successfully trained brains.
    *   **Requirement 5.3:** A "Run" button will command the robot to begin executing the selected skill.
    *   **Requirement 5.4:** The user will see the live video feed of the robot performing the action.

---

#### **5. Out of Scope for MVP**

The following features are explicitly out of scope for this initial release to ensure a focused and timely delivery.

*   **All Advanced AI:** No SmolVLA (language), HIL-SERL (coaching), Reinforcement Learning, or Scene Awareness (VLM Q&A).
*   **All Community Features:** No Brain Hub, sharing, or downloading of models.
*   **All "Future Vision" Features:** No AR overlays or long-horizon task planning.
*   **Advanced Data Management:** The MVP will only support single-demonstration training. Multi-demonstration datasets are out of scope.
*   **Advanced Training Configuration:** No user-configurable model parameters or hyperparameters.

---

#### **6. Success Metrics**

*   **Activation Rate:** Percentage of users who successfully connect to a robot.
*   **Core Loop Completion Rate:** Percentage of users who successfully record, train, and run at least one skill.
*   **Qualitative Feedback:** Direct user feedback collected via surveys and interviews.
