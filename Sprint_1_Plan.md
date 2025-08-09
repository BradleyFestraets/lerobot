### **Sprint 1 Plan: The Core Connection**

**Version:** 1.0
**Status:** Committed
**Author:** Product Owner

---

#### **1. Sprint Goal**

*A user can successfully connect the app to their robot, see its camera feed, and move the arm using on-screen controls.*

This sprint is focused entirely on de-risking the project by proving the fundamental hardware-software communication loop. By the end of this sprint, we will have a functional skeleton app that validates our core connectivity and control architecture.

---

#### **2. Sprint Backlog**

This sprint will pull the following user stories from the MVP Product Requirements Document:

*   **User Story 1:** As a user, I want to easily connect the app to my robot so that I can start interacting with it.
*   **User Story 2:** As a user, I want to manually control my robot in real-time so that I can position it for a task or perform simple actions.

---

#### **3. Task Breakdown & Engineering Requirements**

**3.1. User Story 1: Robot Connection**

*   **Backend / Robot-side Tasks:**
    *   **Task 1.1.1:** Implement a discovery service on the robot's host machine that broadcasts its availability on the local network (e.g., using mDNS/zeroconf).
    *   **Task 1.1.2:** Implement a server (e.g., WebSocket) on the robot's host machine to manage connections and stream data.

*   **Frontend / App-side Tasks:**
    *   **Task 1.2.1:** Design and implement the UI for the "Welcome" screen, including a list view for discovered robots and a connection status indicator.
    *   **Task 1.2.2:** Implement the network discovery client to listen for broadcasts and populate the list of available robots.
    *   **Task 1.2.3:** Implement the connection logic to establish and maintain a connection with the selected robot's server.

*   **Acceptance Criteria (Definition of Done):**
    *   ✅ When the app is launched, it automatically begins scanning for robots.
    *   ✅ A list of discovered robots, identified by name, is displayed to the user.
    *   ✅ Tapping a robot in the list successfully establishes a connection.
    *   ✅ The UI clearly indicates the current connection status (e.g., "Scanning...", "Connecting...", "Connected").

**3.2. User Story 2: Manual Control**

*   **Backend / Robot-side Tasks:**
    *   **Task 2.1.1:** Create an API endpoint on the server to receive and execute 6-DOF movement commands for the robot arm.
    *   **Task 2.1.2:** Create an API endpoint to receive and execute open/close commands for the gripper.
    *   **Task 2.1.3:** Implement the video capture pipeline to stream the robot's camera feed to the connected client with minimal latency.

*   **Frontend / App-side Tasks:**
    *   **Task 2.2.1:** Design and implement the UI for the "Manual Control" screen, including the video display area and control overlays.
    *   **Task 2.2.2:** Implement the on-screen joystick components for arm movement.
    *   **Task 2.2.3:** Implement the on-screen buttons for gripper control.
    *   **Task 2.2.4:** Implement the logic to translate joystick movements into the appropriate 6-DOF commands and send them to the server.
    *   **Task 2.2.5:** Implement the video client to receive and render the live camera feed.

*   **Acceptance Criteria (Definition of Done):**
    *   ✅ Upon successful connection, the user is automatically navigated to the "Manual Control" screen.
    *   ✅ A live video feed from the robot's camera is clearly displayed.
    *   ✅ Moving the on-screen joysticks results in corresponding, real-time movement of the physical robot arm.
    *   ✅ Tapping the "Open" and "Close" buttons operates the physical gripper.
    *   ✅ The video feed remains stable during robot movement.

---

#### **4. Assumptions & Dependencies**

*   This plan assumes the existence of a LeRobot-compatible robot with a functional camera and network connectivity.
*   The engineering team will need to agree on the specific network protocols (e.g., WebSockets, gRPC, mDNS) to be used for communication.
