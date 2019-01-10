# Setting up your equipment profile

To set up your Equipment profile, select the Profiles page from the menu. Click Equipment, and add a new profile, or edit the default profile.

![Equipment profile is customizable to get the right numbers for your system](../.gitbook/assets/image%20%2844%29.png)

**Name:** Name for your equipment profile

**Boil Time:** Boil time for this equipment profile, if you adjust boil time when "Calc boil volume" is activated, the pre-boil volume will change to match the new boil time based on boiloff.

**Description:** Free text field for details about the equipment.

## Volumes

**Batch Volume Target:** Select if you want your Batch Volume to match final volume in fermenter \(recommended\), or end of boil kettle volume.

**Batch Volume:** Your final batch volume target, a factor in calculating your Original Gravity.

**✔ Calc boil volume:** Automatically calculates your Pre-Boil Volume if this is active calculated back from batch volume. Based on your boiloff rate and trub/chiller loss, and 4% shrinkage.

**Pre-Boil Volume:** Set your pre-boil volume manually or have it calculated automatically \(recommended\). This volume is measured at near boiling temp \(after expansion\). **Post-Boil Volume** is also measured at boiling temp \(before chill\).

**Boil Off:** How much you boiloff per hour with your setup, important factor in calculating Pre-Boil Volume.

**Trub/Chiller Loss:** How much you loose in trub/chilling from kettle to fermenter, important factor in brewhouse efficiency. Total volume of the trub left in the kettle and/or cooler, including hop trub.

**Mash-Tun Deadspace:** Recoverable deadspace volume in your mash-tun, used for calculating mash water amount. In a system with a malt pipe, it is the volume before the water reaches the bottom of the malt pipe. Usually 0 in BIAB.

**Mash-Tun Loss:** **Unrecoverable** deadspace volume in your mash-tun and/or mash volume lost in your mash process. This is usually 0 in a one-vessel setup. A factor in mash efficiency.

**Fermenter Loss:** Expected loss from fermenter to bottle/keg. 

**HLT Deadspace** is any dead space in the Hot Liquor Tank \(Sparge Water Heater\). For example, if you use a sparge water heater that has the tap that draws higher than the bottom of the pot, you can set the liters that are not drawn. This volume will be added to the sparge water amount in the Water Adjustment Calculator, for calculating your sparge water additions.

## Efficiency

**Brewhouse Efficiency:** The overall efficiency of you system - includes all losses to the fermenter. Important factor in calculating you Original Gravity. If you don't know you system, a good number to start with might be 65-75%. And you can dial in your excact efficiency after a couple of brews.

**Mash Efficiency:** The efficiency of your mash procedure, up to pre-boil, including sparging. Important factor in calculating your Pre-Boil Gravity.

It is recommended to automatically calculate your mash efficiency by enabling the **Calc mash efficiency** checkbox.

## Advanced

**Hop Utilization:** Normally left at 100%. Average hop utilization for your equipment. This is a global multiplier to the IBU calculation.

**Aroma Hop Utilization:** For calculating IBU on hopstand/whirlpool hops, also used as a factor to calculate increased IBU from boil hops when you have a hopstand. This utilization is used only when no temperature is entered separately on the hop-stand/whirlpool hop in the recipe.

**✔ Calc aroma hop utilization:** If checked, it will automatically your Aroma Hop Utilization based on the entered Hopstand Temperatuer. 

**Hopstand Temperature:** The average temperature of your hopstand, used to automatically calculate your _Aroma Hop Utilization_ when _Calc aroma hop utilization_ is checked. This is also displayed in the brew sheet.

## Mash and sparge water

**Grain Absoprtion Rate**: Amount of water absorbed by the grain per unit of grain. L/kg when using metric units, and qt/lb when using gal/lbs as volume/weight units.

**Water/Grain Ratio**: Amount of effective mash water per unit of grain. L/kg when using metric units, and qt/lb when using gal/lbs as volume/weight units.

**Mash/Sparge Water Calculation Method**:  
  **Default**: Normal calculation of mash/sparge water amounts.  
  **No Sparge**: No sparge, full mash volume.  
  **Custom**: Define your own custom formula. Formulas must result in water amount in Liter.

### Mash Water/Volume

_Settings for calculating mash water_

**✔ Include grain volume in mash limits**: When this is checked the min and max mash **water** limit turns into mash **volume** limit. Which means that the wet mash grain volume is included in the numbers. Then the max mash volume limit becomes the mash-tun max capacity.

**Min:** Minimum limit of mash water, **Max:** Maximum limit of mash water

If the calculated mash water is under the minimum limit, it will take water from the sparge water amount and move it to increase the mash volume, dynamically increasing your water/grain ratio.

If the calculated mash water is over the maximum limit, it will move water to sparge or top-up water to not exceed the limit, dynamically decreasing your water/grain ratio.

### Sparge Water Limit

Use this to avoid getting to much sparge water calculated, if you have limited room in your HLT.

**Max:** Maximum amount of room in your HLT / Sparge Water Heater.

**Overflow Taget:**   
  **Top-Up:** overflow is moved to top-up water \(boil\).  
  **Mash:** If the calculated sparge water amount is above the limit, it will move water to mash \(until maximum mash volume is reached\) and/or top-up water to not exceed the limit.

### Strike Water Temperature

**✔ Calc strike water temperature:** When this is checked a calculated strike temperature is added as a first step in your mash schedule.

**Mash-Tun Heat Capacity in** _**L equivalient water volume**_**:** If your mash-tun is pre-heated set heat capacity to 0. Otherwise use the **Mash-Tun Calibration tool** to get the value for your equipment.

### Sparge Temperature

Enter your desired sparge temperature.

### 

