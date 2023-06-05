TODO demo video

🚙 Vehicles are expensive investments – they need routine maintenance and constant upkeep to avoid costly repairs. At scale, this becomes a complex logistical challenge. Failures can be costly to the fleet owner in vehicle downtime for unexpected maintenance and repairs.​

💡 By tracking the routes these vehicles take and cross-referencing it with vehicle diagnostic data, users can find correlations and develop insights.

## 📝 Design Spec
📍 **Tracker**: sits on the dashboard of the vehicle with a cable connected to the OBD-II port, extracting vehicle diagnostic data and collecting GPS, accelerometer, and gyroscope data via onboard sensors.

🗺 **Web App**: an interactive map to track the vehicle location along with a statistics page with a dashboard of KPIs and calculations over historical data. 

## Block Diagram
![](/assets/images/blockdiagfinal_.svg)

## 💽 Web App
![](/assets/videos/webappoverview.mp4)
 
**DataDriven Custom PCB**

📡 RF circuitry for LTE and GPS functionality

🔌 Power circuitry to support bench, OBD-II, and microUSB supply

💻 Programmable OPT pins & test points for debugging & flexibility

## 📶 Networking
TODO
- With a single on-chip LTE/GNSS modem, our firmware uses time-division multiplexing to concurrently upload UDP datagrams over LTE while maintaining a GPS fix

## 🚙 Vehicle Interface
TODO
- Probe for standard OBD-II PIDs as defined by SAE J1979 on standard CAN and extended CAN

## ☁️ Backend
TODO
- UDP listener service receives & processes messages from the tracker and persists it to the database
- API serves the data at endpoints to our frontend at api.datadrivenucsb.com (e.g., /live/{car_id}, /live_all_cars)


## Sponsors & Mentors
![](/assets/images/caci.png)

[https://www.caci.com/](https://www.caci.com/)

John Buckley, Brian Canty, Stefan Crigler, Martin Fay, Duane Gardner, Austin Hwang, David McCarthy, Eric Nystrom

![](/assets/images/coe.png) 

[https://web.ece.ucsb.edu/~yoga/capstone/](https://web.ece.ucsb.edu/~yoga/capstone/)

![](/assets/images/ce.png)

[https://ce.ucsb.edu](https://ce.ucsb.edu)

Dr. Yogananda Isukapalli, Alex Lai, 
Jimmy Kraemer, Venkat Krishnan
