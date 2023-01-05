---
layout: post
title: Geospatial analytics
---

With the rise of IoT, GPS tracking is more available. Take for example a transport vehicle moving some materials. The geolocation data can tell us more than just where the vehicle is. Using geospatial analytics we can observe the mobility patterns of the vehicle. Clustering the data results in places where the vehicle stopped for work or parking. Geospatial analytics can tell us if the vehicle is working, find the optimal route, spot any unusual behaviour of the vehicle (e.g. unexpected stop), what materials are where and much more. 
<div class="imgFloatContainer">
    <div class="imgFloat">
        <img src="/images/sites_orig.png" width="200"/>
    </div>
    <div class="imgFloat">
        <img src="/images/traj.gif" width="200"/>
    </div>
</div>

The above animation was done using Kepler.gl library, which is very handy for geospatial visualizations and mobility data. It can handle high amounts of data points, which is often the issue with high-frequency GPS data.