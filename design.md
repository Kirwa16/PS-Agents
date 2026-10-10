# ICS 3202 Practical Exercise 3: Designing a Searching Agent

**Group members:** Omwenga Francis (184540), Name 2 (Adm No), Name 3 (Adm No)


**Agent:** Self-driving trailer, Nairobi to Kisumu

---

## Question 1: PEAS Framework and Environment

### 1.1 PEAS

| Component | Description |
|---|---|
| **Performance measure** | Shortest distance; safe arrival (no collisions); cargo delivered intact; low fuel use and travel time; obeys traffic rules and speed limits; on-time delivery |
| **Environment** | Kenyan highway network, towns and junctions, other vehicles (matatus, buses, lorries, motorbikes), pedestrians, livestock and wildlife, weather (rain, fog, night), road conditions (potholes, diversions, steep sections), weighbridges and police checks |
| **Actuators** | Steering, accelerator, brake, gear selection, indicators, headlights, hazard lights, horn, wipers, trailer coupling/brakes, onboard display or alerts |
| **Sensors** | GPS, LIDAR, radar, cameras, ultrasonic sensors, speedometer, odometer, fuel gauge, gyroscope/IMU, tyre pressure sensors, load sensors, rain and light sensors |

### 1.2 Environment properties

| Property | Classification | Justification |
|---|---|---|
| Observable | **Partially observable** | Sensors cannot see round bends, behind large vehicles, or road damage ahead; other drivers' intentions are hidden |
| Agents | **Multi-agent** | Shares the road with other drivers: cooperates by following rules, competes for space when overtaking |
| Deterministic | **Stochastic** | Traffic, weather and breakdowns make outcomes uncertain |
| Episodic | **Sequential** | Current decisions (route, speed, lane) affect later states |
| Static | **Dynamic** | The environment changes while the agent is deciding |
| Discrete | **Continuous** (driving), **discrete** (route choice) | Speed and steering are continuous; the town map is a discrete graph |

---

