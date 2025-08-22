# LiPo Battery Charging Trainer

An interactive web application designed to teach safe battery charging practices for RC (Remote Control) purposes through flashcard-style learning.

## Overview

This single-page web app simulates a battery charger interface where users learn to set correct charging parameters for different battery types and configurations. The app presents random battery scenarios and validates user inputs against real-world safety standards.

## Key Features

### 📱 Responsive Design
- Works seamlessly on desktop, tablet, and mobile devices
- Adaptive layout that stacks vertically on smaller screens
- Touch-friendly controls optimized for mobile interaction

### 🎚️ Three Difficulty Levels

#### Easy Mode
- Single LiPo batteries only
- 1-8S cell configurations (1 to 8 cells in series)
- Capacity range: 300-1800mAh in 50mAh increments
- Perfect for beginners learning basic charging principles

#### Medium Mode
- Mix of LiPo and Li-ion battery types
- LiPo: Same specs as Easy mode
- Li-ion: 3000-5000mAh in 500mAh increments
- Teaches users about different charging characteristics

#### Hard Mode
- Parallel charging scenarios (1-4 identical batteries)
- Tests ability to calculate correct current for multiple batteries
- All batteries in a set have matching cell count and type
- Challenges understanding of parallel charging principles

### 🔋 Battery Visualization

#### LiPo Batteries
- Represented as stacked isometric rectangles with rounded edges
- Each rectangle represents one cell in the series
- Cell length varies based on capacity (up to a reasonable limit)
- Realistic 3D appearance with shadows and gradients

#### Li-ion Batteries
- Depicted as groups of cylindrical cells (18650 style)
- Number of cylinders matches cell count
- Consistent sizing regardless of capacity
- Authentic battery terminal details

#### Parallel Charging Display
- Multiple battery packs shown side by side
- Connected with '+' symbols to indicate parallel configuration
- Clear visual representation of multi-battery setups

### ⚡ Realistic Charger Interface

#### Automatic Cell Detection
- Displays detected cell count (S rating) like real chargers
- Shows single battery cell count for Easy/Medium modes
- Shows cell count of one battery in parallel setups for Hard mode

#### Voltage Control
- Precision voltage setting with 0.01V increments
- Range: 3.00V to 4.50V per cell
- Plus/minus buttons for fine adjustment
- Direct number input with validation
- Monospace display for technical accuracy

#### Current Control
- Current setting with 0.1A increments
- Range: 0.1A to 10.0A
- Plus/minus buttons for easy adjustment
- Direct number input with bounds checking
- Real-time value display

### 🛡️ Safety Rating System

#### LiPo Battery Safety Standards
- **1C and below**: Safe charging rate
- **1-2C**: Fast charging but low risk (monitor temperature)
- **2-3C**: Risky charging with high damage potential
- **Above 3C**: Not recommended - extremely dangerous

#### Li-ion Battery Safety Standards
- **0.5C and below**: Safe charging rate
- **0.5-1C**: Fast charging but low risk (monitor temperature)
- **Above 1C**: Not recommended for Li-ion chemistry

#### Voltage Validation
- LiPo: 4.20V per cell maximum
- Li-ion: 4.10V per cell maximum
- Incorrect voltage settings trigger danger warnings

### 🎨 User Interface Design

#### Modern Aesthetic
- Gradient background with professional color scheme
- Glassmorphism effects with semi-transparent elements
- Clean typography with technical monospace fonts
- Smooth animations and micro-interactions

#### Color-Coded Feedback
- **Green**: Safe charging parameters
- **Yellow**: Fast charging with caution advised
- **Orange**: Risky parameters with warnings
- **Red**: Dangerous settings with strong warnings

#### Interactive Elements
- Hover effects on all interactive components
- Visual feedback for button presses
- Smooth transitions between states
- Responsive button scaling

## Technical Implementation

### Battery Model
- Object-oriented battery class system
- Accurate C-rate calculations
- Safety rating algorithms based on industry standards
- Support for both single and parallel battery configurations

### Responsive Scaling
- CSS Grid layout for main flashcard interface
- Flexbox for control arrangements
- Media queries for mobile optimization
- Scalable battery visualizations

### Input Validation
- Real-time bounds checking on all inputs
- Automatic value correction for out-of-range entries
- Keyboard and mouse input support
- Touch-friendly mobile controls

## Usage Instructions

1. **Select Difficulty**: Choose from Easy, Medium, or Hard modes
2. **Study the Battery**: Examine the battery label and visualization
3. **Set Parameters**: Adjust voltage per cell and charging current
4. **Check Answer**: Submit your settings for safety validation
5. **Learn from Feedback**: Review the safety rating and explanation
6. **Next Question**: Generate a new random battery scenario

## Safety Education Goals

- Understanding C-rate calculations and their importance
- Learning proper voltage settings for different battery chemistries
- Recognizing the risks of fast charging
- Developing intuition for safe charging practices
- Building confidence in real-world battery handling

## Browser Compatibility

- Modern web browsers with ES6 support
- Chrome, Firefox, Safari, Edge (latest versions)
- Mobile browsers on iOS and Android
- No external dependencies required

## File Structure

```
/
├── index.html          # Complete single-page application
└── README.md          # This documentation file
```