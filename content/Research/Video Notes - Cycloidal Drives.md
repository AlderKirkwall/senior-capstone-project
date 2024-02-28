---
note-type:
  - general
related: 
created: 2024-02-05 21:28
---
# Cycloidal Drive
*Two different videos are referenced/linked in this note*
## Anatomy
- high speed input shaft
- eccentric bearing
- cycloidal disks
- ring gear
- slow speed output shaft
- ([00:59](https://youtu.be/mPwbDrXq50Q#t=59.830501999999996))

> [!info] working principle
> Reduction ratio depends on pins on ring gear
> ~~See previous video for more detailed explaination~~ More on that below.
> - ([01:27](https://youtu.be/mPwbDrXq50Q#t=87.99148103051758))
## Version 2
Used bushings this time round rather than bearings for the rollers
- ([02:03](https://youtu.be/mPwbDrXq50Q#t=123.96395999999999))

### Design
1. Roller radius ($R_{r}$) (dependent on what diameter of bushing/pins/etc you'll be using)
- ([02:18](https://youtu.be/mPwbDrXq50Q#t=138.505611))
2. For your reduction ratio, $i$, you'll set your number of rollers ($N$) to one greater than $i$.
- ([02:31](https://youtu.be/mPwbDrXq50Q#t=151.21360611444092))
3. Ring gear pitch
4. Eccentricity

> [!question] Ring Gear Pitch and Eccentricity
> I'm not clear on these two and what they are and how to get them.
> - ([02:49](https://youtu.be/mPwbDrXq50Q#t=169.959876))
>   
> > [!done] Figured it out!
> > I don't know why he called it ring gear pitch, but referring to his first video, R is simply the radius of the ring gear ($\frac{\text{diameter}}{2}$). 
> > 
> > $E$, eccentricity is a value that should be less than half the roller diameter. In other words:
> > $$
> > E<R_{r} \quad\text{OR}\quad E< \frac{d}{2}\ ,\quad \text{where $d$ is diameter}
> > $$
> > - ([06:09](https://youtu.be/OsS9-FzKN6s#t=369.904929))

^3374ba

[link for bushings](https://www.amazon.com/uxcell-Bearings-Wrapped-Oil-Less-Bushings/dp/B07SHSN6NP?th=1&linkCode=sl1&tag=howto045-20&linkId=980eedbbbb6fb9899012839c6908b66a&language=en_US&ref_=as_li_ss_tl)
[link for dowel pins](https://www.amazon.com/uxcell-Stainless-Cylindrical-Support-Elements/dp/B07Z18CKCY?th=1&linkCode=sl1&tag=howto045-20&linkId=744caad9b5d5f03c4bba6a9f2e918781&language=en_US&ref_=as_li_ss_tl)

## Version 1

### Cycloidal Reduction Formula
$$
\begin{aligned}
&i \text{ - ratio}\\
&n \text{ - number of lobes}\\
&N \text{ - number of rollers}
\end{aligned}
$$
$$
i = \frac{n}{N - n}
$$
- ([02:44](https://youtu.be/OsS9-FzKN6s#t=164.086347))

> [!example] Example
> If I want a reduction of 40:1, then:

$$
\begin{aligned}
40 &= \frac{n}{N - n} \implies 40 = \frac{40}{41 - 40}\\ \\
\therefore\quad n &= 40\\
N &= 41
\end{aligned}
$$

> [!important] Why Two Disks
> Two disks are placed 180 degrees out of phase to balance the forces of the moving disks, especially at high speeds. 
> 
> **Wow.** it's that simple...
> - ([03:07](https://youtu.be/OsS9-FzKN6s#t=187.290613))

### Version 1 Design
Four primary parameters when designing a cycloidal drive:
$$
\begin{aligned}
&R \text{ - ring gear radius}\\
&R_{r} \text{ - roller radius}\\
&N \text{ - number of rollers}\\
&E \text{ - eccentricity}
\end{aligned}
$$
- ([04:09](https://youtu.be/OsS9-FzKN6s#t=249.305675))

#### How to Mechatronic's Approach
1. decide what reduction you want ($i$)
2. Number of Rollers: $N = i + 1$
3. Roller radius $R_{r}$ - depends on what you use for the rollers.
4. Ring gear radius $R$ - up to you
5. Eccentricity, or $E$. See [[Video Notes - Cycloidal Drives#^3374ba|my earlier epiphany]]
- ([05:42](https://youtu.be/OsS9-FzKN6s#t=342.752747))

He uses [[Building-a-Cycloidal-Drive-with-SOLIDWORKS]]
Parametric equations from said document:
```
X = (R*cos(t)) - (R r *cos(t+arctan(sin((1 - N)*t)/((R/EN) - cos((1 - N)*t))))) - (E*cos(N *t))
```

```
Y = ( - R *sin(t))+(R r *sin(t+arctan(sin((1 - N)*t)/((R/EN) - cos((1 - N)*t)))))+(E*sin(N *t))
```
- ([07:18](https://youtu.be/OsS9-FzKN6s#t=438.1678410228882))

All this leads to me needing to decide what the [[Cycloidal Drive Parameters|parameters are for my cycloidal drive]].