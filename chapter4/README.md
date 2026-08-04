# Chapter 4: The Lorentz Transformation

## 1. A Problem

In the previous chapters, we discussed the principle of relativity and the principle of the invariance of the speed of light.

The principle of relativity tells us: the laws of physics are the same in all inertial reference frames. No inertial reference frame is special.
The principle of the invariance of the speed of light tells us: the speed of light in a vacuum is the same in all inertial reference frames, constant at: c = 299,792,458 m/s.

These two principles, taken together, give rise to a problem that must be solved:
if different observers are in different states of motion, yet they all measure exactly the same speed of light, then how should the time and space they measure be transformed?

In Newtonian mechanics, this problem is very simple.
Suppose Xiao Ming stands on the ground, and Xiao Hong sits in a spaceship moving at speed v.

Newton held that:
space can be directly added. If Xiao Ming measures the position of an object as s, and Xiao Hong measures the position as s', then:
    s' = s - vt

Time is entirely independent:
    t' = t

This is the Galilean transformation. But the principle of the invariance of the speed of light tells us that this transformation cannot hold.

Because according to the Galilean transformation, velocities should satisfy a simple addition relation.
If the spaceship's speed is v, and the speed of light emitted inside the spaceship is c, then an observer on the ground should measure:
    c' = c + v

That is to say, observers in different states of motion should measure different speeds of light.

But experiment tells us: no. No matter how the light source moves, no matter how the observer moves, the measured speed of light is always c.
Therefore, space and time must be readjusted.

The universe requires a new rule for coordinate transformation.

This rule is precisely the Lorentz transformation.

---

## 2. Light Propagation in Two Reference Frames

To derive the Lorentz transformation, we consider two inertial reference frames.

Definition:
The reference frame where Xiao Ming is located is: the S frame.
The reference frame of Xiao Hong's spaceship is: the S' frame.

Xiao Hong's spaceship moves at speed v in the s-direction relative to Xiao Ming. The two reference frames coincide at a certain instant:
    t = 0

At this time:
    s = 0
    s' = 0

Both simultaneously set their clocks to 0.

Next, consider the same light propagation event, measured separately in the two reference frames.

**Xiao Ming's Measurement**

Xiao Ming considers himself at rest. He turns on a flashlight, and the light propagates in the s-direction. After time t, Xiao Ming measures the light propagation distance as s. From the definition of light speed:
    s = ct

Square both sides and rearrange:
    s² - c²t² = 0

**Xiao Hong's Measurement**

Xiao Hong is in the spaceship. In her own reference frame, she considers herself at rest. She measures the same light propagation process. After time t', she measures the light propagation distance as s'. Due to the invariance of the speed of light:
    s' = ct'

Square both sides and rearrange:
    s'² - c²t'² = 0

The invariance of the speed of light implies a key condition: the same light propagation event, which satisfies the light propagation law s = ct in Xiao Ming's view, must also satisfy s' = ct' in Xiao Hong's view. In other words, the light cone structure must remain invariant across all inertial reference frames.

Therefore, we need to find a coordinate transformation such that the light cone condition s² - c²t² = 0 holds in all reference frames.

Preservation of the light cone requires the spacetime interval to have the same form:

s'² - c²t'² = k(v)(s² - c²t²)

where k(v) is a scale factor that depends on the relative velocity v. The factor k(v) cannot alter the light cone structure, but initially it allows a change in the overall scale. Later, through the existence of the inverse transformation, the symmetry of reference frames, and low-speed continuity, it can be proved that k(v) = 1. Hence the true invariant is s² - c²t². For light propagation events, it equals zero; for ordinary events, it is generally not equal to zero. The task of the Lorentz transformation is to keep this spacetime interval invariant across all inertial reference frames.

---

## 3. How Do the Two Reference Frames Transform?

The question now is:
Given the data measured by Xiao Ming: (s, t)

How does one calculate the data measured by Xiao Hong: (s', t')?

And vice versa. Under the same conventions for spatial direction and units, the only physical parameter distinguishing the two reference frames is the relative velocity v. Thus the transformation relation can only be determined by v.

## Why Must It Be a Linear Relation?

A fundamental requirement of inertial reference frames is: an object moving in uniform rectilinear motion in one inertial frame must also move in uniform rectilinear motion in another inertial frame. If the transformation relation contained nonlinear terms—such as quadratic terms, higher-order terms, or other nonlinear functions—then uniform rectilinear motion, after transformation, would generally no longer preserve its straight-line form, and would instead exhibit a time-dependent velocity. Therefore, under the conditions of inertial frame equivalence, spacetime continuity, and preservation of the origin, the most general continuous coordinate transformation satisfying these requirements is the linear transformation.

Thus we set:
    s' = As + Bt       (1)
    t' = Cs + Dt       (2)

where:
A, B, C, D are four unknown constants. They depend only on the relative velocity v.

---

## 4. Four Conditions to Solve for Four Coefficients

The question now is: how to determine A, B, C, D? Four independent conditions are required.

## First Condition: Motion of the Reference Frame Origins

At the start of the experiment:
    t = 0

Xiao Ming and Xiao Hong's positions coincide. Both set their coordinate origins simultaneously to:
    s = 0
    s' = 0

At this moment, no light has yet been emitted. Subsequently, Xiao Hong moves with the spaceship at speed v.

From Xiao Ming's reference frame, Xiao Hong's coordinate origin moves with the spaceship:
    s = vt

While in Xiao Hong's own reference frame, she is always located at her own coordinate origin:
    s' = 0

Therefore, substituting:
    s' = 0
    s = vt

into equation (1) s' = As + Bt yields:
    0 = A(vt) + Bt

Hence:
    B = -Av

Finally, equation (1) s' = As + Bt becomes:
    s' = As + (-Av)t = A(s - vt)       (3)

---

## Second Condition: Invariance of the Speed of Light

Consider the same beam of light propagating in the s-direction. In Xiao Ming's reference frame:
    s = ct

In Xiao Hong's reference frame:
    s' = ct'

Substituting into equation (3) s' = A(s - vt) yields:
    s' = ct' = A(ct - vt)

Factoring out t:
    ct' = At(c - v)

Hence:
    t' = At(c - v) / c

On the other hand:
    s = ct

Substituting into equation (2) t' = Cs + Dt yields:
    t' = Cct + Dt

Rearranging:
    t' = t(Cc + D)

The two expressions are equal:
    At(c - v) / c = t(Cc + D)

Canceling t:
    A(c - v) / c = Cc + D

Obtaining the second constraint. That is:
    A(1 - v/c) = Cc + D

---

## Third Condition: The Principle of Relativity and Inverse Transformation Symmetry

Now we need to determine the time transformation coefficients. The time transformation contains two unknown quantities, C and D, and requires an additional constraint provided by the principle of relativity.

The core of the principle of relativity is: no inertial reference frame holds a special status; therefore, S → S' and S' → S must be described by the same mathematical structure. Xiao Ming sees Xiao Hong moving at speed v, and Xiao Hong sees Xiao Ming moving at speed -v. Hence, the transformation from S to S' and the inverse transformation from S' to S must have the same structure, differing only in the sign of the velocity. This means the inverse transformation should have the form:

s = A'(s' + vt')

where A' is the spatial coefficient of the inverse transformation. Going from the S frame to the S' frame, and then returning from the S' frame to the S frame, must restore the original coordinates.

From equation (3) s' = A(s - vt), we can obtain:
    s'/A = s - vt
    s = s'/A + vt

Substitute into:
    t' = Cs + Dt

Yielding:
    t' = C(s'/A + vt) + Dt

Expanding:
    t' = Cs'/A + (Cv + D)t

Therefore:
    t = (t' - Cs'/A) / (Cv + D)

Substituting back into:
    s = s'/A + vt

Yielding:
    s = s'/A + v(t' - Cs'/A) / (Cv + D)

Rearranging:
    s = s'[1/A - vC/(A(Cv + D))] + vt'/(Cv + D)

Now consider Xiao Ming's own origin.

In Xiao Ming's reference frame:
    s = 0

In Xiao Hong's reference frame, the origin of Xiao Ming's S frame moves in the negative direction at speed -v.

Therefore:
    s' = -vt'

Substituting into:
    s = s'[1/A - vC/(A(Cv + D))] + vt'/(Cv + D)

Yielding:
    0 = (-vt')[1/A - vC/(A(Cv + D))] + vt'/(Cv + D)

Dividing both sides by vt':
    0 = -[1/A - vC/(A(Cv + D))] + 1/(Cv + D)

Rearranging:
    1/A - vC/(A(Cv + D)) = 1/(Cv + D)

Multiplying both sides by A(Cv + D):
    Cv + D - vC = A

Because:
    Cv = vC

Thus:
    D = A

Obtaining the third condition:
    D = A

---

## Fourth Condition: Isotropy of Space

The principle of relativity requires the forward and inverse transformations to have the same functional structure, i.e., A'(v) = A(-v). Now we need to determine the relation between A(v) and A(-v).

Since space has no special direction, physical laws should not depend on the choice of coordinate axis orientation. If the spatial coordinate direction is reversed, s → -s, then the relative velocity v → -v, but the physical process itself does not change. Therefore, the coefficient describing the spatial transformation can depend only on the magnitude of the velocity, not on its direction:

A(-v) = A(v)

That is, A(v) must be an even function of velocity.

Combining A'(v) = A(-v) with this, we obtain A'(v) = A(v). Therefore, the spatial coefficient in the inverse transformation is the same as the spatial coefficient in the forward transformation.

By isotropy of space, A' = A has been proved. Substituting into the inverse transformation relation:

    1/A - vC/(A(Cv + D)) = A

Multiplying both sides by A:
    1 - vC/(Cv + D) = A²

Using:
    D = A

Yielding:
    1 - vC/(Cv + A) = A²

Rearranging:
    vC/(Cv + A) = 1 - A²

Multiplying both sides by:
    Cv + A

Yielding:

   vC = (1 - A²)(Cv + A)

Expanding:
    vC = (1 - A²)Cv + (1 - A²)A

Rearranging:
    vC - (1 - A²)Cv = (1 - A²)A

Factoring the left side:
    vC[1 - (1 - A²)] = (1 - A²)A

Thus:
    vCA² = (1 - A²)A

Canceling A:
    vCA = 1 - A²

Obtaining:
    C = (1 - A²) / (Av)

This is the fourth condition.

---

## 5. Solving for the Four Coefficients

Now we have:

First condition:
    B = -Av

Second condition:
    A(1 - v/c) = Cc + D

Third condition:
    D = A

Fourth condition:
    C = (1 - A²) / (Av)

Substituting:
    D = A

into the second condition:
    A(1 - v/c) = Cc + A

Subtracting A from both sides:
    -Av/c = Cc

Thus:
    C = -Av/c²

Now:
    C = (1 - A²) / (Av)

and:
    C = -Av/c²

are equal:
    (1 - A²)/(Av) = -Av/c²

Multiplying both sides by Av:
    1 - A² = -A²v²/c²

Rearranging:
    1 = A² - A²v²/c²
 
Factoring:
    1 = A²(1 - v²/c²)
 
Therefore:
    A² = 1 / (1 - v²/c²)
 
Since the direction of velocity remains consistent, taking the positive value:
    A = 1 / √(1 - v²/c²)
 
Define:
    γ = 1 / √(1 - v²/c²)
 
All four coefficients are completely determined:
    A = γ
    B = -γv
    C = -γv/c²
    D = γ

---

## 6. The Lorentz Transformation

Substituting the four coefficients into:
    s' = As + Bt

Yields:
    s' = γ(s - vt)

Time:
    t' = Cs + Dt
   
Yields:
    t' = γ(t - vs/c²)

Finally:
    s' = γ(s - vt)
    t' = γ(t - vs/c²)

where:
    γ = 1 / √(1 - v²/c²)
    This is the Lorentz transformation.

The Lorentz transformation describes:
how spatial coordinates and time coordinates transform between different inertial reference frames.
It is not a set of formulas artificially prescribed, but a result mathematically necessitated by the joint constraints of the invariance of the speed of light and the principle of relativity.

---

### 6.1 Why Must Space and Time Change Together?

Many readers will have a question: why can't space alone change, while time remains unchanged?

Under the assumption that time remains absolute, t' = t, consider only a spatial change: s' = k(s - vt). Then light in Xiao Ming's reference frame, s = ct, when substituted, yields s' = kt(c - v). Xiao Hong measures the speed of light c' = s'/t' = k(c - v). Unless k varies with v, it can never always equal c. Therefore, changing space alone cannot preserve the invariance of the speed of light.

Likewise, if only time changes, t' = kt, while space remains unchanged, s' = s - vt, it is also impossible to maintain s'/t' = c.

Thus, the invariance of the speed of light demands that space and time must adjust together as a unified whole. Changing space alone or changing time alone cannot satisfy the new constraint conditions. The new constraints force the universe to produce a new structure—spacetime. This is why the universe does not possess absolute space and absolute time, but rather a unified spacetime.

---

## 7. The Lorentz Factor γ

The Lorentz factor:
    γ = 1 / √(1 - v²/c²)

It describes the degree of spacetime change under high-speed motion.

When v = 0: γ = 1. The Lorentz transformation reduces to:
    s' = s
    t' = t

This is the situation in classical mechanics. In the everyday low-speed world, we do not perceive relativistic effects, because when v is far smaller than c, γ is almost equal to 1. Classical mechanics is the low-speed approximation of relativity, not a mistake.

As the velocity increases, v → c:
    1 - v²/c² → 0

Therefore: γ → ∞

This shows:

The closer the velocity is to the speed of light, the more pronounced the changes in time and space become.

No object with rest mass can reach the speed of light.

Because accelerating an object with rest mass to the speed of light would require infinite energy.

The speed of light thus becomes the ultimate limit for the motion of information and matter in the universe.

---

## 8. From the Lorentz Transformation to Special Relativity

The Lorentz transformation solves a key problem: why can observers in different states of motion still measure the same speed of light?

The answer is: time and space are not the absolute, unchanging background of Newtonian mechanics. To preserve the invariance of the speed of light, the time and space measured by different observers must undergo corresponding adjustments.

However, the Lorentz transformation itself merely describes the mathematical relationship between different reference frames. It tells us how space transforms and how time transforms. But it has not yet told us: what does this transformation imply? Does time truly slow down? Does space truly contract? What deeper relationships exist among mass, energy, and spacetime?

These questions will be unfolded in the next chapter.

---

## 9. Summary of the Derivation of the Lorentz Transformation

The entire derivation did not presuppose time dilation, nor did it presuppose length contraction. We used only four fundamental conditions:

First, the continuity of inertial motion and the preservation of uniform rectilinear motion; therefore, the continuous coordinate transformation must be linear.

Second, the invariance of the speed of light; therefore, the light cone structure must be preserved.

Third, the principle of relativity; therefore, the forward and inverse transformations must have the same form.

Fourth, the isotropy of space; therefore, the transformation coefficients cannot depend on spatial direction.

Starting from the four unknown coefficients A, B, C, D, through four conditions, we obtained:

A = γ, B = -γv, C = -γv/c², D = γ

Finally arriving at the Lorentz transformation:

s' = γ(s - vt)
t' = γ(t - vs/c²)

The Lorentz transformation is not an artificial design. It is a mathematical structure determined step by step by a logical chain under existing physical conditions.

The first three chapters proposed constraints—conservation laws and symmetries require that the evolution of physical systems be subject to continuous constraints, the invariance of the speed of light provided the requirement of light cone preservation, the principle of relativity provided the requirement of reference frame equivalence, and the isotropy of space provided the requirement of direction independence. Chapter 4, under the joint action of these constraints, derived the spacetime structure that satisfies the conditions. This is precisely the evolutionary process that GULP seeks to express: constraints do not directly give the answer, but they limit the possible forms—when the constraints are strong enough, there is only one answer.

Newtonian space consists of absolute space and absolute time. Experiment revealed the invariance of the speed of light, which conflicted with the Newtonian framework. The universe did not abandon either constraint, but instead accepted both the principle of relativity and the invariance of the speed of light simultaneously. The result of these two constraints acting together is: absolute space and absolute time can no longer exist independently; they are reorganized into a unified spacetime structure.

But constraints can only tell us what form the structure must satisfy; they have not yet answered why the universe possesses these constraints. The Lorentz transformation describes the structure of spacetime, but it does not answer where this structure comes from. The question of evolutionary dynamics still hangs in the distance: what compelled the universe to move from the Galilean transformation to the Lorentz transformation? This inquiry will not stop at Chapter 4; it will extend all the way into deeper physical layers.