# Capstone - Decisions to Be Made

## Design Choices
- [x] Motor specs: ✅ 2024-02-15
	- [x] Torque (considering gearbox reduction) ✅ 2024-02-15
	- [x] Power rating ✅ 2024-02-15
	- [x] Voltage ✅ 2024-02-15
	- See [[3D Models and Specifications]]
	- I plan to run at 24V
- [x] Gearbox: ✅ 2024-02-15
	- [x] Gear Ratio ✅ 2024-02-15
	- [x] Kind: ✅ 2024-02-04
		- [x] cycloidal[^2] ✅ 2024-02-04
		- harmonic
		- planetary
		- Planetary Cycloidal Hub[^1]
- [x] Size of arm ✅ 2024-02-15
	- See [[CADboarding Notes]] and [[CADboard Model MKII.JPG]]
- [ ] Aesthetics/design 
- [x] Kind of gripper ✅ 2024-02-15
	- Basic Servo-actuated gripper
- [ ] Vision System (subtasks)
	- [ ] Where to mount
	- [ ] What kind
- [x] Computer ✅ 2024-02-15
	- [x] What kind ✅ 2024-02-15
	- Raspberry Pi 5
- [ ] Colors 
- [x] Materials ✅ 2024-02-15
	- [x] Kinds of filaments ✅ 2024-02-15
		- I plan to use PLA
	- [x] any metal parts? ✅ 2024-02-15
		- Depending on time, I may machine the drives.
- [>] Control:
	- [x] Do I need to use [GRBL](https://github.com/grbl/grbl) ? Would it be beneficial? ✅ 2024-02-15
		- No. GRBL only [supports 3 axes](https://github.com/grbl/grbl/wiki#:~:text=Grbl%20is%20for%20three%20axis%20machines.%20No%20rotation%20axes%20(yet)%20%E2%80%93%20just%20X%2C%20Y%2C%20and%20Z.)

[^1]: See [Michael Rechtin's Video](https://www.youtube.com/watch?v=IKkw4d7jyu0)
[^2]: See [How to Mechatronic's Video: "What is Cycloidal Drive?"](https://youtu.be/OsS9-FzKN6s?si=o5ehW4OT03ypAVRJ)