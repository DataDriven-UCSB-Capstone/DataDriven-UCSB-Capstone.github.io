TODO demo video

🚙 Vehicles are expensive investments – they need routine maintenance and constant upkeep to avoid costly repairs. At scale, this becomes a complex logistical challenge. Failures can be costly to the fleet owner in vehicle downtime for unexpected maintenance and repairs.​

💡 By tracking the routes these vehicles take and cross-referencing it with vehicle diagnostic data, users can find correlations and develop insights.

## 📝 Design Spec
📍 **Tracker**: sits on the dashboard of the vehicle with a cable connected to the OBD-II port, extracting vehicle diagnostic data and collecting GPS, accelerometer, and gyroscope data via onboard sensors.

🗺 **Web App**: an interactive map to track the vehicle location along with a statistics page with a dashboard of KPIs and calculations over historical data. 

## Block Diagram
![](/assets/images/blockdiagfinal_.svg)

## 💽 Web App
<video controls>
  <source type="video/mp4" src="https://github.com/DataDriven-UCSB-Capstone/DataDriven-UCSB-Capstone.github.io/assets/56094467/b3c4c8e8-3df9-4ab0-8d19-7ed0ce426a43">
</video>

## 📍 Tracker (Custom PCB)
![](/assets/images/pcb.png)

📡 RF circuitry for LTE and GPS functionality

🔌 Power circuitry to support bench, OBD-II, and microUSB supply

💻 Programmable OPT pins & test points for debugging & flexibility

## 📶 Networking
TODO DIAGRAM
With a single on-chip LTE/GNSS modem, our firmware uses time-division multiplexing to concurrently upload UDP datagrams over LTE while maintaining a GPS fix

## Sponsors & Mentors

[![](/assets/images/caci.png)]([https://www.caci.com/](https://www.caci.com/)
)

John Buckley, Brian Canty, Stefan Crigler, Martin Fay, Duane Gardner, Austin Hwang, David McCarthy, Eric Nystrom

[![](/assets/images/coe.png) ]([https://web.ece.ucsb.edu/~yoga/capstone/](https://web.ece.ucsb.edu/~yoga/capstone/)
)

[![](/assets/images/ce.png)]([https://ce.ucsb.edu](https://ce.ucsb.edu))

Dr. Yogananda Isukapalli, Alex Lai, 
Jimmy Kraemer, Venkat Krishnan
