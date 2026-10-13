# Suneo’s Agony — OSINT CTF Writeup

**Category:** OSINT  
**Flag:** `Recon{Hoagland}`

## Challenge overview

The challenge gives us a short story: Suneo Honekawa says someone stole his plane, Electra, and crashed it. The task is to find the crash location. The prompt provides a starting point — the account name `honekawa_n` — and specifies the flag format as `recon[place_of_crash]`.

## Step 1 — Start with the account name

I started with the handle mentioned in the challenge, `honekawa_n`. Following that lead brought me to an Instagram account using the username `honekawa_n578sp`. The profile was the next clue to inspect rather than guessing the location from the challenge text alone.

![Challenge prompt](suneo_evidence_1.png)

![Instagram profile](suneo_evidence_2.jpeg)

## Step 2 — Check the highlight

The profile had a highlight with an image of the aircraft. I checked it closely because a registration printed on an aircraft can be used to search public aviation records.

![Instagram highlight](suneo_evidence_3.jpeg)

## Step 3 — Read the aircraft number

The aircraft image showed the registration `N578SP`. That gave me a specific identifier to search for in aircraft accident records.

![Aircraft registration N578SP](suneo_evidence_4.png)

## Step 4 — Find the accident report

The challenge states that the plane crashed, so I searched for the aircraft registration alongside aircraft crash or accident-report information. I found an accident report for the aircraft and checked its listed location.

![Accident report](suneo_evidence_5.png)

## Step 5 — Confirm the location

The report pointed to **Hoagland** as the accident location. The accompanying map was consistent with that location, so I used Hoagland as the place name for the flag.

![Accident location map](suneo_evidence_6.png)

## Flag

```text
Recon{Hoagland}
```

The solve came down to following the clues in order: the username led to the Instagram profile, the highlight revealed the aircraft registration, and the registration led to an accident report listing Hoagland as the crash location.
