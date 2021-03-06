---
layout: default
title: Supernode 2
category: Networking
---

Supernode 2 (node 570) is located at 1196 Metropolitan Avenue in Brooklyn New York. The installation provides mesh and internet connectivity for building residents as well as some areas of the East Williamsburg and Bushwick neighborhoods.

## Status

[https://stats.570.nycmesh.net](https://stats.570.nycmesh.net)

## Coverage

<img title="Coverage area" src="../assets/images/nycmesh-570-coverage.jpg">

## Photos

<img title="The radios" src="../assets/images/nycmesh-570-radios.png" style="width:49.7%;">
<img title="Point-to-point link to node 227" src="../assets/images/nycmesh-570-227-link.png" style="width:49.7%;">
<img title="The router" src="../assets/images/nycmesh-570-router.png" style="width:49.7%;">
<img title="Battery backup" src="../assets/images/nycmesh-570-battery.png" style="width:49.7%;">

## Hardware

<style>
section td {
  width: 33.33%;
}
</style>

|Description|Model|Manufacturer|Quantity|
|-----------|-----|------------|---:|
| Router | Hex PoE | Mikrotik | 1 |
| Point-to-point radio | AirFiber 24 | UBNT | 1 |
| Point-to-point radio | Nanobeam AC | UBNT | 1 |
| Wide area AP | LiteAP 120 | UBNT | 2 |
| Indoor AP | UniFi AP | UBNT | 1 |
| Application server | Raspberry Pi | RPi Foundation | 1 |
| Inverter/Charger/ATS | APS700HF | Tripp Lite | 2 |
| Battery | EXP12180 | ExpertPower | 1 |

## Schematic

<img title="Schematic" src="../assets/images/nycmesh-570-schematic.png">

## Backhaul

A pair of AirFiber 24s was donated to NYC Mesh and was deployed between 227 and 570 to provide Brooklyn with a near 1Gbps backhaul link to Supernode 1, the Manhattan area of the mesh and the internet.

<img title="Deploying an AF24 at node 227" src="../assets/images/nycmesh-570-227-link-2.png" style="max-width:480px;">

## Battery backup

Shortly after initial installation we noticed the node would go down on a somewhat regular basis. After some investigation and discussion with building residents, the culprit was revealed to be a circuit breaker being tripped by power hungry air conditioners. To insulate the node against short power outages like this we built a simple backup power system out of a 12 volt battery and integrated inverter / charger / automatic transfer switch.

## Routing

570 currently uses BGP to exchange routes with its mesh peers. We hope to upgrade this node to support more dynamic routing protocols soon.
