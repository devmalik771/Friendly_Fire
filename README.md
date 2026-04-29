<h1 align="center">ESE 3500 - Friendly Fire</h1>

<p align="center">
  <span style="display:inline-block; min-width:22%; text-align:center;"><strong>Devan Malik</strong></span>
  <span style="display:inline-block; min-width:22%; text-align:center;"><strong>Marko Mijatovic</strong></span>
  <span style="display:inline-block; min-width:22%; text-align:center;"><strong>Kim Huang</strong></span>
  <span style="display:inline-block; min-width:22%; text-align:center;"><strong>Victor Wanjohi</strong></span>
</p>

---

<h2 align="center">Description</h2>

<p align="center">
  This project is a fully operational laser tag game with separate blaster and chest-mount
  components. The system is fully controlled through a web app, which includes a game dashboard
  for managing gameplay, tracking status, and monitoring the overall match experience.
</p>

---

<h2 align="center">Project Video</h2>

<p align="center">
  <a href="https://drive.google.com/drive/folders/1jIbaAgMy6JAKm02dPGXfAoZNbYtTDbEu?usp=drive_link" target="_blank">
    <img
      src="https://via.placeholder.com/900x500?text=Project+Video+Placeholder"
      alt="Project Video Placeholder"
      width="900"
    />
  </a>
</p>

<p align="center">
  <a href="https://drive.google.com/drive/folders/1jIbaAgMy6JAKm02dPGXfAoZNbYtTDbEu?usp=drive_link"><strong>Open the project video folder</strong></a>
</p>

---

<h2 align="center">Photos</h2>

<table align="center">
  <tr>
    <td align="center"><img src="https://via.placeholder.com/260x180?text=Photo+1" alt="Photo 1" width="260" /></td>
    <td align="center"><img src="https://via.placeholder.com/260x180?text=Photo+2" alt="Photo 2" width="260" /></td>
    <td align="center"><img src="https://via.placeholder.com/260x180?text=Photo+3" alt="Photo 3" width="260" /></td>
    <td align="center"><img src="https://via.placeholder.com/260x180?text=Photo+4" alt="Photo 4" width="260" /></td>
  </tr>
</table>

---

<h2 align="center">Specifications</h2>

### SRS

- SRS 01: The blaster firmware activates the IR LED for a duration of 0.5 seconds immediately after a valid trigger press is detected, ensuring that each shot produces a consistent and clearly identifiable output signal. This timing is controlled precisely in software so that every trigger event results in uniform LED behavior regardless of user input speed.

- SRS 02: The blaster firmware enforces a minimum inter-shot interval of 500 ms (±50 ms) to prevent excessive firing or spamming. During this cooldown period, any additional trigger inputs are ignored, and the system only re-enables firing once the interval has fully elapsed, ensuring consistent gameplay pacing and system reliability.

- SRS 03: The blaster firmware decrements the ammo counter each time a valid shot is fired and prevents any further firing once the ammo count reaches zero. The LCD display updates the visible ammo count within 100 ms of each shot, providing immediate feedback to the user and ensuring the displayed value always reflects the true internal state.

S- RS 04: The reload mechanic is implemented exclusively through a shake-to-reload gesture detected by the MPU6050 accelerometer. When a valid shake pattern is identified, the system initiates a reload sequence that restores the ammo count to its maximum value, providing a responsive and intuitive method for reloading without requiring button input.

- SRS 05: The vest firmware transmits updated player status information, including current health and elimination state, to the BLE module via UART within 500 ms of any change in game state. This ensures that external systems, such as a connected web application, receive timely and accurate updates reflecting in-game events.

- SRS 06: When a RESET command is received from the web application via BLE, both microcontrollers transition back to their initial ready state within 1 second. This reset restores full health, full ammo, and ALIVE status, ensuring the system is quickly ready for a new game session.

- SRS 07: The blaster firmware continuously reads acceleration data from the MPU6050 via I2C at a minimum sampling rate of 20 Hz. A shake-to-reload gesture is detected when acceleration exceeds 2g on any axis for at least three consecutive samples, at which point the system reliably triggers the reload sequence.

### HRS

- Placeholder HRS requirement one.
- Placeholder HRS requirement two.
- Placeholder HRS requirement three.
- Placeholder HRS requirement four.
- Placeholder HRS requirement five.

---

<h2 align="center">Conclusion</h2>

<p align="center">
  This placeholder conclusion summarizes the project, highlights the team’s overall work,
  and leaves space for a concise final reflection on goals, results, and future improvements.
</p>
