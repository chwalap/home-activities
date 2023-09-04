# Home Activity Tracker & Rewards System

## Overview

The Home Activity Tracker & Rewards System is a Python-based application that tracks and rewards domestic activities. It uses a Raspberry Pi 4 as the server to capture NFC tags scanned via smartphones. This system is designed for multi-user environments, specifically focusing on households. The system includes features such as daily, weekly, and monthly leaderboards and to-do lists.

## Key Features

- **Multi-User Support**: Supports multiple users (Paweł and Jacqueline, in this case).
- **NFC Enabled**: Use NFC stickers around the house to report activities like brushing teeth, doing laundry, etc.
- **Activity Points**: Assigns point values to each activity.
- **Leaderboards**: Daily, weekly, and monthly leaderboards.
- **To-Do Lists**: Automatically generated to-do lists based on daily and weekly required activities.
- **Session Persistence**: Uses SQLite to manage sessions, making it robust against server restarts.

## Installation & Setup

### Prerequisites

- Raspberry Pi 4 with Raspbian installed.
- Python 3.x
- NFC-enabled smartphones

### Steps

1. **Clone the Repository**
    ```bash
    git clone [https://github.com/yourusername/HomeActivityTracker.git](https://github.com/chwalap/home-activities.git)
    ```

2. **Navigate to the Directory**
    ```bash
    cd HomeActivityTracker
    ```

3. **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4. **Set Environment Variables**
    Set the Flask secret key as an environment variable.
    ```bash
    export FLASK_SECRET_KEY=your_secret_key_here
    ```

5. **Run the Application**
    ```bash
    python app.py
    ```

## Usage

1. **Set User**
    - Navigate to the homepage and select the user.
  
2. **Report Activity**
    - Simply scan an NFC sticker linked to an activity. The activity will be recorded and points will be allocated accordingly.

## Contributing

Feel free to fork the project, open a PR, or submit an issue.

---

This README provides a good starting point and can be expanded as the project grows. Feel free to adjust as needed.
