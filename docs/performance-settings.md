# Performance Settings

Shaders can be demanding, especially on laptops, older desktops, integrated graphics, and PCs with limited cooling.

Start with conservative settings, then raise quality after you know the game is stable.

## Best Lower-Impact Setup

Use:

- Fabric Loader 26.2
- Iris + Sodium
- Complementary Reimagined
- Server resource pack enabled

Complementary Reimagined usually keeps the game closer to vanilla and can be easier to run than Complementary Unbound.

## First Settings to Lower

Lower these first if FPS is poor:

- Shadow Distance
- Render Distance
- Volumetric Lighting
- Reflections
- Ambient Occlusion
- Clouds

Turn these off first if the game feels blurry or slow:

- Motion Blur
- Depth of Field
- Lens Flare
- Screen Space Reflections on weak GPUs

## Recommended Starting Points

For weaker PCs:

```text
Shader: Complementary Reimagined
Shader profile: Low or Medium
Render Distance: 6 to 8 chunks
Simulation Distance: 4 to 5 chunks
Shadow Distance: 4 to 6 chunks
Volumetric Lighting: Low or Off
Reflections: Low or Off
Motion Blur: Off
Depth of Field: Off
Clouds: Fast or Off
```

For mid-range PCs:

```text
Shader: Complementary Unbound
Shader profile: Medium
Render Distance: 8 to 12 chunks
Simulation Distance: 5 to 8 chunks
Shadow Distance: 8 to 12 chunks
Volumetric Lighting: Low or Medium
Reflections: Medium
Motion Blur: Off
Depth of Field: Off
```

For stronger PCs:

```text
Shader: Complementary Unbound
Shader profile: High
Render Distance: 12 to 16 chunks
Simulation Distance: 8 chunks
Shadow Distance: 12 to 16 chunks
Volumetric Lighting: Medium or High
Reflections: Medium or High
Motion Blur: Personal preference
Depth of Field: Personal preference
```

## Sodium Settings

Sodium usually improves performance without needing much setup.

Good general choices:

- Use fullscreen mode if windowed mode stutters.
- Keep VSync off if it causes input delay or unstable frame pacing.
- Cap FPS to a number your PC can hold consistently.
- Keep graphics drivers updated.

## Practical FPS Targets

Aim for stable performance instead of chasing a peak FPS number.

- 30 FPS: playable for weaker PCs
- 45 to 60 FPS: comfortable for most players
- 90+ FPS: nice if your monitor and GPU can support it

If your FPS jumps between high and low numbers, cap it near the lower stable number. A steady 60 FPS often feels better than 110 FPS that drops constantly.

## Server Settings Still Matter

Client shaders do most of the visual work, but server and world settings can still affect smoothness.

Performance-friendly server choices:

- Avoid excessive entity counts in decorative areas.
- Keep redstone-heavy builds controlled.
- Avoid huge item piles.
- Use reasonable server view distance settings.

These do not replace client tuning, but they help weaker PCs feel less overloaded.
