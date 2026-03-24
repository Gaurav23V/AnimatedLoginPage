# Animated Login Page

## Purpose/Description

A visually appealing, fully animated authentication page featuring smooth transitions between Sign Up and Sign In forms. The page provides a modern user experience with sliding panels and social login options through Google and GitHub.

**Live Demo**: [https://gaurav23v.github.io/AnimatedLoginPage/](https://gaurav23v.github.io/AnimatedLoginPage/)

## Tech Stack

- **HTML5** - Semantic markup structure
- **CSS3** - Styling and animations
  - Keyframe animations
  - CSS transitions
  - Flexbox layout
  - Custom properties
- **JavaScript (Vanilla)** - Interaction handling
- **Font Awesome 6.5.1** - Icon library for social login buttons
- **Google Fonts** - Montserrat typography

## Implementation Details

### Animation System

The page features a sophisticated animation system:

- **Sliding Panels**: Sign-in and sign-up forms slide in/out based on user interaction
- **Toggle Animation**: A central toggle panel smoothly transitions between states
- **Timing**: All animations use a 0.6s ease-in-out transition for consistency
- **Z-index Management**: Careful layering ensures smooth visual transitions

### UI Components

```
┌─────────────────────────────────────┐
│  [Logo/Camp Icon]                   │
│  ┌─────────────┬───────────────────┐│
│  │   Sign Up   │    Toggle Panel   ││
│  │   Form      │    (animated)      ││
│  │             │                    ││
│  │  [Google]   │  "Don't Have an    ││
│  │  [GitHub]   │   Account?"        ││
│  │             │                    ││
│  │  Email      │  [Sign Up Button]  ││
│  │  Password   │                    ││
│  │  [Sign Up]  │                    ││
│  └─────────────┴───────────────────┘│
└─────────────────────────────────────┘
```

### Color Scheme

- **Primary Color**: `#ff9000` (Orange)
- **Gradient**: `#e2e2e2` to `#ffaa4c`
- **Background**: White cards on gradient background
- **Accent**: Orange buttons with white text

### File Structure

```
AnimatedLoginPage/
├── index.html    # Main HTML structure
├── style.css     # All styling and animations (210 lines)
├── script.js     # Toggle functionality (11 lines)
└── README.md
```

## Installation/Setup

No build process required. Simply serve the files:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve

# Or open directly in browser
open index.html
```

## Usage

1. Open `index.html` in a web browser
2. Click "Sign Up" to view the registration form with animated transition
3. Click "Sign In" to view the login form with animated transition
4. Social login buttons (Google, GitHub) are styled but not connected to backend

## Key Features

- **Smooth CSS Animations**: All transitions are hardware-accelerated
- **Responsive Design**: Works on various screen sizes (max-width: 768px, min-height: 480px)
- **Social Login UI**: Buttons for Google+ and GitHub authentication
- **Password Recovery Link**: "Forget Your Password?" option
- **No Dependencies**: Pure HTML/CSS/JS implementation
- **Modern Typography**: Uses Montserrat font family

## Customization

The page can be easily customized:
- Change colors in CSS variables or body background
- Add actual authentication logic to form submissions
- Connect social login buttons to OAuth providers
- Add form validation JavaScript