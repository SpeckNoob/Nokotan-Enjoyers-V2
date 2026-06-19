Mustangs Mimic
====

<p align="center">
  <img src="files/Header NewMustang (3).gif" alt="Demo animation">
</p>


This repository contains the documentation for the Mustangs Mimic team's robot for the 2026 World Robot Olympiad Future Engineers category competition. The robot was designed and built by a team of three.

Table of contents
----

- [The Team](#the-team)
- [The Competition](#the-competition)
- [Photos of the robot](#photos-of-the-robot)
  - [Video](#video)
- [Motors, sensors and systems](#motors-sensors-and-systems)
  - [Movement](#movement)
- [Steering](#steering)
  - [Servo Motor](#servo-motor)
- [Motherboard](#motherboard)
- [Skeleton/Chassis](#skeleton/chassis)
- [Energy Management](#energy-management)
  - [Battery](#battery)
- [Sensors](#sensors)
  - [Ultrasonic Sensor](#Ultrasonic-Sensor)
  - [Gyroscope](#gyroscope)
- [Circuit Diagram](#circuit-diagram)
- [Program and Source Code](#program-and-source-code)
  - [Drive](#drive)
  - [Open Round](#open-round)
  - [Obstacle Round](#obstacle-round)
  - [Camera](#camera)

    
## The Team
----

Mark Chen, Age: 17

![image](https://github.com/user-attachments/assets/263bca30-1d4f-4f59-a675-890829c32520)

School: Panamerican School of Panama, PAS

Hi!, I'm Mark from Panama with Chinese origin born in February 8 2009. I've been participating in WRO since 2022 and this is my second year participating in the Future Engineers category. I enjoy playing piano and I am a part of a school band, other hobbies include cubing (Rubik's cube competitions), gaming, drawing and volleyball.

----

Juan Pablo Gomez, Age: 17

![image](https://github.com/user-attachments/assets/b9244ac9-54e1-4af8-89d1-042ac478571a)

School: Panamerican School of Panama, PAS

Hi, I'm Juan Pablo, from Colombia. I love robotics. I've been working with robots since I was 8 years old. My main hobbies are playing bass, hanging out with friends, playing video games, driving karts, and participating in various sports such as football and volleyball.

----

Julio Chong, Age: 17

![image](https://github.com/user-attachments/assets/39dfb391-f71d-4759-b822-fce67cd3f061)

School: Panamerican School of Panama, PAS

My name is Julio Chong, a panamenian teen with chinese antescedents who was born in August 24, 2008. I've been into robotics since 9th grade on 2023. My hobbies are playing the guitar, cooking, coding, learning new languages and also doing lots of exercise or sport, especially contact sports such as jiujitsu.

----

Ivan Guerrero (Coach), Age: 27


School: Panamerican School of Panama, PAS



----

Team photo
----

<img width="1600" height="1066" alt="image" src="https://github.com/user-attachments/assets/d38d130a-00b1-46c9-9a84-978d18311a11" />

[Back to table of contents](#table-of-contents)

The competition
----

Unlike the structured missions of other WRO categories, Future Engineers presents a broad problem (often related to autonomous vehicles, smart systems, or complex automation), and teams must engineer a full solution. Teams work within defined technical limits (size, cost, sensors, etc.) that mimic real-life engineering conditions. This challenge has two main tasks, the first round which tests the robot's progamming of being able to drive many laps without crashing. The second round adds obstacles that the robot must avoid crashing into and a parking space where the robot should finish.

This challenge emphasizes all aspects of the engineering process, including:

- Mobility: Developing efficient vehicle movement.

- Obstacle managing: Detecting and dodging the different obstacles (Green and Red blocks) with effiency.

- Documentation: Showcasing engineering progress, design planning, and collaboration though a GitHub repository.

Points are awarded based on the performance of the robot. In the first round, points are awarded if the robot does not crash or stop during the round. In the second round, points are awarded for every obstacle the robot is able to detect and avoid, bonus points are rewarded if the robot can succesfully finish in the designated parking space.

[Back to table of contents](#table-of-contents)

## Photos of the robot
----

| Top | Bottom |
|--------|---------|
| Insert Image | Insert Image |

| Left | Right |
|--------|---------|
| Insert Image  | Insert Image  |

| Front | Back |
|--------|---------|
| Insert Image  | Insert Image  |


## Video
---

Video of the robot on Youtube: [Video](INSERT LINK)

[Back to table of contents](#table-of-contents)

## Motors, sensors and systems
----

The robot operates with multiple motors and sensors which will be showcased here.

## Movement
----
The robot uses motors for drving and steering, these components work together to ensure the robot has a smooth and efficient movement.

<img width="2000" height="2000" alt="image" src="https://github.com/user-attachments/assets/01dc2d8e-d34d-4b76-b05e-223f4daa5682" />


|  Voltage |   Rated Current   |   Stall Current    |    Total Length    |  Gearbox Size  |  Weight  |
|----------|-----------------|------------------|--------------|------------------|-----------------|
|  6V~12V |   0.04 A   |        0.67 A       |   34mm   | 15mm x 12mm x 10mm (LxWxH)|  10g  |

The GA12-N20 motor is a solid option for robots because it offers an excellent balance of compact size, torque, efficiency, and affordability. Its built-in gearbox allows the small motor to produce enough force to move robots much heavier than its size would suggest.

|  RPM |  Torque MAX (Kg.mm) |  Torque STALLED (Kg.mm) |
|----------|------------|----------|
|    6V@100     |    3.4      |   17    |
|    12V@200      |         |       |
|    6V@200     |    1.9     |   9.4   |
|    12V@400      |         |       |
|    6V@450     |    1.2     |   5.4    |
|    12V@900      |         |       |


The motor works by converting electrical energy into mechanical energy, specifically rotational motion, through the interaction of magnetic fields. It uses the principle that a current-carrying conductor experiences a force within a magnetic field. This force causes a rotor to spin, which then drives a shaft, producing mechanical work. This is then connected to the wheels with two jammed axles.

To connect the motor to the skeleton, we made an opening in the skeleton to fit the motor inside, then we held it up with a 3D printed piece directly attached to the car with screws.


<img width="592" height="346" alt="image" src="https://github.com/user-attachments/assets/2fe7c915-60aa-48d5-8ed1-5410b5651c7b" />

(Full model is in the "models" repository)

## Steering
----
We experimented with many steering mechanisms but the one we found most success was a belt and gear system. Last year we tried an Anti-Ackerman system which worked but not with the model we made. This year we desided to use a simpler belt and gear design that fit our car the best, although it's not as efficient as other systems like the Ackerman, this one still provides great steering angle and consistency.

![image](https://github.com/user-attachments/assets/c8e9e390-33da-499f-b02f-5bd69cfb3fcb)

## Servo motor:
----

<img width="1080" height="1040" alt="image" src="https://github.com/user-attachments/assets/742dd6ce-9630-4559-8d18-8a8d21dbb712" />

|  Weight |   13.4g   |
| -------- |   --------  |
|  Voltage |   4.8 V - 6.0 V   |
|  Dimension |   22.5 x 12 x 35.5 mm   |
|  Stall Torque (4.8V) |   1.8 kgf·cm   |
|  Stall Torque (6V) |   2.2 kgf·cm   |
|  Speed (4.8V) |   0.1s/60 degree   |
|  Speed (6V) |   0.08s/60 degree   |
|  Dead Band |   5µs  |


The MG90S micro servo motor is a good choice for robots because it provides accurate and reliable position control in a compact, lightweight package. Its metal gears make it stronger and more durable than many other micro servos, allowing it to handle repeated movement and moderate loads without wearing out quickly.

<img width="698" height="343" alt="image" src="https://github.com/user-attachments/assets/6ee0966f-861a-400f-babe-f5133c9d5492" />

The motor is placed on the top with the gear that moves the belt.

## Motherboard
----

![image](https://github.com/user-attachments/assets/badc365a-1382-4089-88d6-2129cc35cae7)

|     Chip     |   Clock   |   ROM   |  SRAM  |  FLASH  |        Interfaces        |  Input voltages  |
|--------------|-----------|---------|--------|---------|--------------------------|------------------|
| ESP-WROOM-32 |   240MHz  |  448KB  |  520KB |   4MB   |  UART , I2C , SPI , CAN  |      6-18V       |

For motor driver, we chose the Acebott ESP32, it's capable of controling not only the motors but the sensors as well. It acts like a bridge between a microcontroller and motors, allowing us to safely control higher voltages and currents than the microcontroller can handle directly

## Skeleton/Chassis
----

This year, instead of making the chassis out of lego, we changed it to 3D printed since it allowed it to be less bulky and lighter unlike the lego version. It also allowed for more complex designs such as in the steering and motor placements, these modifications although harder to add to the robot, it immensely helped the functionality and efficiency of the robot. The model was first made in Tinkercad and later passed to Blender for final touches and took around 2 hours.

![image](https://github.com/user-attachments/assets/9f6c9e10-1ba4-45d7-8874-0108a5bd213f)

We had an accident not long before the competition and the piece that holds the camera broke, so we had to design a new piece that not only was more ressistant but also that gave the camera a better view, the piece was placed at the back of the robot and more elevated than the previous design.

<img width="633" height="346" alt="image" src="https://github.com/user-attachments/assets/eed2861c-0f6b-46a6-b16d-3fc941c07ab7" />

## Energy management
----
## Battery:
----

We chose these batteries because they were small and easy to fit on the robot and they had good runtime compared to the lego spike brain. They also deliver higher electric outputs that could power the new motors we chose.

![image](https://github.com/user-attachments/assets/71818d84-c5d1-4629-8518-718c7c04b7c8)

Model 18605

3.7 V

## Sensors
----

For the robot we used the OpenMV Cam RT62 which allowed the robot to detect walls and the colored blocks more easily. It's a small, low power, microcontroller board which allows you to easily implement applications using machine vision in the real-world. It is a huge improvement from last year's robot since we didn't have access to these type of sensors/camera. A camera gives a robot far more versatility than standard sensors, since it can capture detailed visual information to recognize objects, colors, and surroundings, while single-purpose sensors like ultrasonic or touch only provide narrow data such as distance, contact, or light levels.

![image](https://github.com/user-attachments/assets/b646f95c-ab16-4efc-8822-66b5377803ac)

Dimentions:

-Length: 45 mm

-Width: 36 mm

-Height: 29 mm

|  Microcontroler |   Flash memory   |  RAM   |    Frequency    |  Resolution  |  FPS  | Weight |
|-----------|------------|----------------|--------------|------------------|-------|-------|
|  ISSI2232  |   32MB   |      512KB       |   600 MHz   |    2592 x 1944    |  40  | 20g |

## Ultrasonic Sensor
----
This year`s robot we changed from laser based distance sensor to the HC-SR04 ultrasonic sensor , this is because last year we  noticed that the black walls around the circuit were absorbing the laser, thus making very difficult to have precise information. This time we used 6 ultrasonic sensors to support our camera:s vision and prevent any minute detail, for example an insufficient turning angle, that could encounter our robot wich it could lead to it crash onto an obstacle. The position goes by: 1 on each side, 1 looking at angle of 45 degrees, 1 looking at angle of 135 degrees and finally 2 on the front of the car.

Dimensions:

Echo Output Signal Input TTL lever signal and the range in proportion

Lenght: 45mm

Width: 20mm 

Height: 15mm

|  Working Voltage |   Working Current   |  Working Frequency   |    Range    |  Measuring Angle  |  Trigger Input Signal  |
|-----------|------------|----------------|--------------|------------------|-------|-------|
|  DC 5V  |   15mA   |       40Hz      |   2cm-4m   |    15 degree    |  10µS TTL pulse  |

[Back to table of contents](#table-of-contents)

## Gyroscope
----

This year`s robot we decided on using the GY-521 MPU-6050 to help the robot mantain an striaght position throught the circuit. THe MPU-6050 also help us measure the orientation and turns to let know our robot how much it have ben turning, for example measuring the real amount of turn and stop it when it reaches to 90 degrees.

Gyroscope Features


• Digital-output X-, Y-, and Z-Axis angular rate sensors (gyroscopes) with a
user-programmable full-scale range of ±250, ±500, ±1000, and ±2000°/sec
• External sync signal connected to the FSYNC pin supports image, video
and GPS synchronization
• Integrated 16-bit ADCs enable simultaneous sampling of gyros
• Enhanced bias and sensitivity temperature stability reduces the need for
user calibration
• Improved low-frequency noise performance
• Digitally-programmable low-pass filter
• Gyroscope operating current: 3.6mA
• Standby current: 5μA
• Factory calibrated sensitivity scale factor
• User self-test


Accelerometer Features

The triple-axis MEMS accelerometer in MPU-60X0 includes a wide range of
features:
• Digital-output triple-axis accelerometer with a programmable full scale
range of ±2g, ±4g, ±8g and ±16g
• Integrated 16-bit ADCs enable simultaneous sampling of accelerometers
while requiring no external multiplexer
• Accelerometer normal operating current: 500μA
• Low power accelerometer mode current: 10μA at 1.25Hz, 20μA at 5Hz,
60μA at 20Hz, 110μA at 40Hz
• Orientation detection and signaling
• Tap detection
• User-programmable interrupts
• High-G interrupt
• User self-test

Specs: 

Lenght: 34mm 

Widht: 16mm

Height: 10mm

|  Working Voltage |   Working Current   |  Operating temperature range  |    Communication interface    |  G-Force tolerance  |  ADC Internal converter  |
|-----------|------------|----------------|--------------|------------------|-------|-------|
|  Operating input voltage |   4mA ( max.)   |       -40 to +105℃      |    I2C   |   10,000g (up to 0.2ms)   |  16bit (high precision)  |

[Back to table of contents](#table-of-contents)

## Circuit diagram
----

![electric diagram WRO (1)](https://github.com/user-attachments/assets/a96c6d7c-2828-4230-81ea-050892f3166e)


Pins used:

![electric diagram WRO (2)](https://github.com/user-attachments/assets/95201ec8-1249-4721-9a51-392f6b8be53a)

[Back to table of contents](#table-of-contents)

## Program and source code
----

For programing the robot, we used both Python and Arduino coding languages. Python because the program for the camera required Python usage and it allowed us to have more precise movements, Pyhton is easy to learn, highly versatile, and widely supported: its simple, readable syntax lowers the entry barrier for beginners, yet it’s powerful enough for professionals to use in fields like AI, data science, web development, robotics, and automation. We used Arduino because we wanted to use a ESP32 motor driver which was more viable and more precise than other models. Arduino is good for programming because it’s simple, beginner-friendly, and lets you quickly control hardware like sensors and motors to build real-world projects.

Code for each component
----

Drive
----

For driving, the code works by constantly making the car move forward and stopping once all three laps of the track are completed.

```python

void MoveForward() {
  digitalWrite(EN_PIN, LOW);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Forward);
  digitalWrite(STCP_PIN, HIGH);
  digitalWrite(PWM1_PIN, HIGH);  // Encender PWM a tope
}

void StopMotor() {
  digitalWrite(PWM1_PIN, LOW);  // Apagar PWM
}
```
Additionaly, a part of the code specifies the maximum amount of time that the code can run.

```python

// Control de tiempo
#define TIEMPO_LIMITE_MS 67000  // 1 minuto, 7 segundos
unsigned long tiempoInicio;
bool detenido = false;
```

Servo motor
----

The servo motor is supported by the distance sensors in both right and left sides of the robot, the servo moves accordingly wether the sensors detect a wall on the left or right, additionaly, at the end it stops for a certain amount of time so the robot does not perform more than 3 laps.

```python

  // Servo
  miServo.setPeriodHertz(50);
  miServo.attach(SERVO_PIN, 500, 2400);
  miServo.write(SERVO_CENTER);

  // Sensor izquierdo
  selectOnlyOneMux(MUX_LEFT_ADDR);
  sensorLeft.setTimeout(500);
  if (!sensorLeft.init()) {
    Serial.println("Error: sensor izquierdo no detectado.");
    while (1);
  }
  sensorLeft.setDistanceMode(VL53L1X::Long);
  sensorLeft.setMeasurementTimingBudget(20000);
  sensorLeft.startContinuous(20);

  // Sensor derecho
  selectOnlyOneMux(MUX_RIGHT_ADDR);
  sensorRight.setTimeout(500);
  if (!sensorRight.init()) {
    Serial.println("Error: sensor derecho no detectado.");
    while (1);
  }
  sensorRight.setDistanceMode(VL53L1X::Long);
  sensorRight.setMeasurementTimingBudget(50000);
  sensorRight.startContinuous(50);

  Serial.println("Sistema listo.");

  // Tiempo inicial
  tiempoInicio = millis();
}

void loop() {
  // Verificar si se superó el tiempo límite
  if (!detenido && millis() - tiempoInicio >= TIEMPO_LIMITE_MS) {
    Serial.println("Tiempo límite alcanzado. Deteniendo todo.");
    StopMotor();
    miServo.write(SERVO_CENTER);

```

The sensors detect the distance from the wall to the robot and responds accordingly, the servo motor will activate if the robot is 80cm or closer to the wall.

```python

  // Leer sensor izquierdo
  selectOnlyOneMux(MUX_LEFT_ADDR);
  int distLeft = sensorLeft.read();
  if (sensorLeft.timeoutOccurred()) {
    Serial.println("Timeout sensor izquierdo");
    distLeft = 0;
  }

  // Leer sensor derecho
  selectOnlyOneMux(MUX_RIGHT_ADDR);
  int distRight = sensorRight.read();
  if (sensorRight.timeoutOccurred()) {
    Serial.println("Timeout sensor derecho");
    distRight = 0;
  }

  Serial.print("Izquierdo: "); Serial.print(distLeft);
  Serial.print(" mm | Derecho: "); Serial.println(distRight);

  // Reacción del servo con prioridad
  if (distLeft > OBSTACLE_THRESHOLD) {
    Serial.println("Distancia izquierda > 80 cm → girar a la izquierda");

  StopMotor();  // Prioriza el servo
    delay(100);
    miServo.write(SERVO_LEFT);
    delay(2800);
    miServo.write(SERVO_CENTER);
    delay(200);
    MoveForward();  // Reanuda motor
  } 
  else if (distRight > OBSTACLE_THRESHOLD) {
    Serial.println("Distancia derecha > 80 cm → girar a la derecha");

```

## Open Round
----

At the start of the round and after every turn, the robot ignores any readings that are one meter or further for two seconds. The sensor has to read a distance of more than 1.2 meters to make a turn, if the sensor on the left detects a distance of more than 1.2 meters, the robot will turn left. After three laps the robot will stop in the same spot that it started, at the start of the round the robot is given a number value of 0 and it increases by 1 every time it makes a lap, after 12 laps (sections) the robot will stop at the position that the value of 0 was given. By using this method, the robot is more stable when it comes to making the turns and also avoids getting too close to the walls.

```python

Ronda abierta
#include <Wire.h>
#include <VL53L1X.h>
#include <ESP32Servo.h>
#include "Arduino.h"

// Multiplexores
#define MUX_LEFT_ADDR  0x70
#define MUX_RIGHT_ADDR 0x74
#define MUX_CHANNEL_0  0

// Sensores
VL53L1X sensorLeft;
VL53L1X sensorRight;

// Servo Steam
#define SERVO_PIN 25
#define SERVO_LEFT     15
#define SERVO_CENTER   37
#define SERVO_RIGHT    55
Servo miServo;

// Motor control con shift register
#define SHCP_PIN 18
#define EN_PIN   16
#define DATA_PIN 5
#define STCP_PIN 17
#define PWM1_PIN 19
int M1_Forward = 128;

// Umbral: 1000 mm
#define OBSTACLE_THRESHOLD 1000

int contadorGiros = 0;
bool detenido = false;
unsigned long tiempoInicioRecta = 0;

void selectOnlyOneMux(uint8_t muxAddr) {
  Wire.beginTransmission(MUX_LEFT_ADDR); Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(MUX_RIGHT_ADDR); Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(muxAddr); Wire.write(1 << MUX_CHANNEL_0); Wire.endTransmission();
  delay(2);
}

void MoveForward() {
  digitalWrite(EN_PIN, LOW);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Forward);
  digitalWrite(STCP_PIN, HIGH);
  digitalWrite(PWM1_PIN, HIGH);
}

void StopMotor() {
  digitalWrite(PWM1_PIN, LOW);
}

int lecturaFiltrada(VL53L1X &sensor, uint8_t muxAddr, unsigned long referencia) {
  selectOnlyOneMux(muxAddr);
  int lectura = sensor.read();
  if (lectura <= 0) return 0;
  if ((millis() - referencia < 1800) && lectura > OBSTACLE_THRESHOLD) return 0;
  return lectura;
}

void setup() {
  Serial.begin(115200);
  Wire.begin();

  // Pines motor
  pinMode(SHCP_PIN, OUTPUT);
  pinMode(EN_PIN, OUTPUT);
  pinMode(DATA_PIN, OUTPUT);
  pinMode(STCP_PIN, OUTPUT);
  pinMode(PWM1_PIN, OUTPUT);

  // Servo
  miServo.setPeriodHertz(50);
  miServo.attach(SERVO_PIN, 500, 2400);
  miServo.write(SERVO_CENTER);

  // Sensor izquierdo
  selectOnlyOneMux(MUX_LEFT_ADDR);
  sensorLeft.setTimeout(250);
  sensorLeft.init();
  sensorLeft.setDistanceMode(VL53L1X::Long);
  sensorLeft.setMeasurementTimingBudget(33000);
  sensorLeft.startContinuous(33);

  // Sensor derecho
  selectOnlyOneMux(MUX_RIGHT_ADDR);
  sensorRight.setTimeout(250);
  sensorRight.init();
  sensorRight.setDistanceMode(VL53L1X::Long);
  sensorRight.setMeasurementTimingBudget(33000);
  sensorRight.startContinuous(33);

  tiempoInicioRecta = millis();
  Serial.println("Sistema listo.");
}

void loop() {
  if (detenido) return;

  int distLeft = lecturaFiltrada(sensorLeft, MUX_LEFT_ADDR, tiempoInicioRecta);
  int distRight = lecturaFiltrada(sensorRight, MUX_RIGHT_ADDR, tiempoInicioRecta);

  Serial.print("Izquierdo: "); Serial.print(distLeft); Serial.print(" mm | ");
  Serial.print("Derecho: "); Serial.println(distRight);

  bool giroRealizado = false;

  if (distLeft > OBSTACLE_THRESHOLD) {
    Serial.println("→ Gira a la izquierda");
    StopMotor();
    delay(100);
    miServo.write(SERVO_LEFT);
    delay(2800);
    miServo.write(SERVO_CENTER);
    delay(150);
    MoveForward();
    contadorGiros++;
    tiempoInicioRecta = millis();  // Reinicia tiempo de filtro
    giroRealizado = true;
  }

  if (distRight > OBSTACLE_THRESHOLD) {
    Serial.println("→ Gira a la derecha");
    StopMotor();
    delay(100);
    miServo.write(SERVO_RIGHT);
    delay(2800);
    miServo.write(SERVO_CENTER);
    delay(150);
    MoveForward();
    contadorGiros++;
    tiempoInicioRecta = millis();  // Reinicia tiempo de filtro
    giroRealizado = true;
  }

  if (!giroRealizado) {
    MoveForward();
  }

  if (contadorGiros >= 12) {
    Serial.println("✔ 12 giros completados. Avanzando y deteniendo...");
    MoveForward();
    delay(1000);
    StopMotor();
    miServo.write(SERVO_CENTER);
    digitalWrite(STCP_PIN, LOW);
    shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, 0x00);
    digitalWrite(STCP_PIN, HIGH);
    digitalWrite(PWM1_PIN, LOW);
    detenido = true;
  }

  delay(60);  // Lecturas rápidas
}

```

Open round (FINAL)
----

This is the last update to the code before the 2025 national competition in Panama, it is the most refined and updated version of the previous code.

```python

#include <Wire.h>
#include <VL53L1X.h>
#include <ESP32Servo.h>
#include "Arduino.h"

// =================== Parámetros clave ===================
#define ABS_OPEN_MM                 2300   // umbral “lado abierto” hacia ~3 m (ajusta 2100–2700)
#define DELTA_OPEN_MM                600   // apertura relativa vs. línea base del lado fijo (500–800)
#define TURN_MS                     2875   // giro con motor encendido (tu valor)
#define LOOP_DELAY_MS                 10   // bucle rápido
#define ARM_DELAY_MS                 100   // pequeña desensibilización tras cada giro
#define START_IGNORE_MS              800   // ignorar lecturas grandes al iniciar (0.8 s)
#define POST_FIRST_TURN_IGNORE_MS   1600   // ignorar lecturas grandes tras CADA giro (ajustable)
// ========================================================

// Multiplexores
#define MUX_LEFT_ADDR  0x70
#define MUX_RIGHT_ADDR 0x74
#define MUX_CHANNEL_0  0

// Sensores
VL53L1X sensorLeft;
VL53L1X sensorRight;

// Servo
#define SERVO_PIN     25
#define SERVO_LEFT    10
#define SERVO_CENTER  35
#define SERVO_RIGHT   60
Servo miServo;

// Motor con shift register
#define SHCP_PIN 18
#define EN_PIN   16
#define DATA_PIN 5
#define STCP_PIN 17
#define PWM1_PIN 19
int M1_Forward = 128;

// Estado y filtros
int  contadorGiros     = 0;
bool detenido          = false;
enum Dir { NONE=0, LEFT=1, RIGHT=2 };
Dir fixedDir           = NONE;

float emaL=0, emaR=0; bool emaL_ok=false, emaR_ok=false;
unsigned long lastTurnTS    = 0;         // para ARM_DELAY_MS
unsigned long ignoreUntilTS = 0;         // ventana para ignorar lecturas grandes

// ---------- Utilidades ----------
static inline void selectOnlyOneMux(uint8_t muxAddr) {
  Wire.beginTransmission(MUX_LEFT_ADDR);  Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(MUX_RIGHT_ADDR); Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(muxAddr);        Wire.write(1 << MUX_CHANNEL_0); Wire.endTransmission();
  delayMicroseconds(500);
}

static inline void MoveForward() {
  digitalWrite(EN_PIN, LOW);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Forward);
  digitalWrite(STCP_PIN, HIGH);
  digitalWrite(PWM1_PIN, HIGH);  // motor encendido
}

static inline void StopMotor() {
  digitalWrite(PWM1_PIN, LOW);
}

static inline int readVL(VL53L1X &sensor, uint8_t muxAddr) {
  selectOnlyOneMux(muxAddr);
  int d = sensor.read();
  return d > 0 ? d : 0;  // ignora inválidos
}

static inline void updEMA(float &ema, bool &ok, int x) {
  if (x <= 0) return;
  const float a = 0.20f;                 // EMA_ALPHA
  if (!ok) { ema = x; ok = true; }
  else      { ema = a*x + (1.0f - a)*ema; }
}

// ---------- Giros con motor encendido ----------
void girarIzquierda() {
  Serial.println("→ Giro IZQUIERDA (motor encendido)");
  miServo.write(SERVO_LEFT);
  MoveForward();
  delay(TURN_MS);
  miServo.write(SERVO_CENTER);
  delay(80);
  MoveForward();
  contadorGiros++;
  lastTurnTS = millis();
  // Tras CADA giro: activar ventana de ignorar lecturas grandes
  ignoreUntilTS = millis() + POST_FIRST_TURN_IGNORE_MS;
}

void girarDerecha() {
  Serial.println("→ Giro DERECHA (motor encendido)");
  miServo.write(SERVO_RIGHT);
  MoveForward();
  delay(TURN_MS);
  miServo.write(SERVO_CENTER);
  delay(80);
  MoveForward();
  contadorGiros++;
  lastTurnTS = millis();
  // Tras CADA giro: activar ventana de ignorar lecturas grandes
  ignoreUntilTS = millis() + POST_FIRST_TURN_IGNORE_MS;
}

// ---------- Setup ----------
void setup() {
  Serial.begin(115200);
  Wire.begin();

  // Pines motor
  pinMode(SHCP_PIN, OUTPUT);
  pinMode(EN_PIN,  OUTPUT);
  pinMode(DATA_PIN, OUTPUT);
  pinMode(STCP_PIN, OUTPUT);
  pinMode(PWM1_PIN, OUTPUT);

  // Servo
  miServo.setPeriodHertz(50);
  miServo.attach(SERVO_PIN, 500, 2400);
  miServo.write(SERVO_CENTER);

  // ===== Sensores ToF: Long + 25 ms =====
  selectOnlyOneMux(MUX_LEFT_ADDR);
  sensorLeft.setTimeout(250);
  sensorLeft.init();
  sensorLeft.setDistanceMode(VL53L1X::Long);
  sensorLeft.setMeasurementTimingBudget(25000);
  sensorLeft.startContinuous(25);

  selectOnlyOneMux(MUX_RIGHT_ADDR);
  sensorRight.setTimeout(250);
  sensorRight.init();
  sensorRight.setDistanceMode(VL53L1X::Long);
  sensorRight.setMeasurementTimingBudget(25000);
  sensorRight.startContinuous(25);

  // Ventana inicial: ignorar lecturas grandes por 0.8 s
  ignoreUntilTS = millis() + START_IGNORE_MS;

  Serial.println("Listo: dir fija, giro con motor, y ventanas de ignorar tras CADA giro.");
}

// ---------- Loop ----------
void loop() {
  if (detenido) return;

  const unsigned long now = millis();
  const bool ignoringLarge = (now < ignoreUntilTS);               // ventana activa
  const bool armedTime     = (now - lastTurnTS) >= ARM_DELAY_MS;  // pequeño re-armado
  const bool canTurn       = (!ignoringLarge) && armedTime;       // condición global

  int dL = readVL(sensorLeft,  MUX_LEFT_ADDR);
  int dR = readVL(sensorRight, MUX_RIGHT_ADDR);

  // Actualiza líneas base
  updEMA(emaL, emaL_ok, dL);
  updEMA(emaR, emaR_ok, dR);

  // Log útil
  Serial.print("L: "); Serial.print(dL); Serial.print(" (EMA ");
  Serial.print(emaL_ok ? (int)emaL : -1); Serial.print(") | R: ");
  Serial.print(dR); Serial.print(" (EMA ");
  Serial.print(emaR_ok ? (int)emaR : -1); Serial.print(") | IGNORING=");
  Serial.println(ignoringLarge ? "YES" : "NO");

  // Detección (abs/rel) condicionada por canTurn
  bool leftAbs  = canTurn && (dL >= ABS_OPEN_MM);
  bool rightAbs = canTurn && (dR >= ABS_OPEN_MM);
  bool leftRel  = canTurn && (emaL_ok && (dL - emaL) >= DELTA_OPEN_MM);
  bool rightRel = canTurn && (emaR_ok && (dR - emaR) >= DELTA_OPEN_MM);

  // 1) Si aún no hay dirección fija: decide en el primer evento válido
  if (fixedDir == NONE && canTurn) {
    bool L = leftAbs  || leftRel;
    bool R = rightAbs || rightRel;
    if (L || R) {
      if (L && R) fixedDir = (dL >= dR) ? LEFT : RIGHT;
      else        fixedDir =  L ? LEFT : RIGHT;
      Serial.print("Dirección FIJA: "); Serial.println(fixedDir == LEFT ? "IZQUIERDA" : "DERECHA");
      if (fixedDir == LEFT)  girarIzquierda();
      else                   girarDerecha();
      return;
    }
  }
  // 2) Con dirección fija: SOLO miramos ese lado y respetamos la ventana/armado
  else if (canTurn) {
    if (fixedDir == LEFT) {
      if (leftAbs || leftRel) { girarIzquierda(); return; }
    } else { // RIGHT
      if (rightAbs || rightRel) { girarDerecha(); return; }
    }
  }

  // Avanza recto si no se dispara el giro
  MoveForward();

  if (contadorGiros >= 12) {
    Serial.println("✔ 12 giros completados. Avanzando y deteniendo...");
    MoveForward();
    delay(1000);
    StopMotor();
    miServo.write(SERVO_CENTER);
    digitalWrite(STCP_PIN, LOW);
    shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, 0x00);
    digitalWrite(STCP_PIN, HIGH);
    digitalWrite(PWM1_PIN, LOW);
    detenido = true;
  }

  delay(LOOP_DELAY_MS);
}

```

Obstacle round
----

For the obstacle round, the camera was the main component. It is capable of detecting colors and objects from a distance and act accordingly, the distance sensors also play the same role and are still in use for this round. 

The camera detects the green and red blocks and the robot then knows where to turn and when, then it checks the distance sensors to see if it has space or the need to turn, the rest of the code is mostly the same with some slight modifications so the camera could work. 

Video of the robot on Youtube: [Video](https://youtube.com/shorts/kXKS2O0ia2E?feature=share)

```python

void loop() {
  // UART desde cámara: color detectado
  if (Serial1.available() && !enGiroPorColor) {
    String color = Serial1.readStringUntil('\n');
    color.trim();

    if (color == "ROJO") {
      Serial.println("Color ROJO detectado → giro a la derecha");
      ejecutarGiroColor(SERVO_RIGHT, SERVO_LEFT);
    }
    else if (color == "VERDE") {
      Serial.println("Color VERDE detectado → giro a la izquierda");
      ejecutarGiroColor(SERVO_LEFT, SERVO_RIGHT);
    }
  }

  MoveForward();  // Siempre avanza a media velocidad

  // Lectura sensores de distancia
  selectOnlyOneMux(MUX_LEFT_ADDR);
  int distLeft = sensorLeft.read();
  if (sensorLeft.timeoutOccurred()) {
    Serial.println("Timeout sensor izquierdo");
    distLeft = 0;
  }

  selectOnlyOneMux(MUX_RIGHT_ADDR);
  int distRight = sensorRight.read();
  if (sensorRight.timeoutOccurred()) {
    Serial.println("Timeout sensor derecho");
    distRight = 0;
  }

```

(Update) The information that the camera recieves is passed to UART, then the camera only looks for green and red blocks and only detects the color that is closest, that information is then passed to UART

```python

from machine import UART
import sensor, image, time

uart = UART(1, baudrate=115200)

sensor.reset()
sensor.set_pixformat(sensor.RGB565)
sensor.set_framesize(sensor.QQVGA)  # Baja calidad para más FPS
sensor.skip_frames(time=2000)
sensor.set_auto_gain(False)
sensor.set_auto_whitebal(False)

red_threshold = (30, 100, 15, 127, 15, 127)
green_threshold = (30, 100, -127, -15, 15, 127)

ultimo_color = ""
tiempo_ultimo_envio = time.ticks_ms()
intervalo = 10000  # 10 segundos

while True:
    img = sensor.snapshot()

    rojos = img.find_blobs([red_threshold], pixels_threshold=100, area_threshold=100, merge=True)
    verdes = img.find_blobs([green_threshold], pixels_threshold=100, area_threshold=100, merge=True)

    blob_rojo = max(rojos, key=lambda b: b.pixels(), default=None)
    blob_verde = max(verdes, key=lambda b: b.pixels(), default=None)

    color_detectado = ""
    if blob_rojo and not blob_verde:
        color_detectado = "ROJO"
    elif blob_verde and not blob_rojo:
        color_detectado = "VERDE"
    elif blob_rojo and blob_verde:
        if blob_rojo.pixels() > blob_verde.pixels():
            color_detectado = "ROJO"
        else:
            color_detectado = "VERDE"

    if color_detectado:
        tiempo_actual = time.ticks_ms()
        if (color_detectado != ultimo_color) or (time.ticks_diff(tiempo_actual, tiempo_ultimo_envio) > intervalo):
            uart.write(color_detectado + "\n")
            print("Color enviado:", color_detectado)
            ultimo_color = color_detectado
            tiempo_ultimo_envio = tiempo_actual
    else:
        ultimo_color = ""  # Reiniciar si no hay detección

```

This last part is to ensure the robot does not crash into any wall or block after turning or overturning. It also checks with the distance sensors one more time so it does not misalign from the track's path.

```python

  Serial.print("Izquierdo: "); Serial.print(distLeft);
  Serial.print(" mm | Derecho: "); Serial.println(distRight);

  if (!enGiroPorColor) {
    if (distLeft > OBSTACLE_THRESHOLD) {
      Serial.println("Distancia izquierda > 100 cm → giro a la izquierda");
      StopMotor();
      delay(100);
      miServo.write(SERVO_LEFT);
      delay(2800);
      miServo.write(SERVO_CENTER);
      delay(200);
      MoveForward();
    } else if (distRight > OBSTACLE_THRESHOLD) {
      Serial.println("Distancia derecha > 100 cm → giro a la derecha");
      StopMotor();
      delay(100);
      miServo.write(SERVO_RIGHT);
      delay(2800);
      miServo.write(SERVO_CENTER);
      delay(200);
      MoveForward();
    }
  }

  delay(100);
}
```

Obstacle round (FINAL)

This is the last update to the code before the 2025 national competition in Panama, many components of the previous code were changed for the robot to detect and see the colored blocks more accurately (Each section is highlighted).

```python

/****************************************************
 *  ROBOT 3x3 – ESP32 (Motores + Servo + VL53L1X + Cam UART)
 *  - Secuencia de salida y maniobra final
 *  - Lógica de colores HORARIO y ANTIHORARIO (completa)
 *  - Maniobra especial + reintento del mismo índice
 *  - Memoria de vuelta 1 (colores usados) → reproducir vuelta 2 y 3
 ****************************************************/

#include <Wire.h>
#include <VL53L1X.h>
#include <ESP32Servo.h>
#include "Arduino.h"

// =================== Multiplexores / VL53 ===================
#define MUX_LEFT_ADDR   0x70
#define MUX_RIGHT_ADDR  0x74
#define MUX_CHANNEL_0   0
VL53L1X sensorLeft, sensorRight;

// =================== Servo ===================
#define SERVO_PIN        25
#define SERVO_LEFT        5
#define SERVO_CENTER     35   // centro "normal" (luego de terminar en giro a la DER)
#define SERVO_CENTER_L   45   // centro "luego de terminar en giro a la IZQ"
#define SERVO_RIGHT      75
Servo miServo;

// =================== Motor (shift register) ===================
#define SHCP_PIN 18
#define EN_PIN   16
#define DATA_PIN 5
#define STCP_PIN 17
#define PWM1_PIN 19
const int M1_Forward = 128;
const int M1_Reverse = 64;
const int M1_Stop    = 0;

// =================== UART CÁMARA (Serial1: RX=3, TX=1) ===================
#define CAM_BAUD 115200
#define CAM_RX   3
#define CAM_TX   1

// =================== Parámetros (MODULAR) ===================
// Micro-pasos salida
#define PASO_AVANZAR_MS      250
#define PASO_RETRO_MS        230
#define PAUSA_MS             150
#define ESTABILIZA_MS        130

// Maniobra final (giro contrario)
#define FINAL_PRE_AVANCE_MS  300
#define FINAL_AVANZAR_MS     1600
#define FINAL_RETRO1_MS       500
#define FINAL_AVANZAR2_MS     600
#define FINAL_RETRO2_MS      1000

// Timings base de colores
#define GREEN1_LEFT_MS       1400  // 1.4 s (Ajustado a tu última tabla de horario 1.º=VERDE)
#define GREEN1_RIGHT_MS      1400
#define GREEN1_RIGHT2_MS     2800
#define GREEN1_FINAL_RETRO   1000
#define GREEN1_MID_RETRO      500   // retro tras centro en 1.º=VERDE (horario)

#define RED1_RIGHT_MS        1600
#define RED1_LEFT_MS         1600

#define SEG_1S               1000
#define SEG_2S               2000
#define GIRO_LARGO_MS        2800   // 2.8 s (giro largo)

// Avances/generales
#define CONT_TURN_MS         2000   // 2.0 s para tramos simétricos
#define CONT_FORWARD_MS      2000
#define RETRO_CORTO_MS        300
#define RETRO_LARGO_MS       2000

// Timeouts SOLO en ramas que admiten "NINGUNO"
#define WAIT_NO_COLOR_MS    10000

// Salida del estacionamiento (ciclos)
#define NUM_CICLOS_IZQ  9   // izquierda (antiho) – micro-ciclos
#define NUM_CICLOS_DER  6   // derecha  (horario) – micro-ciclos

// =================== Estado global ===================
enum Sentido { HORARIO=0, ANTIHORARIO=1 };
Sentido sentido = HORARIO;  // se fija tras la salida

// Memoria de colores “usados” por la lógica (vuelta 1)
char memColores[9];           // índices 1..8 (‘G’, ‘R’, ‘N’)
bool memoriaLlena = false;

// Control de vueltas
uint8_t vueltaActual = 1;     // 1, 2, 3
bool usarMemoria = false;     // true en vueltas 2 y 3

// =================== Utilidades MUX ===================
void selectOnlyOneMux(uint8_t muxAddr) {
  Wire.beginTransmission(MUX_LEFT_ADDR);  Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(MUX_RIGHT_ADDR); Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(muxAddr);        Wire.write(1 << MUX_CHANNEL_0);  Wire.endTransmission();
  delay(2);
}

// =================== Motores ===================
void MoveMotor(int dir, int speed) {
  if (speed < 0)   speed = 0;
  if (speed > 255) speed = 255;
  digitalWrite(EN_PIN, LOW);
  analogWrite(PWM1_PIN, speed);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, dir);
  digitalWrite(STCP_PIN, HIGH);
}

void MoveForward() {
  digitalWrite(EN_PIN, LOW);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Forward);
  digitalWrite(STCP_PIN, HIGH);
  digitalWrite(PWM1_PIN, HIGH);
}

void StopMotor() {
  analogWrite(PWM1_PIN, 0);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Stop);
  digitalWrite(STCP_PIN, HIGH);
}

void retro(int ms) {
  MoveMotor(M1_Reverse, 128);
  delay(ms);
  StopMotor();
}

// =================== Movimientos compuestos ===================
void avanzarRecto(int ms, int centro) {
  StopMotor();
  miServo.write(centro);
  delay(ESTABILIZA_MS);
  MoveForward();
  delay(ms);
  StopMotor();
}
void avanzarConGiro(int angServo, int ms) {
  StopMotor();
  miServo.write(angServo);
  delay(ESTABILIZA_MS);
  MoveForward();
  delay(ms);
  StopMotor();
}
inline void giroLargoHorario()    { avanzarConGiro(SERVO_RIGHT, GIRO_LARGO_MS); }
inline void giroLargoAntiHorario(){ avanzarConGiro(SERVO_LEFT,  GIRO_LARGO_MS); }

void servoCentroTrasDer() { miServo.write(SERVO_CENTER);   delay(ESTABILIZA_MS); }
void servoCentroTrasIzq() { miServo.write(SERVO_CENTER_L); delay(ESTABILIZA_MS); }

// =================== Cámara ===================
void limpiarBufferCamara() { while (Serial1.available()) Serial1.read(); }

char leerColorBloqueante() {
  limpiarBufferCamara();
  for (;;) {
    if (Serial1.available()) {
      String t = Serial1.readStringUntil('\n');
      t.trim(); t.toLowerCase();
      if (t == "verde") return 'G';
      if (t == "rojo")  return 'R';
    }
    delay(2);
  }
}

char leerColorConTimeout(unsigned long timeout_ms) {
  limpiarBufferCamara();
  unsigned long t0 = millis();
  while (millis() - t0 < timeout_ms) {
    if (Serial1.available()) {
      String t = Serial1.readStringUntil('\n');
      t.trim(); t.toLowerCase();
      if (t == "verde") return 'G';
      if (t == "rojo")  return 'R';
    }
    delay(2);
  }
  return 'N';
}

// Interfaz de lectura para vivo/memoria
char leerColorPaso(uint8_t idx, bool permitirNinguno, unsigned long to_ms) {
  if (usarMemoria) {
    char c = memColores[idx];
    Serial.print("[MEM paso "); Serial.print(idx); Serial.print("] -> ");
    Serial.println(c);
    return c;
  } else {
    char c = permitirNinguno ? leerColorConTimeout(to_ms) : leerColorBloqueante();
    // Guardar en memoria vuelta 1
    if (vueltaActual == 1) memColores[idx] = c;
    return c;
  }
}

// =================== Medición distancia (para salida) ===================
int lecturaSimple(VL53L1X &sensor, uint8_t muxAddr) {
  selectOnlyOneMux(muxAddr);
  int v = sensor.read();
  return (v > 0) ? v : 0;
}
int lecturaPromedio(VL53L1X &sensor, uint8_t muxAddr, uint8_t n=3) {
  long s=0; uint8_t val=0;
  for (uint8_t i=0;i<n;i++) { int x=lecturaSimple(sensor,muxAddr); if (x>0){s+=x;val++;} delay(10); }
  if (!val) return 0;
  return (int)(s/val);
}

// =================== Secuencia de salida (micro-ciclos) ===================
inline void microCiclo(int angLado, int centroAlVolver) {
  avanzarConGiro(angLado, PASO_AVANZAR_MS);
  miServo.write(centroAlVolver);
  delay(ESTABILIZA_MS);
  retro(PASO_RETRO_MS);
  delay(PAUSA_MS);
}
void secuenciaSalidaIzquierda() { // antiho
  for (uint8_t i=0;i<NUM_CICLOS_IZQ;i++) microCiclo(SERVO_LEFT, SERVO_CENTER_L);
}
void secuenciaSalidaDerecha() { // horario
  for (uint8_t i=0;i<NUM_CICLOS_DER;i++) microCiclo(SERVO_RIGHT, SERVO_CENTER);
}

// =================== Maniobra final (giro contrario al lado elegido) ===================
void maniobraFinal(bool eligioIzquierda) {
  // 1) Recto 0.3 s
  avanzarRecto(FINAL_PRE_AVANCE_MS, SERVO_CENTER);

  // 2) Giro contrario 1.6 s
  const bool contrarioEsIzq = !eligioIzquierda;
  const int angContrario = contrarioEsIzq ? SERVO_LEFT : SERVO_RIGHT;
  const int centroSegun = contrarioEsIzq ? SERVO_CENTER_L : SERVO_CENTER;
  avanzarConGiro(angContrario, FINAL_AVANZAR_MS);

  // 3) Centro y retro 0.5 s
  miServo.write(centroSegun); delay(ESTABILIZA_MS);
  retro(FINAL_RETRO1_MS);

  // 4) Mismo giro 0.6 s
  avanzarConGiro(angContrario, FINAL_AVANZAR2_MS);

  // 5) Centro y retro 1.0 s
  miServo.write(centroSegun); delay(ESTABILIZA_MS);
  retro(FINAL_RETRO2_MS);
}

// =================== Maniobras Especiales ===================
// HORARIO: NINGUNO → IZQ 0.5 → DER 0.5 → DER 2.8 → centro → retro 2.0
void maniobraEspecialHorario() {
  // IZQ 0.5
  avanzarConGiro(SERVO_LEFT, 500);
  // DER 0.5
  avanzarConGiro(SERVO_RIGHT, 500);
  // DER 2.8
  giroLargoHorario();
  // centro+retro 2.0
  servoCentroTrasDer();
  retro(RETRO_LARGO_MS);
}
// ANTIHORARIO: NINGUNO → DER 0.5 → IZQ 0.5 → IZQ 2.8 → centro(45) → retro 2.0
void maniobraEspecialAntiHo() {
  // DER 0.5
  avanzarConGiro(SERVO_RIGHT, 500);
  // IZQ 0.5
  avanzarConGiro(SERVO_LEFT, 500);
  // IZQ 2.8
  giroLargoAntiHorario();
  // centro+retro 2.0
  servoCentroTrasIzq();
  retro(RETRO_LARGO_MS);
}

// =================== Núcleo de lógica: HORARIO ===================
void ejecutarHorario() {
  Serial.println("== LÓGICA HORARIO (giro largo DER 2.8 s) ==");

  // ---------- 1.º color ----------
  Serial.println("[1] Esperando color...");
  char c1 = leerColorPaso(1, false, 0);

  if (c1=='G') {
    // VERDE → IZQ 1.4 → DER 1.4 → DER 2.8 → centro → retro 1.0 → leer 2.º
    avanzarConGiro(SERVO_LEFT,  GREEN1_LEFT_MS);
    avanzarConGiro(SERVO_RIGHT, GREEN1_RIGHT_MS);
    giroLargoHorario();
    servoCentroTrasDer();
    retro(GREEN1_FINAL_RETRO);
  } else {
    // ROJO → DER 1.6 → IZQ 1.6 → quieto
    avanzarConGiro(SERVO_RIGHT, RED1_RIGHT_MS);
    avanzarConGiro(SERVO_LEFT,  RED1_LEFT_MS);
    StopMotor();
  }
  limpiarBufferCamara();

  // ---------- 2.º color ----------
  Serial.println("[2] Leyendo 2.º (reglas según 1.º)...");
  char c2;
  if (c1=='G') {
    // sin NINGUNO aquí (bloqueante)
    c2 = leerColorPaso(2, false, 0);
    if (c2=='G') {
      // IZQ 1.6 → DER 1.6 → quieto (servo=35)
      avanzarConGiro(SERVO_LEFT,  1600);
      avanzarConGiro(SERVO_RIGHT, 1600);
      servoCentroTrasDer(); StopMotor();
    } else { // ROJO
      avanzarConGiro(SERVO_RIGHT, 1600);
      avanzarConGiro(SERVO_LEFT,  1600);
      servoCentroTrasIzq(); StopMotor();
    }
  } else {
    // 1.º=ROJO: admite NINGUNO con maniobra especial
    c2 = leerColorPaso(2, true, WAIT_NO_COLOR_MS);
    if (c2=='G') {
      // recto 1.0 → DER 2.8 → quieto
      avanzarRecto(SEG_1S, SERVO_CENTER);
      giroLargoHorario();
      servoCentroTrasDer(); StopMotor();
    } else if (c2=='R') {
      // retro 0.3 → DER 2.8 → quieto
      retro(RETRO_CORTO_MS);
      giroLargoHorario();
      servoCentroTrasDer(); StopMotor();
    } else { // N
      maniobraEspecialHorario();
      limpiarBufferCamara();
      // reintento MISMO índice
      c2 = leerColorPaso(2, true, WAIT_NO_COLOR_MS);
      // vuelve a aplicar la rama (para no duplicar, haremos una mini-llamada recursiva simple)
      if (c2=='G') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoHorario(); servoCentroTrasDer(); StopMotor(); }
      else if (c2=='R'){ retro(RETRO_CORTO_MS); giroLargoHorario(); servoCentroTrasDer(); StopMotor(); }
      else { /* si vuelve N, ya quedó mejor posicionado; continúa */ }
    }
  }
  limpiarBufferCamara();

  // ---------- 3.º color ----------
  Serial.println("[3] Leyendo 3.º (depende de 2.º)...");
  char c3;
  bool permitirN3 = (c2=='G') ? true : true; // en horario, 3.º admite N en ambas ramas (según tu tabla)
  c3 = leerColorPaso(3, permitirN3, WAIT_NO_COLOR_MS);

  if (c2=='G') {
    if (c3=='R') {
      // DER 2.0 → IZQ 2.0 → quieto (servo=45)
      avanzarConGiro(SERVO_RIGHT, CONT_TURN_MS);
      avanzarConGiro(SERVO_LEFT,  CONT_TURN_MS);
      servoCentroTrasIzq(); StopMotor();
    } else { // VERDE o N
      // recto 2.0 → DER 2.8 → centro → retro 1.0
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      giroLargoHorario(); servoCentroTrasDer(); retro(1000);
    }
  } else { // c2=='R'
    if (c3=='G') {
      // IZQ 2.0 → DER 2.0 → recto 1.0 → DER 2.8 → centro → retro 1.0
      avanzarConGiro(SERVO_LEFT, CONT_TURN_MS);
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      avanzarRecto(SEG_1S, SERVO_CENTER);
      giroLargoHorario(); servoCentroTrasDer(); retro(1000);
    } else { // ROJO o N
      // recto 2.0 → quieto
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 4.º color (ramificado por 2.º y 3.º) ----------
  Serial.println("[4] Leyendo 4.º...");
  // Reglas: (2=G,3=G|N), (2=G,3=R), (2=R,3=G), (2=R,3=R|N)
  bool permitirN4 = ((c2=='G' && c3!='R') || (c2=='R' && c3!='G')) ? false : false; // en tu última corrección removiste “Ninguno” en varias; lo dejamos sin N por defecto
  char c4 = leerColorPaso(4, permitirN4, WAIT_NO_COLOR_MS);

  if (c2=='G' && (c3=='G' || c3=='N')) {
    if (c4=='G') { avanzarConGiro(SERVO_LEFT,1600); avanzarConGiro(SERVO_RIGHT,1600); servoCentroTrasDer(); StopMotor(); }
    else         { avanzarConGiro(SERVO_RIGHT,1600); avanzarConGiro(SERVO_LEFT,1600);  servoCentroTrasIzq(); StopMotor(); }
  }
  else if (c2=='G' && c3=='R') {
    if (c4=='G') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoHorario(); servoCentroTrasDer(); retro(1000); StopMotor(); }
    else         { giroLargoHorario(); servoCentroTrasDer(); retro(1000); StopMotor(); }
  }
  else if (c2=='R' && c3=='G') {
    if (c4=='G') { avanzarConGiro(SERVO_LEFT,1600); avanzarConGiro(SERVO_RIGHT,1600); servoCentroTrasDer(); StopMotor(); }
    else         { avanzarConGiro(SERVO_RIGHT,1600); avanzarConGiro(SERVO_LEFT,1600);  servoCentroTrasIzq(); StopMotor(); }
  }
  else { // (c2=='R' && (c3=='R' || c3=='N'))
    if (c4=='G') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoHorario(); servoCentroTrasDer(); retro(1000); StopMotor(); }
    else         { giroLargoHorario(); servoCentroTrasDer(); retro(1000); StopMotor(); }
  }
  limpiarBufferCamara();

  // ---------- 5.º color ----------
  Serial.println("[5] Leyendo 5.º...");
  char c5 = leerColorPaso(5, true, WAIT_NO_COLOR_MS); // aquí sí admitimos N en la rama (4=G) per tabla

  // Si 4.º=G
  if (c4=='G') {
    if (c5=='R') {
      avanzarConGiro(SERVO_RIGHT, CONT_TURN_MS);
      avanzarConGiro(SERVO_LEFT,  CONT_TURN_MS);
      servoCentroTrasIzq(); StopMotor();
    } else { // G o N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      giroLargoHorario(); servoCentroTrasDer(); retro(1000);
    }
  } else { // 4.º=R
    if (c5=='G') {
      avanzarConGiro(SERVO_LEFT, CONT_TURN_MS);
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      avanzarRecto(SEG_1S, SERVO_CENTER);
      giroLargoHorario(); servoCentroTrasDer(); retro(1000);
    } else { // R o N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER); StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 6.º color ----------
  Serial.println("[6] Leyendo 6.º...");
  char c6 = leerColorPaso(6, false, 0); // en 6.º (según tu última versión) no forzamos N salvo cuando 5º=R se añadió N especial, ya se usó en 5.º
  if (c5=='G') {
    if (c6=='G') { avanzarConGiro(SERVO_LEFT,1600); avanzarConGiro(SERVO_RIGHT,1600); servoCentroTrasDer(); StopMotor(); }
    else         { avanzarConGiro(SERVO_RIGHT,1600); avanzarConGiro(SERVO_LEFT,1600);  servoCentroTrasIzq(); StopMotor(); }
  } else { // 5.º=R o N
    if (c6=='G') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoHorario(); servoCentroTrasDer(); retro(1000); StopMotor(); }
    else         { giroLargoHorario(); servoCentroTrasDer(); retro(1000); StopMotor(); }
  }
  limpiarBufferCamara();

  // ---------- 7.º color ----------
  Serial.println("[7] Leyendo 7.º...");
  char c7 = leerColorPaso(7, false, 0);
  if (c6=='G') {
    if (c7=='G') { avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER); giroLargoHorario(); servoCentroTrasDer(); retro(1000); }
    else         { avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS); avanzarConGiro(SERVO_LEFT,CONT_TURN_MS); servoCentroTrasIzq(); StopMotor(); }
  } else {
    if (c7=='G') {
      avanzarConGiro(SERVO_LEFT,CONT_TURN_MS);
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      avanzarRecto(SEG_1S, SERVO_CENTER);
      giroLargoHorario(); servoCentroTrasDer(); retro(1000);
    } else {
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER); StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 8.º color (regla especial horario) ----------
  Serial.println("[8] Leyendo 8.º (regla especial)...");
  char c8 = leerColorPaso(8, false, 0); // no importa el color para el final, pero dejamos lectura por consistencia

  // Regla especial que pediste para HORARIO:
  // Si 7.º = ROJO → (aquí iría maniobra especial) y luego avanza 1 s
  // Si 7.º = VERDE → solo avanza 1 s
  if (c7=='R') {
    maniobraEspecialHorario();
    avanzarRecto(SEG_1S, SERVO_CENTER);
  } else {
    avanzarRecto(SEG_1S, SERVO_CENTER);
  }
  StopMotor();
}

// =================== Núcleo de lógica: ANTIHORARIO ===================
void ejecutarAntiHorario() {
  Serial.println("== LÓGICA ANTIHORARIO (giro largo IZQ 2.8 s) ==");

  // ---------- 1.º color ----------
  Serial.println("[1] Esperando color...");
  char c1 = leerColorPaso(1, false, 0);

  if (c1=='R') {
    // ROJO → DER 1.4 → IZQ 1.4 → IZQ 2.8 → centro(45) → retro 1.0
    avanzarConGiro(SERVO_RIGHT, 1400);
    avanzarConGiro(SERVO_LEFT,  1400);
    giroLargoAntiHorario();
    servoCentroTrasIzq();
    retro(1000);
  } else {
    // VERDE → IZQ 1.6 → DER 1.6 → quieto
    avanzarConGiro(SERVO_LEFT, 1600);
    avanzarConGiro(SERVO_RIGHT,1600);
    StopMotor();
  }
  limpiarBufferCamara();

  // ---------- 2.º color (pauta replicable en 4.º y 6.º) ----------
  Serial.println("[2] Leyendo 2.º (depende de 1.º)...");
  char c2;
  if (c1=='G') {
    // admite N con maniobra especial ANTIHO
    c2 = leerColorPaso(2, true, WAIT_NO_COLOR_MS);
    if (c2=='G') {
      retro(RETRO_CORTO_MS);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    } else if (c2=='R') {
      avanzarRecto(SEG_1S, SERVO_CENTER);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    } else {
      maniobraEspecialAntiHo();
      limpiarBufferCamara();
      // reintento MISMO índice
      c2 = leerColorPaso(2, true, WAIT_NO_COLOR_MS);
      if (c2=='G'){ retro(RETRO_CORTO_MS); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); }
      else if (c2=='R'){ avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); }
    }
  } else {
    // 1.º=ROJO: sin “ninguno”
    c2 = leerColorPaso(2, false, 0);
    if (c2=='G') {
      avanzarConGiro(SERVO_LEFT,1600);
      avanzarConGiro(SERVO_RIGHT,1600);
      StopMotor();
    } else {
      avanzarConGiro(SERVO_RIGHT,1600);
      avanzarConGiro(SERVO_LEFT,1600);
      StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 3.º color (pauta replicable en 5.º y 7.º) ----------
  Serial.println("[3] Leyendo 3.º (depende de 2.º)...");
  char c3 = leerColorPaso(3, true, WAIT_NO_COLOR_MS); // aquí sí usamos N

  if (c2=='R' || c2=='N') {
    if (c3=='G') {
      avanzarConGiro(SERVO_LEFT,CONT_TURN_MS);
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      StopMotor();
    } else {
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    }
  } else { // c2==G
    if (c3=='R') {
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      avanzarConGiro(SERVO_LEFT, CONT_TURN_MS);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    } else { // G o N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 4.º color ----------
  Serial.println("[4] Leyendo 4.º...");
  char c4;
  if (c3=='R') {
    c4 = leerColorPaso(4, false, 0);
    if (c4=='G') { avanzarConGiro(SERVO_LEFT,1600); avanzarConGiro(SERVO_RIGHT,1600); StopMotor(); }
    else         { avanzarConGiro(SERVO_RIGHT,1600); avanzarConGiro(SERVO_LEFT,1600);  StopMotor(); }
  } else { // 3.º = VERDE o N → con “ninguno” = maniobra especial ANTIHO
    c4 = leerColorPaso(4, true, WAIT_NO_COLOR_MS);
    if (c4=='R') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); StopMotor(); }
    else if (c4=='G'){ giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); StopMotor(); }
    else {
      maniobraEspecialAntiHo();
      limpiarBufferCamara();
      // reintenta 4.º
      c4 = leerColorPaso(4, true, WAIT_NO_COLOR_MS);
      if (c4=='R') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); StopMotor(); }
      else if (c4=='G'){ giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); StopMotor(); }
    }
  }
  limpiarBufferCamara();

  // ---------- 5.º color ----------
  Serial.println("[5] Leyendo 5.º...");
  char c5 = leerColorPaso(5, true, WAIT_NO_COLOR_MS);
  if (c4=='G') {
    if (c5=='R') {
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      avanzarConGiro(SERVO_LEFT, CONT_TURN_MS);
      StopMotor();
    } else { // G o N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    }
  } else { // 4.º = R
    if (c5=='G') {
      avanzarConGiro(SERVO_LEFT,CONT_TURN_MS);
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      // luego IZQ 2.8
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    } else { // R o N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER); StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 6.º color ----------
  Serial.println("[6] Leyendo 6.º...");
  char c6 = leerColorPaso(6, true, WAIT_NO_COLOR_MS);
  if (c5=='G') {
    if (c6=='G') { avanzarConGiro(SERVO_LEFT,1600); avanzarConGiro(SERVO_RIGHT,1600); StopMotor(); }
    else if (c6=='R'){ avanzarConGiro(SERVO_RIGHT,1600); avanzarConGiro(SERVO_LEFT,1600);  StopMotor(); }
    else { // N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    }
  } else { // 5.º=R o N
    if (c6=='G') { avanzarRecto(SEG_1S,SERVO_CENTER); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); StopMotor(); }
    else if (c6=='R'){ giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); StopMotor(); }
    else { // N
      avanzarRecto(CONT_FORWARD_MS, SERVO_CENTER);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    }
  }
  limpiarBufferCamara();

  // ---------- 7.º color ----------
  Serial.println("[7] Leyendo 7.º...");
  char c7 = leerColorPaso(7, true, WAIT_NO_COLOR_MS);
  if (c6=='G') {
    if (c7=='G') { avanzarRecto(CONT_FORWARD_MS,SERVO_CENTER); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000); }
    else if (c7=='R'){ avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS); avanzarConGiro(SERVO_LEFT,CONT_TURN_MS); StopMotor(); }
    else { // N
      avanzarRecto(CONT_FORWARD_MS,SERVO_CENTER); giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    }
  } else { // 6.º=R o N
    if (c7=='G') {
      avanzarConGiro(SERVO_LEFT,CONT_TURN_MS);
      avanzarConGiro(SERVO_RIGHT,CONT_TURN_MS);
      giroLargoAntiHorario(); servoCentroTrasIzq(); retro(1000);
    } else if (c7=='R') {
      avanzarRecto(CONT_FORWARD_MS,SERVO_CENTER); StopMotor();
    } else {
      avanzarRecto(CONT_FORWARD_MS,SERVO_CENTER); StopMotor();
    }
  }
  limpiarBufferCamara();

  // ---------- 8.º color (regla especial antiho) ----------
  Serial.println("[8] Leyendo 8.º (regla especial)...");
  char c8 = leerColorPaso(8, false, 0);

  // Regla especial ANTIHO:
  // Si 7.º = VERDE → maniobra especial antiho y luego avanza 1 s
  // Si 7.º = ROJO  → solo avanza 1 s
  if (c7=='G') {
    maniobraEspecialAntiHo();
    avanzarRecto(SEG_1S, SERVO_CENTER);
  } else {
    avanzarRecto(SEG_1S, SERVO_CENTER);
  }
  StopMotor();
}

// =================== Secuencia de una vuelta (1..8) ===================
void ejecutarVuelta(Sentido s) {
  if (s==HORARIO) ejecutarHorario();
  else            ejecutarAntiHorario();
}

// =================== Setup ===================
void setup() {
  Serial.begin(115200);
  Wire.begin();

  // UART cámara
  Serial1.begin(CAM_BAUD, SERIAL_8N1, CAM_RX, CAM_TX);

  // Pines motor
  pinMode(SHCP_PIN, OUTPUT);
  pinMode(EN_PIN,   OUTPUT);
  pinMode(DATA_PIN, OUTPUT);
  pinMode(STCP_PIN, OUTPUT);
  pinMode(PWM1_PIN, OUTPUT);

  // Servo
  miServo.setPeriodHertz(50);
  miServo.attach(SERVO_PIN, 500, 2400);
  miServo.write(SERVO_CENTER);
  StopMotor();

  // VL53
  selectOnlyOneMux(MUX_LEFT_ADDR);
  sensorLeft.setTimeout(250); sensorLeft.init();
  sensorLeft.setDistanceMode(VL53L1X::Long);
  sensorLeft.setMeasurementTimingBudget(50000);
  sensorLeft.startContinuous(50);

  selectOnlyOneMux(MUX_RIGHT_ADDR);
  sensorRight.setTimeout(250); sensorRight.init();
  sensorRight.setDistanceMode(VL53L1X::Long);
  sensorRight.setMeasurementTimingBudget(50000);
  sensorRight.startContinuous(50);

  Serial.println("== Inicio: Salida estacionamiento ==");
  // Elegir lado por mayor distancia
  int dL = lecturaPromedio(sensorLeft,  MUX_LEFT_ADDR, 3);
  int dR = lecturaPromedio(sensorRight, MUX_RIGHT_ADDR,3);
  Serial.print("Dist IZQ="); Serial.print(dL);
  Serial.print(" | DER=");   Serial.println(dR);

  bool eligioIzquierda = (dL >= dR);
  if (eligioIzquierda) {
    Serial.println("Salida: IZQUIERDA (=> ANTIHORARIO)");
    secuenciaSalidaIzquierda();
    sentido = ANTIHORARIO;
  } else {
    Serial.println("Salida: DERECHA (=> HORARIO)");
    secuenciaSalidaDerecha();
    sentido = HORARIO;
  }

  Serial.println("Maniobra final (giro contrario)...");
  maniobraFinal(eligioIzquierda);

  Serial.println("== Preparado para Vuelta 1 ==");
}

// =================== Loop ===================
void loop() {
  // Vuelta 1 (lee cámara y memoriza)
  if (vueltaActual == 1) {
    usarMemoria = false;
    ejecutarVuelta(sentido);
    memoriaLlena = true;
    vueltaActual = 2;
    Serial.println("== Fin Vuelta 1. Memoria lista. Comienza Vuelta 2 ==");
    delay(400);
    return;
  }

  // Vuelta 2 (reproduce memoria)
  if (vueltaActual == 2 && memoriaLlena) {
    usarMemoria = true;
    ejecutarVuelta(sentido);
    vueltaActual = 3;
    Serial.println("== Fin Vuelta 2. Comienza Vuelta 3 ==");
    delay(400);
    return;
  }

  // Vuelta 3 (reproduce memoria)
  if (vueltaActual == 3 && memoriaLlena) {
    usarMemoria = true;
    ejecutarVuelta(sentido);
    Serial.println("== Fin Vuelta 3. Programa finaliza ==");
    while (true) { StopMotor(); delay(1000); }
  }

  // Seguridad
  StopMotor();
  delay(1000);
}

```

Camera
----

The camera is programmed to detect the red and green colors, the camera has other functions but for the sake of simplicity we only used in to detect colors. The camera was programmed with Arduino

```arduino

from machine import UART
import sensor
import image
import time

UART a ESP32 (TX en P4)
uart = UART(1, baudrate=115200)

Configuración de la cámara
sensor.reset()
sensor.set_pixformat(sensor.RGB565)
sensor.set_framesize(sensor.HD720)
sensor.skip_frames(time=2000)
sensor.set_auto_gain(False)
sensor.set_auto_whitebal(False)

Umbrales
red_threshold = (30, 100, 15, 127, 15, 127)
green_threshold = (30, 100, -127, -15, 15, 127)

clock = time.clock()

while True:
    clock.tick()
    img = sensor.snapshot()

    # Detectar rojo (máximo 1)
    rojos = img.find_blobs([red_threshold], pixels_threshold=200, area_threshold=200, merge=True)
    verdes = img.find_blobs([green_threshold], pixels_threshold=200, area_threshold=200, merge=True)

    if len(rojos) > 0:
        blob = rojos[0]
        img.draw_rectangle(blob.rect(), color=(255, 0, 0))
        img.draw_cross(blob.cx(), blob.cy(), color=(255, 0, 0))
        uart.write("ROJO\n")
        print("ROJO")
    elif len(verdes) > 0:
        blob = verdes[0]
        img.draw_rectangle(blob.rect(), color=(0, 255, 0))
        img.draw_cross(blob.cx(), blob.cy(), color=(0, 255, 0))
        uart.write("VERDE\n")
        print("VERDE")

    time.sleep_ms(300)  # Da tiempo al ESP32 a leer sin saturarse

```

(Update) This part of the code trades fps for quality to make it easier to detect the color blocks, it uses the inferior part of the camera so it can see the ground and it ignores the the servo motor because the range of the camera can see the motor and the motor is colored so it could interfer with the reading.

```python

from machine import UART
import sensor, image, time

# Configuración de UART para enviar los datos al ESP32
uart = UART(1, baudrate=115200)

# Inicialización del sensor de la cámara
sensor.reset()
sensor.set_pixformat(sensor.RGB565)  # Formato de color RGB
sensor.set_framesize(sensor.QVGA)  # Resolución más baja para mejorar FPS (160x120)
sensor.skip_frames(time=2000)  # Esperar 2 segundos para estabilizar la cámara
sensor.set_auto_gain(False)  # Desactivar ganancia automática para controlar la exposición
sensor.set_auto_whitebal(False)  # Desactivar balance de blancos automático

# Umbrales ajustados para evitar la confusión con naranja
red_threshold = (40, 100, 15, 127, 15, 127)  # Umbral rojo más restringido
green_threshold = (30, 100, -127, -15, 15, 127)  # Umbral verde

# Variables para controlar el envío de datos
ultimo_color = ""
tiempo_ultimo_envio = time.ticks_ms()
intervalo = 10000  # Intervalo de 10 segundos entre envíos de color

# Función para ajustar la exposición y mejorar la detección bajo diferentes condiciones de luz
def ajustar_iluminacion():
    img = sensor.snapshot()
    promedio = 0
    for pixel in img:
        promedio += pixel[0]  # Tomar un valor de la componente R (Rojo)
    promedio = promedio // (img.width() * img.height())  # Promedio de la imagen

    # Ajustar la ganancia en función de la iluminación
    if promedio < 100:  # Condición de poca luz
        sensor.set_auto_gain(True)
    else:
        sensor.set_auto_gain(False)

# Función para detectar los colores usando find_blobs (más eficiente)
def detectar_color_blobs(img):
    # Limitar la región a la parte superior de la imagen (evitar la franja en el piso)
    region_superior = (0, 0, img.width(), img.height() // 2)  # Tomar solo la mitad superior de la imagen

    rojos = img.find_blobs([red_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    verdes = img.find_blobs([green_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    return rojos, verdes

while True:
    # Ajustar la iluminación según el entorno
    ajustar_iluminacion()

    # Capturar una nueva imagen
    img = sensor.snapshot()

    # Detectar rojo y verde usando blobs (más eficiente)
    rojos, verdes = detectar_color_blobs(img)

    # Filtrar los blobs para encontrar los que tengan un tamaño adecuado (aproximadamente 10 cm de alto)
    rojos_validos = [blob for blob in rojos if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto
    verdes_validos = [blob for blob in verdes if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto

    # Determinar el color detectado
    color_detectado = ""
    if len(rojos_validos) > len(verdes_validos):
        color_detectado = "ROJO"
    elif len(verdes_validos) > len(rojos_validos):
        color_detectado = "VERDE"

    # Enviar el color detectado si ha cambiado o si ha pasado el intervalo de tiempo
    if color_detectado:
        tiempo_actual = time.ticks_ms()
        if (color_detectado != ultimo_color) or (time.ticks_diff(tiempo_actual, tiempo_ultimo_envio) > intervalo):
            uart.write(color_detectado + "\n")  # Enviar el color por UART
            print("Color enviado:", color_detectado)
            ultimo_color = color_detectado
            tiempo_ultimo_envio = tiempo_actual
    else:
        ultimo_color = ""  # Reiniciar si no se detecta ningún color

```

(Update) Now it only sees half of its visor and it only detects the color closest to it

```python

from machine import UART
import sensor, image, time

# Configuración de UART para enviar los datos al ESP32
uart = UART(1, baudrate=115200)

# Inicialización del sensor de la cámara
sensor.reset()
sensor.set_pixformat(sensor.RGB565)  # Formato de color RGB
sensor.set_framesize(sensor.QVGA)  # Resolución más baja para mejorar FPS (320x240)
sensor.skip_frames(time=2000)  # Esperar 2 segundos para estabilizar la cámara
sensor.set_auto_gain(False)  # Desactivar ganancia automática para controlar la exposición
sensor.set_auto_whitebal(False)  # Desactivar balance de blancos automático

# Umbrales ajustados para evitar la confusión con naranja
red_threshold = (30, 100, 15, 127, 15, 127)  # Umbral rojo más restringido
green_threshold = (30, 100, -127, -15, 15, 127)  # Umbral verde

# Variables para controlar el envío de datos
ultimo_color = ""
tiempo_ultimo_envio = time.ticks_ms()
intervalo = 10000  # Intervalo de 10 segundos entre envíos de color

# Función para ajustar la exposición y mejorar la detección bajo diferentes condiciones de luz
def ajustar_iluminacion():
    img = sensor.snapshot()
    promedio = 0
    for pixel in img:
        promedio += pixel[0]  # Tomar un valor de la componente R (Rojo)
    promedio = promedio // (img.width() * img.height())  # Promedio de la imagen

    # Ajustar la ganancia en función de la iluminación
    if promedio < 100:  # Condición de poca luz
        sensor.set_auto_gain(True)
    else:
        sensor.set_auto_gain(False)

# Función para detectar los colores usando find_blobs (más eficiente)
def detectar_color_blobs(img):
    # Limitar la región a los 3/4 superiores de la imagen (evitar la franja en el piso)
    region_superior = (0, 0, img.width(), img.height() // 2)  # Usar solo la mitad superior de la imagen

    rojos = img.find_blobs([red_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    verdes = img.find_blobs([green_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    return rojos, verdes

# Función para obtener el blob más cercano
def obtener_blob_mas_cercano(rojos, verdes):
    # Verificar que haya blobs en ambos colores
    if not rojos and not verdes:
        return None, None

    # Encontrar el blob más cercano (el que tiene el valor de 'y' más bajo)
    rojo_cercano = min(rojos, key=lambda b: b[1], default=None)  # Minimo valor de 'y' para los rojos
    verde_cercano = min(verdes, key=lambda b: b[1], default=None)  # Minimo valor de 'y' para los verdes

    # Comparar cuál de los dos colores está más cerca
    if rojo_cercano and verde_cercano:
        if rojo_cercano[1] < verde_cercano[1]:  # Si el rojo está más cerca
            return "ROJO", rojo_cercano
        else:  # Si el verde está más cerca
            return "VERDE", verde_cercano
    elif rojo_cercano:  # Si solo se detecta rojo
        return "ROJO", rojo_cercano
    elif verde_cercano:  # Si solo se detecta verde
        return "VERDE", verde_cercano
    return None, None

while True:
    # Ajustar la iluminación según el entorno
    ajustar_iluminacion()

    # Capturar una nueva imagen
    img = sensor.snapshot()

    # Detectar rojo y verde usando blobs (más eficiente)
    rojos, verdes = detectar_color_blobs(img)

    # Filtrar los blobs para encontrar los que tengan un tamaño adecuado (aproximadamente 10 cm de alto)
    rojos_validos = [blob for blob in rojos if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto
    verdes_validos = [blob for blob in verdes if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto

    # Obtener el blob más cercano
    color_detectado, blob_detectado = obtener_blob_mas_cercano(rojos_validos, verdes_validos)

    # Si se ha detectado un color, dibujar el marco y enviar el color
    if color_detectado and blob_detectado:
        # Dibujar un rectángulo alrededor del blob más cercano
        img.draw_rectangle(blob_detectado[0], blob_detectado[1], blob_detectado[2], blob_detectado[3], color=(255, 0, 0))  # Rojo
        img.draw_string(blob_detectado[0], blob_detectado[1] - 10, color_detectado, color=(255, 0, 0))  # Etiqueta con el color

        # Enviar el color detectado si ha cambiado o si ha pasado el intervalo de tiempo
        tiempo_actual = time.ticks_ms()
        if (color_detectado != ultimo_color) or (time.ticks_diff(tiempo_actual, tiempo_ultimo_envio) > intervalo):
            uart.write(color_detectado + "\n")  # Enviar el color por UART
            print("Color enviado:", color_detectado)
            ultimo_color = color_detectado
            tiempo_ultimo_envio = tiempo_actual
    else:
        ultimo_color = ""  # Reiniciar si no se detecta ningún color

```

Camera code (FINAL)

This is the last update to the code before the 2025 national competition in Panama, the camera is now programmed for quality and precision rather than fps.

```python

# OpenMV color detector for ESP32 robot
# Sends: b"verde\n" or b"rojo\n" via UART(1) @ 115200
# Shows live overlay (rectangles + labels) in the OpenMV IDE preview.

from machine import UART
import sensor, image, time
from collections import deque

# ------------- UART to ESP32 -------------
# On most OpenMV boards, UART(1) uses P4/P5 (check your board silkscreen).
uart = UART(1, baudrate=115200, timeout_char=100)

# ------------- Camera setup -------------
sensor.reset()
sensor.set_pixformat(sensor.RGB565)          # color
sensor.set_framesize(sensor.QVGA)            # 320x240 for speed
sensor.set_auto_gain(False)                  # IMPORTANT: keep OFF for color thresholds
sensor.set_auto_whitebal(False)              # IMPORTANT: keep OFF for color thresholds
sensor.skip_frames(time=500)                 # small warmup so it starts almost immediately
clock = time.clock()

# ------------- Tuned LAB thresholds -------------
# These ranges are robust against a white track (white has a~0, b~0; we push away from that).
# Tweak here if your lighting is very different:
# Tuple format: (Lmin, Lmax, Amin, Amax, Bmin, Bmax)
RED_T   = (15, 85,   25, 127,  -10, 127)
GREEN_T = (10, 85, -128, -20,   -10, 127)

# ------------- Detection ROI -------------
# We ignore borders and most of the floor to avoid noise.
# ROI covers center 60% width and top 75% height (reduce masked area as you requested).
def compute_roi(img):
    w, h = img.width(), img.height()
    roi_x = int(w * 0.20)
    roi_y = 0
    roi_w = int(w * 0.60)
    roi_h = int(h * 0.75)
    return (roi_x, roi_y, roi_w, roi_h)

# ------------- Sensitivity & stability -------------
PIXELS_THRESHOLD = 60     # lower -> more sensitive (min connected pixels)
AREA_THRESHOLD   = 80     # lower -> more sensitive (min bounding box area)
MIN_H_PX         = 10     # ignore tiny blobs by height
REFRESH_MS       = 400    # resend color at least every 0.4s even if unchanged
DEBOUNCE_N       = 5      # frames for majority vote
DEBOUNCE_K       = 3      # need >= K of last N frames to accept a new label

last_sent_label  = None
last_send_time   = time.ticks_ms()
history          = deque(maxlen=DEBOUNCE_N)

# ------------- Optional: mild adaptive exposure (keeps colors readable) -------------
# We make tiny adjustments without enabling full auto-gain/auto-WB (which would break color thresholds).
def mild_exposure_nudge(img):
    # Compute statistics in the ROI to judge brightness
    roi = compute_roi(img)
    stats = img.get_statistics(roi=roi)
    # Luma proxy via mean of RGB565 is coarse; we use l_mean from LAB using .statistics() in RGB is not direct.
    # Simple heuristic: if very dark, briefly allow auto gain to catch up, then turn it off.
    global auto_gain_counter
    l_estimate = (stats.mean())  # 0..255 rough
    if l_estimate < 55:
        sensor.set_auto_gain(True)
    else:
        sensor.set_auto_gain(False)

# ------------- Pick the "closest" blob -------------
# We use the smallest y (higher on the image) as "closer" in your usage
def pick_blob(blobs):
    if not blobs:
        return None
    return min(blobs, key=lambda b: b.y())

def label_from_frame(img):
    roi = compute_roi(img)

    rojos = img.find_blobs([RED_T], pixels_threshold=PIXELS_THRESHOLD,
                           area_threshold=AREA_THRESHOLD, merge=True, roi=roi)
    verdes = img.find_blobs([GREEN_T], pixels_threshold=PIXELS_THRESHOLD,
                            area_threshold=AREA_THRESHOLD, merge=True, roi=roi)

    # Filter tiny blobs by height
    rojos  = [b for b in rojos  if b.h() >= MIN_H_PX]
    verdes = [b for b in verdes if b.h() >= MIN_H_PX]

    br = pick_blob(rojos)
    bg = pick_blob(verdes)

    # Decide based on presence and vertical position
    if br is None and bg is None:
        return None, None
    if br is not None and bg is None:
        return "rojo", br
    if br is None and bg is not None:
        return "verde", bg

    # Both present: choose the one with smaller y() (higher in the image)
    if br.y() < bg.y():
        return "rojo", br
    else:
        return "verde", bg

def stable_vote_push(label):
    history.append(label)
    if history.count(label) >= DEBOUNCE_K:
        return True
    return False

def maybe_send(label):
    global last_sent_label, last_send_time
    now = time.ticks_ms()
    # Send if changed OR it's time to refresh
    if (label != last_sent_label) or (time.ticks_diff(now, last_send_time) >= REFRESH_MS):
        token = (label + "\n").encode()
        uart.write(token)
        print("TX:", label)  # also print to IDE serial
        last_sent_label = label
        last_send_time = now

# ------------- Main loop -------------
while True:
    clock.tick()
    img = sensor.snapshot()

    # Mild exposure nudge to keep detection robust without ruining thresholds
    mild_exposure_nudge(img)

    # Detect
    label, blob = label_from_frame(img)

    # Draw ROI
    rx, ry, rw, rh = compute_roi(img)
    img.draw_rectangle(rx, ry, rw, rh, color=(200, 200, 200))  # light ROI box

    if label is None:
        # Draw hint text
        img.draw_string(4, 4, "No color", color=(255, 255, 255), scale=1)
        # Reset vote history on no color (optional): allows quicker switching
        history.append(None)
    else:
        # Draw blob box + label
        color_draw = (0, 255, 0) if label == "verde" else (255, 0, 0)
        img.draw_rectangle(blob.rect(), color=color_draw, thickness=2)
        img.draw_cross(blob.cx(), blob.cy(), color=color_draw, size=5)
        img.draw_string(blob.x(), max(0, blob.y()-12), label, color=color_draw, scale=2)

        # Stability (debounce) + send
        if stable_vote_push(label):
            maybe_send(label)

    # Optional FPS overlay
    img.draw_string(4, img.height()-12, "FPS: %0.1f" % clock.fps(), color=(255,255,255), scale=1)

```

[Back to table of contents](#table-of-contents)



