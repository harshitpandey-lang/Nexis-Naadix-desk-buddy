# Development Journal

## Phase 1 — Project Ideation

### 3 April 2026

This project started with a simple question:

> Can a physical device control a computer like a human without directly modifying the operating system?

To answer this, I began studying USB Human Interface Devices (HID), including keyboards, mice, scan codes, USB descriptors, and how computers interpret physical input devices. The goal was to understand whether an AI-generated plan could eventually be converted into keyboard and mouse actions.

During this stage I spent most of my time researching, sketching ideas, and defining the overall system architecture. The concept evolved into a desk companion capable of receiving natural language commands and controlling a computer through standard HID protocols.

### 18 April 2026

I started documenting the project more seriously and created a portfolio channel to track progress. At this point the focus was still on defining the final vision.

The larger goal was no longer just building a device. The goal became building an intelligent desk environment capable of improving productivity through automation.

### 21 April 2026

This marked the beginning of OAI.

OAI (Online AI) was designed as the cloud intelligence layer of the project. I spent this phase exploring how an AI model could convert natural language into structured action plans.

The initial architecture focused on:

* Command understanding
* Intent extraction
* Planning
* Structured JSON outputs

This was the first major step toward turning a spoken command into an executable workflow.

### 22 April 2026

I revisited the architecture and redesigned the entire OAI concept.

During this stage I documented:

* What OAI is
* Why Nexis needs OAI
* How commands would travel through the system
* How HID actions would eventually be generated

This redesign established the foundation that the rest of the project still follows today.

### 24 April 2026

The long-term vision became clearer.

The project was no longer about controlling a computer.

It became about:

* Productivity enhancement
* Workflow automation
* Voice interaction
* Physical AI interfaces

This phase helped transform scattered ideas into a focused project roadmap.

## Phase 2 — Building OAI

### 25 April 2026

This was the day I began implementing OAI.

Since most of the hardware had not yet been acquired, I decided to start with the software architecture first. The objective was to create an online agent capable of converting a normal human command into structured actions that could later be executed through HID devices.

At this stage the focus was on:

* Command normalization
* Intent understanding
* System architecture
* Action generation

This was the first working version of the project beyond sketches and diagrams.

### 26 April 2026

Development continued on the OAI system.

A significant amount of time was spent documenting the code and improving maintainability. Since the project was becoming larger than initially expected, I started adding detailed comments and explanations throughout the codebase.

The goal was to ensure that future changes could be made without having to completely relearn the architecture.

### 27 April 2026

I spent time refining the hardware architecture and evaluating component choices.

Initially the ESP32-S3 was considered the primary controller because of its built-in WiFi, Bluetooth, and USB HID capabilities. During this stage I explored how the touchscreen would be integrated into the user experience and how execution approval could be handled through the device itself.

This phase helped bridge the gap between software planning and physical hardware design.

### 28 April 2026

This became one of the most important milestones in the project.

The core OAI architecture was completed:

* Normalizer
* Planner
* Validator
* Executor
* HID Mapping
* Communication Layer

For the first time, the system could take a natural language command, break it into logical steps, verify those steps, and prepare them for execution.

This transformed OAI from an idea into a functional software system.

### 29 April 2026

Development continued with:

* Feedback system work
* Preferences handling
* Testing
* Documentation

The focus shifted from creating features to making the existing architecture reliable and understandable.

---

## Phase 3 — Deployment

### 1 May 2026

After multiple debugging sessions, OAI was successfully deployed online.

Several issues had to be resolved:

* API migration
* Environment configuration
* GitHub setup
* Deployment errors
* UI testing

By the end of this phase, the software portion of the project was functioning through a cloud deployment and accessible through GitHub.

This represented the completion of the first major subsystem of Nexis.

### 2 May 2026

Further work was done on deployment reliability and testing.

The objective was not just to make the system work, but to ensure it could remain accessible and stable through an online environment.

This stage also marked the point where I started preparing for the transition into hardware development.

### 8 May 2026

The architecture was formally documented.

At this stage I clarified the role of OAI within the complete system:

* Understand commands
* Create execution plans
* Validate actions
* Return structured outputs

Importantly, OAI was never intended to directly control hardware. Instead, it acts as the intelligence layer responsible for generating safe and structured instructions for Nexis to execute.

---

## Phase 4 — Hardware Acquisition

### 19 May 2026

After spending several weeks on software, I finally obtained some of the required hardware.

The most important addition was a Raspberry Pi 4 Model B along with supporting accessories.

During this stage I also worked on early enclosure concepts and rough CAD designs. Although the designs were still incomplete, they provided a clearer picture of the final device layout.

Progress was slower than expected because of academic commitments and examinations, but this period helped transition the project from a software-only concept into a physical product.

## Phase 5 — Mechanical Design

### 24–25 May 2026

With the software foundation completed and hardware beginning to arrive, I shifted my focus toward the physical design of Nexis.

Fusion 360 became the primary design tool for creating the enclosure. The goal was not simply to place components inside a box but to create a desk companion that felt intentional and usable.

The enclosure design focused on:

* Front-facing display
* Dedicated control buttons
* Rotary encoder integration
* Speaker placement
* PCB mounting locations
* Raspberry Pi accessibility

During this period I completed the majority of the external structure and established the overall form factor of the device. The process required multiple iterations and a significant amount of experimentation due to hardware constraints and limited prior CAD experience.

### Key Lesson

Mechanical design is often underestimated. A design that works electronically may not work physically. Component placement, mounting methods, cable routing, and serviceability all need to be considered early.

---

## Phase 6 — Learning KiCad

### 28 May 2026

This marked my first serious experience with PCB design.

Before this project I had never designed a complete PCB, so a considerable amount of time was spent learning the fundamentals before actual development could begin.

Resources used included:

* Official KiCad documentation
* Community tutorials
* Philip's Lab content
* Datasheets
* Practical experimentation

The initial objective was to understand:

* Symbols
* Footprints
* Net connections
* ERC checks
* PCB workflow

At the same time I selected the primary modules for the design:

* MAX98357A
* INMP441
* Power subsystem
* Raspberry Pi interface
* User controls

This phase was less about producing a finished PCB and more about building the knowledge required to design one correctly.

---

## Phase 7 — PCB Schematic Development

### 29 May 2026

After becoming comfortable with the basic workflow, I began creating the actual Nexis schematic.

The schematic gradually evolved from disconnected modules into a complete electrical system.

Integrated subsystems included:

* Audio input
* Audio output
* Raspberry Pi interface
* User controls
* Power management
* Expansion headers

A major challenge during this stage was understanding how all components interact electrically while maintaining a clean and maintainable schematic.

As a first-time KiCad user, progress was slower than expected, but every revision improved both the design and my understanding of PCB development.

---

## Phase 8 — PCB Layout

### 29–30 May 2026

Once the schematic reached a stable state, work began on PCB layout.

This involved:

* Footprint assignment
* Component placement
* Routing
* Power distribution
* Connector placement

Special attention was given to components that directly affect usability:

* Buttons
* Rotary encoder
* Audio subsystem
* Raspberry Pi mounting

## By the end of this phase the rough PCB layout was completed and the project had reached a stage where manufacturing preparation could begin.

## Phase 9 — Final Mechanical Integration

### 30 May 2026

With both CAD and PCB development progressing, I returned to the enclosure and integrated mounting features.

Completed work included:

### PCB Mounting

* PCB support pillars
* Fastener locations
* Internal structure

### Speaker Mounting

* Dedicated speaker cavity
* Structural support

### Front Panel

* Display opening
* Button locations
* Rotary encoder placement

### Rear Section

* Internal component space
* Structural framework

Several mechanical details remain intentionally unfinished because they depend on final hardware testing and PCB validation.

Examples:

* Final port cutouts
* Battery retention system
* Display mounting refinements

These will be completed after physical prototyping.

---

# Current Project Status

## Completed

### OAI

* Architecture
* Development
* Validation
* Deployment

### Hardware

* Component Selection
* System Architecture
* CAD Design
* PCB Schematic
* Initial PCB Layout

### Documentation

* Research Notes
* Development Journal
* BOM
* Architecture Planning

---

## In Progress

### PCB

* Design validation
* Manufacturing preparation

### Firmware

* ESP32 HID implementation
* Communication testing

### Mechanical Design

* Final enclosure refinement

---

## Future Work

### Hardware

* PCB fabrication
* Soldering and assembly
* Wiring integration

### Firmware

* HID testing
* WiFi communication
* User interaction

### Validation

* End-to-end testing
* Reliability improvements

---

# Reflection

This project started as a simple idea inspired by the concept of a highly capable personal workstation.

What began as research into USB HID systems eventually evolved into a complete ecosystem consisting of:

* OAI (cloud intelligence)
* Nexis (physical interface)
* Custom electronics
* Custom enclosure
* Embedded firmware

The most valuable part of this journey has not been the final design itself but the amount of learning required to reach it.

The project introduced me to:

* System architecture
* AI workflows
* Embedded systems
* CAD design
* PCB development
* Hardware documentation

Nexis is still evolving, but it has already achieved its primary goal: turning an ambitious idea into a tangible engineering project.

# Nexis Timeline

03 Apr 2026
Project ideation and HID research.

18 Apr 2026
Project vision documentation and portfolio planning.

21 Apr 2026
Initial OAI architecture exploration.

22 Apr 2026
OAI redesign and architecture definition.

24 Apr 2026
Project goals and long-term vision established.

25 Apr 2026
OAI implementation started.

25 Apr 2026
Early hardware experimentation and documentation.

26 Apr 2026
Code documentation and architecture refinement.

27 Apr 2026
Hardware architecture planning.

28 Apr 2026
Core OAI components completed.

29 Apr 2026
Feedback system and testing work.

01 May 2026
GitHub integration and debugging.

02 May 2026
Render deployment and online testing.

08 May 2026
OAI architecture documentation.

19 May 2026
Hardware acquisition and early CAD planning.

24 May 2026
Front enclosure CAD design.

25 May 2026
Rear enclosure CAD design.

28 May 2026
KiCad learning and PCB schematic creation.

29 May 2026
PCB schematic development.

29 May 2026
PCB component placement and integration.

30 May 2026
PCB design completion and enclosure refinement.

