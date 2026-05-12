# Voice Assistant - EchoEats

A powerful voice-enabled assistant for EchoEats food ordering application that allows users to navigate, search, filter, and order food using natural voice commands.

## Features

### Core Functionality
- **Voice Navigation** - Navigate to different pages using voice commands
- **Food Ordering** - Add items to cart with quantity specifications
- **Category Filtering** - Filter food items by categories (Pizza, Burger, Main Course, etc.)
- **Voice Login/Logout** - Secure authentication via voice
- **Text-to-Speech** - Voice responses for all actions
- **Multi-command Support** - Process multiple commands with pause detection

### 🗣️ Voice Commands

| Command Type | Examples | Action |
|-------------|----------|--------|
| **Navigation** | "go to home", "show cart", "open orders" | Navigates to specified page |
| **Filter** | "show me pizzas", "show burgers", "display main course" | Filters items by category |
| **Order** | "add one pizza", "add three burgers", "order two biryani" | Adds items to cart |
| **Login** | "login", "sign in" | Initiates voice login flow |
| **Logout** | "logout", "sign out" | Logs out current user |
| **Checkout** | "go to checkout", "proceed to payment" | Opens payment modal |

## 🚀 How It Works

### 1. **Activation**
- Click the 🎤 microphone button floating at the bottom-right
- Voice panel opens with "Listening..." indicator

### 2. **Speaking Commands**
- Speak naturally (e.g., "show me pizzas")
- Pause for 1.5 seconds to process
- Assistant responds verbally and executes action

### 3. **Login Flow**
- Say "login"
- Assistant asks for email
- Speak your email
- Assistant asks for password
- Speak your password
- Confirmation of successful login

### 4. **Ordering Flow**
- Say "add two pepperoni pizza"
- Items added to cart immediately
- Verbal confirmation
- Cart updates in real-time

## 🛠️ Technical Implementation

### Core Components

```javascript
// Key features implemented
- SpeechRecognition for voice input
- SpeechSynthesis for voice output
- Context API for state management
- Backend API integration
- Real-time UI updates
```

### Processing Logic

1. **Transcript Collection** - Captures user speech
2. **Pause Detection** - 1.5s silence triggers processing
3. **Command Parsing** - Sends to backend AI for interpretation
4. **Action Execution** - Performs navigation, filter, or order
5. **Voice Feedback** - Speaks confirmation to user

### Supported Pages
- `/` - Home page
- `/about` - About page
- `/login` - Login page
- `/cart` - Cart page
- `/cart#payment-modal` - Checkout with payment
- `/orders` - Orders history
- `/#items` - Menu items section

## 📦 Dependencies

```json
{
  "react-speech-recognition": "^3.10.0",
  "react-router-dom": "^6.x"
}
```

## 🔧 Configuration

The voice assistant requires:
- Browser support for Web Speech API
- Backend endpoint at `http://localhost:3000/voice`
- Groq API key for AI processing
- MySQL database for user and order data

## 🎨 UI Features

- **Wave Animation** - Visual feedback when listening
- **Speaking Indicator** - Shows when assistant is responding
- **Command History** - Prevents duplicate processing
- **Smooth Animations** - Panel slide-in/out effects
- **Responsive Design** - Works on all device sizes

## ⚡ Performance Optimizations

- Debounced transcript processing (1.5s delay)
- Processed commands tracking to avoid repeats
- Efficient state management via Context
- Real-time cart updates with intervals

## 🐛 Troubleshooting

**No voice response**
- Check browser speech synthesis support
- Ensure microphone permissions are granted
- Verify audio output devices

**Commands not recognized**
- Speak clearly with natural pauses
- Check internet connection for API calls
- Verify backend is running

**Login issues**
- Ensure correct email format
- Password is case-sensitive
- Check network connectivity

## 📝 Example Usage

```javascript
// User says: "show me pizzas"
// Assistant: "Showing you all pizzas"
// UI: Filters to show only pizza items

// User says: "add three pepperoni pizza"
// Assistant: "Added 3 Pepperoni Pizza to cart"
// UI: Cart updates with 3 Pepperoni Pizza

// User says: "go to checkout"
// Assistant: "Taking you to checkout"
// UI: Navigates to /cart#payment-modal
```

## 🔒 Security Notes

- Passwords are handled securely via backend
- Session management for non-logged-in users
- Cart persistence across sessions
- Secure API endpoints

## 🚀 Future Enhancements

- Multi-language support
- Custom voice commands
- Order tracking via voice
- Voice-based payment confirmation
- Personalized recommendations

---

*Built with ❤️ for EchoEats - Voice-Based Food Ordering System
# Outputs
1[mainpage.png]<img width="1907" height="1014" alt="main page" src="https://github.com/user-attachments/assets/4c6a9cb9-012c-4561-8ea2-4c3d0e1fd2db" />
2[menupage.png]<img width="1865" height="1010" alt="menu" src="https://github.com/user-attachments/assets/bdbd61e7-fc38-49d3-b7ec-3db332b5585a" />
3[cartpage.png]<img width="1864" height="991" alt="cart" src="https://github.com/user-attachments/assets/dca8837d-6f5e-431d-b125-56dcd4f25327" />
4[orderpage.png]<img width="1870" height="969" alt="order page" src="https://github.com/user-attachments/assets/2e830fd8-ce97-4791-8d9b-351000aeda58" />
5[aboutpage.png]<img width="1872" height="1012" alt="about" src="https://github.com/user-attachments/assets/39f9b2ef-a7c9-40c5-a5b7-2affdd870adc" />




