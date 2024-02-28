# Motor Torque Calculation

So, torque is equal to power over rotations per minute:
$$
\tau = \frac{P}{RPM}
$$
and power is equal to current times voltage.
$$
P = IV
$$
That means that if we know the max and min currents and voltages of a motor, we should be able to determine a torque range. But torque at what distance?…

I'm thinking that we only need to know the torque at the shaft itself.

I also have the python script I wrote for calculating torque from KV rating, max current, and max voltage


> [!update] Using published torque vs. speed curves
> For now, I'm relying on the published torque vs speed curves for the motors I've chosen
