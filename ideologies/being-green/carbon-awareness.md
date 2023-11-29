# Energy Efficiency

## Contents

- [Introduction](#introduction)
- [The key concepts](#the-key-concepts)
  - [Carbon intensity](#carbon-intensity)
  - [Variability of carbon intensity](#variability-of-carbon-intensity)
  - [Dispatchability and curtailment](#dispatchability-and-curtailment)
  - [Marginal carbon intensity](#marginal-carbon-intensity)
  - [Energy markets](#energy-markets)
- [How to be more carbon aware](#how-to-be-more-carbon-aware)
  - [Demand shifting](#demand-shifting)
  - [Spatial shifting](#spatial-shifting)
  - [Temporal shifting](#temporal-shifting)

## Introduction

Not all electricity is produced in the same way. In different locations and times, electricity is generated using a variety of sources with varying carbon emissions. Some sources, such as wind, solar, or hydroelectric, are clean, renewable sources that emit little carbon. On the other hand, fossil fuel sources emit carbon at varying degrees to produce electricity. For example, both gas and coal emit more carbon than renewable sources, but gas-burning power plants emit less carbon than coal-burning power plants.

Carbon awareness is the idea of doing more when more energy comes from low carbon sources and doing less when more energy comes from high carbon sources.

## The key concepts

### Carbon intensity

Carbon intensity measures how much carbon (CO2e) is emitted per kilowatt-hour (KWh) of electricity consumed. The standard unit of carbon intensity is gCO2eq/kWh, or grams of carbon per kilowatt hour.

If your computer is plugged directly into a wind farm, its electricity would have a carbon intensity of 0 gCO2eq/kWh since a wind farm emits no carbon to produce that electricity. However, most people can't plug directly into wind farms; instead, they plug into power grids supplied with electricity from various sources.

Once on a grid, you can't control which sources supply the electricity you are using; you simply get a mix of everything. So, your carbon intensity will be a mix of all the current power sources in a grid, both the lower- and the higher-carbon sources.

### Variability of carbon intensity

Carbon intensity varies by location since some regions have an energy mix containing more clean energy sources than others.

Carbon intensity also changes over time due to the inherent variability of renewable energy caused by the unpredictability of weather conditions. For example, when it's cloudy or the wind isn't blowing, carbon intensity increases since more of the electricity in your mix comes from sources that emit carbon.

### Dispatchability and curtailment

Electricity demand varies during the day, and supply always needs to be able to meet that demand. A brownout (a dip in the voltage level of the power line) occurs if a utility doesn't produce enough electricity to meet demand. Conversely, if a utility produces more electricity than is required, then to stop infrastructure burning out, breakers trip and we have blackouts.

There needs to be a balance between the demand and supply of electricity at all times and the responsibility for this usually falls to the utility provider.

In the case of fossil fuels such as coal, it is easier to control the power produced for this supply; this is called dispatchability. However, in the case of renewable power sources such as wind farms, the power produced cannot easily be controlled (we can't control how much the wind blows). If the power source produces more electricity than is needed, that electricity is thrown away; this is called curtailment.

### Marginal carbon intensity

If you suddenly need to access more power - for example, you need to turn on a light - that energy comes from the marginal power plant. The marginal power plant is dispatchable, which means marginal power plants are often powered by fossil fuels.

Marginal carbon intensity is the carbon intensity of the power plant that would have to be employed to meet any new demand.

Fossil-fueled power plants rarely scale down to 0. They have a minimum functioning threshold, and some don't scale; they are considered a consistent, always-on baseload. Because of this, we sometimes have the scenario where we curtail (throw away) renewable energy while still consuming energy from fossil fuel power plants.

In these situations, the marginal carbon intensity will be 0 gCO2eq/kWh since we know that any new demand will match the renewable energy we are curtailing.

### Energy Markets

When the demand for electricity goes down, utilities need to reduce the supply to balance supply and demand. They can do this in one of two ways:

1. Buy less energy from fossil fuel plants
   - Energy from fossil fuel plants is usually the most expensive so this is the preferred method. This directly translates to burning fewer fossil fuels.
2. Buy less energy from renewable sources
   - Renewable sources are the cheapest, so they prefer not to do this. If a renewable source doesn't manage to sell all of its electricity, it has to throw the rest away.

Reducing the amount of electricity consumed in your applications can help decrease the energy's carbon intensity seeing as the first thing to be scaled back are fossil fuels.

When the demand for electricity goes up, utilities need to increase the supply to balance supply and demand.

## How to be more carbon aware

There is a global transformation happening right now. All around the world, electricity grids are changing from primarily burning fossil fuels to sourcing energy from lower carbon sources like wind and solar. This is one of our best hopes for meeting our global reduction targets. As green software practitioners, let's see some of the ways we can help accelerate that transition.

The primary driver for the transition is economic rather than any sustainability target. Renewables are winning because they are cheaper and getting even more affordable over time. So, to help accelerate the transition, we need to make renewable plants more profitable and fossil fuel plants less profitable. The best way to do that is to use more electricity when it's coming from lower-carbon sources like renewables and less electricity when it's coming from higher-carbon sources.

Carbon intensity is lower when more energy comes from lower-carbon sources and higher when it comes from higher-carbon sources.

### Demand shifting

Being carbon aware means responding to shifts in carbon intensity by increasing or decreasing your demand. If your work allows you to be flexible with when and where you run workloads, you can shift accordingly - consuming electricity when the carbon intensity is lower and pausing production when it is higher. For example, training a Machine Learning model at a different time or region with much lower carbon intensity.

Studies show these actions can result in 45% to 99% carbon reductions depending on the number of renewables powering the grid.

Demand shifting can be further broken down into spatial and temporal shifting.

Demand shifting is the strategy of moving computation to regions or times when the carbon intensity is lowest. Demand shaping is a similar strategy. However, instead of moving demand to a different region or time, we shape our computation to match the existing supply.

### Spatial shifting

Spatial shifting means moving your computation to another physical location where the current carbon intensity is lower. It might be a region that naturally has lower carbon sources of energy. For example, moving to different hemispheres depending on the season for more sunlight hours.

### Temporal shifting

If you can't shift your computation spatially to another region, another option you have is to shift to another time. Perhaps later in the day or night when it's sunnier or windier and, therefore, the carbon intensity is lower. This is called temporal demand shifting. We can predict future carbon intensity reasonably well through advances in weather forecasting.
