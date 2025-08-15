B407 Chab Mod
-----------------------------------

🛠️ Description:
This patch tweaks the default Bell 407 flight model in Microsoft Flight Simulator to provide a more realistic and immersive helicopter flying experience, especially for advanced virtual pilots.

🎯 Key Modifications:
- Adjusted cyclic sensitivity (more responsive left/right control)
- Reduced over-sensitivity of tail rotor pedals
- Smoothed out collective response to avoid excessive climb/descent rates
- Improved trim responsiveness
- Slight increase in general stability while keeping manual control feel

We also took the datas of the Rolls-Royce/Allison 250-C47B to adjust these engine settings:



| Indicators         | realist areas                                         |
| ------------------ | ----------------------------------------------------- |
| Torque (%)         | Green untill 93 %, yellow untill 100 %, red sfter 100%|
| Np rotor (%)       | Green 90–107 %, yellow 108–110 %, red >110            |
| Speed (KIAS)       | Green ≤ 140, Yellow 141‑142, Red >142                  |
| N1 (%)             | Green 63–105, yellow <63, red <60                     |

The [FUEL_PRESSURE] section has been revised to reflect more realistic fuel system behavior based on official Bell 407 performance and maintenance documentation.

✅ What was changed:

Default placeholder values were replaced with accurate PSI ranges corresponding to operational limits of the fuel boost pumps and warning thresholds.

📌LowLimit set to 8 psi to trigger warnings when pressure falls below minimum safe operating value.

- Green range (8–25 psi) reflects nominal boost pump output.

- Yellow (25–30 psi) and Red (>30 psi) ranges indicate abnormal/high-pressure conditions.

- Ensures the fuel pressure gauge behaves realistically during startup, cruise, and emergencies.




📁 Contents:
This mod only contains a modified "flight_model.cfg" and also a "helicopter.cfg files (Added),egines.cfg and "cockpi.cfg" placed in the correct path to override the default aircraft parameters. It does not duplicate the full aircraft, making the installation clean and lightweight.

📦 Type of mod: Partial override (non-intrusive patch)

-----------------------------------

🔄 How to uninstall:
To revert to the original Bell 407 flight model, simply remove the following folder from your `Community` folder:
`b407_chab_mod`

Author: Julien Chabbey (from Romandy AI Studio)
