# Running Coach: Research Notes & Plan Rationale

> Captured 2026-05-25. Source notes for `index.html` so the WHY behind each session is preserved.

## Athlete Profile

- 6 years old, daughter
- Baseline (2026-05-24): 100m in 25s, 60m in 14s, standing long jump 1.2m at 3/10 success rate
- Moderately active, plays sport for fun (not yet trained)
- Normal trainers (no spikes / proper sprint shoes)
- Reports being out of breath after one 100m

## Goal

School athletics tryout on **2026-06-13** (19 days from the start of training).

Qualifying minimums (not selection criteria, just gate to even try out):
- 100m under 20 seconds
- 60m under 12 seconds
- Standing long jump over 1.2 metres

## Training Constraints

- 2 to 3 days per week (Tue / Thu + one weekend day)
- Cycling track 5 minutes from home (used for sprints)
- Home garden 5m by 7m (used for jumps and short drills)
- Parent-led, not coach-led. Cues must be simple enough for Will to deliver without sports-science background.

## Source Material

| Source | URL | Key takeaways used |
|---|---|---|
| US youth strength coach | https://www.youtube.com/watch?v=ZpoTvgoUZSI | Acceleration mechanics, external-focus cues for kids, "push the ground away" framing |
| Swedish football academy | https://www.youtube.com/watch?v=OJnSV8Bl6wo&t=9s | Game-like sprint drills, keeping intensity high but session count low for pre-pubescents |

Plus two research briefs (synthesised in chat, not saved separately):
1. Standing long jump development for 5 to 7 year olds
2. 19-day youth sprint preparation under realistic 2-3 day constraints

## Core Scientific Constraints (THE LOAD-BEARING STUFF)

These are the rules the plan is built on. If you ever change the plan, do not break these:

### 1. No anaerobic adaptation before puberty

Pre-pubescent kids do not respond to "speed endurance" or lactic conditioning the way teenagers and adults do. Their cardiovascular and hormonal systems are not ready. Training for it just produces tired, discouraged kids with no actual gain.

**Implication:** When Jayna is out of breath after one 100m, the answer is NOT to push through with conditioning. It is to teach pacing and breathing rhythm so she does not blow up in the first 30 metres.

The 60m pace being faster than the 100m pace (per metre) confirms this. She is going all-out too early then dying. It is a pacing problem, not a fitness problem.

### 2. External focus cues outperform internal focus cues for young kids

"Push the ground away from you" beats "extend your hip and knee fully." Kids cannot translate body-part instructions into movement. They CAN respond to imagery and targets.

**Implication:** Every cue in the plan is external. Examples used:
- Sprint: "Punch the sky," "Push the ground back"
- Jump: "Reach for the ceiling," "Jump over the noodle"
- Pacing: "Save some petrol for the end"

### 3. Technique and neural patterning, not strength or volume

NSCA Long-Term Athletic Development position stand: at this age, training is about laying down clean movement patterns. Volume is low. Quality is everything. Stop when form degrades.

**Implication:** All sessions are short (20 to 30 mins). Jump count caps at around 15 to 20 quality reps. Sprint reps capped at 4 to 6 full efforts. When she said she could do more jumps but was getting worse, Will correctly stopped her. This is the rule, not the exception.

### 4. Standing long jump is a two-foot, counter-movement, full-body action

The 1.2m at 3/10 success rate is a technique consistency problem, not a power problem. She CAN hit 1.2m. She just cannot do it reliably.

**Implication:** The plan does not train her to jump further. It trains her to hit 1.2m reliably. The key elements:
- Two feet planted side by side, takeoff together
- Arm swing back, then explosive swing forward
- Bend the knees (counter-movement), then explode up AND forward
- Aim trajectory at about 45 degrees, not flat

**Critical drill: "Jump Over the Noodle."** Roll a towel onto a couple of plastic cups about 25cm high, place it 40cm in front of her toes. She has to clear the noodle. This forces her to jump UP and forward, not flat. Flat trajectory was the silent killer of her distance.

## Why The Plan Is Shaped This Way

### 9-session structure, not daily

Two to three sessions per week for 19 days = roughly 9 sessions. Each session has a SINGLE focus. We never train sprints and jumps in the same session because:
1. Cognitive load for a 6yo is real. One movement pattern per day.
2. Recovery between explosive sessions matters even at this age.

### Phase structure

| Phase | Sessions | Purpose |
|---|---|---|
| Phase 1 | 1_A, 1_B, 1_C | Foundation. Teach the movement. End with a baseline retest. |
| Phase 2 | 2_A, 2_B, 2_C | Add power and race-specific elements. Teach pacing. |
| Phase 3 | 3_A, 3_B, 3_C | Sharpen, rehearse the tryout, then peak on the day. |

### Why the 100m approach is pacing, not conditioning

Jayna's 60m pace per metre is faster than her 100m pace per metre. That means she is going too hard early. The fix is rhythm and breathing, not engine size.

Sessions teach: "First 30m hard, middle 40m smooth, last 30m drive." We rehearse this multiple times before the tryout so her body knows the shape of a 100m, not just an all-out sprint.

### Why we test before the real tryout

Session 1_C and 3_B are dress rehearsals. The goal is not just to measure progress. It is to remove the novelty of being timed under pressure. By tryout day she has done this 3 times.

## Things to AVOID (also baked into the plan)

- Telling her to "run faster." Useless cue. Replace with "punch the sky harder."
- Running back-to-back 100m efforts with short rest. This trains lactic tolerance she cannot biologically develop yet, and it kills her motivation.
- Coaching mid-sprint. Coach BEFORE the rep, observe DURING, give one note AFTER.
- More than 6 full sprint efforts in a session. Quality degrades fast.
- Static stretching as warm-up. Use dynamic warm-up (skips, leg swings, butt kicks).
- Upgrading to spikes or sprint shoes before tryout. Not enough time to adapt. Normal trainers are correct for now.
- Treating jumps and sprints the same week as identical "leg days." They are different neural patterns.

## If The Plan Stops Working

Decision tree for if Jayna plateaus or regresses:

| Symptom | Likely cause | Adjustment |
|---|---|---|
| Sprint time stalls | Form breakdown under fatigue | Shorter reps, longer rest |
| Jumps go flat (less distance) | Lost the counter-movement | Re-do noodle drill, slow tempo |
| Jumps inconsistent | Two-foot timing off | Wall-facing practice, focus arm swing |
| Loses motivation | Too much testing, not enough play | Skip a test session, add a game format |
| Out of breath after one 100m still | Pacing not learned | Drill the "30-40-30" breakdown explicitly |

## Tooling

The plan is delivered via the webapp at https://willfung28.github.io/running-coach/ (source: this repo, `index.html`). The app:
- Shows each session's drills with bilingual zh-HK / English explanations
- Lets Will log times and jump distances
- Tracks progress against baseline
- Saves to localStorage on the phone

Plan structure is in the `SESSIONS` const inside `index.html`. Each session is `{name, intro, logFields, drills: [{title, desc, tips}]}`.

## Updated

2026-05-25 HKT
