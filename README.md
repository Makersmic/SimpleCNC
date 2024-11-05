# SimpleCNC
This repository documents the design, build, and setup process for a custom CNC router built with a focus on flexibility, affordability, and functionality for crafting various materials, including MDF, particle board, and aluminum. The CNC router is designed with modular G-code workflows, customizable macros, and tool-specific configurations for optimized and repeatable cutting paths.

##Project Overview

###Goals
Cost-Effective Build: Construct a robust CNC router on a limited monthly budget by sourcing affordable components and salvaging parts.
Precision and Flexibility: Design a machine capable of handling a range of materials with variable spindle speeds and multiple cutting tool configurations.
Modular Workflow: Streamline G-code operations with reusable macros, allowing for efficient setup and execution of custom parts.

###Key Components

Frame and Rails: Built from 2020 and 2040 aluminum extrusions, providing stability and flexibility for future upgrades.
Stepper Motors: Nema 17 motors with TB6600 drivers ensure controlled and reliable movement.
Lead Screws: T12 lead screws with 2mm pitch for precise linear travel on X and Y axes.
Spindle: Variable speed palm router adapted as a spindle for versatile material compatibility.
Control: Klipper firmware on a RUMBA board, with Mainsail/Moonraker for remote management and real-time monitoring.
###Features
Macro-Based G-code Execution: Separate setup, tool change, and cutting commands for repeatable and consistent workflows.
Adjustable Offsets: Customized workspace offset macros allow for precise positioning without relying on traditional G54 commands, enhancing compatibility with Klipper.
Flexible Power Control: Spindle power is managed through Klipper’s SET_PIN command, enabling real-time adjustments and safety stops.
Detailed Documentation: Step-by-step documentation for the design, build, and setup process is available for others interested in DIY CNC machines.
##Repository Structure
/docs: Documentation for setup, wiring, and component selection.
/config: Configuration files, including printer.cfg for Klipper, macros, and G-code templates.
/gcode: Sample G-code files for test cuts and setup operations.
/cad: 3D models and design files for custom parts and modifications.
/scripts: Scripts for post-processing G-code, including Excel-based post-processors with VBA for workflow automation.
##Getting Started
Hardware Setup: Follow the assembly instructions in the /docs directory for mechanical and electrical setup.
Firmware Installation: Use the configuration files in /config to install and tune Klipper on your controller board.
First Cuts: Execute the sample G-code files in /gcode to verify machine performance and troubleshoot.
Macro Integration: Implement customizable macros for offsets, homing, and spindle control to optimize cutting operations.
##Future Plans
Modular G-code Workflow: Continue developing a macro-based G-code system to simplify setup and part loading.
Advanced Tooling and Materials: Testing additional materials and advanced tooling strategies, including endmill-specific configurations.
User Interface Improvements: Enhancing Mainsail integration and exploring GUI improvements for ease of use.
##Contributing
Contributions are welcome! If you have improvements, bug fixes, or recommendations for additional features, please submit a pull request.
