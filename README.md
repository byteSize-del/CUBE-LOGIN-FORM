# 3D Cube Login Form

This project features a visually engaging 3D cube login form built with HTML, CSS, and JavaScript. The login form rotates through three cube faces: email entry, password entry, and a success screen, each with smooth animated transitions.

## Demo

![Cube Login Demo](Screenshot.png)
*(Add your demo GIF or screenshot here)*

## Features

- **3D Cube Animation:** The login steps are presented on rotating faces of a cube for a unique experience.
- **Animated Transitions:** Each face's content animates as it becomes active.
- **Email & Password Validation:** Basic checks for valid email format and password length.
- **Responsive Design:** Adapts to mobile and desktop screens.
- **Success Feedback:** A success icon and message appear upon successful login.

## How It Works

1. **Email Face:**  
   - Enter your email and click "Next".
   - Validates for non-empty input and proper email format.

2. **Password Face:**  
   - Enter your password and click "Submit" (or use Enter key).
   - Checks for non-empty input and a minimum length of 6 characters.

3. **Success Face:**  
   - Displays a confirmation and success icon.

Cube rotation and content transitions are handled by CSS and JavaScript event listeners.

## Usage

1. Download or copy `form.html` to your project folder.
2. Open `form.html` in your browser.
3. Interact with the form to experience the cube animation.

## Code Structure

- **HTML:** Contains the cube faces for email, password, and success steps.
- **CSS:** Handles cube 3D effects, face transitions, and responsive design.
- **JavaScript:** Manages face switching, validation, and transition logic.

## Customization

- You can adjust colors, gradients, border radius, and animation timing in the CSS.
- To integrate with a backend, replace the `console.log` in the submit handler with your server request logic.

## Example

```html
<!-- See 'form.html' for full code -->
<div class="cube-container">
  <div class="cube" id="cube">
    <!-- Face 1: Email -->
    <div class="cube-face front">
      <h2>Login</h2>
      <input type="email" id="email" placeholder="Enter your email">
      <button id="nextBtn">Next</button>
    </div>
    <!-- Face 2: Password -->
    <div class="cube-face right">
      <h2>Password</h2>
      <input type="password" id="password" placeholder="Enter your password">
      <div class="button-row">
        <button class="back-btn" id="backBtn">← Back</button>
        <button id="submitBtn">Submit</button>
      </div>
    </div>
    <!-- Face 3: Success -->
    <div class="cube-face back">
      <div class="success-content">
        <div class="success-icon"></div>
        <h2>Login Successful!</h2>
        <p>Welcome back! You have been successfully logged in.</p>
      </div>
    </div>
  </div>
</div>
```

## License

MIT License

---

*Inspired by modern UI/UX patterns for interactive forms.*
