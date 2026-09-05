# Garage Ops Enhancements

This repository contains project documentation, assigned job profiles, hardware references and member-developed work for Garage@EEE enhancement projects.

## What is GIP?

**Garage-Initiated Projects (GIP)** is a structured project-development initiative where Garage members work on real Garage needs while gaining practical technical and project experience.

For AY2026/27, GIP is being introduced as a pilot programme with two pathways.

### Guided Portfolio Projects

* Projects are proposed in response to identified Garage needs.
* Project Leads or Persons-in-Charge guide the assigned members.
* The initial project scope, deliverables and team size are defined before development begins.

### Member-Proposed Projects

* Members may propose their own ideas for improving Garage.
* Proposals are reviewed based on relevance, feasibility, available resources, safety and mentor support.

## Awards

Projects may be recognised through the following award categories:

* 🏆 **Grand Garage Impact Award** — prize amount to be confirmed
* 🏆 **Garage Impact Award** — prize amount to be confirmed
* 👥 **People’s Choice Award** — prize amount to be confirmed
* ♻️ **Sustainability and Handover Award** — prize amount to be confirmed

These awards recognise project impact, usefulness to the Garage community, sustainability, documentation quality and successful project handover.

## Current Projects

### Talking Robot

The Talking Robot project consists of:

* **Moving Pet Bot**
* **Stationary Desk Buddy**

Both robots share the same lightweight LLM, voice and Garage@EEE knowledge-retrieval system. The Pet Bot also includes movement, obstacle detection, table-edge detection and computer vision.

### More Tea

More Tea is a Linorobot2-based tour and navigation robot using ROS 2, a Jetson host and an ESP32 micro-ROS controller.

The main development focus is reliable navigation, including motor control, encoder feedback, LiDAR, IMU, mapping, localization, Nav2 and touchscreen-selected destinations. Perception and manipulation are later extensions after navigation has passed acceptance testing.

## Repository Structure

* `skills-journeys/` — general learning and skills-development documents
* `talking-robot/` — Pet Bot and Desk Buddy timelines, hardware reports, job profiles and member work
* `more-tea/` — More Tea timeline, hardware report, job profiles and member work

Each project contains a `job-profiles/` folder. Members should enter their assigned role folder to find:

* Role responsibilities
* Weekly tasks
* Relevant hardware and interfaces
* Component and voltage information
* Testing and evidence requirements
* Folders for uploading programs, designs and results

## How Members Should Use This Repository

1. Open the folder for the assigned project.
2. Read the project timeline, hardware-components report and general job-profile document.
3. Open the assigned folder under `job-profiles/`.
4. Check the tasks for the current active week.
5. Upload programs, PCB files, CAD files, configurations and test evidence into the relevant work folder.
6. Document component ratings, voltages, interfaces and test results before integration.
7. Submit changes through the agreed review process before merging them into the main project.
