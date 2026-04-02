# Instance Description for the case study based on an offshore oil spill accident

## 1. Overview

This instance is designed for the **Floating targets team orienteering problem with arrival-time-dependent profits (FTOPATP)**, capturing the key characteristics of dynamic oil spill response operations, including:

- Multi-depot configuration
- Time-dependent profit decay
- Drifting oil spill locations
- Dynamic service (containment) time and required response resources

The instance consists of **3 depots** and **30 oil spill response tasks**, with associated spatial, temporal, and operational attributes.

---

## 2. Node Information

Each node in the instance is described by the following attributes:

| Field     | Description |
|----------|------------|
| ID       | Node identifier (Depot: D*, Customer: C*) |
| Type     | Node type (`d1`: depot, `c1`: oil slick sites) |
| Lat., Lon. | Geographic coordinates (WGS84) |
| x, y     | Projected coordinates (e.g., UTM) |
| profit   | Initial response profit |
| vx, vy   | Drift velocity in x and y directions (km/h) |
| k1       | Profit decay rate |
| k2       | Demand growth coefficient |
| k3       | Service time growth coefficient |
| Service  | Initial service time (h)|
| Demands  | Initial resource demand (t)|

---

## 3. Fleet Information

Definitions:

- Q: Max loading capacity of emergency fleets
- v:  Cruising speed of emergency fleets
- Tmax: Maximum duration of response work
- fleet_D0: Number of emergency fleets that can be dispatched
---

## 4. Example Data Row Interpretation
**Example Node:**
- **Node**: C1
- **Type**: c1
- **Lat**: 38.3818
- **Lon**: 121.7357
- **x**: 337785.62
- **y**: 4290688.72
- **profit**: 2350000
- **vx**: 1.23599
- **vy**: -0.05907
- **k1**: 58800
- **k2**: 2.34
- **k3**: 0.09
- **Service**: 1.42
- **Demands**: 50

