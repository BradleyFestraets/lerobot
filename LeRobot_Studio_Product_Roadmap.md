### **Product Roadmap: LeRobot Studio**

**Version:** 1.0
**Status:** Draft
**Author:** Product Owner

---

#### **1. Introduction**

This document provides a strategic, high-level overview of the planned evolution for the LeRobot Studio application. It is organized into thematic phases, each delivering a significant new layer of value to our users. This roadmap is a living document and will be updated based on user feedback, technical discoveries, and strategic priorities.

---

### **Phase 1: The MVP - The Core Learning Loop**

*   **Theme:** Enable the fundamental user journey of teaching a robot a new skill through demonstration.
*   **Target Persona:** Alex the Hobbyist.
*   **Goal:** To deliver a functional, end-to-end imitation learning experience that is simple, rewarding, and validates our core product assumptions.

| Key Features |
| :--- |
| **Robot Connection:** Auto-discovery and connection to LeRobot-compatible hardware. |
| **Manual Control (Live Drive):** Direct, real-time teleoperation for setup and simple tasks. |
| **Demonstration Recording:** A simple interface to record a single demonstration for a single skill. |
| **Model Training:** A one-click process to train a basic imitation learning model. |
| **Skill Execution:** A simple interface to run the newly trained skill on the robot. |

---

### **Phase 2: The Intelligent Assistant - Language & Awareness**

*   **Theme:** Make the robot a more intuitive and interactive partner by giving it the ability to see and understand.
*   **Target Persona:** Alex the Hobbyist (enhanced experience), Dr. Chen the Researcher (initial appeal).
*   **Goal:** To move beyond simple command-execution to a more conversational and aware interaction model.

| Key Features |
| :--- |
| **Scene Awareness (VLM):** Integrate a Vision-Language Model to allow users to ask questions about the robot's environment (e.g., "How many blocks are on the table?"). |
| **AR Highlighting:** Provide visual feedback by highlighting objects in the live video feed that the robot is referring to. |
| **Language-Assisted Learning (SmolVLA):** Upgrade the training pipeline to incorporate natural language descriptions, enabling the robot to be controlled with text commands. |
| **Conversational Interface:** Evolve the "Run a Skill" screen into a chat-based interface for both commanding and questioning the robot. |

---

### **Phase 3: The Advanced Learner - Continuous Improvement & Simulation**

*   **Theme:** Introduce powerful, state-of-the-art training paradigms for advanced users and researchers.
*   **Target Persona:** Dr. Chen the Researcher.
*   **Goal:** To provide tools that accelerate research, enable the creation of more robust models, and allow the robot to learn from its mistakes.

| Key Features |
| :--- |
| **Interactive Coaching (HIL-SERL):** A "Coach Mode" that allows users to correct the robot's mistakes in real-time and use that feedback to fine-tune the model. |
| **The Virtual Training Ground:** An integrated simulation environment where the robot can learn safely and efficiently. |
| **Reinforcement Learning (RL) Pipeline:** An interface for training models from scratch using a visual reward editor instead of human demonstrations. |
| **Synthetic Data Generation:** Tools to automatically vary the simulation environment to improve the model's robustness in the real world. |

---

### **Phase 4: The Collaborative Platform - Community & Ecosystem**

*   **Theme:** Build a network effect by connecting our users and enabling them to share their creations.
*   **Target Persona:** All users.
*   **Goal:** To foster a vibrant community that collectively accelerates the pace of robotic learning.

| Key Features |
| :--- |
| **The Brain Hub:** An integrated, user-friendly browser for a community hub of trained models. |
| **One-Click Download:** Allow users to seamlessly download and deploy community-trained "brains" on their own robots. |
| **Simple Upload:** A streamlined process for users to share their own trained models with the community. |
| **User Profiles & Leaderboards:** Basic community features to encourage participation and recognize top contributors. |

---

### **Future Vision: The Autonomous Partner**

*   **Theme:** Explore the next frontier of robotics, moving from a tool that follows commands to a partner that can anticipate needs.

| Potential Features |
| :--- |
| **Cognitive Core (Voice & LLM Reasoning):** A hands-free, voice-controlled interface and a powerful LLM for advanced reasoning and dynamic problem-solving. |
| **AR Safety Overlays:** A holographic "ghost" of the robot's intended path, shown for user confirmation before any physical action is taken. |
| **Long-Horizon Task Planning:** The ability for the robot to understand complex, multi-step goals and generate its own plan to achieve them. |
| **Proactive Assistance:** The ultimate goal where the robot can perceive its environment and proactively offer help without being prompted. |
