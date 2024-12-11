# Git Assignment - Hero Vired

## Table of Contents

- [Project Overview](#project-overview)
- [Features Implemented](#features-implemented)
- [Repository Structure](#repository-structure)
- [How to Use the Project](#how-to-use-the-project)
- [Workflow Details](#workflow-details)
- [Collaborators and Reviews](#collaborators-and-reviews)
- [Releases](#releases)
- [Acknowledgments](#acknowledgments)

## Project Overview
This repository contains solutions for the **Hero Vired Git Assignment**. It demonstrates the use of Git and GitHub for version control, collaborative development, branching, and stashing, along with a Python application showcasing multiple functionalities.

## Features Implemented

### **1. Calculator Plus Application**
- **Basic Features**:
  - Addition
  - Subtraction
  - Multiplication
  - Division
- **Enhanced Features**:
  - Square root calculation
  - Division bug fix: Handles division by zero gracefully by raising an exception.

### **2. Git LFS Integration**
- Added and tracked large binary files (>200MB) efficiently using Git LFS.
- Verified LFS setup by cloning the repository on another machine.

### **3. Geometry Calculator**
- Calculates:
  - Area of a Circle
  - Area of a Rectangle
- Utilized Git stash to switch between incomplete features without committing changes.

## Repository Structure
```
├── main
│   ├── calculator_plus_app
│   │   └── calculator.py
│   └── geometry_calculator
│       └── geometry.py
├── feature/sqrt
│   └── calculator.py
├── lfs
│   └── large_binary_file.bin
├── README.md
└── .gitattributes (for Git LFS tracking)
```

## How to Use the Project

### Prerequisites
- Python 3.x
- Git installed on your system

### Steps to Clone and Use
1. Clone the repository:
   ```bash
   git clone https://github.com/Karthikn/git_assignment_HeroVired.git
   ```

2. Navigate to the repository:
   ```bash
   cd git_assignment_HeroVired
   ```

3. Run the Calculator Plus application:
   ```bash
   python calculator_plus_app/calculator.py
   ```

4. Run the Geometry Calculator application:
   ```bash
   python geometry_calculator/geometry.py
   ```

### For LFS Verification
- Ensure Git LFS is installed: [Git LFS Documentation](https://git-lfs.github.com/)
- Clone the repository on another machine and confirm large files are downloaded.

## Workflow Details

### **Branching Strategy**
- **`dev` Branch**: Active development branch.
- **`feature/sqrt` Branch**: Added square root functionality.
- **`lfs` Branch**: Used for Git LFS setup.
- **`geometry-calculator` Branch**: Sub-branches for circle and rectangle area features.

### **Bug Fix**
- Critical bug in `divide()` function fixed in the `dev` branch and propagated to other branches using rebase.

### **Stashing Example**
- Used `git stash` to save and switch between `circle-area` and `rectangle-area` feature branches.

### **Pull Requests (PRs)**
- PRs created for each feature branch to merge into the `main` branch.
- Code reviews performed by collaborators.

## Collaborators and Reviews
- **Owner**: [Karthikn](https://github.com/Karthikn)
- **Collaborators**: Added [aakashrawat1910] for code reviews.
- Reviewed and approved changes for `feature/sqrt` and `geometry-calculator` branches.

## Releases
- **Version 1.0**: Basic Calculator Plus application.
- **Version 2.0**: Enhanced with square root functionality and bug fixes.

## Acknowledgments
- [Hero Vired Assignment Guidelines](https://vlearn.hero-vired.com)
- [Git LFS Documentation](https://git-lfs.github.com/)
