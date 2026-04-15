# Smart-Trolley
The Smart Trolley System is an IoT-based retail automation project designed to simplify shopping by eliminating manual billing queues. It uses an ESP32, RFID (RC522), and dual IR sensors to automatically detect, identify, and bill items in real-time.

This system simulates modern automated stores like Amazon Go, where products are tracked seamlessly without manual scanning. 
Features
🔄 Automatic item add/remove detection using dual IR sensors
📡 RFID-based product identification
💰 Real-time billing and total calculation
🖥️ 16x2 I2C LCD for live display
🔔 Buzzer feedback for user interaction
🟢🔴 LED indicators for success and error states
⚡ Fast and efficient ESP32-based processing

Working Principle
The system works using IR sensor sequencing + RFID validation:

➕ Adding Item
IR1 detects object → IR2 detects object
System enters Add Mode
User taps RFID tag
Item name & price displayed
Total bill updated
➖ Removing Item
IR2 detects object → IR1 detects object
System enters Remove Mode
RFID scanned
Item removed from total
⚠️ Error Handling
If RFID is not scanned within 5 seconds → UNKNOWN OBJECT

Installation & Setup

Install Arduino IDE
Install required libraries:
MFRC522
LiquidCrystal_I2C
Select Board: ESP32 Dev Module
Upload the code

Challenges Faced

RFID UID formatting mismatch
ESP32 pin compatibility issues
IR sensor noise & false triggering
Library compatibility errors
Connect hardware as per pin configuration

Future Scope

📱 Mobile App Integration
☁️ Cloud-based billing system
💳 Online payment gateway
⚖️ Weight sensor (HX711) integration
📊 Data analytics for shopping behavior

License

This project is open-source and available under the MIT License.

Author

Shrishailya Jangam
Electronics & Computer Engineering Student

Output Images 

<img width="900" height="1600" alt="IMG-20251120-WA0017 jpg" src="https://github.com/user-attachments/assets/f59c1381-805d-46ad-a847-33be1fc88008" />

