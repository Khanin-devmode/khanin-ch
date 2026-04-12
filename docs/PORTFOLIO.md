

# Portfolio of what I've built and it's details.

## AudioAreanaLab

### Value Proposition
When comparing headphones traditionally, users often only receive information from reviewers and not hearing by themselves. AudioAreanaLab provides a platform for users to compare headphones by listening to them themselves and comparing them in real-time. So users can make informed decisions based on their personal preferences.

### Features
- Real-time audio comparison.
- Mobile friendly.
- Product pages to browse headphones.
- Product detail pages with audio samples.
- Product comparison feature with real-time swiching playback and frequency response visualization.

### Architecture
- Angular SSR with express.js.
- Firebase firestore for database.
- AWS s3 to store audio files and streaming.
- AWS cloudfront for content delivery.
- Implemented Design system with components. SCSS modules.
- Hosting on Render.com

### Audio engineering workflow.
#### Hardware
- Audio interface
- Binural mic for iems measurement. + Signal Implifier
- Hi-res DAC and Amplifier.

#### Software
- DAW: Audacity
- Loudness measurement: Youlean Loudness Meter
- Focusrite Control
- REW (Room EQ Wizard)

#### Workflow
- All headphoes are normalized wiht high/low pass filtered pink noise.
- Verify both ears produce the same loudness level.
- Heapdhones are recorded at safe level loudness at 80dB SPL to ensure it's capabilities at safe listening levels.
- Measure frequency response using REW (Room EQ Wizard) for each headphone.
- Clip the audio files and upload to s3 and it's frequency response data.

## Khanin.ch

## Convertrai

## Realmsup

## Fontpalette

## Design system AIS v1,v2 and v3

## Zatca demo, Agentic AI Project management.

## Krungthai bank. Mobile banking app. Fund redemption and subscription.
