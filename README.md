# JWT Session Authentication Server (Authentication Security Engineering Lab)

## Project Introduction

The JWT Session Authentication Server is a defensive cybersecurity project that explores how modern login mechanisms can be designed to resist database-driven attacks.

This project demonstrates the transition from insecure authentication logic to a protected implementation using secure query handling, attack detection techniques, and structured logging.

It acts as a controlled simulation environment where authentication vulnerabilities can be studied and mitigated through practical engineering solutions.

The system highlights how improper input handling can lead to unauthorized access and how secure coding practices can effectively neutralize such risks.

## Key Functional Highlights

* Robust credential verification mechanism backed by structured database storage
* Implementation of secure query handling techniques to prevent manipulation of authentication logic
* Integrated detection layer that identifies potentially malicious login inputs
* Automatic logging of abnormal authentication attempts for monitoring and analysis
* Controlled comparison between insecure and hardened authentication workflows
* Lightweight database initialization and user record management
* Command-line driven interaction model enabling safe security testing scenarios
* Demonstration of defensive programming principles applied to identity verification systems
* Practical simulation of real-world authentication attack surfaces and mitigation strategies
* Modular design allowing easy extension into full secure web authentication frameworks


## Core Security Capabilities

* Secure user authentication using database-backed credential validation
* Detection of suspicious input patterns associated with injection attempts
* Implementation of parameterized SQL queries to prevent query manipulation
* Real-time logging of abnormal authentication behaviour
* Automatic database initialization and controlled user storage
* Comparison between vulnerable and secure authentication workflows
* Lightweight command-line interaction for controlled testing
* Demonstration of defensive software architecture in authentication systems

## How the System Works

1. The application initializes a local SQLite database and creates a user table if it does not exist.
2. A default user record is inserted to simulate a production login environment.
3. During login:

    * User input is analyzed for suspicious SQL patterns.
    * Potential attack attempts are logged to a dedicated security log file.
4. The secure authentication module performs credential verification using parameterized queries.
5. The vulnerable module demonstrates how unsafe string-based queries can be exploited.

This workflow helps illustrate both attack methodology and defensive mitigation strategies.


## Project Structure
```
jwt-session-auth-server/
│
├── app_secure.py        → Secure login implementation
├── app_vulnerable.py    → Demonstration of insecure authentication
├── users.db             → Local authentication database
├── attack_logs.txt      → Security event logging file
└── README.md
```


## Technologies Used

* Python
* SQLite Database
* Secure Query Parameterization
* Input Pattern Analysis
* Defensive Security Logging


## Example Usage

Run the secure version:
```
python app_secure.py
```
Run the vulnerable version (for learning demonstration):
```
python app_vulnerable.py
```

Try different login inputs to observe:

* Normal authentication behavior
* Detection of suspicious login attempts
* Differences between secure and insecure query execution


## Performance Characteristics

* Fast local database operations
* Minimal system resource consumption
* Efficient authentication query execution
* Lightweight detection overhead
* Suitable for educational penetration testing simulations

## Security Significance

This project demonstrates applied defensive engineering skills in:

* Secure authentication design
* Database protection methodology
* Input validation strategies
* Attack surface reduction
* Logging and monitoring integration
* Secure software development mindset

It reflects real challenges faced in backend security engineering and identity management systems.


## Educational Outcomes

Through this implementation, the following competencies are developed:

* Understanding authentication vulnerabilities
* Designing secure database interaction layers
* Implementing detection-based defensive controls
* Developing structured cybersecurity lab environments
* Translating theoretical security concepts into working systems
* Building research-ready cybersecurity demonstration tools


## Intended Use

This system is developed strictly for:

* Cybersecurity learning
* Secure coding experimentation
* Vulnerability research
* Academic security demonstrations

It must only be executed in controlled environments.


## Author

Developed as part of a practical cybersecurity engineering initiative focused on authentication security and defensive system architecture.


## License

This project is released for educational and research purposes.
Users are responsible for ethical usage and authorized testing only.
