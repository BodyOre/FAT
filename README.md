# Body Ore — Fitness Assessment Toolkit (FAT)

An interconnected collection of free fitness and nutrition calculators built for **Body Ore**.

FAT is designed to help users understand key body-composition and nutrition metrics, see how those metrics relate to one another, and take the next step toward personalised training and nutrition coaching.

## Calculators

* **BMI** — Body Mass Index
* **WHtR** — Waist-to-Height Ratio
* **Body-Fat Estimate** — circumference-based estimate using the U.S. Navy method
* **Calorie Needs** — BMR, TDEE and goal-based calorie targets
* **Protein** — daily protein target based on body weight and goal
* **Goal Weight / Time** — estimated goal weight based on body-fat target and estimated lean mass
* **Macros** — protein, carbohydrate and fat targets based on linked calorie and protein results

## Interconnected by Design

FAT uses a shared assessment state so users enter their core information once and the calculators reuse it.

Typical flow:

**Body measurements → Body composition → Calories & protein → Goal → Macros → Coaching**

For example:

* BMI uses height and weight.
* WHtR uses waist and height.
* Body-fat estimation uses sex, height, waist, neck and, where required, hip.
* Calorie needs use age, sex, height, weight, activity and goal.
* Protein uses body weight and goal.
* Goal weight uses current weight, estimated body fat and target body fat.
* Macros use the linked calorie and protein targets.

## Units

Height and weight use metric units.

Circumference measurements support:

* centimetres (cm)
* inches (in)

The selected circumference unit is used consistently throughout the toolkit, with conversion handled internally for calculations where required.

## Coaching Integration

The toolkit is also designed as a **Body Ore coaching funnel** rather than just a collection of standalone calculators.

Results include relevant next steps and a **Start Your Program** CTA.

The coaching email is pre-addressed to:

`HeyCoach@proton.me`

with the subject:

`Coaching Enquiry — Body Ore`

Assessment results can be included in the pre-filled email so the trainer receives useful context along with the user's enquiry.

## Design

The toolkit follows the visual language used across Body Ore:

* **Fraunces** — display headings
* **Inter** — interface/body text
* **IBM Plex Mono** — numerical results
* Warm stone/off-white surfaces
* Emerald accent
* Strong borders and restrained editorial styling
* Responsive layouts for desktop and mobile

## Technical Stack

The current implementation is a lightweight static web application using:

* HTML
* CSS
* Vanilla JavaScript
* Tailwind CSS via CDN

No backend or database is required for the calculator functionality.

## Disclaimer

The calculations provided by FAT are intended for **general fitness and educational purposes**.

They are estimates and should not be treated as medical diagnoses or a substitute for professional medical assessment.

Body composition estimates are particularly sensitive to measurement technique and should be interpreted accordingly.

## Body Ore

FAT is part of the **Body Ore** fitness and sports-nutrition ecosystem.

Website: [https://bodyore.github.io/BodyOre/](https://bodyore.github.io/BodyOre/)
