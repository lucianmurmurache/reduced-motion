# reduced-motion

A simple, lighweight package that makes sure your animations do not run when the user animations preference is disabled.

## Features

- Easy integration with any web project.
- Focus on accessibility and user preference.
- Lightweight and straightforward, with minimal dependencies.

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
<link rel="stylesheet" href="node_modules/reduced-motion/css/index.css">

```

## How It Works

`reduced-motion` automatically applies styles that reduce or remove motion when the user has indicated a preference for reduced motion through their system settings.

## Performance concerns

This package employs a media query to ascertain if users have opted to disable animations on their devices. The CSS overrides, designed to cater to this preference, are activated only when this setting is detected. In scenarios where the preference for reduced motion is enabled, the package meticulously targets both elements and pseudo-elements across the document. It then adjusts the animation timing, modifies the background-attachment property, and alters the scroll behavior to ensure a seamless and comfortable browsing experience for users sensitive to motion. This approach guarantees that the performance impact is minimal and only comes into effect when the user's preferences explicitly call for reduced motion, thereby maintaining an optimal balance between accessibility and efficiency.

## Contributing

We welcome contributions to `reduced-motion`! Please check out our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to proceed. Join us in making the web more accessible to everyone.

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project, you agree to abide by its terms.

## License

`reduced-motion` is available under the ISC License. See the [LICENSE](LICENSE) file for more info.
