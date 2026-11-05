# Model Notes: Seedance 2.5 and Kling 4.0 for the Bicep Heart Trend

We did **not** run our own tests. This page separates three kinds of information:

- **A. Official facts.** Taken from the providers' own pages.
- **B. Third-party reports.** Other people's reviews, summarized. Usually one run or a few runs.
- **C. Our inferences.** Our reasoning, not facts. The uncertainty here is high.

All sources were accessed **2026-11-05**. Prices change; check the source before relying on them.

## A. Official facts

| Dimension | Seedance 2.5 (ByteDance Seed) | Kling 4.0 (Kuaishou) |
|---|---|---|
| Launch | API generally available Aug 2026 (per Runway dev docs) [S4] | Officially launched 2026-10-15 [K1]; API fully open 2026-10-28 [K2] |
| Clip length | Up to 30 s per generation, extendable twice [S1] | 3–30 s via API [K2] |
| Resolution | 480p / 720p / 1080p, no 4K [S2] | 720P / 1080P [K2][K3] |
| Multi-subject | Official blog: stability in multi-subject interaction and physical plausibility of complex motion "still have room for improvement" [S5] | No comparable self-assessment found on pages we read (not found ≠ doesn't exist) |
| Reference inputs | Up to 30 images / 10 videos / 10 audio [S5] | Not stated on pages we read |
| Official API price | BytePlus ModelArk: 480p/720p $10.70 per million tokens, 1080p $11.70 (no video input); failed generations not billed [S2] | 720P $0.157/s, 1080P $0.235/s (no video input); 4.0 Flash 720P $0.094/s [K3] |
| Hands / pets | No specific statement | No specific statement |

API prices are not the same as consumer app prices.

## B. Third-party reports (summarized)

- **VdoBloom**, 8 identical prompts: overall nearly tied (Kling 3.81 / Seedance 3.78). Kling won the hand test (shuffling cards); Seedance won fast motion and physics. Kling refused one harmless prompt. [T1]
- **Soku** (via fal): product-photo-to-video, Seedance completed the full hand action, while Kling's thumb covered the label. fal pricing: Seedance ~$0.473/s vs Kling $0.157/s (about 3×). [T2]
- **CellCog**, 10 tests: subjective preference favored Seedance 10–0 (texture, less "plastic" look). A stricter frame-by-frame review was 7–3, with total scores 408 vs 401 out of 700. [T3]
- **Crimson Spark**, citing Tech Times: in Kling, faces and hands can still drift between keyframes. [T4]
- **aivs.tv**, motion transfer: Seedance may carry the reference actor's face into the output. [T7]
- Resellers list 9:16 output for Seedance 2.5 [T5][T6].

## C. Our inferences (not facts)

1. **Each model has its own strengths.** For the bicep heart (mostly static arms plus a small movement, often two people or a pet), there's no evidence that either model is better. Kling has a published win on hand detail [T1]. Seedance has published wins on photo fidelity and realism [T2][T3]. Strict scoring puts them close [T3].
2. **Couples are hard for both.** Seedance's own blog flags multi-subject interaction [S5]. Expect several retries for two-person videos.
3. **Pets are unknown.** We found no official or third-party pet test.
4. **Cost.** At 720p, Kling's official per-second price is roughly a third of Seedance's price on fal [K3][T2]. For high volume, Kling is likely cheaper. Official-to-official comparisons are harder because the billing units differ (tokens vs seconds).
5. **Reseller versions can't be verified.** Third-party platforms label their model "Seedance 2.5", but none of the public pages we read let users verify which model is actually serving requests. We have no evidence that any of them are wrong. We just can't verify them independently.

## Other models
MiniMax H3 appears only in [T1]. We didn't check its official docs. Veo, Sora, and others aren't covered here.

## Sources
Accessed 2026-11-05.
- [S1] https://seed.bytedance.com/en/seedance2_5
- [S2] https://ai.byteplus.com/ark/region:ap-southeast-1/docs/model-pricing (page updated 2026-11-02)
- [S3] https://openrouter.ai/bytedance/seedance-2.5
- [S4] https://dev.runway.com/learn/seedance-2-5-api
- [S5] https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5
- [K1] https://ir.kuaishou.com/news-releases/news-release-details/kling-ai-officially-launches-next-generation-kling-40-raising/
- [K2] https://kling.ai/document-api/updates/api.md
- [K3] https://kling.ai/document-api/pricing/base/video.md
- [T1] https://vdobloom.com/blog/kling-4-vs-seedance-2-5-vs-minimax-h3/
- [T2] https://soku.ai/compare/seedance-vs-kling
- [T3] https://cellcog.ai/blog/seedance-2-5-vs-kling-4-0/
- [T4] https://crimsonsparkagency.com/insights/kling-4-vs-seedance-2-5-brand-video.html
- [T5] https://letz.ai/blog/seedance-25-announcement
- [T6] https://dreamina.capcut.com/seedance/seedance-2-5-aspect-ratio
- [T7] https://aivs.tv/p/2112439793930133608/
