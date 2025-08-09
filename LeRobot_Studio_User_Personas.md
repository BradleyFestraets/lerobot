### **User Personas: LeRobot Studio**

**Version:** 1.0
**Status:** Draft
**Author:** Product Owner

---

#### **Introduction**

This document details the primary and secondary user personas for the LeRobot Studio application. These personas should guide our design, development, and testing efforts, ensuring we are building a product that meets the needs of our target users.

---

### **Primary Persona (MVP Target): Alex the Hobbyist**

**(Image: A young person in their late teens or early twenties, at a workbench cluttered with electronics, tools, and a partially assembled robot arm. They are looking at the robot with a mix of concentration and excitement.)**

*   **Quote:** *"I built this cool robot arm, and I see all these amazing AI videos online. I just want to make mine do something smart without having to become a professional programmer."*

*   **Bio:** Alex is a 19-year-old university student studying mechanical engineering. They love tinkering with electronics, 3D printing, and building things. They successfully followed an online guide to assemble an SO-101 robot arm and have it connected to their laptop. Alex is fascinated by AI and robotics but finds the software side intimidating. They've tried looking at some Python scripts but were quickly overwhelmed by the setup and complex code.

*   **Demographics:**
    *   **Age:** 18-25
    *   **Occupation:** Student / Hobbyist
    *   **Technical Skills:** Comfortable with hardware assembly and following guides. Basic to no programming experience. Not familiar with command-line interfaces.

*   **Goals & Motivations:**
    *   To see their physical creation come to life with AI.
    *   To learn the basic principles of how AI robotics works through a hands-on, visual process.
    *   To accomplish a simple but tangible task (e.g., get the robot to pick up a specific object).
    *   To have a cool project to show their friends or include in their portfolio.

*   **Frustrations & Pain Points:**
    *   Feels that the software/AI side of robotics is a "wall" they can't get past.
    *   Intimidated by text-based coding environments and complex setup procedures.
    *   Doesn't know where to start with training an AI model.
    *   Finds existing robotics software (like ROS) to have an extremely steep learning curve.

---

### **Secondary Persona (Future Target): Dr. Chen the Researcher**

**(Image: A person in their mid-30s in a university research lab, standing in front of a more advanced robot arm. They are looking thoughtfully at a monitor displaying graphs and data.)**

*   **Quote:** *"My research is in human-robot interaction, not in writing low-level drivers. I need a tool that lets me rapidly prototype new learning algorithms and collect data efficiently so I can focus on the science."*

*   **Bio:** Dr. Chen is a 35-year-old post-doctoral researcher at a university. Their work focuses on reinforcement learning and how humans can more effectively teach robots complex tasks. They are comfortable with Python and AI concepts but find that setting up new experiments, collecting demonstration data, and managing different hardware interfaces is tedious and time-consuming. It distracts from their primary research goals.

*   **Demographics:**
    *   **Age:** 28-45
    *   **Occupation:** Academic Researcher / Robotics Engineer
    *   **Technical Skills:** Proficient in Python, PyTorch, and AI/ML concepts. Familiar with Linux and command-line tools.

*   **Goals & Motivations:**
    *   To accelerate the pace of their research by reducing setup and data collection time.
    *   To easily test and compare different learning algorithms (e.g., HIL-SERL vs. standard Imitation Learning).
    *   To have a reliable and standardized platform for collecting high-quality demonstration data.
    *   To leverage advanced features like simulation and synthetic data to improve model robustness.

*   **Frustrations & Pain Points:**
    *   Spends too much time on engineering (data pipelines, hardware drivers) and not enough on research.
    *   The process of collecting teleoperated data is often clunky and requires custom scripts for each new project.
    *   Wishes for a unified interface that could handle everything from data collection to training and evaluation without constant context switching.
    *   Finds it difficult to onboard new students in the lab due to the complexity of the existing toolchain.
