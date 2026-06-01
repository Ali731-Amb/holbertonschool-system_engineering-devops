# Web Infrastructure Design

## Description

This project covers the design of web infrastructures, from a simple single-server stack to a scaled, secured and monitored multi-server architecture.
Each task requires whiteboarding a diagram and being able to explain every component and design decision without notes.

---

## Learning Objectives

By the end of this project, you should be able to:

- Draw a diagram covering a complete web stack
- Explain what each component is doing
- Explain system redundancy
- Define the following acronyms: LAMP, SPOF, QPS

### Key acronyms

- **LAMP**: Linux, Apache, MySQL, PHP — a classic web stack combining an OS, web server, database and scripting language
- **SPOF** (Single Point of Failure): a component whose failure causes the entire system to go down
- **QPS** (Queries Per Second): a metric measuring the number of requests a server handles per second

---

## Requirements

- A README.md file at the root of the project folder is mandatory
- For each task, whiteboard the diagram (on paper, whiteboard, or software) and take a screenshot
- Upload the screenshot to an image hosting service (e.g. imgur)
- Insert the screenshot link into the answer file, then push to GitHub and insert the GitHub file link into the URL box
- Each task will be manually reviewed and whiteboarded in front of a mentor, staff member or student
- No computer or notes allowed during the whiteboarding session
- You have 30 minutes per exercise — answer what is asked, avoid unnecessary details

---

## Tasks

### 0. Simple web stack
Design a one-server web infrastructure hosting `www.foobar.com`.

Components: 1 server, Nginx, application server, codebase, MySQL, domain name with www A record pointing to IP `8.8.8.8`.

**Screenshot**: [![insert link here](file:///C:/Users/xalis/Downloads/Decision-Making%20Option%20Flow-2026-06-01-085037.png)]

---

### 1. Distributed web infrastructure
Design a three-server web infrastructure hosting `www.foobar.com`.

Components: 1 HAProxy load balancer (Round Robin, Active-Active), 2 servers each with Nginx, application server, codebase and MySQL (Primary-Replica cluster).

**Screenshot**: [![insert link here](file:///C:/Users/xalis/Downloads/Decision-Making%20Option%20Flow-2026-06-01-091223.png)]

---

### 2. Secured and monitored web infrastructure
Design a secured, encrypted and monitored three-server infrastructure hosting `www.foobar.com`.

Components: 3 firewalls, 1 SSL certificate (HTTPS), 3 monitoring clients reporting to Sumo Logic.

**Screenshot**: [![insert link here](file:///C:/Users/xalis/Downloads/Decision-Making%20Option%20Flow-2026-06-01-091936.png)]

---

### 3. Scale up
Design a scaled infrastructure with split components and a redundant load balancer.

Components: 1 additional server, HAProxy cluster (Active-Passive), dedicated servers for web server (Nginx), application server and database (MySQL).

**Screenshot**: [![insert link here](file:///C:/Users/xalis/Downloads/Decision-Making%20Option%20Flow-2026-06-01-133255.png)]

---

## Author

AMBLARD Alison — Holberton School