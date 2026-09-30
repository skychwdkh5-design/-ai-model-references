# AI MODEL — MASTER REFERENCE LIBRARY

This repository contains the permanent reference images for ONE consistent AI character.

## Base URL

https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/

---

# FACE REFERENCES

## face_front.jpg
Front-facing facial reference.

Use primarily for:
- frontal portraits
- front-facing close-ups
- facial identity
- facial features
- eyes, nose, lips, jawline and general appearance

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_front.jpg


## face_3q.jpg
Three-quarter facial reference.

Use primarily when the face is shown at approximately a 3/4 angle.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_3q.jpg


## face_3q_opposite.jpg
Opposite three-quarter facial reference.

Use when the requested 3/4 angle is opposite to face_3q.jpg.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_3q_opposite.jpg


## face_profile_left.jpg
Left-facing profile facial reference.

Use primarily for left-facing side/profile views.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_profile_left.jpg


## face_profile_right.jpg
Right-facing profile facial reference.

Use primarily for right-facing side/profile views.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_profile_right.jpg


---

# FULL BODY REFERENCES

## fullbody_front.png
Primary front-facing full-body reference.

Use primarily for:
- body proportions
- height/proportions
- front-facing standing poses
- overall physique

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_front.png


## fullbody_3q_front.png
Three-quarter full-body reference.

Use primarily for standing 3/4 poses and body proportions viewed at an angle.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_3q_front.png


## fullbody_back.png
Back-view full-body reference.

Use primarily for:
- back-facing poses
- body proportions from behind
- back silhouette

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_back.png


## fullbody_profile_right.png
Full-body side/profile reference.

Use primarily for side-view standing poses and body proportions in profile.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_profile_right.png


---

# SEATED REFERENCES

## seated_front.png
Front/near-front seated reference.

Use for seated poses viewed primarily from the front.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/seated_front.png


## seated_profile_left.png
Side seated reference.

Use for seated poses viewed from the side/profile.

Raw URL:
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/seated_profile_left.png


---

# REFERENCE SELECTION RULES

All images in this repository represent the SAME AI character.

The character's identity must remain consistent across generations.

Before every image generation:

1. Analyze the requested camera angle, framing and pose.

2. Automatically select the most appropriate reference image or images from this library.

3. Do NOT ask the user to manually select references when the appropriate references can be determined automatically.

4. For facial identity, prioritize the FACE REFERENCES.

5. For body proportions and physique, prioritize the FULL BODY REFERENCES.

6. For seated compositions, use the appropriate SEATED REFERENCE together with a suitable FACE REFERENCE when useful.

7. For full-body generations, normally use:
   - one appropriate FACE reference
   - one appropriate FULL BODY reference

8. Match reference angles to the requested output whenever possible.

9. If the requested angle falls between available references, select the closest matching references.

10. Multiple references may be used when supported by the generation model.

11. Use the RAW URLs listed in this document as image inputs when calling Replicate.

12. Never require the user to manually copy GitHub URLs for normal generations.

13. Preserve facial identity, recognizable facial geometry, body proportions and overall character consistency.

14. Clothing, environment, lighting, pose, camera, expression and styling may change according to the user's request unless explicitly locked.

15. Do not treat clothing visible in reference images as part of the character's permanent identity.

---

# DEFAULT REFERENCE LOGIC

Front portrait:
face_front.jpg

3/4 portrait:
face_3q.jpg OR face_3q_opposite.jpg depending on direction.

Left profile portrait:
face_profile_left.jpg

Right profile portrait:
face_profile_right.jpg

Front full body:
face_front.jpg + fullbody_front.png

3/4 full body:
face_3q.jpg or face_3q_opposite.jpg + fullbody_3q_front.png

Side full body:
appropriate face profile + fullbody_profile_right.png

Back full body:
fullbody_back.png

Front seated:
face_front.jpg + seated_front.png

Side seated:
appropriate face profile + seated_profile_left.png
