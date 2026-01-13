---
layout: archive
title: "PhD Research"
permalink: /research/
author_profile: true
---

<style>
  body {
    text-align: justify;
  }
  .author__bio {
    text-align: left !important;
  }
</style>

My research project has revolved around developping and studying new landing technologies for drones to enable them to land safely in harsh outdoor conditions. The project started because of one main challenge that most small multirotors face: They are typically designed to land in undisturbed, predictable conditions and on horizontal, human-made surfaces. To be as lighweight as possible, multirotors often have rigid landing gears that act as a spring during the impact from landing, especially at faster descent speeds, which can make the landing phase very risky if there is any inclination of the landing surface.
Unfortunately, the real outdoor world is not often perfectly even and horizontal, and a lot of new potential drone applications would benefit from a more robust and reliable landing technology. As it is right now, landing is still often considered as the most challenging phase of a drone mission. 
<!-- something like 66% of mission failures and crashes happen during takeoff or landing (K. W. Williams et al., 2004).  -->
For my PhD research, I decided to explore how the use of a friction-based damping landing gear, combined with thrust reversal at impact, could expand the landing envelope of multirotors and enable safer missions in harsh outdoor conditions.  

The project is broken down into 3 phases: Phase 1 focusses on using friction and reverse thrust to land rapidly on inclined surfaces such as rooftops. Phase 2 studies how a similar technology can be ported to landings on fast-moving vehicles (such as a 120 km/h pickup truck on the highway) or vehicles moving in rough, unpreditable terrain (boats, ATVs). Phase 3 explores the design of novel feet made of opposing retractable spikes and added to the landing gear legs to land on steeply inclined ice surfaces such as glaciers and icebergs. Keep scrolling to see all of our cool demonstrations!
<!-- Such a technology could make the UAV missions a lot safer and could potentially contribute to the creation of new drone applications in the real world. -->

## Phase 1: Friction-Based Dampers and Reverse Thrust to Land Multirotors on Steep Rooftops
Small multirotors are typically not capable of landing in complex situations, such as on inclined surfaces, in wind gusts or at high impact velocities. 
In phase 1 of my PhD research, I explored the use of lightweight friction shock absorbers, combined with rapid thrust reversal, to increase the landing envelope of small quadrotors. The friction shock absorbers serve to dissipate the drone’s kinetic energy and the reverse thrust increases the maximum slope inclination at which it can land. 
I designed a landing gear prototype and implemented it to a DJI F450 drone. The friction shock absorber design consists of multiple parallel disks that rotate relative to each other during impact to generate friction, while a small 10-g DC motor with a higly-reduced gearbox applies a compression force on the disks to adjust the friction torque. Current sensors allow precise adjustement of the friction torque, and small torsion springs in the system allow a reset of the legs to their initial position when friction is removed from the disks.
Meanwhile, my research partner (John Bass) created a 2D model of the drone and legs to generate landing maps and to evaluate the benefits of using friction shock absorbers and reverse thrust. 
Finally, we tested the technology in real outdoor conditions. The overall system enables drones to safely land on surfaces of up to 60° and at vertical speeds of up to 2.75 m/s, thus increasing the landing envelope by a factor of 8, compared to traditional multirotors.  
The video below shows our landing technology in real-world scenarios!

<iframe width="560" height="315" src="https://www.youtube.com/embed/tG1K_63q00Y" frameborder="0" allowfullscreen></iframe>

For more information on that part of my project, [go check out my paper](https://ieeexplore.ieee.org/abstract/document/9779538){:target="_blank"} published in *IEEE Robotics and Automation Letters* (2022 edition) or <a href="/files/paper1_landingOnRooftops.pdf" download target="_blank">download it</a> here.


## Phase 2: Upgraded Friction Shock Absorbers and Reverse Thrust to Land on High-Speed Ground Vehicles
Typical landing gears of small UAVs limit their capability to land on vehicles moving at more than 20‐50 km/h due to high drag, high pitch angles and potentially high relative horizontal velocities. To enable landing at higher speeds, we studied how our same combination of lightweight friction shock absorbers and reverse thrust could simplify the entire landing sequence. We designed a new lightweight friction-based damping landing gear that allows for for rapid descents (i.e., 3 m/s) toward the vehicle. For the purpose of this study, we also designed a new custom high-power drone to fly at 130 km/h, and programmed a simple leveling maneuver to level the drone at the last instant before impact. Simulations show that the proposed system is (1) more robust at higher descent speed contrary to traditional configurations, (2) can touchdown at almost any time during the leveling maneuver, thus reducing the timing constraints, and (3) is robust to many environmental, design and operational factors, maintaining a success rate above 80% at up to 100 km/h. Compared to standard multirotors, this approach expands the possible states envelope at touchdown by a factor of 60. A total of 38 experimental trials were conducted where a drone  successfully landed on a pickup truck moving at speeds ranging from 10 to 110 km/h.

<!-- Drone design, landing gear design, 2D model and controller, Monte Carlo Simulations (sensitivity analysis). -->

The video below demonstrates the achieved performances of the landing technology. We rented a dragway race track near Montreal (Canada) for a day to conduct a total of 38 experimental trials, where our drone successfully landed on a pickup truck moving at speeds ranging from 10 to 110 km/h!

<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/OHBPAHqLN08" frameborder="0" allowfullscreen></iframe> -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/tTUVr1Ogag0" frameborder="0" allowfullscreen></iframe>

<!-- For more information on how we landed our drone on high-speed vehicles, [go check out this paper](https://onlinelibrary.wiley.com/doi/10.1002/rob.70069){:target="_blank"} published in *Journal of Field Robotics* (2025 edition) or <a href="/files/paper2_landingOnVehicles.pdf" download target="_blank">download it</a> here. -->

**Landing on an Trailer in Rough Terrain**  
With robust control and precise tracking of the ground vehicle, achieving similar landing performance to what I described earlier is likely possible. However, when the vehicle moves over rough and unpredictable terrain, precisely timing the maneuver and syncing the drone’s descent with the vehicle’s motion becomes much more challenging. That's where having a damping landing gear and reverse thrust greatly simplifies the autonomous landing sequence! In the following demo, we successfully landed our drone autonomously on a trailer pulled by a Warthog over rough terrain during our field trials at the *NSERC Canadian Robotics Network* ([NCRN](https://ncrn-rcrc.mcgill.ca/){:target="_blank"}), near Toronto (Canada).  
Big thanks to [Clearpath Robotics](https://clearpathrobotics.com/){:target="_blank"} for lending us the Warthog!

<iframe width="560" height="315" src="https://www.youtube.com/embed/jA9Zfpel1O8" frameborder="0" allowfullscreen></iframe>  
<br> <!-- Adds vertical space -->

**Landing on a High-Speed Canoe**  
As a fun experiment, during the 2024 field trials of the *NSERC Canadian Robotics Network*, we decided to test our technology in riskier conditions... We mounted a platform on a canoe and autonomously landed our drone on it while it was being towed at 30~km/h by an electric motor! No crashes!
<iframe width="560" height="315" src="https://www.youtube.com/embed/E-ns-MxMJvU" frameborder="0" allowfullscreen></iframe>  
<br>

<!-- 
**Landing on a Vehicle on an Off-Road Path in the Forest**  
Using the same global system (DART UAV and target beacon mounted on pickup truck), we also demonstrated how our landing technology can enable a drone to land on a pickup truck moving on a rough dirt road in a forest near Sherbrooke (Quebec, Canada). On bumpy roads, the pickup undergoes strong vertical accelerations which can result in faster or slower impact speeds. Without the proper landing technology, this can easily result in a mission failure!

<iframe width="560" height="315" src="https://www.youtube.com/embed/_EjhQPquMnw" frameborder="0" allowfullscreen></iframe>  
<br>

**Landing on a Vehicle in an Urban Setting**  
Finally, we also demonstrated a landing sequence on a moving vehicle in an urban setting, at the *Interdisciplinary Institute for Technological Innovation* (Université de Sherbrooke). A simplified robust landing strategy could open facilitate the implementation of scenarios such as hybrid ground-air delivery, where a drone handles last-mile drop-offs before returning to the ground vehicle for the ride back, or multi-city missions where a drone hitches a ride to conserve power. power consumption before the mission. While our focus was mainly on the landing gear, it’s always exciting to imagine the broader applications!

<iframe width="560" height="315" src="https://www.youtube.com/embed/hJn3TGY4muU" frameborder="0" allowfullscreen></iframe>   -->
  
## Phase 3: Spike-Equipped Friction Shock Absorbers and Reverse Thrust to Land on Steep Iceberg and Glacier Slopes
In Phase 3 of my PhD research, I focused on designing specialized spiked feet to enable drones to land on steep ice surfaces, such as glaciers and icebergs. Once again, friction-based shock absorbers proved essential for dampening impact energy and maintaining constant contact between the spikes and the ice, preventing rebounds. Reverse thrust was also critical, as it provided the necessary pressure to keep the spikes engaged during the drone's post-impact sliding and braking. The spikes were designed to be retractable (inspired from cats!) so the drone can land facing either upward or downward. The proposed solution enabled successful landings on 24 icebergs and glaciers in Iceland during a two-week field trial.

The official demo video is coming soon!

<div style="display: flex; gap: 10px; margin-bottom: 10px;">
  <img src="../images/droneOnIceberg3.png" alt="Drone landed on iceberg" style="width: 48%; border: 0.5px solid black;">
  <img src="../images/droneOnGlacier.jpg" alt="Drone landed on glacier" style="width: 48%; border: 0.5px solid black;">
</div>

<div style="display: flex; justify-content: center;">
  <img src="../images/droneOnIceberg2.jpg" alt="Drone coasted in Iceland" style="width: 48%; border: 0.5px solid black;">
</div>

<!-- The ability to land and stay on icebergs for long periods of time could enable the use of drones as remote sensors to track and monitor large icebergs coming towards offshore oil rigs in Eastern Canada's coastal regions, allowing companies to react proactively to avoid collisions and oil leaks in the ocean. These UAV-based missions have been explored by companies like C-Core in the past to replace current expensive solutions using manned aircraft to manually track incoming icebergs, but placing beacons or drones on icebergs has proven very challenging, due to the strong winds, slippery surfaces and icebergs' inherit risk of rolling. Placing a drone on a straight surface instead of an inclined one can also be dangerous because water puddles will form in these lower areas during warmer days. 
UAVs capable of landing on steep ice and snow could also be beneficial to explorers or rescue teams as a deployable tool to detect avalanches or weak ice structures in higher risk areas, and is also very relevant to space exploration, as extra-terrestrial robots often need to deal with icy/snowy terrain.
To deal with the challenging conditions of ice, I redesigned a new high-power drone (Thrust-to-Weight of 7) equipped with the same friction-based damping landing gear as used in previous work, and with the same reverse thrust implementation. I modified the feet of the landing gear with new specilized feet that use opposite retractable spikes made of hardened high-speed tool steel to penetrate the ice. These special feet allow the drone to successfully land at any yaw orientation relative to the slope, at angles up to 60°.
The novel landing strategy was field tested during 2 weeks in Iceland, in Solheimjokull and in Glacier Lagoon (Vatnajokull glacier), where managed to land the drone on 22 icebergs and 2 glaciers with zero crash.
The public demonstration video is coming, along with our paper on that topic! -->


