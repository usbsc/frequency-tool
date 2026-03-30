# Frequency Tool - Real-Time Audio Analyzer

A self-contained, browser-based frequency analyzer that captures real-time audio from your microphone and displays it with multiple interactive visualizations.

## 🎯 Features

### Visualizations
- **Frequency Spectrum (FFT)**: Real-time frequency bars showing which frequencies are present in your audio
- **Waveform Display**: Oscilloscope-style time-domain view of the audio signal
- **Power Level Gauge**: Interactive meter showing current signal strength
- **Waterfall Display**: Time-frequency heatmap showing how frequencies evolve over time

### Interactive Controls
- **Start/Stop Buttons**: Enable/disable microphone input
- **Frequency Range**: Zoom in on specific frequency ranges (0-20 kHz)
- **FFT Size**: Adjust frequency resolution (256-2048 bins)
- **Smoothing Control**: Fine-tune the visualization smoothing (0-0.99)
- **Real-Time Stats**: Peak frequency, power levels, and sample rate

## 🚀 Getting Started

1. **Open the analyzer**: Open `index.html` in any modern web browser
2. **Grant microphone access**: Your browser will request permission to access your microphone
3. **Click "Start"**: Begin analyzing your audio in real-time
4. **Explore the controls**: Adjust frequency range, FFT size, and smoothing

No installation, dependencies, or build tools required!

## 💻 Browser Compatibility

- ✅ Chrome/Chromium (recommended)
- ✅ Firefox
- ✅ Edge
- ✅ Safari (iOS 14.5+)

Requires:
- ES6 JavaScript support
- Web Audio API
- Canvas 2D API

## 🎨 Design

- Modern dark theme with cyan/blue gradients
- Responsive layout (works on desktop, tablet, mobile)
- Smooth 60fps canvas rendering
- Professional UI with status indicators and real-time statistics

## 🔧 Technical Details

Built with vanilla JavaScript using:
- **Web Audio API**: Microphone capture and FFT analysis via `AnalyserNode`
- **Canvas 2D**: High-performance rendering for visualizations
- **No external dependencies**: Single HTML file with embedded CSS and JavaScript

### Key Components
- `AnalyserNode.getByteFrequencyData()`: FFT frequency bins
- `AnalyserNode.getByteTimeDomainData()`: Waveform samples
- Canvas-based rendering: Spectrum bars, waveform line, waterfall heatmap
- Real-time statistics: Peak frequency detection, power level calculation

## 📊 Use Cases

- **Audio Analysis**: See the frequency content of music, voices, or instruments
- **Sound Design**: Visualize audio while adjusting EQ or effects
- **Educational**: Learn about frequency, FFT, and signal processing
- **Debugging**: Identify unwanted frequencies or noise in your audio

## 🎧 Tips

1. Use headphones or speakers in a quiet environment for best results
2. Start with a lower frequency range (0-2000 Hz) to see clear peaks
3. Adjust smoothing based on your preference (higher = smoother but slower response)
4. Watch the waterfall display to see frequency changes over time

## 📝 Example Scenarios

- **Music**: Open a song on another app and watch the spectrum dance
- **Speech**: Speak into your microphone and see formants and harmonics
- **Noise**: Identify specific noise frequencies that might be problematic
- **Instruments**: Play an instrument and analyze its frequency content

## 🔗 Related Resources

- [Web Audio API Documentation](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [FFT and Frequency Analysis](https://en.wikipedia.org/wiki/Fast_Fourier_transform)
- [Canvas 2D API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)

## 📄 License

Public domain - Feel free to use, modify, and share!

---

**Frequency Tool v1.0** — Real-Time Audio Analysis Tool | Created with Web Audio API
