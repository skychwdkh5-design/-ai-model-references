AI MODEL — MASTER REFERENCE LIBRARY
This repository contains the permanent reference images for ONE consistent AI character.
All images in this repository represent the SAME AI character.
Base URL
https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/
DIRECTION SYSTEM
All directions are defined by SCREEN DIRECTION — where the nose/face points in the FINAL IMAGE as seen by the viewer. Never by the character’s anatomical left/right side.
FRONT — face or body directed straight at the camera
NOSE_LEFT — nose/face points toward the LEFT side of the image
NOSE_RIGHT — nose/face points toward the RIGHT side of the image
BACK — character is turned with their back to the camera
UNFIXED — direction not yet confirmed; must NOT be assumed or guessed (reserved for future references; no file in this library is currently UNFIXED)
File names are identifiers only. The Direction field and visually verified image content are authoritative. Never infer direction from a file name.
REFERENCE SUMMARY
FACE REFERENCES
face_front.jpg
Frame type: FACE_FRONT Direction: FRONT
Use primarily for:
frontal portraits
front-facing close-ups
facial identity
facial features
eyes, nose, lips, jawline and general appearance
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_front.jpg
face_3q.jpg
Frame type: FACE_3Q Direction: NOSE_RIGHT
Directional authority for ALL three-quarter NOSE_RIGHT generations (portraits and full body). Use when the face is shown at approximately a 3/4 angle with the nose pointing toward the RIGHT side of the image.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_3q.jpg
face_3q_opposite.jpg
Frame type: FACE_3Q Direction: NOSE_LEFT
Directional authority for ALL three-quarter NOSE_LEFT generations (portraits and full body). Use when the face is shown at approximately a 3/4 angle with the nose pointing toward the LEFT side of the image.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_3q_opposite.jpg
face_profile_left.jpg
Frame type: FACE_PROFILE Direction: NOSE_LEFT
Visually verified: the nose/face points toward the LEFT side of the image.
Use for profile portraits where the nose points to the LEFT side of the image. Facial and directional authority for side-view NOSE_LEFT generations (standing and seated).
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_profile_left.jpg
face_profile_right.jpg
Frame type: FACE_PROFILE Direction: NOSE_RIGHT
Visually verified: the nose/face points toward the RIGHT side of the image.
Use for profile portraits where the nose points to the RIGHT side of the image. Facial and directional authority for side-view NOSE_RIGHT generations (standing and seated).
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/face_profile_right.jpg
FULL BODY REFERENCES
fullbody_front.png
Frame type: FULLBODY_FRONT Direction: FRONT
Primary full-length reference.
Use primarily for:
full-length body proportions
leg length and height proportions
front-facing standing poses
overall physique
In three-quarter and side NOSE_RIGHT full-body generations: contributes leg length and full-length proportions only. Never a direction source in those generations.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_front.png
fullbody_3q_front.png
Frame type: THREE_QUARTER_LENGTH_FRONT (mid-thigh up, near-front, slight natural turn, low camera angle) Direction: FRONT
Visually verified: near-front view, framed from mid-thigh up.
NOT a three-quarter-angle reference. The “3q” in the file name means three-quarter LENGTH, not a 3/4 view. NEVER use this file to determine NOSE_LEFT or NOSE_RIGHT. It must never override the requested direction.
Use primarily for:
torso/body identity, bust, waist and hip proportions and volume (including in 3/4 generations, as a proportions/volume-only reference)
front / near-front waist-up and thigh-up shots
Contains no knees, lower legs or feet — do not use it for leg length or full-length proportions; use fullbody_front.png for those.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_3q_front.png
fullbody_back.png
Frame type: FULLBODY_BACK Direction: BACK
Use primarily for:
back-facing poses
body proportions from behind
back silhouette
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_back.png
fullbody_profile_right.png
Frame type: FULLBODY_PROFILE Direction: NOSE_LEFT
Visually verified: face and body both point toward the LEFT side of the image. WARNING: the file name is misleading. Do NOT infer direction from the file name. This file is NOT a NOSE_RIGHT reference and must never be used in NOSE_RIGHT generations.
Use primarily for side-view NOSE_LEFT standing poses and full-length body proportions in profile.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/fullbody_profile_right.png
SEATED REFERENCES
seated_front.png
Frame type: SEATED_FRONT Direction: FRONT (front / near-front)
Use for seated poses viewed primarily from the front.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/seated_front.png
seated_profile_left.png
Frame type: SEATED_PROFILE Direction: NOSE_LEFT
Visually verified: both the face and the seated body orientation point toward the LEFT side of the image.
Use for side-view NOSE_LEFT seated poses. In side seated NOSE_RIGHT generations: proportions only, never a direction source.
Raw URL: https://raw.githubusercontent.com/skychwdkh5-design/-ai-model-references/refs/heads/main/seated_profile_left.png
REFERENCE SELECTION RULES
All images in this repository represent the SAME AI character.
The character’s identity must remain consistent across generations.
Before every image generation:

1. Analyze the requested camera angle, framing and pose.
2. Determine the requested direction using the DIRECTION SYSTEM (screen direction only).
3. Automatically select the most appropriate reference image or images from this library.
4. Do NOT ask the user to manually select references when the appropriate references can be determined automatically.
5. For facial identity, prioritize the FACE REFERENCES.
6. For body proportions and physique, prioritize the FULL BODY REFERENCES.
7. For seated compositions, use the appropriate SEATED REFERENCE together with a suitable FACE REFERENCE when useful.
8. For full-body generations, normally use:
  • one appropriate FACE reference
  • one appropriate FULL BODY reference
9. Match reference directions to the requested output whenever possible.
10. If the requested angle falls between available references, select the closest matching references.
11. Never mirror or flip reference images. If a body reference exists only in the opposite direction, use it for proportions only and describe the required direction in the prompt.
12. Never assume a direction for files marked UNFIXED.
13. Multiple references may be used when supported by the generation model.
14. Use the RAW URLs listed in this document as image inputs when calling Replicate.
15. Never require the user to manually copy GitHub URLs for normal generations.
16. Preserve facial identity, recognizable facial geometry, body proportions and overall character consistency.
17. Clothing, environment, lighting, pose, camera, expression and styling may change according to the user’s request unless explicitly locked.
18. Do not treat clothing visible in reference images as part of the character’s permanent identity.

────────

DEFAULT REFERENCE LOGIC

Front portrait:
face_front.jpg

3/4 portrait, NOSE_RIGHT:
face_3q.jpg

3/4 portrait, NOSE_LEFT:
face_3q_opposite.jpg

Profile portrait, NOSE_LEFT:
face_profile_left.jpg

Profile portrait, NOSE_RIGHT:
face_profile_right.jpg

Front full body:
face_front.jpg + fullbody_front.png

3/4 full body, NOSE_RIGHT:
face_3q.jpg + fullbody_3q_front.png + fullbody_front.png
(face_3q.jpg sets facial identity and direction; fullbody_3q_front.png contributes torso/waist/hip proportions and volume only; fullbody_front.png contributes leg length and full-length proportions only; no mirroring)

3/4 full body, NOSE_LEFT:
face_3q_opposite.jpg + fullbody_3q_front.png + fullbody_front.png
(face_3q_opposite.jpg sets facial identity and direction; fullbody_3q_front.png contributes torso/waist/hip proportions and volume only; fullbody_front.png contributes leg length and full-length proportions only; no mirroring)

Side full body, NOSE_RIGHT:
face_profile_right.jpg + fullbody_front.png
(face_profile_right.jpg sets facial identity and direction; fullbody_front.png contributes full-length proportions only; do NOT use fullbody_profile_right.png because its visually verified direction is NOSE_LEFT; no mirroring)

Side full body, NOSE_LEFT:
face_profile_left.jpg + fullbody_profile_right.png
(fullbody_profile_right.png is visually verified NOSE_LEFT despite its file name; no mirroring)

Back full body:
fullbody_back.png

Front seated:
face_front.jpg + seated_front.png

Side seated, NOSE_LEFT:
face_profile_left.jpg + seated_profile_left.png

Side seated, NOSE_RIGHT:
face_profile_right.jpg + seated_profile_left.png
(seated_profile_left.png is used for proportions only; direction is set by face_profile_right.jpg and the prompt; no mirroring)
