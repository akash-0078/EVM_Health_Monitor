# Sleep, Stress, and Pulse Monitoring Using Eulerian Video Magnification (EVM)

## **Overview**
This project addresses the need for non-contact, affordable health monitoring solutions, enabling real-time detection of sleep patterns, stress levels, and pulse rates using a webcam or pre-recorded video. The system leverages Eulerian Video Magnification (EVM) and signal processing techniques to amplify subtle physiological changes.

---

## **Key Features**
- **Sleep Monitoring**: Tracks breathing patterns without wearable devices.
- **Stress Detection**: Identifies irregular breathing and heart rate variability.
- **Pulse Monitoring**: Extracts pulse signals using subtle color variations in the hand or face.

---

## **Implementation**
1. **Input Source**: Webcam or video file for real-time analysis.
2. **Frame Preprocessing**:
   - Convert frames to grayscale for intensity-based signal extraction.
   - Detect Region of Interest (ROI) for face or hand.
3. **Signal Processing**:
   - Extract breathing and pulse signals from detected ROI.
   - Apply Butterworth bandpass filter for noise reduction.
4. **Visualization**:
   - Display breathing and pulse signals in real-time.
   - Provide stress/relaxation notifications based on thresholds.

---

## **Results**
- **Breathing Rate**: 16-24 BPM (Normal to Stressed Range).
- **Pulse Rate**: 68-110 BPM (Relaxed to Anxious States).
- **Stress Levels**:
  - Relaxed: Breathing Rate: 12-18 BPM, Pulse Rate: 60-90 BPM.
  - Stressed: Breathing Rate: >20 BPM, Pulse Rate: >100 BPM.

---

## **Tech Stack**
- **Programming Language**: Python
- **Libraries/Tools**: OpenCV, NumPy, Matplotlib, Butterworth Filtering
- **Signal Processing Method**: Eulerian Video Magnification (EVM)

---

## **Future Improvements**
- Enhance signal accuracy with advanced filters and precise ROI tracking.
- Introduce GPU acceleration for real-time processing.
- Adapt to dynamic environments (lighting and motion).
- Explore AI integration for multi-person monitoring and emotion analysis.
