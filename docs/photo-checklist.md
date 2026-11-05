# Photo Checklist for AI Bicep Heart Videos

Image-to-video models animate what they can see. A good input photo matters more than the model.

## Use a photo that has
- [ ] Chest or waist up, with **both arms, the shoulders, and the area between shoulder and head** visible, because the whole move happens there ([ViralRemix](https://viralremix.org/bicep-heart-trend), [MimicZip](https://mimiczip.com/bicep-heart))
- [ ] Short sleeves or a tank top if possible, so the model can see the arm ([ViralRemix](https://viralremix.org/bicep-heart-trend))
- [ ] Sharp focus on faces and arms, no motion blur
- [ ] Even, front-facing light
- [ ] Plain or uncluttered background
- [ ] Arms not hidden by bags, other people, or clothing
- [ ] Portrait orientation if possible (output is usually 9:16)
- [ ] At least ~1000 px on the short side

## Per mode
- **1 person (the original format):** one person alone, looking at the camera ([MimicZip](https://mimiczip.com/bicep-heart)).
- **Couple (spin-off):** the heart is still made by one person, so use a clear photo of the person sending it. Multi-subject scenes are a known weak spot for current models (Seedance's own blog says so; see [model-notes.md](model-notes.md)), so if both people are in the frame, expect to retry.
- **Pet (AI-only spin-off):** pets have no biceps, so the result is an approximation ([ViralRemix](https://viralremix.org/bicep-heart-trend)). Use a photo with the pet's face and outline clearly visible. No public model test covers pets.

## Avoid
- Group photos with more than the people you want animated
- Heavy beauty filters or stylized edits
- Sunglasses or hats that hide faces
- Photos of anyone who hasn't agreed to being animated, including celebrities and minors you aren't the guardian of

## After generation
Check hands and fingers frame by frame (the most common artifact), check faces still look like the people in the photo, and label the clip as AI-generated when you post it.

## Sources (accessed 2026-11-05)
- https://viralremix.org/bicep-heart-trend
- https://mimiczip.com/bicep-heart
