[[How Stepper Motors Work - Electric motor|Omnivore How Stepper Motors Work - Electric motor]]

```timestamp-url 
 https://www.youtube.com/watch?v=09Mpkjcr0bo
 ```

*Steppers - Basic Types and how they work*

```timestamp 
 01:34
 ```
offer *precision* control

```timestamp 
 02:35
 ```
typical step count is 200

## Types
```timestamp 
 03:15
 ```
- Hybrid
	- most commonly used
	- uneven number of teeth
```timestamp 
 07:27
 ```
- Permanent magnet 
	- dimetrically polarized rotor
```timestamp 
 08:21
 ```
- Variable Reluctance
	- ferromagnetic rotor (rather than a perm. magnet)
```timestamp 
 09:33
 ```
- Hybrid
	- combination of variable reluctance and perm. magnet steppers
	- the offset in the teeth of the rotor's poles causes an attraction and repulsion when a coil pair is activated.
		- this also results in high precision and torque. A sort of magnetic alignment

## Control methods
```timestamp 
 11:53
 ```
- Wave drive
	- simplest
	- one phase activated at a time
	- low torque, not smooth, large steps
- Full Step
	- Two phases are activated at once
	- higher torque averaged alignment
- Half Step
	- 1 then 2 then 1, repeat. (phase activations)
	- slightly less torque
- Microstep
	- As one phase activates, the previous is deactivating. Sine wave profile with offset phases.