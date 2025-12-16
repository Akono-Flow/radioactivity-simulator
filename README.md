# Nuclear Stability Simulator - User Guide

## 📚 Overview

The Nuclear Stability Simulator is an interactive web-based educational tool designed to help students understand radioactive decay and nuclear stability concepts. This application visualizes the Band of Stability and allows users to practice predicting decay modes for different nuclides.

## 🎯 Features

### 1. **Interactive Band of Stability Plot**
- Visual representation of the nuclear stability region
- Reference lines showing N:P ratios (1:1 and 1.5:1)
- Bismuth limit line (Z = 83)
- Color-coded regions for different decay modes
- Click-to-plot functionality

### 2. **Prediction System**
- Plot any nuclide by entering Z (protons) and N (neutrons)
- Random nuclide generator for practice
- Multiple prediction options:
  - Alpha decay (α)
  - Beta minus decay (β⁻)
  - Beta plus decay (β⁺)
  - Electron capture
  - Stable
- Immediate feedback with explanations
- Educational explanations based on nuclear physics principles

### 3. **Comprehensive Statistics Tracking**
- Total attempts and correct predictions
- Accuracy percentage
- Breakdown by decay mode
- Persistent storage (saved in browser)

### 4. **Study Notes**
- Complete reference material on radioactivity
- Definitions and concepts
- Decay mode explanations with examples
- Applications of radioisotopes

### 5. **Customizable Settings**
- Grid display options
- Adjustable point sizes
- Element label display modes
- Color customization for all decay regions
- Animation speed controls
- Settings persistence

### 6. **Dataset Management**
- Upload custom datasets (JSON or CSV)
- Download current dataset
- Reset to default dataset
- Sample datasets provided

## 🚀 Getting Started

### Opening the Application

1. Simply open the `radioactivity-simulator.html` file in any modern web browser
2. No installation or internet connection required (after initial load)
3. Works on desktop, tablet, and mobile devices

### Basic Usage

#### Plotting a Nuclide

**Method 1: Manual Input**
1. Go to the "Simulation" tab
2. Enter the atomic number (Z) - number of protons
3. Enter the neutron number (N)
4. Click "✏️ Plot Nuclide"

**Method 2: Random Generation**
1. Click "🎲 Random Nuclide" to generate a practice problem
2. The nuclide will be automatically plotted

**Method 3: Click on Plot**
1. Click anywhere on the Band of Stability plot
2. The nearest nuclide position will be plotted

#### Making Predictions

1. After plotting a nuclide, review the nuclide information displayed
2. Note the N:P ratio and element details
3. Select your prediction from the five options
4. Get immediate feedback
5. Click "💡 Show Explanation" for detailed reasoning

## 📊 Understanding the Band of Stability

### Key Concepts

**Stable Region (Green):**
- For Z ≤ 20: N:P ratio ≈ 1:1 (equal neutrons and protons)
- For 20 < Z ≤ 83: N:P ratio gradually increases toward 1.5:1
- Nuclides in this region are stable

**Alpha Decay (Red):**
- Occurs for all elements with Z > 83 (beyond Bismuth)
- Nuclide emits an alpha particle (²He⁴)
- Both Z and mass number decrease

**Beta Minus Decay (Blue):**
- Occurs when a nuclide has excess neutrons
- Located to the left of the stability band
- Neutron converts to proton + electron
- Z increases by 1, mass number unchanged

**Beta Plus / Electron Capture (Purple):**
- Occurs when a nuclide has excess protons
- Located to the right of the stability band
- Proton converts to neutron
- Z decreases by 1, mass number unchanged

### Reference Lines

- **Red dashed line:** N:P = 1:1 ratio
- **Green dashed line:** N:P = 1.5:1 ratio
- **Yellow dashed line:** Z = 83 (Bismuth limit)

## 📁 Custom Datasets

### JSON Format

Create a file with the following structure:

```json
[
  {"z": 1, "n": 0},
  {"z": 1, "n": 1},
  {"z": 2, "n": 1},
  ...
]
```

- `z`: Atomic number (number of protons)
- `n`: Neutron number

### CSV Format

Create a file with the following structure:

```csv
z,n
1,0
1,1
2,1
...
```

First row is the header, subsequent rows contain z and n values.

### Uploading Custom Data

1. Go to the "Simulation" tab
2. Scroll to "📁 Data Management"
3. Click "📤 Upload Custom Dataset"
4. Select your JSON or CSV file
5. The plot will update with your custom data

## ⚙️ Settings

### Grid Display
- **Major Grid Lines Only:** Shows grid lines every 10 units
- **Major and Minor Grid Lines:** Shows more detailed grid
- **No Grid Lines:** Clean plot without grid

### Point Size
- Adjust the size of plotted nuclide markers (3-10 pixels)

### Show Element Labels
- **On Hover:** Shows element symbol when hovering near a nuclide
- **Always:** Always displays element symbols
- **Never:** No element labels shown

### Color Customization
- Customize colors for all stability regions
- Changes are reflected immediately in the plot

### Animation Speed
- Control the speed of UI animations
- Options: Slow, Medium, Fast, None

## 📈 Statistics

The Statistics tab tracks your learning progress:

- **Total Attempts:** How many predictions you've made
- **Correct Predictions:** How many you got right
- **Accuracy Rate:** Percentage of correct predictions
- **Decay Mode Breakdown:** Performance by decay type

Statistics are saved in your browser and persist between sessions.

## 💡 Study Tips

1. **Start with Extremes:** Begin by practicing with Z < 20 and Z > 83 where rules are clearer
2. **Focus on Ratios:** Pay close attention to the N:P ratio
3. **Use Random Practice:** Generate random nuclides to test yourself
4. **Read Explanations:** Always read the explanation, even when correct
5. **Track Progress:** Monitor your statistics to identify weak areas
6. **Review Notes:** Refer to the Notes tab when confused

## 🎓 Educational Context

### Aligned with CSEC/CAPE Chemistry

This simulator supports learning objectives for:
- Nuclear chemistry
- Radioactivity and decay modes
- Stability of atomic nuclei
- Applications of radioisotopes

### Key Learning Outcomes

After using this simulator, students should be able to:
- Identify stable vs unstable nuclides
- Predict decay modes based on N:P ratios
- Understand the band of stability concept
- Explain why different decay modes occur
- Apply nuclear stability principles to real isotopes

## 🔧 Technical Requirements

- **Browser:** Modern web browser (Chrome, Firefox, Safari, Edge)
- **JavaScript:** Must be enabled
- **Storage:** Uses localStorage for saving settings and stats
- **Screen:** Best viewed on screens 1024px width or larger
- **Internet:** Required only for initial load (for Google Fonts)

## 📝 Tips for Teachers

### Classroom Use

1. **Demonstration Mode:** Use on projector to explain concepts
2. **Practice Sessions:** Students can work individually or in pairs
3. **Competitions:** Track accuracy for class competitions
4. **Custom Datasets:** Create datasets focused on specific elements
5. **Assessment:** Use random nuclide feature for quick quizzes

### Homework Assignments

- Assign practice sessions with accuracy targets
- Have students explain their reasoning in writing
- Create worksheets that reference specific nuclides
- Ask students to create their own custom datasets

## 🐛 Troubleshooting

**Plot not displaying:**
- Refresh the page
- Check if JavaScript is enabled
- Try a different browser

**Settings not saving:**
- Check if cookies/localStorage are enabled
- Ensure not in private/incognito mode

**Dataset upload fails:**
- Verify file format (JSON or CSV)
- Check for proper structure
- Ensure no special characters in data

**Performance issues:**
- Reduce animation speed in settings
- Close other browser tabs
- Try on a device with better specifications

---

**Version:** 1.0  
**Created for:** Educational use in chemistry instruction  
**Purpose:** Interactive learning tool for CSEC/CAPE Chemistry students

