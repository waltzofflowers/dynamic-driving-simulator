# Earth's Geometry and Coordinate System

## Latitude and Longitude

### Latitude
- **Latitude lines** are parallel to each other and run horizontally around the globe.
- The **Equator** is at 0° latitude.
- The **North Pole** is at 90° North, and the **South Pole** is at 90° South.
- The distance between two lines of latitude is always approximately **111.32 kilometers** or **111,320 meters**, no matter where you are on Earth.

### Longitude
- **Longitude lines** converge at the **North** and **South Poles** and are widest apart at the **Equator**.
- The distance between two lines of longitude varies depending on the latitude. The greatest distance between two lines of longitude is at the Equator, and this distance shrinks as you move towards the poles.

## Calculations for Longitude and Latitude

### Longitude

1. At the **Equator**, 1 degree of longitude is about **111.32 kilometers** (or **111,320 meters**).
2. As you move towards the poles, the distance between two lines of longitude decreases. The formula to calculate the distance between two lines of longitude is:

        Change in Longitude = 111,320 meters × cos⁡(latitude in radians) (1)


- **111,320 meters** represents the distance per degree of longitude at the Equator.
- **cos(latitude)** reduces this distance as you move north or south of the Equator. At the Equator (latitude 0°), **cos(0°) = 1**, meaning the distance per degree of longitude is largest. At the poles (latitude 90° North or South), **cos(90°) = 0**, meaning degrees of longitude collapse to a point.

#### Example:
- **At the Equator (0° latitude)**, 1 degree of longitude = **111,320 meters**.
- **At 40° North latitude**, the cosine of 40° is approximately **0.766**. So, 1 degree of longitude would be approximately:

        111,320 × 0.766 ≈ 85,430 meters (2)
        

### Latitude

- The distance between two lines of latitude is the same at all locations on Earth because the Earth is nearly spherical.
- **1 degree of latitude** is always **111.32 kilometers** or **111,320 meters**, regardless of your location on the Earth.
- To calculate the change in latitude, we can directly use:

        Change in Latitude = Vertical Displacement / 111,320
    

This is simpler because the distance per degree of latitude does not change depending on the position on Earth.

## Summary of Key Points

- **Latitude** lines are evenly spaced and always represent a distance of **111,320 meters** per degree, regardless of location.
- **Longitude** lines are widest at the Equator and shrink in distance as you approach the poles. The distance between lines of longitude at a specific latitude can be calculated using the formula (1) above. Where **cos(latitude)** scales the distance as you move away from the Equator.
