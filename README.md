# **Vasofón: Your Family Intercom**

Vasofón is a family intercom application designed to simplify communication within your household. Unlike traditional messaging apps, Vasofón focuses on device-based interaction rather than user accounts, creating an intuitive and fun system for everyone.

The name "Vasofón" is a playful take on the classic "cup and string telephone," capturing the app's spirit of simple, direct family connection.

### **Key Features**

* **Device-Centric Registration:** The system registers each device (phone, tablet, computer) to a single family group. This allows multiple family members to share a single device without complex login/logout procedures.  
* **Intelligent Messaging:** The app automatically sends messages directly to a person if it knows their current device. If not, it uses a **broadcast** to all family devices to find the intended recipient.  
* **Effortless "Login":** User identification is handled simply by responding to a broadcast message. The first person to acknowledge a message on a device is temporarily "logged in."  
* **Family Bot:** A built-in bot handles all system notifications, such as new device registration requests and future reminders, keeping user-to-user conversations clean and focused.  
* **"Virtual Flip-Flop":** A special, humorous feature for grabbing a family member's attention in a fun, non-intrusive way.

### **Technical Stack**

Vasofón is built with a modern, scalable, and asynchronous architecture, making it fast and efficient.

* **Backend:** Python with **FastAPI** for a high-performance, asynchronous server, deployed on **GCP App Engine**.  
* **Database:** **PostgreSQL**, managed via **GCP Cloud SQL**, to securely store all group, device, and user information.  
* **Real-time Communication:** **WebSockets** for persistent connections and **Firebase Cloud Messaging (FCM)** for push notifications on Android devices.  
* **Frontend:** The application will be a cross-platform solution for **Android**, **Windows**, and **Linux**, ensuring a consistent experience across all devices.

### **Licensing**

This project is licensed under the **GNU Affero General Public License (AGPL)**. This means the source code is free to use, modify, and distribute. However, if you use this code to run a public service, you are required to share your changes with the community. This license helps protect the core project while allowing for a sustainable, open-source model.
