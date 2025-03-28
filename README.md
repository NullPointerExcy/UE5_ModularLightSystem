# UE5 Modular Light System

Developed with Unreal Engine 5

> ⚠️ Licensing Note  
This project is released under the MIT License.  
However, redistribution or republishing this package (in whole or parts) on the Unreal Engine Marketplace (Fab) or any other asset store is **not allowed**.  
Please respect the intent of the open source release.

A modular, dynamic, and highly customizable lighting system for Unreal Engine 5, built entirely with Blueprints.  
This system is designed for both gameplay logic and level design, allowing interactive lights, circuit behavior, and visual feedback directly in the editor.

This project is **completely free** and will also be released on the **Unreal Engine Marketplace (FAB)** once finalized.

---

## Features

- **Modular Light Blueprint**: Easily place and configure lights with custom behavior.
- **Parallel & Series Circuits**: Simulate realistic chain reactions (e.g. if a light breaks, the chain is affected).
- **Trigger Volumes**: Use box, sphere or capsule trigger zones to toggle lights.
- **Light Switch Blueprints**: Link light switches to one or more lights or triggers.
- **Destroyable Lights**: Optional damage system for destructible light actors.
- **Sound Integration**: Individual audio slots for:
    - Switch toggling
    - Light activation/deactivation
    - Flicker
    - Destruction
- **Gradient Lighting**: Color blending support with optional flickering interpolation.
- **Custom Settings**: Change light radius, color, type, orientation and more.
- **Smart Interaction**: Lights check if they're interactable before reacting.
- **Visual Debug Lines**: Circuit connections are drawn in the editor for easy overview.
- **Text Labels**: Show how many connections each light has and in which mode (Series/Parallel).

---

## How to Use

1. Add the Interaction Manager to the Level
Drag and drop BP_InteractionManager from
`Content/Levels/LightSwitch/Blueprints/Light/Manager/` into your level.

2. Enhanced Input System Required
Make sure your project uses the Enhanced Input System.
You must have an input action called `IA_Use` (Or you can change it inside the Blueprint).

3. Set the Input Mapping
Open `BP_InteractionManager` and add your input mapping context to the Input Mapping field.
This ensures the interaction key (like `E`, `F`, etc.) works correctly.

4. Use Light Components
You can now use:
 - BP_Light
 - BP_LightSwitchTrigger

Both are located under
`Content/Levels/LightSwitch/Blueprints/Light/Components/`

> ⚠️ A full documentation will be created later.
Feel free to explore and try it out already, it's designed to be modular and intuitive!

---

## Planned Features

- [ ] Save/Load system for light states
- [ ] Energy-based gameplay integration (power limiters, voltage drop, etc.)
- [ ] Light presets (e.g. flickering neon, broken halogen, sci-fi light pulses)
- [ ] Merged Editor UI / Widget for circuit overview (Currently uses debug lines and text labels, and lines are kinda broken in UE)
- [ ] Custom material support for emissive light meshes
- [ ] ... if you have suggestions, feel free to contribute or contact me
- [ ] FAB Marketplace release

---

## Requirements

- Unreal Engine 5.5+
- Blueprint-only project (no C++ required)
- Tested in UE 5.5.4 and should work out of the box

---

## Project Status

This project is actively developed. The core system is fully functional and stable.  
Contributions, feedback and suggestions are welcome!

---

## License

This project is licensed under the MIT License, see the [LICENSE](./LICENSE) file for details.

**Note:** You are **not permitted** to upload this content to the Unreal Marketplace (Fab) or any other commercial asset store without explicit permission from the author.

---

## Support

If you like this project, feel free to share it.  
Once the FAB release is live, links will be added here.
