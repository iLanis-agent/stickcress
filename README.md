# Stickcress 1.0 TEST
Native Android Tatebo-Yokobo straight-stick puzzle. Android 8+ (min26), target35. Package com.gg007.stickcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Tatebo-Yokobo on a 4x4 grid with four fixed dark cells. Every light cell starts with a horizontal line; tap it to switch horizontal/vertical. Neighboring aligned line segments merge into one maximal straight stick. A white number gives that whole stick length in cells. A stick may have at most one white number; unnumbered sticks are allowed. A dark number counts neighboring line ends pointing into that dark cell, not all neighboring cells. Lines never pass through dark cells. All light cells must hold one line. Undo/reset and next/levels; saved palette and optional H/V labels. Known Tatebo-Yokobo adaptation.

## Download and status
https://mega.co.nz/#!QUkVGBZT!rc8Jl7-ynrlfPn4SFjhGFCbfDSeRwF1lzQjllHxWXic
APK SHA256 596488147342a83b9704e05c2205c70845a9613f61af002be924c42c9f88a29a; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
A portable seed-691109 generator enumerates all 4,096 H/V assignments for each four-dark-cell layout and greedily removes clues while retaining one solution. An independent graph-component checker compares with the production run scanner on all 65,536 masks for each of twelve boards: 786,432 comparisons. It independently checks aligned components, clue length, at most one white clue and dark-cell line ends. Twelve unique clue boards and twelve different solutions. Bounds, dark-cell locks, undo/reset and solved lock pass. Actual drawing-adapter taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/H/V labels. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 200 live studio descriptions and the byte-current 803-entry web registry using functional terms. No Tatebo-Yokobo or straight-stick length/dark-endpoint-count match in this partial corpus. Strokehaven also switches H/V, but checks room majority and forbidden triples; Stickcress instead merges maximal straight sticks, constrains their lengths and counts endpoints entering fixed dark cells. Weavebriar places crossing paired bars into a network; Stickcress has no crossings, pairs or connectivity rule. Known Tatebo-Yokobo adaptation; original generated layouts, code and visuals. No copied layouts/code/art or global invention claim. Archived official rules and five independent rule references agree on core constraints; a community index confirms the genre. No history claim.
Rules https://www.janko.at/Raetsel/Tateboo-Yokoboo/index.htm ; independent rules https://puzzles.twistymaze.com/help/sticks .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/stickcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.stickcress.StickBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Stickcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, H/V labels and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 201-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/aincwf8n8nye-stickcress-source-archive . Repository https://github.com/iLanis-agent/stickcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
