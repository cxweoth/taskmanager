# taskmanager

A Versatile Task Scheduling and Lifecycle Management Library

TaskManager is a robust and versatile Python library designed for efficient task scheduling and lifecycle management across multiple platforms. Optimized for both Windows and Linux systems, it offers seamless performance even in environments with limited computational resources, without the need for heavy external dependencies or specialized setups.

## Key Features

- **Flexible Scheduling Options**: Supports a variety of scheduling needs, including periodic tasks, daily fixed-time tasks, and weekly tasks set to specific times.

- **Lifecycle Management**: Advanced lifecycle control monitors the execution status of tasks, issuing events when tasks exceed their allotted time and forcibly stopping them if they do not terminate within this period.

- **Automatic Logging**: Features automatic logging capability, allowing users to specify the path for storing logs, crucial for tracking and analyzing system operations.

- **Lightweight and User-Friendly**: Designed with a focus on user experience and system efficiency, ensuring smooth operation on less powerful systems.

- **Cross-Platform Compatibility**: Delivers consistent performance and user experience on both Windows and Linux operating systems.

## Installation

```bash
pip install taskmanager
```
## Usage
Here's a quick start example of how to use taskmanager:

```python
from taskmanager import Scheduler

# Create a new scheduler instance
scheduler = Scheduler()

# Schedule your tasks
scheduler.every(10).minutes.do(job)
scheduler.every().hour.do(job)
scheduler.every().day.at("10:30").do(job)
scheduler.every().monday.do(job)
scheduler.every().wednesday.at("13:15").do(job)

# Start the scheduler
scheduler.run()
```

For more detailed usage, please refer to the [documentation]().

## Contributing
Contributions to taskmanager are welcome! Please refer to the [contributing guidelines]() for more information.

