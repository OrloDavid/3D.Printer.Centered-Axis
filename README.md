# David Orlo Centered-Z Mod for Cartesian 3D Printers
I've developed a modification for Cartesian 3D printers that significantly improves tramming/leveling and reduces Z wobble/banding or completely eliminates it with Rev.2 or Rev.3. 

This mod not only enhances resolution but also increases Z axis speed, making your printer more reliable and efficient. It's straightforward to implement and reversible if needed.

## TLDR
### Rev.1 
- Good way to get started, minimal parts needed (printed parts, nuts and bolts)
- Unless your Z Lead is bent to hell, it should resolve any and all Z Wobble / Banding issues you have
- If you love Z-Hop then your in for a treat because your Z Speeds should at minimum double (Over Single Lead Setup
- I have squared up my printer (Level / Tram) 1 time since performing this mod, and have moved it 3 times now
- I haven't needed to re-mesh my bed other than for tempurature profiles after this Mod

### Rev.2
- Takes things a step further by relocating the Z Stepper to the top of the printer, this not only removes the weight from the gantry but also changes the dynamics of the force used to move the gantry, and the auto-leveling / auto-balancing effect it has
- Changes to a Non-Captive Z Stepper, the LEAD SCREW NO LONGER SPINS! (Watch the Videos)
- The Stepper required is cheap, like $20, also a good time to change your Z Lead to a 1 or 2 start if your using a 4 start
- Faster with a 2 start Lead then a nornal setup with a 4 start
- Ability to use standard aluminum gantry plates for Stepper and Lead Screw Mounting, or print your own

### Rev.3
- This is what was originally planned as the end result with direct drive conversion in mind
- Fully centered / Fully balanced Design with a beautifully minimalistic approach
- Linear rails are required on the X and Y axis due to the location of the drive belts, steppers and Lead Screw Mount
- Utilizing off the shelf components once again, no machining or custom pieces required



### Centered-Z Mod: Rev.1
### Reduce / Eliminate Z-wobble
### Consistently Reliable Tram & Level
### Z Speed up to 3x Faster

### Benefits of the Mod
- Resolves common tramming/leveling issues.
- Reduces Z Wobble / Z Banding.
- Increases resolution without speed loss. (w/ Lead screw change)
- Achieves much faster Z speeds.
- Reduces the likelihood of issues.
- Simple to perform and easy to reverse if not suitable.

### Parts and Resources /Links Below
- **Main Components**:
  1. Right Hand Extruder Mount
  2. Upper Lead Screw Mount
  3. Lower Stepper Motor Mount

- **Additional Hardware Needed**:
  1. T-Nuts and Screws for mounting.
  2. Lead Screw Coupler (Oldham Coupler recommended).
  3. Stepper Motor Extension wires.

- **3D File Design Iterations**:
  3D Parts marked "Rev.X" are for iteration tracking (not in reference to a specific mod). "Final" indicates no further improvements planned.
  These are designed to fit on 2020/2040 Aluminum and should clear most roller and belt setups on the X gantry.
- **3D Files Availability**:
  - [Tinkercad (Login Required)](https://www.tinkercad.com/users/0RxhGZwzXXM-david-m-orlo)
  - [Thingiverse Designs](https://www.thingiverse.com/a_makers_life/designs)
  - [Printables Profile](https://www.printables.com/@DavidmOrlo_1689053)

### Firmware or Hardware Changes
1. **Change Stepper Rotation Direction** (Choose one):
   - Marlin: Toggle True/False for Z Stepper in Config File.
   - Klipper: Add/remove '!' on the Z Stepper DIR line in Config File.
   - Hardware: Flip Stepper Wires ([Guide](https://www.youtube.com/watch?v=AgyNM7FQrmk)).

2. **Suggested Firmware Change**:
   - Increase Z Park Height (especially for 8mm Lead Screw).
   - Marlin: `#define Z_AFTER_HOMING  35`
   - Klipper: `z_hop: 35` (Please verify this setting).

### Visual Resources
- [Centered-Z Photo Gallery](https://www.reddit.com/r/3Dprinting/comments/19266bk/cartesian_centered_z_mod_tramming_and_z_wobble)
- [Short Video Clip](https://www.youtube.com/watch?v=bj_Ha_a9KHw)
- [David Orlo's YouTube Channel](https://www.youtube.com/@DavidMiOo)




# Centered-Z Mod: Rev.2
# Great for Bowden Setups
# 100% Eliminate Z-wobble (The Lead Screw Doesn't Spin)
# Consistent  Tram & Level
# Increased Z resolution
# Further Increases to possible Z Speed up to 5x

- This is the second revision of the Centered-Z mod. 
- The first version served as a proof of concept, offering an easy solution with minimal modifications required.

### Parts and Resources / Links

#### Main Components:
1. Right Hand Extruder Mount (3D File below)
2. Lower Lead Screw Mount
3. Upper Stepper Motor Mount
4. Non-Captive Nema 17 Stepper Motor (Also known as Linear Stepper Motor)
5. Lead Bushing (e.g., Oldham)
6. Lead Nut POM
7. 10mm ID Collar/Clamp to prevent rod spinning

#### Suggested Parts:
- 4mm Lead screw (not required but recommended)
- Oldham bushing for Lead Screw mount (useful if screw and motor aren't perfectly aligned)

#### Part Examples:
(Note: I don't benefit from these links; they are for reference and purchase if needed)
- [Stepper | Nema 17 | Lead Screw](https://www.aliexpress.us/item/3256803648260596.html?spm=a2g0o.productlist.main.103.326f35bbLO30vd&algo_pvid=97efe516-a016-4d0b-8e66-21029317047c&algo_exp_id=97efe516-a016-4d0b-8e66-21029317047c-51&pdp_npi=4%40dis%21USD%2119.00%2118.62%21%21%2119.00%2118.62%21%40210318b917053565121418467e054d%2112000027301681696%21sea%21US%212909867875%21&curPageLogUid=RkxrJtfhheEm&utparam-url=scene%3Asearch%7Cquery_from%3A)
- [Top Stepper Motor Mount](https://www.aliexpress.us/item/3256802878774335.html?spm=a2g0o.productlist.main.11.a9b2467crCiumx&algo_pvid=faaf2824-1438-49bb-88e7-a02e20a4cc50&algo_exp_id=faaf2824-1438-49bb-88e7-a02e20a4cc50-5&pdp_npi=4%40dis%21USD%212.06%211.11%21%21%212.06%211.11%21%402101f49b17053567668596885e5dce%2112000030218719101%21sea%21US%212909867875%21&curPageLogUid=LItJ7Zed5iVa&utparam-url=scene%3Asearch%7Cquery_from%3A)
- [Bottom Lead Screw Mount](https://www.aliexpress.us/item/3256801123455446.html?spm=a2g0o.productlist.main.87.a9b2467crCiumx&algo_pvid=faaf2824-1438-49bb-88e7-a02e20a4cc50&algo_exp_id=faaf2824-1438-49bb-88e7-a02e20a4cc50-43&pdp_npi=4%40dis%21USD%216.43%214.50%21%21%216.43%214.50%21%402101f49b17053567668596885e5dce%2112000015653351825%21sea%21US%212909867875%21&curPageLogUid=tfiy9nrBjFNc&utparam-url=scene%3Asearch%7Cquery_from%3A)
- [Z-Lead Stay Collar](https://www.aliexpress.us/item/3256805778216004.html?spm=a2g0o.productlist.main.59.52e01efcJVA9Wq&algo_pvid=644c6a9d-fe33-4dfe-908d-d30a7ab86a65&aem_p4p_detail=20240115141855841042356289920002137125&algo_exp_id=644c6a9d-fe33-4dfe-908d-d30a7ab86a65-29&pdp_npi=4%40dis%21USD%214.49%213.59%21%21%214.49%213.59%21%402101df8a17053571350367077e3537%2112000035080149652%21sea%21US%212909867875%21&curPageLogUid=69KWOvVsCKKN&utparam-url=scene%3Asearch%7Cquery_from%3A&search_p4p_id=20240115141855841042356289920002137125_6)
- [POM Lead Nut](https://www.aliexpress.us/item/2251832714527198.html?spm=a2g0o.productlist.main.11.1e594c54MQrz2X&algo_pvid=edf11102-2131-4d93-8de0-5d6c2e65703b&algo_exp_id=edf11102-2131-4d93-8de0-5d6c2e65703b-5&pdp_npi=4%40dis%21USD%215.00%215.00%21%21%215.00%215.00%21%402101f49717053572273783292e7682%2165830829557%21sea%21US%212909867875%21&curPageLogUid=i7aKhFmRWhrg&utparam-url=scene%3Asearch%7Cquery_from%3A)
- [Oldham Bushing for Lead Screw](https://www.aliexpress.us/item/3256805721528606.html?spm=a2g0o.productlist.main.1.64d41289rBEist&algo_pvid=490784c4-f71d-4501-b8ef-eb7748156f04&algo_exp_id=490784c4-f71d-4501-b8ef-eb7748156f04-0&pdp_npi=4%40dis%21USD%219.16%213.30%21%21%2165.51%2123.60%21%402101df8a17053573430538818e3524%2112000034799746254%21sea%21US%212909867875%21&curPageLogUid=FdFdl59bYIPw&utparam-url=scene%3Asearch%7Cquery_from%3A)

#### 3D File Design Iterations:
3D Parts marked "Rev.X" are for iteration tracking (not in reference to a specific mod). "Final" indicates no further improvements planned.
These are designed to fit on 2020/2040 Aluminum and should clear most roller and belt setups on the X gantry.

#### 3D Files Availability:
- [Tinkercad (Login Required)](https://www.tinkercad.com/users/0RxhGZwzXXM-david-m-orlo)
- [Thingiverse Designs](https://www.thingiverse.com/a_makers_life/designs)
- [Printables Profile](https://www.printables.com/@DavidmOrlo_1689053)

### Visual Resources
- [Centered-Z Photo Gallery](https://www.reddit.com/r/3Dprinting/comments/19266bk/cartesian_centered_z_mod_tramming_and_z_wobble)
- [Short Video Clip](https://www.youtube.com/watch?v=QR7mz33CQAs)



# Centered-Z Mod: Rev.3
# Ideal for Direct Drive Setup 
# Beautifully Minimalistic Design Approach

- This is the version that was envisioned originally by its creator David Orlo
- Absolute centered-design, this time taking things a step further and centering the X stepper and Y Stepper motors in addition to the Z stepper
- Why the Y Steper you ask? See what I did there? 
- Noise and space saving, most of the time the Y stepper hangs off the printer and causes the printer to have a larger footprint than necessary. In addition to this, I've found that relocating the Y Stepper to a more centralized position reduced noise levels generated by that stepper significantly.
- On my Anycubic printer this was the noisiest stepper by a fair margin. The aluminum extrusion would resonated it certain frequencies and it was unbearable enough that I would alter my print speeds to avoid specific resonances.
