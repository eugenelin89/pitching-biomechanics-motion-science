# PBMS — Pitching Biomechanics & Motion Science
## A 24-Month Independent Study Program

**Version:** 1.0 (22 October 2026)  
**Format:** Self-directed, evidence-based curriculum; 12 modules in four semesters  
**Suggested pace:** 8–12 hours/week for 24 months (approximately 830–1,250 hours)  
**Intended audience:** Curious pitchers, coaches, students, engineers, researchers, and developers who want to understand *how pitching movement is measured and studied*.  
**Status:** Independent curriculum—not a UBC or Stanford degree, not university-approved, not a coaching/medical credential.

> **Program motto:** Measure carefully. Model honestly. Interpret evidence with humility.

**This file is the complete learning guide.** Start with [the first 30 days](#7-your-first-30-days), follow [the four-semester plan](#6-the-24-month-curriculum), and preserve your work in a private study portfolio. You may publish your own non-identifying notes and analysis code once licensing and consent are checked.

---

## Table of contents

1. [Purpose, outcomes, and boundaries](#1-purpose-outcomes-and-boundaries)
2. [How this curriculum was reverse-engineered](#2-how-this-curriculum-was-reverse-engineered)
3. [University course crosswalk: UBC and Stanford](#3-university-course-crosswalk-ubc-and-stanford)
4. [Books, free courses, and software](#4-books-free-courses-and-software)
5. [How to study and demonstrate mastery](#5-how-to-study-and-demonstrate-mastery)
6. [The 24-month curriculum](#6-the-24-month-curriculum)
7. [Your first 30 days](#7-your-first-30-days)
8. [Month-by-month roadmap](#8-month-by-month-roadmap)
9. [Baseball biomechanics research seminar](#9-baseball-biomechanics-research-seminar)
10. [Laboratory protocols, data quality, and ethics](#10-laboratory-protocols-data-quality-and-ethics)
11. [Capstone project guide](#11-capstone-project-guide)
12. [Assessment rubrics and graduation checklist](#12-assessment-rubrics-and-graduation-checklist)
13. [Weekly timetable and pace adjustments](#13-weekly-timetable-and-pace-adjustments)
14. [Career and mentorship pathway](#14-career-and-mentorship-pathway)
15. [References and official sources](#15-references-and-official-sources)
16. [Glossary](#16-glossary)

---

## 1. Purpose, outcomes, and boundaries

### The goal

Become technically capable of reading pitching-biomechanics research, analyzing movement data, designing repeatable experiments, judging measurement accuracy, and communicating defensible conclusions to researchers and coaches.

The target is **competence in quantitative pitching biomechanics and longitudinal movement analysis**, not a collection of coaching slogans. An eventual professional expert typically builds on this foundation with supervised lab experience, graduate-level work and/or many years of applied research.

### What you should be able to do at graduation

1. Identify major bones, joints, muscles and anatomical reference planes relevant to throwing.
2. Explain movement using position, velocity, acceleration, force, torque, momentum and energy.
3. Distinguish **kinematics** (motion) from **kinetics** (forces and moments).
4. Analyze pitching phases and report precisely defined biomechanical variables.
5. Separate 2D projected video measurements from true 3D anatomical measurements.
6. Build reproducible Python analyses from appropriately licensed datasets.
7. Explain camera calibration, filtering, landmark uncertainty and their effects.
8. Perform basic statistical tests, regression, reliability and agreement analyses.
9. Explain what inverse kinematics, inverse dynamics and musculoskeletal simulation require.
10. Formulate and complete a small, ethical, reproducible pitching study.
11. Critique papers and avoid interpreting correlation as causation.
12. Communicate findings and limitations to coaches without prescribing medical care.

### Important scientific boundaries

- A 2D elbow angle from a single video is **not automatically** an anatomically accurate 3D elbow joint angle.
- Shoulder or elbow **joint position** cannot directly reveal actual ligament force, tissue strain or individual injury risk.
- Net joint moments from inverse dynamics are **not equivalent** to individual muscle or ligament forces.
- A pattern correlated with pitch velocity is not automatically a change that will improve every athlete.
- Without an appropriate validated reference, make **relative, projected, repeatability** claims—not absolute anatomical or injury-prevention claims.
- Avoid diagnosing injuries or suggesting that a delivery is medically safe/unsafe. Work with qualified medical professionals for health decisions.

### Minimum prerequisites

- Algebra, trigonometry, unit conversions, graphs, spreadsheets.
- High-school physics helps. If calculus is new, start the MIT calculus course alongside PB 102.
- Python basics help, but are taught in PB 301.
- You do **not** need a biomechanics laboratory to begin.

**Optional four-week preparation:** Review algebra, right-triangle trigonometry, unit vectors, graph slopes and Python/Jupyter basics before Semester 1. This preparatory period is separate from the 24-month schedule if needed.

---

## 2. How this curriculum was reverse-engineered

### University pathway A: UBC Bachelor of Kinesiology

The University of British Columbia (Vancouver) offers a **Bachelor of Kinesiology, Neuromechanical and Physiological Sciences** option. Its published BKin degree requirements include a **120-credit degree**, a first- and second-year kinesiology core, and upper-level selections. The relevant path builds human anatomy, physiology, motor learning, research methods, statistics, biomechanics, programming and laboratory investigation.

- [UBC BKin degree requirements](https://vancouver.calendar.ubc.ca/faculties-colleges-and-schools/school-kinesiology/bachelor-kinesiology/degree-requirements)
- [UBC Neuromechanical and Physiological Sciences option](https://vancouver.calendar.ubc.ca/faculties-colleges-and-schools/school-kinesiology/bachelor-kinesiology/neuromechanical-and-physiological-sciences)
- [UBC official KIN course descriptions](https://vancouver.calendar.ubc.ca/course-descriptions/subject/kinv)

The actual BKin lower-level core includes KIN 110, 120, 131, 132, 150, 160, 205, 206, 211, 216, 232, 235 and 262, as well as degree writing and elective requirements. **Not every core course is needed for this narrowly focused independent program.** In the Neuromechanical and Physiological Sciences option, students select seven courses (21 credits) from an approved upper-level menu, then complete other upper-level/elective requirements.

### University pathway B: Stanford biomechanical engineering

Stanford's 2026–27 **BS in Engineering, Biomechanical Engineering subplan** combines biology and engineering mechanics. Stanford's Mechanical Engineering graduate program also provides a **Biomechanical Engineering depth area**. The independent program draws especially on motion analysis, multi-body mechanics, tissues and movement modelling.

- [Stanford undergraduate Biomechanical Engineering major](https://ughb.stanford.edu/majors-minors/biomechanical-engineering-major-program)
- [Stanford graduate Mechanical Engineering degree requirements](https://bulletin.stanford.edu/programs/ME-MS)
- [Stanford biomechanical engineering course list](https://me.stanford.edu/groups/biomechanical-engineering-program/biomechanical-engineering-courses)

**Interpretation:** UBC supplies the biological and human-movement foundation; Stanford supplies advanced engineering and computational depth. Neither offers a formal "pitching biomechanics" major. The pitching specialization in this file is independently designed and added on top.

### Source-integrity rule

A university's *official course title and catalog description* are not a complete syllabus. The expanded topic lists and assignments below are **PBMS learning objectives**, not claims that each university teaches every item in precisely that way. Where a specific prior course outline is available, it is linked separately. Course offerings, faculty and required texts can change.

---

## 3. University course crosswalk: UBC and Stanford

### 3.1 UBC foundations: actual courses, selected topics, PBMS mapping

| UBC course | University subject area and expanded topics to learn | PBMS |
|---|---|---|
| **KIN 110 — Human Anatomy** | Bones and landmarks; skeletal, muscular and neural systems; shoulder complex; humerus, elbow/forearm; spine, pelvis, hip and lower limb; anatomical planes and directional terminology | PB 101 |
| **KIN 131 — Neural and Musculoskeletal Physiology** | Skeletal and muscular systems, motor units, contraction, neural/neuro-hormonal control, integrative physiology | PB 103 |
| **KIN 132 — Visceral Anatomy and Physiology** | Cardiovascular, respiratory, urinary, digestive and immune systems; useful supporting context, but not a priority for narrow pitching mechanics study | Optional background |
| **KIN 205 — Research Methods in Kinesiology** | Study questions, evaluation of research methods, confounding, study types, validity, reliability, ethics and scientific writing | PB 203, 403 |
| **KIN 206 — Introduction to Statistics in Kinesiology** | Descriptive and inferential statistics, probability, statistical assumptions, tests, regression and distribution-free methods | PB 203, 402 |
| **KIN 211 — Human Motor Behaviour I** | How movement skills are learned and controlled; feedback, practice, motor variability and skill acquisition | PB 202 |
| **KIN 216 — Biomechanics I** | Quantitative motion analysis; linear/angular kinematics and kinetics; Newton's laws; moments; free-body diagrams; energy; muscle forces | PB 102, 201 |
| **KIN 235 — Exercise Physiology I** | Physiological responses to exercise, fatigue, metabolic and muscular adaptation | PB 103, 401 |

### 3.2 UBC advanced selection: actual course options, selected topics

| UBC course | Relevant self-study topics | PBMS |
|---|---|---|
| **KIN 310 — Human Functional Musculoskeletal Anatomy** | Muscle attachments, joint function, innervation, surface anatomy, applied shoulder, trunk and leg motion | PB 101, 202 |
| **KIN 311 — Sensorimotor Control of Human Movement** | Sensory/perceptual input, voluntary movement, proprioception, feedback, cognitive and motor control | PB 202 |
| **KIN 313 — Neuromuscular Integration of Human Movement** | Central and peripheral sensorimotor systems; posture, coordination and balance control | PB 202 |
| **KIN 316 — Biomechanical Properties of Tissues** | Muscle force–length/force–velocity; moment arms; muscle-tendon units; stress, strain, hysteresis; EMG; bones/ligaments | PB 202, 303 |
| **KIN 318 — Programming and Data Science for Kinesiology** | Python data types, data loading/cleaning, algorithms, plotting, exploratory analysis | PB 301 |
| **KIN 324 — Prevention of Athletic Injuries** | Injury-related literature, exposure, prevention principles, limits of risk prediction | PB 401 (critical reading) |
| **KIN 345 — Foundations of Coaching** | Conditioning, program planning, training psychology, athlete evaluation; an additional option, **not** part of the specific seven-course neuromechanical selection | Applied seminar |
| **KIN 418 — Computational Modelling of Human Sensori-Motor Control and Learning** | Bayesian reasoning, learning algorithms, simulation and Python models | PB 303, 403 |
| **KIN 419 — Laboratory Investigations in Neuromechanical Kinesiology** | Experimental studies in biomechanics, motor behaviour and neurophysiology; protocol design, signals and instrumentation | PB 302, 403 |
| **KIN 479 — Scientific Communication and Research Skills in Neuromechanical Kinesiology** | Scientific communication, computation, presenting experimental results; optional advanced reference, not a required course for every BKin student | PB 403 |

For the most biomechanics-focused *seven-course* illustration, a student could investigate KIN **310, 311, 313, 316, 318, 418, 419**, subject to UBC requirements, eligibility and scheduling. PBMS studies a **selection of topics** from these courses without implying university credit.

### 3.3 Real UBC course outlines and specified reading

- **[KIN 216: Biomechanics I, 2024W Term 2](https://educ-kin2016.sites.olt.ubc.ca/files/2025/01/KIN-216-2024W-T2-Outline.pdf).** Published topics include linear/angular movement, kinematics vs kinetics, quantitative problems and mechanics of human motion. A [2023 KIN 216 outline](https://educ-kin2016.sites.olt.ubc.ca/files/2023/09/KIN216-2023W.pdf) lists *Basic Biomechanics*, 9th ed., by Susan J. Hall.
- **[KIN 316: Biomechanical Properties of Tissues, 2024W Term 2](https://educ-kin2016.sites.olt.ubc.ca/files/2025/01/KIN-316-2024W-T2-Outline.pdf).** Actual referenced readings include Whiting & Zernicke, *Biomechanics of Musculoskeletal Injury*, Ch. 3; Lieber, *Skeletal Muscle Structure, Function & Plasticity*, 2002 ed., Ch. 2–3; and McGill, *Low Back Disorders*, Ch. 4–5. Lecture modules include muscle structure, EMG, force–length, force–velocity, joint geometry and wearable tracking. Check legal access to assigned excerpts instead of reproducing them here.
- **[KIN 206: Introduction to Statistics in Kinesiology, 2024W Term 2](https://educ-kin2016.sites.olt.ubc.ca/files/2025/01/KIN-206-2024W-T2-Outline.pdf).** Required text listed: Howard T. Tokunaga, *Fundamental Statistics for the Social and Behavioral Sciences*, 2nd ed. Includes statistical assumptions, research literacy and JASP analysis.

These linked outlines are **historical reference examples**; they are not guarantees of what a future instructor will assign.

### 3.4 Stanford engineering courses: actual university courses

| Stanford course | Course theme; PBMS topic selection | PBMS |
|---|---|---|
| **ENGR 14 — Intro to Solid Mechanics** | 2D/3D equilibrium, external loads, structures, stress and deformation | PB 102, 201 |
| **ENGR 15 — Dynamics** | Newtonian motion, rigid-body dynamics, free-body diagrams, equations of motion | PB 201 |
| **ME 80 — Mechanics of Materials** | Stress, strain, bending, torsion, material response | PB 202 |
| **ME 70 — Introductory Fluids Engineering** | Fluid mechanics, conservation, forces in fluids; lower priority for body mechanics, useful for ball-flight interest | Optional |
| **ME 102/103 — Product Realization** | CAD, engineering design, prototyping, fabrication and testing | Optional instrumentation |
| **ME 281 / BIOE 281 — Biomechanics of Movement** | Motion capture, EMG, force plates, imaging, muscle-tendon mechanics, musculoskeletal geometry | PB 302, 303 |
| **ME 283 — Introduction to Biomechanics and Mechanobiology** | Tissue viscoelasticity, bone and muscle mechanics, mechanical adaptation | PB 202 |
| **ME 287 — Soft Tissue Mechanics** | Nonlinear elasticity, viscoelasticity, poroelasticity, properties of soft tissues | PB 202, 303 |
| **ME 381 — Orthopaedic Bioengineering** | Musculoskeletal anatomy and mechanics; orthopaedic applications | PB 202, 401 |
| **ME 485 / BIOE 485 — Modeling and Simulation of Human Movement** | Joint and muscle-tendon models, forward dynamics, control, collision/contact, medical-image-based geometry | PB 303 |

Stanford courses are presented as **inspiration and relevant possible selections**, not as one official mandatory sequence. See the official program links above. Graduate-level syllabi may have substantial prerequisites and course availability may change.

### 3.5 What was deliberately left out

Full UBC/Stanford degrees also include breadth, writing, general education, broader health sciences, design and other requirements. PBMS omits much of that to maximize relevance to biomechanical analysis. The tradeoff is significant: PBMS is **not** academically or professionally equivalent to completing those university programs.

---

## 4. Books, free courses, and software

### 4.1 Core reading library (purchase/borrow only what you need)

| ID | Resource | Read these parts for PBMS | Cost / notes |
|---|---|---|---|
| **R1** | [OpenStax, *Anatomy & Physiology 2e*](https://openstax.org/books/anatomy-and-physiology-2e/pages/preface) | Ch. 6 bone; 7 axial skeleton; 8 appendicular skeleton; 9 joints; 10 muscle tissue; 11 muscular system; Ch. 12–14 nervous system | **Free**, first choice for anatomy |
| **R2** | [Donald Neumann, *Kinesiology of the Musculoskeletal System*, 4th ed.](https://shop.elsevier.com/books/neumann-s-kinesiology-of-the-musculoskeletal-system/neumann/978-0-323-71859-2) | Ch. 2 joints; 3 muscle; 4 biomechanics; **5 shoulder; 6 elbow/forearm; 9–10 axial skeleton; 12 hip; 13 knee; 14 ankle/foot** | Paid/borrowed; useful detailed anatomy reference |
| **R3** | Susan J. Hall, *Basic Biomechanics*, 9th ed. | Linear/angular motion, forces, moments, energy, free-body diagrams, human movement | Paid/borrowed; named by UBC KIN 216 2023 outline |
| **R4** | [Thomas K. Uchida & Scott L. Delp, *Biomechanics of Movement*](https://biomech.stanford.edu/) | Muscle structure/mechanics, rigid-body mechanics, musculoskeletal geometry, measurement, modelling and simulation; use chapter topics rather than edition-dependent chapter numbers | Paid book; **free companion lectures, assignments, models and data** |
| **R5** | Richard L. Lieber, *Skeletal Muscle Structure, Function & Plasticity* | Muscle architecture, contraction, force–length, force–velocity, adaptation; UBC KIN 316 2002 ed. specifies Ch. 2–3 extracts | Specialist reference; optional unless available |
| **R6** | W. C. Whiting & R. F. Zernicke, *Biomechanics of Musculoskeletal Injury* | Stress/strain, tissue loading, injury biomechanics; UBC KIN 316 historical outline cites Ch. 3 of 1998 ed. | Specialist reference |
| **R7** | Howard T. Tokunaga, *Fundamental Statistics for the Social and Behavioral Sciences*, 2nd ed. | Descriptive and inferential statistics, assumptions, testing | Listed in UBC KIN 206 2025 outline |
| **R8** | Research methods textbook such as *Research Methods in Kinesiology* by Kowalski and colleagues | Study designs, reliability, validity, ethics, scientific reporting | **Suggested**, not claimed here to be a current required book |
| **R9** | Stuart McGill, *Low Back Disorders* | Selected tissue/loading and trunk-function concepts; UBC KIN 316 historical outline cites Ch. 4–5 of 2008 ed. | Optional specialist reference |

**Suggested purchase order:** start free with R1; borrow R2 and R3; obtain R4 when studying advanced modelling; add R5–R9 only when needed. Do not buy all nine at once. Chapter numbers refer to editions named here; confirm against the edition you can actually access.

### 4.2 Free courses and study sequence

| Resource | Use for | When |
|---|---|---|
| [MIT 18.01SC — Single Variable Calculus](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/) | Derivatives, integrals, changing rates, optimization | PB 102 |
| [MIT 18.02SC — Multivariable Calculus](https://ocw.mit.edu/courses/18-02sc-multivariable-calculus-fall-2010/) | Vectors, 3D space, gradients, partial derivatives | PB 102 → 201 |
| [MIT 18.06SC — Linear Algebra](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/) | Matrices, rotations, coordinate transforms, least squares | PB 201 → 302 |
| [MIT 8.01SC — Classical Mechanics](https://ocw.mit.edu/courses/8-01sc-classical-mechanics-fall-2016/) | Forces, energy, torque, angular momentum | PB 102 |
| [MIT 2.003SC — Engineering Dynamics](https://ocw.mit.edu/courses/2-003sc-engineering-dynamics-fall-2011/) | Rigid-body dynamics, equations of motion, momentum and energy | PB 201 |
| [Biomechanics of Movement companion resources](https://biomech.stanford.edu/) | Homework, lectures, simulation models and examples | PB 201–303 |
| [OpenSim](https://opensim.stanford.edu/) | Musculoskeletal modelling, inverse kinematics/dynamics and tutorials | PB 303 |
| [OpenCV](https://opencv.org/get-started/) | Frames, camera calibration and computer vision | PB 301–302 |
| [Python NumPy](https://numpy.org/doc/stable/), [pandas](https://pandas.pydata.org/docs/), [SciPy](https://docs.scipy.org/doc/scipy/), [Matplotlib](https://matplotlib.org/stable/), [statsmodels](https://www.statsmodels.org/stable/) | Scientific analysis, signals, statistics and visualization | PB 203, 301–403 |

*Learning goal:* complete selected relevant lessons and exercises; you do not need to finish every entire MIT course when a prerequisite is already mastered.

### 4.3 Software setup

Install Python 3.11+ (or another version supported by your scientific tools), a virtual environment, JupyterLab, NumPy, pandas, SciPy, Matplotlib and statsmodels. Add OpenCV when you begin video analysis. Add OpenSim only when you reach PB 303 and have checked its current compatibility requirements.

Keep two separate work areas:

- **Study notes and publicly shareable code:** references, explanations, synthetic examples, and code you authored.
- **Private athlete data:** recordings, consent records, identifiers, and raw/derived measurements tied to real people.

**Do not put identifiable video, health information, minors' recordings, consent forms, personal contact details or restricted third-party datasets into a public repository.**

---

## 5. How to study and demonstrate mastery

### The five-step learning loop (every week)

1. **Read/learn:** 2–3 focused lessons from an assigned section.
2. **Derive:** hand-calculate one relationship or write a diagram with correctly labeled units.
3. **Implement:** reproduce an example with real or synthetic numerical data.
4. **Apply:** explain how the idea changes the interpretation of a pitch.
5. **Critique:** write down assumptions, error sources and conclusions you cannot justify.

### Portfolio folder layout (recommended, locally)

Use a private working directory such as:

```text
pbms-study/
  learning-log.md
  reading-notes/
  assignments/
  labs/
  notebooks/
  protocols/
  research-critiques/
  reports/
  private-athlete-data/    # never publish
```

Maintain a `learning-log.md` entry each week: *hours completed, lessons, one solved problem, one observation, one uncertainty, and next week's action*. Maintain a bibliography of each research paper's DOI or stable URL.

### Passing a module

A module is complete only after you have:

- Read or worked through its core concepts.
- Completed every listed hands-on deliverable.
- Explained the terms and assumptions without consulting notes.
- Earned at least **80/100** on its self-evaluation rubric.
- Revised the work after at least one round of error-checking or external feedback when available.

A perfect-looking graph with an invalid measurement definition **does not pass**. Scientific honesty matters more than appearance.

---

## 6. The 24-month curriculum

**Structure:** 12 modules, three running in parallel during each six-month semester. Each semester also includes short research-paper critiques. The suggested hour counts are **estimates for independent study**, not official university credit hours.

### SEMESTER 1 — Foundations of human movement (Months 1–6)

#### PB 101 — Functional Anatomy of Pitching (approximately 60–75 hours)

**Inspired by:** UBC KIN 110 and KIN 310.  
**Prerequisites:** None.  
**Primary readings:** R1 Ch. 6–11; R2 Ch. 2–3, 5–6, 9–10, 12–14.

**Topic units**
1. Anatomical planes and axes: sagittal, frontal, transverse; flexion/extension, abduction/adduction, internal/external rotation; distinguish global direction from local joint motion.
2. The skeleton: clavicle, scapula, humerus, radius, ulna, vertebrae, pelvis, femur, tibia; bony landmarks used in measurement.
3. Shoulder complex: glenohumeral joint, scapulothoracic motion, rotator cuff, scapular stabilizers; why the shoulder is not a simple ball-and-socket in practice.
4. Elbow and forearm: flexion/extension, pronation/supination, bony structures, ligament anatomy at a **descriptive** level.
5. Trunk and pelvis: axial rotation, lateral flexion, spinal and hip mechanics; pelvic orientation versus thoracic orientation.
6. Lower limb: hip extension/rotation, knee flexion/extension, ankle motion, support and balance during stride and lead-leg action.

**Assignments:** (A) A labeled full-body anatomical diagram; (B) a 30-term flash-card deck; (C) annotated still frames at stride start, lead-foot contact and release; (D) two pages explaining the kinetic chain in anatomical language without injury claims.

**Exit test:** Identify 20 landmarks/motions and explain five joint/segment actions correctly; distinguish trunk rotation from shoulder internal rotation.

#### PB 102 — Physics and Mathematics of Human Motion (approximately 75–95 hours)

**Inspired by:** UBC KIN 216, Stanford ENGR 14, MIT mechanics/calculus.  
**Prerequisites:** Algebra and trigonometry.  
**Readings:** R3 linear/angular mechanics; MIT 8.01SC and selected 18.01SC/18.02SC.

**Topic units**
1. Quantities, units and vectors: distance, displacement, scalars vs vectors, radians vs degrees, unit conversion and coordinate choices.
2. Kinematics: position–time, average and instantaneous velocity/acceleration, derivatives, numerical finite differences, sample rate.
3. Dynamics: Newton's three laws, free-body diagrams, reaction forces, mass, force and acceleration.
4. Rotational motion: angular position, velocity, acceleration, moment arms, torque; radians/sec and degrees/sec.
5. Momentum and energy: linear/angular momentum, impulse, work, kinetic energy, power; what "energy transfer" does and does not imply.
6. Applied pitching problems: toy forearm model, bat/ball flight distinction, controlled frame-timing calculations, dimensional checks.

**Assignments:** At least 25 solved numerical problems with units; plot angular position and computed angular velocity of a synthetic signal; explain why differentiation amplifies noise.

**Exit test:** Derive and calculate velocity from sampled angle data; solve a basic torque/moment-arm exercise; identify three ways the simplified mechanical model differs from a real human arm.

#### PB 103 — Muscle and Neuromuscular Physiology (approximately 50–70 hours)

**Inspired by:** UBC KIN 131 and KIN 235.  
**Readings:** R1 Ch. 10, 12–14, selected 17; R5 selected muscle-function concepts.

**Topic units**
1. Muscle fibre, fascicle, myofibril, sarcomere, actin/myosin and contraction.
2. Motor units, neural control, excitation–contraction coupling and recruitment.
3. Concentric/eccentric/isometric muscle action; tendon elasticity.
4. Force–length and force–velocity principles; simplified limitations.
5. Proprioception, sensory feedback, motor planning and coordinated movement.
6. Fatigue, recovery and adaptation as research concepts—not individualized training or medical prescriptions.

**Assignments:** Explain a force–velocity graph; annotate possible eccentric/concentric phases of a **simplified model**, explaining why video alone cannot prove individual muscle activation; build a concept map from neural command to joint motion.

**Exit test:** Explain the difference among neural drive, EMG activity, muscle force and measured body-segment motion.

**Semester 1 synthesis:** A 5–8 page illustrated analysis of a pitch explaining anatomy and basic mechanics; include a clearly labeled model and at least five limitations.

### SEMESTER 2 — Dynamics, control and scientific inference (Months 7–12)

#### PB 201 — Rigid-Body and Multisegment Dynamics (approximately 65–85 hours)

**Inspired by:** Stanford ENGR 15; MIT 2.003SC; Stanford ME 281 foundations.  
**Prerequisites:** PB 102.  
**Readings:** MIT dynamics; R3; R4 selected mechanics chapters.

**Topic units**
1. Matrix/vector basics and coordinate frames; local versus global reference.
2. 2D rigid-body translation and rotation; segment centres of mass.
3. Joint constraints, connected segment models and simplified anthropometry.
4. Moment of inertia, angular momentum, Newton–Euler equations.
5. Forward versus inverse dynamics; external load and inertial measurement requirements.
6. Numerical solutions, error propagation, model simplification and assumption checks.

**Assignments:** Two-link arm model with diagrams and code; calculate sample segment accelerations and net moments for a **fully specified toy problem**; show how an altered length or mass assumption changes the estimated results.

**Exit test:** State precisely which measured inputs are needed for inverse dynamics and why a lone smartphone video is insufficient for validated internal joint-force claims.

#### PB 202 — Motor Control and Tissue Mechanics (approximately 65–85 hours)

**Inspired by:** UBC KIN 211/311/313/316; Stanford ME 80/283/287/381.  
**Prerequisites:** PB 101, PB 103, PB 102.  
**Readings:** R2 Ch. 2–4; R5–R6 selected; UBC KIN 316 reference outline.

**Topic units**
1. Coordination, skill acquisition, practice, variability and feedback.
2. Proprioception, feedforward control, feedback delays and sensory integration.
3. Tissue stress/strain, elastic modulus, stiffness, loading and deformation.
4. Muscle-tendon force–length and force–velocity relations and moment arms.
5. Viscoelasticity, hysteresis, time-dependence and fatigue-related mechanisms.
6. EMG fundamentals; what surface EMG can and cannot reveal; tissue-adaptation evidence and uncertainty.

**Assignments:** Draw a conceptual force–length relationship and stress–strain curve; identify untestable assumptions when applying these concepts to a video; critically read one tissue-mechanics paper.

**Exit test:** Differentiate joint angle, joint moment, tendon load and ligament force; explain why none is interchangeable with the others.

#### PB 203 — Research Design and Statistics (approximately 65–85 hours)

**Inspired by:** UBC KIN 205 and 206.  
**Prerequisites:** Algebra; basic spreadsheets.  
**Readings:** R7 and R8; UBC KIN 206 outline; free stats software documentation.

**Topic units**
1. Research questions, hypotheses, observational studies, repeated-measures experiments and confounding.
2. Sampling, selection bias, measurement validity, reliability and data dictionaries.
3. Distributions, means, medians, standard deviation, percentiles, visualization.
4. Probability, confidence intervals, effect sizes and statistical tests; assumptions.
5. Correlation, regression, within-athlete versus between-athlete associations; regression diagnostics.
6. Missing data, multiple comparisons, uncertainty, reproducibility and transparent reporting.

**Assignments:** Analyze a synthetic dataset; produce a reproducible notebook showing descriptive statistics, scatterplots, regression and confidence intervals; critique a causal claim based only on correlation.

**Exit test:** Explain why 50 pitches from one pitcher are not 50 independent athletes; select an appropriate analysis that respects repeated measures.

**Semester 2 synthesis:** Prepare a research protocol, a data dictionary and a 6–10 page analysis of a small consented/synthetic pitching dataset. No anatomical validity claims without a reference measurement.

### SEMESTER 3 — Scientific computing, instrumentation and simulation (Months 13–18)

#### PB 301 — Scientific Programming and Motion Data (approximately 65–85 hours)

**Inspired by:** UBC KIN 318.  
**Prerequisites:** PB 203; basic Python.  
**Tools:** Python, Jupyter, NumPy, pandas, SciPy, Matplotlib, statsmodels.

**Topic units**
1. Reproducible environments, project structure, version control and unit tests.
2. CSV/Parquet loading, identifiers, dictionaries, missing data and data provenance.
3. Timestamps, sampling rates, frame indices, synchronization and event labeling.
4. Smoothing, low-pass filtering, differentiation and edge effects; justify filter choices.
5. Time normalization, repeated trials, within-athlete trends, grouped analyses.
6. Regression, confidence intervals, graphical diagnostics, exported reports and reproducible notebooks.

**Assignments:** Recreate one published or provided computation from suitable example data; build a test suite for angle/unit conversions; build a plotting pipeline and automatically generate a methods/limitations report.

**Exit test:** A clean repository/notebook where an independent reviewer can reproduce a result from permitted input data and understand all transformations.

#### PB 302 — Biomechanics Laboratory and Motion Capture (approximately 75–100 hours)

**Inspired by:** UBC KIN 419 and Stanford ME 281.  
**Prerequisites:** PB 101, 102, 203, 301; basic linear algebra.  
**Tools:** Phone/high-speed camera, tripod, calibration target, OpenCV; more advanced instruments optional.

**Topic units**
1. Sampling, shutter speed, temporal resolution, motion blur and event uncertainty.
2. Image projection, perspective, camera intrinsics/extrinsics, lens distortion.
3. Camera placement, parallax, scaling, calibration and repeatable filming protocol.
4. Human landmark annotation, occlusion, pose-tracker error, anatomical landmarks vs pixels.
5. Multi-camera synchronization, triangulation, 3D coordinate frames; requirements for anatomical reference definitions.
6. Overview of markers, markerless motion capture, force plates, IMUs, EMG and their strengths/limitations.

**Assignments:** Calibrate a camera with OpenCV; record a non-sensitive **controlled object/joint demonstration** from two viewpoints; compare projected angle estimates; repeat 3 times; document timing and position error. Real athlete filming is optional and subject to the ethics rules below.

**Exit test:** Produce a measurement error budget and explain the conditions under which a 2D image angle can and cannot approximate a 3D anatomical measure.

#### PB 303 — Computational Musculoskeletal Modelling (approximately 65–90 hours)

**Inspired by:** Stanford ME 281/485 and UBC KIN 418.  
**Prerequisites:** PB 201–202, 301–302; calculus/linear algebra.  
**Resources:** R4 companion models, OpenSim documentation and tutorials.

**Topic units**
1. Segment models, joints, coordinates and generalized degrees of freedom.
2. Forward kinematics versus inverse kinematics; markers and marker fitting.
3. Inverse dynamics, external forces, anthropometric assumptions and uncertainty.
4. Muscle-tendon geometry, moment arms, activation dynamics and force estimates.
5. Optimization, muscle redundancy, forward simulation and controllers.
6. Model validation, sensitivity analyses, solver failures and reporting assumptions.

**Assignments:** Complete an official OpenSim introductory tutorial; inspect an appropriate sample model; vary one stated parameter and report its effects; write a technical note explaining why a generic example model does **not** validate pitching biomechanics.

**Exit test:** Explain every required input and output of an OpenSim workflow at a conceptual level and label which values are observations, assumptions and model estimates.

**Semester 3 synthesis:** Build a reproducible, carefully scoped motion-analysis pipeline and technical report. Validate repeatability before making accuracy claims.

### SEMESTER 4 — Pitching specialization, validation and original research (Months 19–24)

#### PB 401 — Advanced Baseball Pitching Biomechanics (approximately 70–90 hours)

**Inspired by:** Peer-reviewed baseball research; applied kinesiology and graduate movement biomechanics.  
**Prerequisites:** PB 101–303 core concepts.  
**Readings:** Primary baseball papers from `9 and newly found literature.

**Topic units**
1. Define pitching phases consistently: initiation/windup, stride, arm cocking, acceleration, deceleration and follow-through; avoid assuming every delivery fits rigid phase labels.
2. Event identification: lead-foot contact, maximum shoulder external rotation, release and task-specific timing; report annotation uncertainty.
3. Pelvis, trunk, shoulder and elbow motions; coordinate conventions and joint-angle pitfalls.
4. Lead-leg action, stride, whole-body sequencing, timing and mechanical variability.
5. Performance associations: within-pitcher versus between-pitcher data, ball velocity, pitch selection, individual adaptation.
6. Injury-related research: workload, fatigue, tissue loading and observational study limits; no single-metric injury prediction.

**Assignments:** Analyze 10 carefully selected papers; construct a concept map comparing competing findings; identify which metrics a camera-based system could reasonably measure and which would need 3D capture or force data.

**Exit test:** Explain five pitching findings with source citations, study design, limitations and at least one plausible alternative interpretation for each.

#### PB 402 — Measurement Reliability and Validation (approximately 70–90 hours)

**Inspired by:** UBC research/statistics plus measurement-science literature.  
**Prerequisites:** PB 203, 301, 302.

**Topic units**
1. Construct validity, criterion validity, repeatability and reproducibility.
2. Within-rater and between-rater variation; test/retest design, blinded duplicate scoring.
3. Systematic bias, MAE, RMSE, ICC and when coefficients may mislead.
4. Bland–Altman plots, limits of agreement and comparison against independently measured references.
5. Camera position, sampling, motion blur, annotation and algorithm sensitivity.
6. Predefined acceptance criteria, failure-case analysis and reporting uncertainty.

**Assignments:** Build a dataset with repeated annotations and controlled camera offsets; estimate within-rater and between-rater errors; produce a validation report that distinguishes **agreement** from **correlation**. Do not invent universal "good enough" accuracy thresholds; justify them for each intended use.

**Exit test:** Given a high correlation but large measurement bias, correctly conclude that agreement has not been demonstrated.

#### PB 403 — Independent Capstone Research (approximately 90–120 hours)

**Inspired by:** UBC KIN 419/479 and research-intensive Stanford biomechanical engineering.  
**Prerequisites:** All prior modules; ethics and data governance checklist.

**Topic units**
1. Define a narrow, answerable scientific question.
2. Review literature and draft hypotheses, variables and outcome definitions.
3. Create protocol, consent plan where necessary, data dictionary and preregistered analysis plan when appropriate.
4. Collect/obtain permitted data; conduct quality assurance and document exclusions.
5. Analyze, visualize, quantify uncertainty, test robustness and report negative results.
6. Write, revise and present a reproducible scientific report.

**Required deliverables:** protocol, bibliography, analysis plan, permitted anonymized or synthetic dataset description, reproducible notebook/code, validation/limitations section, 10–20 page paper or equivalent technical report, 10-minute oral presentation.

**Exit test:** Independent critique by a suitably experienced mentor/reviewer where available. If no mentor is available, publish only after a conservative self-audit using the rubric in `12.

---

## 7. Your first 30 days

A concrete four-week start matters more than purchasing equipment. Suggested schedule: **9 hours/week**.

### Week 1 — Vocabulary and pitching phases
- [ ] Read OpenStax Ch. 6 overview and Ch. 9 (joints).
- [ ] Read [The Clinician's Guide to Baseball Pitching Biomechanics](https://pmc.ncbi.nlm.nih.gov/articles/PMC9950989/).
- [ ] Create a glossary of 20 terms (e.g., anatomical vs camera reference plane, flexion, rotation, torque).
- [ ] Sketch a pitch as 5–6 major phases; note that phase boundaries require operational definitions.
- [ ] Write a one-page paper summary: research question, methods, claims and caveats.

### Week 2 — Anatomy of the throwing arm
- [ ] Study OpenStax Ch. 8, 10 and 11 (select the shoulder/elbow muscle sections).
- [ ] Read or borrow Neumann Ch. 5–6 if available.
- [ ] Draw the scapula, shoulder and elbow with landmarks.
- [ ] Annotate 3–5 **permitted** still images of pitching.
- [ ] Write down three anatomical conclusions that cannot be made from a single side-view image.

### Week 3 — Kinematics and torque
- [ ] Study selected MIT 8.01SC lessons and Hall/R3 topics on vectors, angular motion, force and torque.
- [ ] Solve five kinematics problems and five force/torque problems with units.
- [ ] Calculate angular velocity from a **synthetic** angle/time table, first by hand and then in a spreadsheet or Python.
- [ ] Show how reducing frame rate changes event-timing resolution.

### Week 4 — Experimental thinking
- [ ] Read [Oyama et al.'s 2D video reliability/validity paper](https://pubmed.ncbi.nlm.nih.gov/27705057/).
- [ ] Define five candidate pitching measurements operationally (landmarks, plane, units, event, sample rate).
- [ ] Conduct a repeated annotation exercise on permitted video or a synthetic stick-figure sequence.
- [ ] Produce a 2–3 page "Baseline PBMS Report": what you measured, what varied, what you still do not know.
- [ ] Set up your private study folder and schedule next month's sessions.

**First-month success criterion:** Explain why a repeatable pixel-based angle is not necessarily a valid anatomical joint angle; demonstrate one complete calculation with units and assumptions.

---

## 8. Month-by-month roadmap

Three modules proceed in parallel each semester. Use the final week of each month for a review, progress report and corrections.

| Month | Focus | Tangible output |
|---|---|---|
| **1** | Anatomical terminology, pitching phases, basic vectors | Glossary + baseline report |
| **2** | Shoulder/elbow anatomy; movement derivatives | Anatomical diagrams + calculation set |
| **3** | Trunk, pelvis, hips and lead leg; Newton's laws | Annotated kinetic-chain report |
| **4** | Muscle contraction, motor units, force–length | Muscle mechanics concept map |
| **5** | Angular momentum, work/energy, fatigue basics | Toy arm model + 25 solved problems |
| **6** | Review, evaluate errors, Semester 1 report | 5–8 page synthesis + self-test |
| **7** | Coordinate frames, matrix/vector review | Coordinate transformation notebook |
| **8** | Linked segments and rigid-body dynamics | Two-link dynamic model |
| **9** | Motor learning, feedback and variability | Variability critique |
| **10** | Stress/strain, muscle-tendon and tissue mechanics | Tissue mechanics note |
| **11** | Research design, probability, statistical tests | Reproducible stats notebook |
| **12** | Repeated measures, validity and sampling | Research protocol + Semester 2 report |
| **13** | Python scientific environment, clean data | Reproducible repository/notebook |
| **14** | Frame time, filtering, event detection | Time-series pipeline |
| **15** | Camera geometry and calibration | Calibration report |
| **16** | Pose annotation, occlusion, camera offsets | Two-view sensitivity study |
| **17** | OpenSim, inverse kinematics/dynamics concepts | Tutorial report |
| **18** | Model uncertainty and project hardening | Pipeline + Semester 3 technical report |
| **19** | Pitch phases, sequencing and evidence | Structured literature matrix |
| **20** | Velocity relationships, within-athlete studies | Research critique series |
| **21** | Repeated annotation, agreement statistics | Reliability validation report |
| **22** | Capstone design and ethical data collection | Approved/appropriate study protocol |
| **23** | Analyze data, test robustness | Results notebook + draft paper |
| **24** | Revise, peer critique, present | Final capstone portfolio |

If you fall behind, **protect conceptual accuracy**. Move the entire timeline rather than skipping validation or pretending to master a prerequisite.

---

## 9. Baseball biomechanics research seminar

Study approximately **40–60 papers across the full program**: normally one substantial paper every 1–2 weeks, with more focused baseball-specific reading during Semester 4. The first three papers are compulsory:

1. **Diffendaffer et al. (2023).** [The Clinician's Guide to Baseball Pitching Biomechanics](https://pmc.ncbi.nlm.nih.gov/articles/PMC9950989/) — phases, kinematics, kinetics, evidence-informed clinical interpretation. DOI: [10.1177/19417381221078537](https://doi.org/10.1177/19417381221078537).
2. **Oyama et al. (2017).** [Reliability and Validity of Quantitative Video Analysis of Baseball Pitching Motion](https://pubmed.ncbi.nlm.nih.gov/27705057/) — 2D reliability versus 3D anatomical validity. DOI: [10.1123/jab.2016-0011](https://doi.org/10.1123/jab.2016-0011).
3. **Uhlrich et al. (2023).** [OpenCap: Human Movement Dynamics from Smartphone Videos](https://pmc.ncbi.nlm.nih.gov/articles/PMC10586693/) — multi-camera markerless methods and musculoskeletal dynamics. **Do not assume published accuracy for walking/jumping carries over to high-speed pitching.**

### Research-reading themes

- **Weeks/months 1–6:** Anatomy, kinetic-chain descriptions, kinematics versus kinetics.
- **7–12:** Motion-control variability, repeated measures, muscle/tendon modelling.
- **13–18:** Camera calibration, pose estimation, marker-based and markerless tracking, signal processing.
- **19–24:** Pitching phases and sequencing; trunk/pelvis timing; shoulder/elbow kinetics; performance and ball velocity; fatigue and workload; youth/adult differences; validation.

### Paper critique template (one page per paper)

- **Citation/DOI and year:**
- **Research question/hypothesis:**
- **Participants:** age, level, sample size and sampling method.
- **Measurements/instruments:** marker-based? phone video? force plates? sampling rate?
- **What was directly observed vs model-estimated?**
- **Statistical design:** cross-sectional, repeated measures, controlled experiment?
- **Key results:** actual quantities/effect sizes, not merely "significant."
- **Validity, reliability and confounding:**
- **Alternative explanations:**
- **What can a coach/researcher safely infer?**
- **What cannot be concluded?**
- **One replication or follow-up question:**

### Public dataset option: OpenBiomechanics

[Driveline's OpenBiomechanics Project](https://github.com/drivelineresearch/openbiomechanics) provides a pitching module with **411 fastball trials from 100 athletes** in its documented snapshot, along with data dictionaries and analysis examples. Most pitching participants are collegiate-level; the sample is not representative of all youth pitchers.

**Important licensing restriction:** Its software has an MIT code license, while its datasets and biomechanics documentation use **CC BY-NC-SA 4.0 with an additional professional-organization/financial-analysis exclusion**. Do not use the dataset or derivative data in commercial product research, development, training, benchmarking or validation without suitable permission/licensing. This public syllabus merely **links** to the resource; it does not redistribute the dataset or confer usage rights. Before any use, read [LICENSE-DATA.md](https://github.com/drivelineresearch/openbiomechanics/blob/main/LICENSE-DATA.md), [LICENSE-CODE.md](https://github.com/drivelineresearch/openbiomechanics/blob/main/LICENSE-CODE.md) and [DATASHEET.md](https://github.com/drivelineresearch/openbiomechanics/blob/main/DATASHEET.md).

**Permitted educational practice tasks, subject to the actual license:** reproduce a supplied example; inspect the data dictionary; plot distributions; analyze ball-speed associations; compare per-trial summary metrics with time series where available; report sampling limitations. If the license does not permit your situation, use synthetic data or a dataset with appropriate rights instead.

---

## 10. Laboratory protocols, data quality, and ethics

### Lab 1 — Simple angular measurement (Semester 1)

**Question:** Can a projected angle be consistently measured on a clearly defined synthetic/two-link target?

1. Create or find a permitted diagram with defined joint landmarks.
2. Specify the measured points and angle convention.
3. Record angle in degrees, label camera plane, log measurement steps.
4. Repeat annotation 3–5 times with a delay, blinded to earlier values if possible.
5. Report average, range and standard deviation; explain what the measurement actually represents.

### Lab 2 — Camera-position sensitivity (Semester 3)

**Question:** How sensitive is a projected motion angle to camera orientation?

1. Use a non-sensitive moving model or a consenting adult participant.
2. Fix the target's controlled motion and record tripod location, lens and settings.
3. Capture from a standardized reference view, then introduce **measured** deviations in azimuth/elevation/distance.
4. Keep consistent timestamps, lighting and landmark definitions.
5. Analyze angle differences as a function of viewpoint; show plots, raw samples and uncertainty.
6. State whether you validated repeatability, viewpoint sensitivity or **true anatomical accuracy**; do not conflate them.

### Lab 3 — Frame rate and signal-processing sensitivity (Semester 3)

**Question:** How do sampling and filtering choices alter peak angular velocity or event timing?

1. Use synthetic known ground-truth motion first.
2. Downsample to various frame rates and add known noise.
3. Compare numerical derivatives with and without justified filtering.
4. Inspect edge effects and missed extrema.
5. Report errors and describe why results may differ for real pitching footage.

### Lab 4 — Reliability and agreement (Semester 4)

1. Write a protocol **before seeing the final outcomes**.
2. Define 3–5 measurements, landmarks, events, acceptable source footage and exclusions.
3. Have at least two rounds of blinded annotations; add a second independent rater if possible.
4. Quantify within-rater and between-rater error and appropriate confidence intervals.
5. For accuracy claims, compare with an *independent and fit-for-purpose* reference measurement. Show bias, Bland–Altman limits of agreement, MAE/RMSE as applicable—not correlation alone.
6. Report sample selection, failures, sensitivity, and uncertainty. **Do not assign a universal acceptable error threshold without defending its intended application.**

### Example measurement dictionary

| Field | Definition to record | Common pitfall |
|---|---|---|
| `athlete_code` | Consented pseudonymous ID; mapping retained privately | A pseudonym does not guarantee anonymity |
| `trial_id` | Unique session/trial identifier | Duplicate pitch records |
| `session_date` | Coarse/private session date when needed | Public re-identification risk |
| `handedness` | Recorded throwing hand | Mirroring coordinates incorrectly |
| `camera_view` | Side/back/oblique plus actual position and settings | "Side view" not geometrically standardized |
| `frame_rate_fps` | Acquisition rate, not simply exported video FPS | Incorrect time estimates |
| `event_frame` | Number and operational definition | Disagreement on lead-foot contact/release |
| `angle_2d_deg` | Defined three-point or segment-relative **projected** angle | Mislabeling as anatomical 3D rotation |
| `rater_id` | Anonymous observer ID | Missing rater-variance analysis |
| `quality_flag` | Occluded, blurred, off-plane, uncertain | Silently excluding difficult trials |
| `ball_velocity` | Instrument, units, calibration and time | Unknown velocity precision |
| `data_rights` | Consent/license/allowed use | Publishing unlicensed footage or data |

### Human subjects and athlete privacy

- Prefer synthetic or non-identifying examples for initial exercises.
- Use appropriate consent before recording/analysing others; for minors, follow relevant parent/guardian and institutional requirements. **Consent to analysis does not automatically mean consent to public publication.**
- Limit collected personal information; secure private recordings and records; define retention/deletion rules; do not disclose athlete identities or performance/health data without permission.
- Formal human-subject research (especially intended for publication) may require an institution's research-ethics review. Do not substitute this self-study guide for that process.
- Do not expose anyone to additional pitching volume, altered mechanics or physical risk merely to make the experiment more interesting.
- Injury, discomfort or rehabilitation questions should be handled with qualified healthcare professionals.

---

## 11. Capstone project guide

### Recommended title

**Reliability and Viewpoint Sensitivity of Selected Two-Dimensional Pitching Measurements in Standardized Video**

This deliberately modest question is more defensible than claiming accurate 3D elbow torque or individualized injury prediction from ordinary 2D video.

### Example hypotheses

- **H1:** Repeated annotations of selected 2D metrics show measurable within-rater variation.
- **H2:** Camera viewpoint differences cause systematic changes in some projected angles.
- **Exploratory:** Metrics and events differ in measurement stability; report which ones and how much.

### Minimal capstone method

1. **Literature review:** at least 12 directly relevant papers and a clearly articulated gap.
2. **Protocol:** define camera locations, recording settings, target/athlete inclusion, event definitions and quality-control steps.
3. **Data:** if consented athlete data cannot be obtained appropriately, use a controlled mechanical model or permitted synthetic data; explicitly state the resulting generalizability limit.
4. **Repeated measurements:** duplicate annotations, rerating, and optional second rater.
5. **Statistics:** variability, bias, appropriate uncertainty, optional repeated-measures models; avoid pseudo-replication.
6. **Sensitivity:** vary camera positions and/or detection settings by known amounts.
7. **Robustness:** examine outliers, alternate filtering choices, failures and missingness.
8. **Communication:** distinguish evidence supported by your data from hypotheses needing independent 3D validation.

### Final submission contents

- `research-question.md` — one clear question, hypotheses, estimands and scope.
- `protocol.md` — collection, events, operational definitions, privacy and quality.
- `data-dictionary.md` — variables, units, equipment, processing and provenance.
- `analysis.ipynb` or equivalent — reproducible calculations.
- `figures/` — captions with units, uncertainty and sample sizes.
- `report.md` or PDF — abstract, intro, methods, results, discussion, limitations, references.
- `limitations.md` — what is *not* validated and why.
- `review-log.md` — reviewer criticism, changes and unresolved items.

Only publish those components for which you own all necessary rights and for which personal information is removed with appropriate authorization.

### Optional Asymmetri Motion application

If you also develop a pitching-analysis product, treat the capstone as **independent measurement-science education**. Useful research questions include reproducibility, longitudinal stability and camera-placement sensitivity. Do not equate a feature's consistent trendline with anatomical validity or clinical utility. Do not transfer OpenBiomechanics' noncommercially licensed data into a commercial app pipeline without proper rights.

---

## 12. Assessment rubrics and graduation checklist

### Module grading rubric (100 points)

| Component | Points | Evidence |
|---|---:|---|
| Conceptual accuracy | 25 | Correct definitions, anatomy, physical relationships and assumptions |
| Quantitative reasoning | 20 | Equations, units, numerical checks, uncertainty |
| Reproducibility | 20 | Traceable data, readable method, code/tests where appropriate |
| Research literacy | 15 | Source quality, comparison of evidence and identification of limitations |
| Deliverables and communication | 10 | Required artifacts, readable reports, figures and citations |
| Ethics and scientific restraint | 10 | Consent, licensing, no unsupported claims or cherry-picking |
| **Total** | **100** | **80+ to pass**, and no unresolved serious ethics/data-validity failure |

Use the same rubric for each PB course with emphasis shifted to the relevant skills. When self-grading, retain a written explanation of any deductions.

### Semester examinations

- **Semester 1:** Oral anatomy quiz, 25 mechanical problems, annotated pitch, written limitations.
- **Semester 2:** Multi-segment model, research protocol, statistical notebook, repeated-measures explanation.
- **Semester 3:** Camera error study, validated processing pipeline, OpenSim exercise with model limitations.
- **Semester 4:** Reliability report, critically reviewed bibliography, capstone and presentation.

### Graduation evidence

- [ ] Twelve module deliverables with grades and corrections.
- [ ] All four semester synthesis reports.
- [ ] 40–60 structured paper critiques, with direct citations and evolving understanding.
- [ ] Reproducible analysis code and synthetic/permitted example data.
- [ ] A documented camera/measurement error-budget experiment.
- [ ] Clear explanation of 2D versus 3D measurement and of kinematics versus kinetics.
- [ ] One ethics- and licensing-conscious capstone.
- [ ] At least one critical external review **if feasible**; otherwise a clearly stated self-review limitation.
- [ ] No unsupported claims that PBMS grants a degree, medical qualification or research certification.

**Practical definition of success:** Another technically literate person can reproduce your analyses and understand exactly what your conclusions do and do not establish.

---

## 13. Weekly timetable and pace adjustments

### Baseline: nine hours per week

| Activity | Hours/week |
|---|---:|
| Textbook reading and lectures | 2 |
| Math and worked problems | 2 |
| Coding/data analysis | 2 |
| Video/lab/measurement exercises | 2 |
| Scientific paper critique | 1 |
| **Total** | **9** |

**Typical week:** Two reading sessions, two problem-solving/coding sessions, one practical lab, and one research-paper critique. End with a brief learning log.

### Alternative pacing

- **6 hours/week:** Prioritize essentials and extend the timeline—do not assume the 24-month completion date still holds.
- **8–12 hours/week:** Target 24 months, approximately **832–1,248** hours over 104 weeks.
- **15 hours/week:** More room for advanced engineering and extensive paper replication, but do not substitute hours for supervised lab experience.

The program is a **selective** and integrated pathway. It is not equivalent to 12 complete semester-length accredited courses taught at university contact-hour intensity.

### Quarterly review questions

1. Which claims can I now justify with data?
2. Which measurements remain unvalidated?
3. Which mistakes did I find and correct?
4. What was the most informative failed experiment?
5. What must I learn before the next module?
6. Has a researcher/coach reviewed any of my assumptions?

---

## 14. Career and mentorship pathway

### Possible academic routes

- **UBC:** BKin with neuromechanics/physiology selection, complemented by mathematics, programming, engineering and faculty-supervised research opportunities.
- **Stanford or comparable institution:** Mechanical engineering, biomechanical engineering, bioengineering, applied mathematics or related undergraduate study; advanced movement biomechanics at MS/PhD level.
- **Research-intensive path:** Bachelor's foundations → research assistantship/lab training → master's/PhD or equivalent substantial research experience → ongoing peer review and collaboration.

### Three complementary mentors to seek

1. **Biomechanics researcher:** validated kinematics, kinetics, statistics and motion capture.
2. **Experienced pitching coach:** ecological and practical interpretation of performance measurements.
3. **Qualified sports medicine professional:** tissue/injury interpretation within proper medical scope.

A mentor can identify instrument limitations, flawed assumptions and inappropriate claims much faster than reading more papers alone. The [International Society of Biomechanics in Sports](https://isbs.org/) is one possible route to academic communities and conferences.

### What this program does and does not promise

After two disciplined years, you may be ready to contribute to supervised quantitative pitching research and build more scientifically credible analytical tools. **It does not make you automatically equivalent to an experienced lab director, clinician or PhD biomechanist.** That requires considerably more real research, instrumentation experience and independent scrutiny.

---

## 15. References and official sources

### University program records
1. [UBC BKin degree requirements](https://vancouver.calendar.ubc.ca/faculties-colleges-and-schools/school-kinesiology/bachelor-kinesiology/degree-requirements).
2. [UBC Neuromechanical and Physiological Sciences option](https://vancouver.calendar.ubc.ca/faculties-colleges-and-schools/school-kinesiology/bachelor-kinesiology/neuromechanical-and-physiological-sciences).
3. [UBC KIN course descriptions](https://vancouver.calendar.ubc.ca/course-descriptions/subject/kinv).
4. [UBC KIN 216 outline, 2024W Term 2](https://educ-kin2016.sites.olt.ubc.ca/files/2025/01/KIN-216-2024W-T2-Outline.pdf).
5. [UBC KIN 316 outline, 2024W Term 2](https://educ-kin2016.sites.olt.ubc.ca/files/2025/01/KIN-316-2024W-T2-Outline.pdf).
6. [UBC KIN 206 outline, 2024W Term 2](https://educ-kin2016.sites.olt.ubc.ca/files/2025/01/KIN-206-2024W-T2-Outline.pdf).
7. [Stanford BS Biomechanical Engineering, 2026–27](https://ughb.stanford.edu/majors-minors/biomechanical-engineering-major-program).
8. [Stanford Mechanical Engineering MS degree rules](https://bulletin.stanford.edu/programs/ME-MS).
9. [Stanford biomechanics courses](https://me.stanford.edu/groups/biomechanical-engineering-program/biomechanical-engineering-courses).

### Textbooks and open instructional materials
10. [OpenStax Anatomy & Physiology 2e](https://openstax.org/books/anatomy-and-physiology-2e/pages/preface).
11. [Neumann, 4th edition—publisher and contents](https://shop.elsevier.com/books/neumann-s-kinesiology-of-the-musculoskeletal-system/neumann/978-0-323-71859-2).
12. [Uchida & Delp, *Biomechanics of Movement*; free companion materials](https://biomech.stanford.edu/).
13. [MIT OpenCourseWare](https://ocw.mit.edu/).
14. [OpenSim](https://opensim.stanford.edu/).

### Research, validation and data-rights reading
15. [Diffendaffer et al., *The Clinician's Guide to Baseball Pitching Biomechanics*](https://pmc.ncbi.nlm.nih.gov/articles/PMC9950989/).
16. [Oyama et al., *Reliability and Validity of Quantitative Video Analysis of Baseball Pitching Motion*](https://pubmed.ncbi.nlm.nih.gov/27705057/).
17. [OpenCap research article](https://pmc.ncbi.nlm.nih.gov/articles/PMC10586693/).
18. [OpenBiomechanics repository](https://github.com/drivelineresearch/openbiomechanics), [dataset datasheet](https://github.com/drivelineresearch/openbiomechanics/blob/main/DATASHEET.md) and [data license](https://github.com/drivelineresearch/openbiomechanics/blob/main/LICENSE-DATA.md).

**Last reviewed:** October 22, 2026. Always consult current university catalogs, revised research findings, edition-specific book contents, course availability and dataset licenses before use.

---

## 16. Glossary

- **Anatomical angle:** Joint or segment rotation defined in a stated anatomical coordinate system.
- **Projected/2D angle:** Image-plane angle derived from pixels or 2D landmarks; generally depends on viewpoint.
- **Kinematics:** Description of positions, angles, velocities and accelerations without necessarily finding the forces causing them.
- **Kinetics:** Forces and moments related to movement; often requires loads, inertial properties and dynamic modelling.
- **Torque / moment:** Turning effect of a force relative to an axis, often in N·m.
- **Inverse kinematics:** Estimating model joint coordinates that best match observed motion data.
- **Inverse dynamics:** Estimating net joint moments/forces from motion and appropriate external-load/inertial information under a model.
- **Forward dynamics:** Simulating motion from applied forces/controls and model dynamics.
- **Muscle redundancy:** Many muscle-force combinations can produce a similar net joint moment; extra assumptions/optimization are needed.
- **Reliability:** Consistency or repeatability of measurement under stated conditions.
- **Validity:** Whether the instrument/variable measures the intended construct accurately enough for a specified purpose.
- **Agreement:** Closeness of two methods' numerical measurements; not the same as strong correlation.
- **Within-athlete variation:** Differences among trials or sessions of the *same* pitcher; not the same as between-athlete differences.
- **Pseudo-replication:** Treating non-independent observations (e.g., many pitches from one athlete) as independent athletes.
- **Sensitivity analysis:** Testing how conclusions change when assumptions, inputs or analytic choices vary.
- **Error budget:** Organized accounting of identifiable measurement and model uncertainty.
- **Ground truth / reference standard:** Independently established measurement suitable for the specific quantity being validated; no method is perfect.
- **Pre-registration:** Recording intended hypotheses, methods and analyses before observing study outcomes where practical.
- **Evidence-based coaching:** Using research and measurements alongside expertise and athlete context; not letting one number dictate a mechanical change.

---

*PBMS is an independently authored educational plan informed by public university calendars and research literature. UBC, Stanford, MIT, OpenSim, Driveline and the cited authors have not endorsed this curriculum. University materials remain the property of their respective owners; this file summarizes and links to them rather than reproducing their textbooks or syllabi.*