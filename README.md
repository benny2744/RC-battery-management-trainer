# LiPo Battery Charging Trainer

A comprehensive web-based interactive flashcard application for learning safe RC battery charging practices. This trainer teaches users to correctly configure charging parameters for different battery types through visual feedback and safety validation.

## Features

### 🔋 Battery Types Supported
- **LiPo (Lithium Polymer)**: Standard RC batteries with 4.20V max voltage per cell
- **HV LiPo (High Voltage)**: High-voltage LiPo batteries with 4.35V max voltage per cell  
- **Li-ion**: Lithium-ion batteries with 4.10V max voltage per cell

### 📊 Five Progressive Difficulty Levels

1. **Level 1 - Single LiPo**: Basic training with single LiPo batteries (1-8S, 300-1800mAh)
2. **Level 2 - LiPo & HV LiPo**: Introduces high-voltage LiPo batteries alongside standard LiPo
3. **Level 3 - All Battery Types**: Mix of LiPo, HV LiPo, and Li-ion batteries
4. **Level 4 - Balance Charging**: Multiple batteries (1-4) of the same type for balance charging scenarios
5. **Level 5 - Advanced Parallel**: Complex configurations including Li-ion parallel cells (1P-4P) with multiple batteries

### ⚡ Realistic Charger Interface

- **Auto Cell Detection**: Automatically displays detected cell count (S rating)
- **Voltage Control**: Adjustable max voltage per cell (3.00-4.50V, 0.1V increments)
- **Current Control**: Adjustable charging current (0.0-50.0A, 0.1A increments)
- **Direct Input**: Both button controls and direct number input supported
- **Real-time Validation**: Color-coded field feedback (green=good, orange=acceptable, red=dangerous)

### 🛡️ Advanced Safety Features

#### Optional Safety Checks
- **Minimum Voltage Testing**: Toggleable field for testing knowledge of safe discharge limits
- **Storage Voltage Testing**: Toggleable field for long-term storage voltage knowledge

#### C-Rating Safety Classifications
- **LiPo/HV LiPo**: 1C=Safe, 1-2C=Fast/Low Risk, 2-3C=Risky, >3C=Dangerous
- **Li-ion**: 0.5C=Safe, 0.5-1C=Fast/Low Risk, >1C=Dangerous

#### Voltage Validation
- Automatic validation against correct voltage per battery type
- Multi-tier feedback system with specific error messages
- Prevents overcharging and undercharging scenarios

### 🎨 Visual Battery Representation

#### LiPo Batteries
- **Isometric stacked rectangles** representing individual cells
- **Variable width** based on capacity (larger capacity = wider cells)
- **Color coding**: Standard LiPo (red gradient), HV LiPo (orange gradient)

#### Li-ion Batteries  
- **Cylindrical cell visualization** representing 18650-style cells
- **Parallel configuration support** showing multiple columns for P-ratings
- **Realistic styling** with positive terminal indicators

#### Multiple Battery Display
- **Visual multipliers** showing battery count with circular indicators
- **Plus symbols** connecting batteries in balance charging scenarios
- **Responsive scaling** for different screen sizes

### 🌐 Bilingual Support
- **English** and **Chinese (中文)** language options
- **Complete translation** of all interface elements and safety messages
- **Culturally appropriate** safety terminology and warnings

### 📱 Responsive Design
- **Mobile-optimized** layout with touch-friendly controls
- **Tablet support** with adaptive grid layouts
- **Desktop experience** with full feature set
- **Automatic layout switching** based on screen size

## Technical Implementation

### Battery Configuration Logic
- **Randomized generation** based on difficulty level
- **Realistic capacity ranges** matching real-world RC batteries
- **Proper C-rating calculations** for parallel and balance charging scenarios
- **Accurate voltage specifications** for each battery chemistry

### Safety Validation System
- **Multi-parameter validation** checking voltage, current, and optional parameters
- **Context-aware feedback** with specific recommendations
- **Progressive difficulty** building from basic to advanced concepts
- **Real-time field validation** with immediate visual feedback

### User Interface Features
- **Flashcard-style layout** with question/answer sections
- **Interactive controls** with smooth animations
- **Color-coded feedback** system for immediate understanding
- **Skip functionality** for exploring different battery configurations

## Usage

1. **Select Difficulty**: Choose from 5 progressive levels based on your experience
2. **Enable Optional Features**: Toggle minimum voltage or storage voltage testing as needed
3. **Choose Language**: Select English or Chinese interface
4. **Configure Parameters**: Adjust voltage and current settings using buttons or direct input
5. **Get Feedback**: Real-time field validation shows safety levels
6. **Check Answer**: Submit for comprehensive safety analysis
7. **Learn & Progress**: Skip to new questions or advance difficulty levels

## Educational Value

This trainer provides comprehensive education on:
- **Battery chemistry differences** and their charging requirements
- **C-rating calculations** for safe charging speeds
- **Parallel and balance charging** concepts
- **Voltage management** for battery longevity and safety
- **Real-world scenarios** encountered in RC hobby applications

Perfect for RC hobbyists, drone pilots, and anyone working with rechargeable battery systems who needs to understand safe charging practices.

## File Structure

```
/
├── index.html          # Complete single-page application
└── README.md          # This documentation file
```