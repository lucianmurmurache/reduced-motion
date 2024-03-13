# reduced-motion

A simple, lighweight package that makes sure your animations do not run when users disable animation preferences.

## Features

- Easy integration with any web project.
- Focus on accessibility and user preference.
- Lightweight and straightforward, with no dependencies.

## Installation

Install `reduced-motion` using npm:

```bash
npm i reduced-motion

```

Or with yarn:

```bash
yarn add reduced-motion

```

## Usage

After installing, import `reduced-motion` into your project:

```bash
import 'reduced-motion/css';
```

Or link directly in your HTML file:

```bash
<link rel="stylesheet" href="https://unpkg.com/reduced-motion/dist/index.min.css" />

```

## How It Works

`reduced-motion` automatically applies styles that reduce motion when the user has indicated a preference for reduced motion through their system settings. It also removes video backgrounds, namely it targets the video elements which have the `autoplay` attribute.

## Testing

To test the package once you've added it to your project, you simply need to disable animations on your device. Follow the steps below:

- Windows 10: Settings > Ease of Access > Display > Show animations in Windows.
- Windows 11: Settings > Accessibility > Visual Effects > Animation Effects
- macOS: System Preferences > Accessibility > Display > Reduce motion.

- iOS: Settings > Accessibility > Motion.
- Android 9+: Settings > Accessibility > Remove animations.

- Plasma/KDE: System Settings > Workspace Behavior -> General Behavior > "Animation speed" is set all the way to right to "Instant".
- GTK/GNOME: Settings > Accessibility > Seeing > Reduced animation is turned on.

## Performance concerns

This package utilises a media query to check if users have disabled animations on their devices. When this setting is detected, CSS overrides are activated to accommodate this preference. In cases where reduced motion is enabled, the package meticulously targets elements and pseudo-elements throughout the document. It adjusts animation timing, modifies the background-attachment property, and alters scroll behavior. Additionally, it hides video elements with the autoplay attribute to ensure a smooth and comfortable browsing experience for users sensitive to motion. This approach ensures minimal performance impact, activating only when users explicitly opt for reduced motion. Thus, it maintains an optimal balance between accessibility and efficiency.

## Contributing

Check out the [CONTRIBUTING.md](https://github.com/lucianmurmurache/reduced-motion/blob/main/CONTRIBUTING.md) for guidelines on how to proceed. Let's make the web more accessible to everyone.

## Code of Conduct

This project is released with a [Contributor Code of Conduct](https://github.com/lucianmurmurache/reduced-motion/blob/main/CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.

## License

`reduced-motion` is available under the ISC License. See [LICENSE](https://github.com/lucianmurmurache/reduced-motion/blob/main/LICENSE) for more info.
