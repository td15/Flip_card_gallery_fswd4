# 3D Flip Card - Interactive Design

A modern, responsive web project featuring interactive 3D flip cards built with pure HTML and CSS. Each card rotates 180° on hover to reveal additional content on the back.

## 🎯 Features

- **3D Flip Animation**: Smooth 180° rotation around the Y-axis on hover
- **Pure CSS Implementation**: No JavaScript required - uses only CSS transforms and transitions
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Modern UI**: Clean design with gradients, shadows, and smooth animations
- **Accessibility**: Proper focus states and semantic HTML structure
- **Performance Optimized**: Hardware-accelerated animations using CSS transforms

## 🛠️ Technologies Used

- **HTML5**: Semantic markup with proper structure
- **CSS3**: Advanced features including:
  - `transform: rotateY()` for 3D rotation
  - `transition` for smooth animations
  - `transform-style: preserve-3d` for 3D space
  - `perspective` for depth perception
  - `backface-visibility: hidden` to hide card backs
  - CSS Grid for responsive layout
  - Google Fonts (Poppins) for typography

## 📁 Project Structure

```
3d-flip-card/
├── index.html          # Main HTML file with semantic structure
├── style.css           # CSS with 3D flip effects and styling
└── README.md           # Project documentation
```

## 🎨 Key CSS Properties Explained

### 3D Flip Effect
```css
/* Container with 3D perspective */
.flip-card {
    perspective: 1000px;
}

/* Inner container with 3D transforms */
.flip-card-inner {
    transition: transform 0.6s ease;
    transform-style: preserve-3d;
}

/* Flip on hover */
.flip-card:hover .flip-card-inner {
    transform: rotateY(180deg);
}

/* Hide back faces */
.flip-card-front,
.flip-card-back {
    backface-visibility: hidden;
}

/* Back face initially rotated */
.flip-card-back {
    transform: rotateY(180deg);
}
```

## 🚀 How to Use

1. **Clone or download** the project files
2. **Open `index.html`** in your web browser
3. **Hover over the cards** to see the flip effect
4. **Resize the browser** to test responsive behavior

## 📱 Responsive Design

The project includes comprehensive responsive design:

- **Desktop**: 4-column grid layout
- **Tablet**: 2-column grid layout
- **Mobile**: Single column layout with optimized spacing

## 🎭 Animation Details

- **Duration**: 0.6 seconds
- **Easing**: `ease` for natural motion
- **Trigger**: Hover state
- **Additional Effects**: 
  - Scale effect on hover
  - Fade-in animation on page load
  - Button hover effects

## 🎨 Design Features

- **Gradient Backgrounds**: Beautiful purple gradient theme
- **Card Shadows**: Subtle depth with box-shadow
- **Rounded Corners**: Modern 20px border-radius
- **Skill Tags**: Interactive skill badges on card backs
- **Call-to-Action Buttons**: Styled buttons with hover effects

## 🔧 Customization

### Changing Colors
Modify the CSS variables in the gradient backgrounds:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Adjusting Animation Speed
Change the transition duration:
```css
transition: transform 0.6s ease; /* Adjust 0.6s to your preference */
```

### Adding More Cards
Simply copy the `<article class="flip-card">` structure and modify the content.

## 🌟 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## 📝 Requirements Met

✅ **Semantic HTML**: Uses `<article>`, `<section>`, `<h3>`, `<p>`, `<img>`  
✅ **3D Flip Effect**: `rotateY(180deg)` on hover  
✅ **Smooth Animation**: 0.6s transition with ease easing  
✅ **3D Space**: `transform-style: preserve-3d` and `perspective`  
✅ **Backface Hiding**: `backface-visibility: hidden`  
✅ **Modern Design**: Clean typography, shadows, rounded corners  
✅ **Google Fonts**: Poppins font family  
✅ **Visual Distinction**: Different colors and layouts for front/back  
✅ **Interactive Elements**: Hover effects and call-to-action buttons  

## 🎯 Learning Objectives

This project demonstrates:
- Advanced CSS 3D transforms
- CSS transitions and animations
- Responsive design principles
- Modern UI/UX patterns
- Semantic HTML structure
- CSS Grid layout system

## 📄 License

This project is open source and available under the MIT License. 