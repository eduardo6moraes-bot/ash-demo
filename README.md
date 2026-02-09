# ASH — AI-Driven Cinematic Visual Intelligence

ASH is an AI-driven cinematic visual intelligence demo that orchestrates AI-generated video and imagery into immersive, high-end visual experiences with a futuristic corporate aesthetic.

## Problem & Solution

**The Problem:** Traditional cinematic production is expensive, time-consuming, and inaccessible. High-quality cinematography requires specialized crews, expensive equipment, and weeks of production. Small teams and startups are locked out of professional visual storytelling.

**The Solution:** ASH demonstrates how generative AI can replace traditional cinematic production pipelines. Using AI-generated video and image synthesis, we create broadcast-quality cinematics in hours instead of weeks, at a fraction of the cost.

**Why It Matters Now:** The convergence of AI image/video generation, affordable compute, and sophisticated prompting techniques makes this feasible today. Teams can now access cinematic-grade visuals without a studio.

## Why It Matters

ASH directly impacts three audiences:

- **Agencies & Studios** — Reduce production timelines and costs while expanding creative capacity
- - **Marketing Teams** — Produce on-demand cinematic assets for campaigns, launches, and events without waiting for production houses
  - - **Startups** — Access broadcast-quality visuals typically reserved for enterprises with big budgets
   
    - ## Live Demo
   
    - [View ASH Demo](https://eduardo6moraes-bot.github.io/ash-demo/)
   
    - ## Concept
   
    - Four 10-second cinematic clips form a 40-second visual arc:
   
    - | # | Clip | Camera Motion | Narrative |
    - |---|------|---------------|-----------|
    - | 1 | IGNITION | Dolly forward | Entry — anticipation, precision |
    - | 2 | STRUCTURE | Slow orbit | Observation — contemplation |
    - | 3 | EXPANSION | Push-in | Scale — quiet power |
    - | 4 | SILENCE | Dolly backward | Closure — serenity |
   
    - Arc: (a breathing cycle)
    - **enter → observe → expand → retreat**
   
    - ## Visual Identity
   
    - - **Palette:** Deep blacks, metallic grays, cold blue, amber accents
      - - **Surfaces:** Polished floors, dark glass, brushed metal, volumetric light
        - - **Camera:** Slow, controlled — dolly, orbit, push-in
          - - **Lighting:** Low-key, backlit, volumetric
            - - **Constraints:** No people, no text, no logos, no UI
             
              - ## Tech Stack
             
              - | Component | Tool |
              - |-----------|------|
              - | Video Generation | Runway Gen-3 |
              - | Image Generation | Craiyon / Midjourney |
              - | Frontend | HTML, CSS, JavaScript |
              - | Hosting | GitHub Pages |
              - | Video Assembly | FFmpeg |
             
              - ## Project Structure
             
              - ```
                ash-demo/
                ├── index.html
                ├── assets/
                │ ├── video/
                │ │ └── ash-final.mp4
                │ ├── clips/
                │ │ ├── 01-ignition.mp4
                │ │ ├── 02-structure.mp4
                │ │ ├── 03-expansion.mp4
                │ │ └── 04-silence.mp4
                │ └── images/
                │   └── cover.png
                ├── pitch/
                │ ├── ash-pitch.mp4
                │ └── ash-deck.pdf
                └── README.md
                ```

                ## Video Assembly

                ```bash
                echo "file 'assets/clips/01-ignition.mp4'" > filelist.txt
                echo "file 'assets/clips/02-structure.mp4'" >> filelist.txt
                echo "file 'assets/clips/03-expansion.mp4'" >> filelist.txt
                echo "file 'assets/clips/04-silence.mp4'" >> filelist.txt

                ffmpeg -f concat -safe 0 -i filelist.txt -c copy assets/video/ash-final.mp4
                ```

                ## Use Cases

                - Corporate brand videos and visual identities
                - - Immersive event presentations
                  - - Product launch cinematics
                    - - AI-powered creative pipeline demonstrations
                      - - Visual prototyping for agencies and studios
                       
                        - ## Hackathon
                       
                        - Built for [lablab.ai Hackathon 2026](https://lablab.ai)
                       
                        - ## License
                       
                        - MIT
                       
                        - ## Pending Assets
                       
                        - The following assets are currently placeholders and need to be replaced with final files:
                       
                        - - `assets/video/ash-final.mp4` — Final 40s cinematic video (1920x1080, H.264)
                          - - `assets/images/cover.png` — Project cover image (16:9, 1920x1080)
                            - - `assets/images/01-threshold.png` — Clip 01 thumbnail
                              - - `assets/images/02-construct.png` — Clip 02 thumbnail
                                - - `assets/images/03-grid.png` — Clip 03 thumbnail
                                  - - `assets/images/04-fade.png` — Clip 04 thumbnail
                                    - - `pitch/ash-pitch.mp4` — Pitch video (3-5 min)
                                      - - `pitch/ash-deck.pdf` — Slide deck PDF
