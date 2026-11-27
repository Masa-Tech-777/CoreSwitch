CoreFlow Extreme v2.7.13 for Windows 11 x64


Developed in Japan for Windows 11 (x64), CoreFlow Extreme lets you choose how your CPU responds when plugged in or on battery. For example, you can keep more headroom for work at your desk and try a lower frequency cap for watching videos on battery. Settings, help buttons, confirmation dialogs and the user guide are available in Japanese and English. Monitor follows the language selected in the main app.

■ What you can adjust

- Maximum frequency sets the CPU frequency cap, up to the maximum verified in the CPU specifications database. Enter 0 to remove the cap.
- Minimum frequency is a reference in MHz that Extreme converts to the Windows minimum processor performance percentage. For example, entering the lowest allowed value of 400 MHz gives neither a target the CPU must reach nor a floor it must stay above.
- Boost mode controls how Windows requests performance above the base frequency under load. Choose a mode separately for plugged-in and battery use.

Extreme applies your settings to a copy of the selected plan. Select Keep Settings within 15 seconds to save your choices for that plan.

■ Choosing a boost mode

- 0 Disabled tells Windows to leave CPU boost off.
- 1 Enabled (Standard) allows boost when needed. The CPU and Windows decide how far to raise the frequency.
- 2 Aggressive requests boost more readily under load.
- 3 Efficient Enabled considers power efficiency while providing the performance needed.
- 4 Efficient Aggressive uses efficiency-oriented or aggressive boost behavior depending on how the CPU is controlled.
- 5 Aggressive at Guaranteed uses the CPU’s guaranteed performance level as a baseline. Windows calculates how much extra performance to request.
- 6 Efficient Aggressive at Guaranteed requests the highest possible performance in the range above the CPU’s guaranteed performance level.

“Efficient” describes a policy that considers power efficiency. “Guaranteed” names a CPU performance level. Two modes can behave similarly on the same PC, and the numbers do not rank speed or power use. Use the question-mark button beside the field to read about the selected mode.

■ What changed in v2.7.13

Version 2.7.13 corrects stale Monitor readings after a sampling interruption, trial time accounting, and the responsiveness and English messages of the update check.


Power plan recovery in v2.7.12. If the previously active plan was deleted, Extreme returns to the source of the current dedicated plan when that source still exists. It checks the Windows record of the switch for manual selections during recovery. If the record is unavailable or arrives too late, checks immediately before and after the switch can miss a simultaneous selection. To keep display and sleep timeouts for future sessions, set them on the normal plan in Windows.

To inspect temperatures and clocks in more detail, select Launch HWiNFO in Monitor. See “Inspect CPU temperatures and clocks in more detail with HWiNFO” below for setup instructions.

Version 2.7.5 displays CPU specifications on two lines so frequency units remain visible.

Version 2.7.4 preserves a power plan selected in Windows while settings are being prepared. Crash recovery is scoped to the session that created the plans. If a setting cannot be read before applying changes, Monitor continues to show the current control state.

Extract the entire ZIP. If a previous copy is running, exit and restore its settings from the notification area. Run CoreFlow_Extreme.exe and approve the Windows administrator prompt. Keep the LiveMonitor folder beside the main executable.

Choose a plan and review the settings for AC and battery power. Apply tests the settings on a copy of the selected plan. Select Keep within 15 seconds to save. Let the confirmation expire to return to the previous settings. Selecting another Windows plan during confirmation cancels the pending change and preserves your selection.

Closing the main window keeps the app in the notification area. Click its icon once to reopen the windows. Exit and Restore removes the dedicated plans and retains your confirmed settings for the next launch. A full reset clears the registration and saved CPU settings.

The trial allows 60 minutes of cumulative use. After purchase, follow the license registration dialog for the Machine ID and order details. See User_Guide_EN.txt for settings and clock readings. Temperature monitoring is optional. Third-party notices, license texts and sources are in THIRD_PARTY_NOTICES.txt, licenses, source, and LiveMonitor/Temperature.

MasaTech / Itachi, Spica and Mahiru
Support   masatech.dev.apps@gmail.com
BOOTH     https://masatech.booth.pm/

From v2.7.3 onward, use a signed license key beginning with CFX2-. If you have an older key, request a replacement with your Machine ID and order details.

■ Updating in place

1. Extract the entire new ZIP to a separate location.
2. In the running copy of Extreme, choose Exit and Restore from the notification area. Wait for Monitor to close.
3. Copy the contents of the extracted CoreFlow Extreme folder into the folder containing your existing CoreFlow_Extreme.exe and replace the files. Keep the main app and LiveMonitor from the same package and open Extreme from its usual location.

Inspect CPU temperatures and clocks in more detail with HWiNFO

HWiNFO, created by Martin Malík (REALiX), is a separate application for checking individual CPU core temperatures, Core Clock and Effective Clock. Available sensors vary by PC.

1. Select Launch HWiNFO in the upper-right corner of Monitor and select OK in the explanation. If Monitor finds HWiNFO, it opens the app.

2. If you need HWiNFO, select Official download page and get the installer or portable version from https://www.hwinfo.com/download/. If it is installed but not found, choose Select installed EXE... and select HWiNFO64.exe. You can also set or change its location in Extreme under Help > Set HWiNFO executable....

3. In HWiNFO, open the Sensors window and check the Current column for the CPU sensor you want to inspect.

Free use of HWiNFO 64 is for non-commercial purposes. Check the official licensing terms for business use. HWiNFO measures independently. For Monitor’s own temperature display, see the PawnIO steps below.

For example, Monitor can show CPU Package at 60°C while HWiNFO shows a maximum of 76°C for Core 0. The first is a current package reading. The second is the highest reading from one core since sampling began or statistics were reset. In the HWiNFO Sensors window, compare the Current column for the same sensor. Monitor uses Intel CPU Package or AMD Core (Tctl/Tdie) when it can identify a single primary sensor. Distance to TjMax measures the headroom to the temperature limit.

Monitor samples temperature roughly once a second. The two applications read at different times and can catch different peaks. To compare minimum, maximum and average readings, reset both sets of statistics at about the same time and observe the same workload for the same duration. Monitor averages valid samples. Pauses and missing readings contribute no samples. To investigate a brief event, start HWiNFO CSV logging beforehand and note the time it happens.

Monitor estimates observed clock speed over an interval using Windows counters. HWiNFO’s Core Clock samples the core at a point in time. Effective Clock averages over the polling interval, including time the core was idle. Choose the metric you want to compare and use the same workload and period.

Display CPU temperature for the first time

If Monitor shows a setup prompt in the temperature panel, select View PawnIO setup steps.

To display CPU temperature, Extreme uses the PawnIO driver created by namazso. Install it from the author’s official website if you want temperature readings. Frequency settings, CPU usage and Monitor’s observed clock are available without PawnIO.

1. Select Open PawnIO website. On the official site, choose Download Now to get the signed Official edition.
2. Run the installer and select the monitor icon with a downward arrow in the lower-left corner. Read the notice and select OK.
3. When you see “PawnIO was successfully installed.”, select OK and close the setup window with the X in its upper-right corner. Restart Windows if the installer asks you to.
4. Close Monitor and select Show Monitor in Extreme to reopen it. If measurement is paused, select Resume.

If temperature is still unavailable, check the status in Temperature details. For a permission error, open Monitor from Extreme after approving the Windows administrator prompt. If the temperature module is missing, extract the entire product ZIP again. Available sensors vary by PC.

Tested hardware and what to check on your PC

CPU temperature display has been verified on a dynabook S73/FR with a Core i7-10510U, Windows 11 x64 and PawnIO installed. Equivalent readings and power-control behavior on Ryzen and hybrid P/E-core machines still need hardware verification. If the CPU database cannot establish an upper limit, Extreme cannot apply a nonzero frequency cap. Application also stops if Windows cannot read the required power settings. Extra processor efficiency-class settings are used only when readable. Windows power mode, manufacturer thermal and power limits, and workload all affect observed clocks and fan noise. Monitor's clock estimate requires a known base clock and working Windows counters. Use the 60-minute trial to check temperature display, apply a setting and restore your original plan on your own PC.
