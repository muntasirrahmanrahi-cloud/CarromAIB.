# Carrom Aim Bot V3 — Auto-calibrated live overlay

## What changed
- Automatic board calibration from the four dark corner pockets.
- No manual corner/scale setup is required for the supplied portrait Carrom layout.
- Pocket centers and approximate pocket radius are recalculated from the live frame.
- Coin/queen/striker segmentation is recalculated from the live frame.
- Chooses among direct and one-cushion candidate trajectories.
- Draws striker -> ghost hit point -> cushion (if needed) -> pocket.
- Recalibrates continuously, so different screen resolutions/board positions can be handled.
- Does not auto-click or inject touch input.

## Important limitation
This is visual auto-calibration, not perfect physics calibration. A single screenshot cannot reveal the game's exact friction, collision restitution, or shot-power curve. Those parameters remain approximate and may need tuning after observing real shots.

## Build
Open the `CarromAimBot` folder in Android Studio, build/install the debug APK, allow "display over other apps", then grant screen-capture permission and open the game.
