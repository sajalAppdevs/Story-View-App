# Story View App

A modern Flutter application that implements a WhatsApp-style story viewer with support for both images and videos. This app demonstrates how to create an engaging story viewing experience similar to popular social media platforms.

## Features

- 📸 Support for both image and video stories
- ⏱️ Customizable story duration
- 👆 Tap gestures for navigation (left/right)
- 🎨 Customizable progress indicator
- 🖼️ Cached network image support
- 📱 Responsive design
- 👤 User profile integration
- 🕒 Story timestamp display
- 🎬 Video playback support
- 💫 Smooth transitions between stories

## Tech Stack

- Flutter SDK (>=2.19.6 <3.0.0)
- Dependencies:
  - cached_network_image: ^3.2.3
  - video_player: ^2.6.1
  - flutter_story_view: ^0.0.2
  - intl: ^0.18.1

## Getting Started

### Prerequisites

- Flutter SDK installed on your machine
- Android Studio / VS Code with Flutter extensions
- An Android or iOS device/emulator

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Story-View-App.git
```

2. Navigate to the project directory:
```bash
cd Story-View-App
```

3. Install dependencies:
```bash
flutter pub get
```

4. Run the app:
```bash
flutter run
```

## Usage

The app demonstrates a WhatsApp-style story view implementation. Here's how to use it:

```dart
FlutterStoryView(
  storyItems: [
    StoryItem(
      url: "your_image_url",
      type: StoryItemType.image,
      duration: 3
    ),
    StoryItem(
      url: "your_video_url",
      type: StoryItemType.video,
      duration: 10
    ),
  ],
  onComplete: () {
    // Handle completion
  },
  onPageChanged: (index) {
    // Handle page change
  },
)
```

## Customization

The story view can be customized with various properties:

- `indicatorHeight`: Customize the height of the progress indicator
- `indicatorColor`: Change the background color of the progress indicator
- `indicatorValueColor`: Modify the progress indicator's fill color
- `enableOnHoldHide`: Toggle the ability to hide UI elements on hold
- `caption`: Add captions to your stories
- `userInfo`: Display user information with the story

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
