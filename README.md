# HCIprojectSmartMuseum
project

Smart Museum Interactive System

Team:

    Mahmoud Rafaat
    Abdullah Ayman
    Ahmed Adel

Description:

This project implements an interactive system for a smart museum, designed to enhance visitor engagement and provide a personalized exploration experience. The system leverages a combination of technologies:

    Mobile App (C#): Developed with C# and socket programming, the mobile app acts as the primary interface for visitors. It interacts with the server, displays museum maps, guides navigation, and presents information about exhibits.
    Python Integration: Python is used for skeleton detection with MediaPipe and movement classification with DollarPy. Additionally, Python scripts handle marker recognition using TUIO (Tangible User Interface Objects).
    Server: Stores and processes data from various sources, including the mobile app, beacons, and museum staff input.
    Content Management System (CMS): Allows museum staff to manage and update exhibit information, including multimedia content.

Functionality:

    Visitor Enters Museum:
        Mobile app detects Bluetooth beacons and communicates with the server.
        Server identifies the visitor's location and retrieves relevant exhibit information from the CMS.

    Navigation:
        The mobile app displays a map highlighting the visitor's location and suggests nearby exhibits.
        Visitors can explore at their own pace.

    Information Delivery:
        As visitors approach an exhibit:
            The mobile app automatically displays information (text, historical context).
            Interactive elements like AR overlays and audio narration in multiple languages may be available.

    Personalization (Optional):
        Visitors can opt-in to receive personalized recommendations based on past interactions and preferences (analyzed by the system).

    Performance Tracking:
        Anonymized data on visitor behavior (time spent, exhibits explored, content accessed) is collected to:
            Understand visitor interests.
            Improve exhibit organization and information delivery.
            Develop personalized content and tours based on demographics and preferences.

Marker Recognition (TUIO):

    Python scripts running on a separate machine or integrated into the server process data from a camera to recognize markers placed in the museum environment.
    Recognized markers can trigger specific actions within the mobile app, such as displaying additional content or activating interactive elements.

Context-Based Content Loading:

    The mobile app communicates context information (e.g., visitor location, marker type) to the server.
    The server retrieves appropriate content (text, images, audio, video) based on the context and sends it to the mobile app for display.

Additional Considerations:

    Socket communication between the C# mobile app and Python scripts using libraries like ZeroMQ or a similar solution.
    User interface design for the mobile app should be intuitive and user-friendly for all age groups.
    Security measures to protect visitor data privacy.
    Error handling and logging for robust system operation.

Getting Started (Placeholder):

    Specific instructions on setting up the development environment (C# and Python), installing dependencies, and running the system will be added here once development progresses.

Future Development:

    Enhance the system with additional features such as gamification elements, social interaction capabilities, and real-time location tracking (subject to visitor consent).
    Continuously improve personalization algorithms based on user feedback and interaction data.
