# AnimationBuilder Actionscript 3 Documentation

## Overview
AnimationBuilder is an Actionscript 3 utility for converting Adobe Animate timeline animations into SVG and CSS animations. It simplifies exporting animations by handling frame conversion, anchor points, CSS generation, and animation management.

---

## Features
- **Frame Conversion**: Converts timeline frames to time-based CSS percentages.
- **Anchor Point Calculation**: Determines anchor points for precise CSS transforms.
- **Animation Storage**: Stores frames, easing, duration, delay, and properties.
- **CSS Export**: Generates `@keyframes` and inline CSS animation properties.
- **Reporting**: Outputs full CSS animations with frame delays.

---

## Installation
Clone the repository and integrate `AnimationBuilder.as` into your Animate project:
```bash
git clone https://github.com/motionharvest/Animation-Builder.git
```

---

## Usage
### Import the Class
```actionscript
import AnimationBuilder;
```

### Initialize
```actionscript
var ab:AnimationBuilder = new AnimationBuilder(stage, targets);
```

### Add Animations Per Frame
```actionscript
ab.add("targetName");
```

### Export CSS Report
```actionscript
ab.report();
```

---

## API Reference
### `AnimationBuilder`
- `constructor(stage:Stage, targets:Object)`: Initializes with the current stage and target objects.
- `add(targetName:String)`: Adds animations for the specified target per frame.
- `report()`: Outputs the final CSS animations report.

---

## License
[MIT License](LICENSE)

---

## Contributing
Pull requests are welcome! For major changes, please open an issue first.

---

## Acknowledgments
Created by [Motion Harvest](https://github.com/motionharvest).

---

[View the Source Code](https://raw.githubusercontent.com/motionharvest/Animation-Builder/refs/heads/master/AnimationBuilder.as)
