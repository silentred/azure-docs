---
title: 'Locations and connectivity providers: Azure ExpressRoute | Microsoft Docs'
description: This article provides a detailed overview of locations where services are offered and how to connect to Azure regions. Sorted by location.
services: expressroute
documentationcenter: na
author: cherylmc
manager: timlt
editor: ''

ms.assetid: feb67da3-5abc-4acb-bad4-f78e3c541ded
ms.service: expressroute
ms.devlang: na
ms.topic: conceptual
ms.tgt_pltfrm: na
ms.workload: infrastructure-services
ms.date: 09/03/2019
ms.author: cherylmc
---
# ExpressRoute partners and peering locations

> [!div class="op_single_selector"]
> * [Locations By Provider](expressroute-locations.md)
> * [Providers By Location](expressroute-locations-providers.md)


The tables in this article provide information on ExpressRoute geographical coverage and locations, ExpressRoute connectivity providers,and ExpressRoute System Integrators (SIs).

> [!Note]
> Azure regions and ExpressRoute locations are two distinct and different concepts, understanding the difference between the two is critical to exploring Azure hybrid networking connectivity. 
>
>

## Azure regions
Azure regions are global datacenters where Azure compute, networking and storage resources are located. When creating an Azure resource, a customer needs to select a resource location. The resource location determines which Azure datacenter (or availability zone) the resource is created in.

## ExpressRoute locations
ExpressRoute locations (sometimes referred to as peering locations or meet-me-locations) are co-location facilities where Microsoft Enterprise edge (MSEE) devices are located. ExpressRoute locations are the entry point to Microsoft’s network – and are globally distributed, providing customers the opportunity to connect to Microsoft’s network around the world. These locations are where ExpressRoute partners and ExpressRoute Direct customers issue cross connections to Microsoft’s network. In general, the ExpressRoute location does not need to match the Azure region. For example, a customer can create an ExpressRoute circuit with the resource location *East US*, in the *Seattle* Peering location.

You will have access to Azure services across all regions within a geopolitical region if you connected to at least one ExpressRoute location within the geopolitical region. 

## <a name="locations"></a>Azure regions to ExpressRoute locations within a geopolitical region
The following table provides a map of Azure regions to ExpressRoute locations within a geopolitical region.

| **Geopolitical region** | **Zone** | **Azure regions** | **ExpressRoute locations** |
| --- | --- | --- | --- |
| **Australia Government** | 1 | Australia Central, Australia Central 2 |Canberra, Canberra2 |
| **Europe** | 1 |France Central, France South, North Europe, West Europe, UK West, UK South |Amsterdam, Amsterdam2, Copenhagen, Dublin, Frankfurt, London, London2, Marseille, Newport(Wales), Paris, Stockholm, Zurich |
| **North America** | 1 |East US, West US, East US 2, West US 2, Central US, South Central US, North Central US, West Central US, Canada Central, Canada East |Atlanta, Chicago, Dallas, Denver, Las Vegas, Los Angeles, Miami, New York, San Antonio, Seattle, Silicon Valley, Silicon Valley2, Washington DC, Washington DC2, Montreal, Quebec City, Toronto |
| **Asia** | 2 |East Asia, Southeast Asia |Hong Kong SAR, Kuala Lumpur, Singapore, Singapore2, Taipei |
| **India** | 2 |India West, India Central, India South |Chennai, Chennai2, Mumbai, Mumbai2 |
| **Japan** | 2 |Japan West, Japan East |Osaka, Tokyo |
| **Oceania** | 2 |Australia Southeast, Australia East |Auckland, Melbourne, Perth, Sydney | 
| **South Korea** | 2 |Korea Central, Korea South |Busan, Seoul|
| **UAE** | 3 | UAE Central, UAE North | Dubai, Dubai2 |
| **South Africa** | 3 |South Africa West, South Africa North |Cape Town, Johannesburg |
| **South America** | 3 |Brazil South |Sao Paulo |

## Azure regions and geopolitical boundaries for national clouds
The table below provides information on regions and geopolitical boundaries for national clouds.

| **Geopolitical region** | **Azure regions** | **ExpressRoute locations** |
| --- | --- | --- |
| **US Government cloud** |US Gov Arizona, US Gov Iowa, US Gov Texas, US Gov Virginia, US DoD Central, US DoD East  |Chicago, Dallas, New York, Phoenix, San Antonio, Seattle, Silicon Valley, Washington DC |
| **China East** |China East, China East2 |Shanghai, Shanghai2 |
| **China North** |China North, China North2 |Beijing, Beijing2 |
| **Germany** |Germany Central, Germany East |Berlin, Frankfurt |

Connectivity across geopolitical regions is not supported on the standard ExpressRoute SKU. You will need to enable the ExpressRoute premium add-on to support global connectivity. Connectivity to national cloud environments is not supported. You can work with your connectivity provider if such a need arises.

## <a name="partners"></a>ExpressRoute connectivity providers

The following table shows connectivity locations and the service providers for each location. If you want to view service providers and the locations for which they can provide service, see [Locations by service provider](expressroute-locations.md). 

**Local Azure Regions** are the ones that [ExpressRoute Local](expressroute-faqs.md) at each peering location can access. **n/a** indicates that ExpressRoute Local is not available at that peering location.


### Production Azure
| **Location** | **Owner and address** | **Local Azure regions** | **Service providers** |
| --- | --- | --- | --- |
| **Amsterdam** | [Equinix AM5](https://www.equinix.com/locations/europe-colocation/netherlands-colocation/amsterdam-data-centers/am5/) | West Europe | Aryaka Networks, AT&T NetBond, British Telecom, Colt, Equinix, euNetworks, GÉANT, InterCloud, Interxion, KPN, IX Reach, Level 3 Communications, Megaport, NTT Communications, Orange, Tata Communications, TeleCity Group, Telefonica, Telenor, Telia Carrier, Verizon, Zayo |
| **Amsterdam2** | [Interxion AMS8](https://www.interxion.com/Locations/amsterdam/schiphol/) | West Europe | CenturyLink Cloud Connect, DE-CIX, Colt, Interxion, Vodafone |
| **Atlanta** | [Equinix AT2](https://www.equinix.com/locations/americas-colocation/united-states-colocation/atlanta-data-centers/at2/) | n/a | Equinix, Megaport |
| **Auckland** | [Vocus Group NZ Albany](https://www.vocus.co.nz/business/cloud-data-centres) | n/a | Devoli, Kordia, Megaport, Spark NZ, Vocus Group NZ |
| **Busan** | [LG CNS](https://datacenter.lgcns.com/Contents/En/Menu_1/Locations_1.aspx) | Korea South | LG CNS |
| **Canberra** | [CDC](https://cdcdatacentres.com.au/content/about-cdc) | Australia Central | CDC |
| **Canberra2** | [CDC](https://cdcdatacentres.com.au/content/about-cdc) | Australia Central 2| CDC |
| **Cape Town** | [Teraco CT1](https://www.teraco.co.za/data-centre-locations/cape-town/) | South Africa West | Internet Solutions - Cloud Connect, Liquid Telecom, Teraco |
| **Chennai** | Tata Communications | South India | Global CloudXchange (GCX), SIFY, Tata Communications |
| **Chennai2** | Airtel | South India | Airtel |
| **Chicago** | [Equinix CH1](https://www.equinix.com/locations/americas-colocation/united-states-colocation/chicago-data-centers/ch1/) | North Central US | Aryaka Networks, AT&T NetBond, CenturyLink Cloud Connect, Cologix, Comcast, Coresite, Equinix, InterCloud, Internet2, Level 3 Communications, Megaport, PacketFabric, PCCW Global Limited, Sprint, Telia Carrier, Verizon, Zayo |
| **Copenhagen** | [Interxion CPH1](https://www.interxion.com/Locations/copenhagen/) | n/a | Interxion |
| **Dallas** | [Equinix DA3](https://www.equinix.com/locations/americas-colocation/united-states-colocation/dallas-data-centers/da3/) | n/a | Aryaka Networks, AT&T NetBond, Cologix, Equinix, Internet2, Level 3 Communications, Megaport, Neutrona Networks, Telmex Uninet, Telia Carrier, Transtelco, Verizon, Zayo|
| **Denver** | [CoreSite DE1](https://www.coresite.com/data-centers/locations/denver/de1) | West Central US | CoreSite, Megaport, Zayo |
| **Dubai** | [PCCS](https://www.pacificcontrols.net/cloudservices/index.html) | UAE North | Etisalat UAE |
| **Dubai2** | [du datamena](http://datamena.com/solutions/data-centre) | UAE North | du datamena, Orixcom |
| **Dublin** | [Equinix DB3](https://www.equinix.com/locations/europe-colocation/ireland-colocation/dublin-data-centers/db3/) | North Europe | Colt, eir, Equinix, Interxion, Megaport |
| **Frankfurt** | [Interxion FRA11](https://www.interxion.com/Locations/frankfurt/) | n/a | DE-CIX, Interxion, Orange |
| **Hong Kong SAR** | [Equinix HK1](https://www.equinix.com/locations/asia-colocation/hong-kong-colocation/hong-kong-data-center/hk1/) | East Asia | Aryaka Networks, British Telecom, CenturyLink Cloud Connect, Chief Telecom, China Telecom Global, Equinix, Megaport, NTT Communications, Orange, PCCW Global Limited, Tata Communications, Telia Carrier, Verizon |
| **Johannesburg** | [Teraco JB1](https://www.teraco.co.za/data-centre-locations/johannesburg/#jb1) | South Africa North | British Telecom, Internet Solutions - Cloud Connect, Liquid Telecom, Orange, Teraco |
| **Kuala Lumpur** | [TIME dotCom Menara AIMS](https://www.aims.com.my/co-location/points-of-presence.html) | n/a | TIME dotCom |
| **Las Vegas** | [Switch LV](https://www.switch.com/las-vegas) | n/a | CenturyLink Cloud Connect, Megaport |
| **London** | [Equinix LD5](https://www.equinix.com/locations/europe-colocation/united-kingdom-colocation/london-data-centers/ld5/) | UK South | AT&T NetBond, British Telecom, Colt, Equinix, InterCloud, Internet Solutions - Cloud Connect, Interxion, Jisc, Level 3 Communications, Megaport, MTN, NTT Communications, Orange, PCCW Global Limited, Tata Communications, Telehouse - KDDI, Telenor, Telia Carrier, Verizon, Vodafone, Zayo |
| **London2** | [Telehouse North Two](https://www.telehouse.com/global-data-centers/emea/london-data-centers/telehouse-north-two/) | UK South | IX Reach, Equinix |
| **Los Angeles** | [CoreSite LA1](https://www.coresite.com/data-centers/locations/los-angeles/one-wilshire) | n/a | CoreSite, Equinix, Megaport, Neutrona Networks, NTT, Zayo |
| **Marseille** |[Interxion MRS1](https://www.interxion.com/Locations/marseille/) | France South | DE-CIX, Interxion, Jaguar Network |
| **Melbourne** | [NextDC M1](https://www.nextdc.com/data-centres/m1-melbourne-data-centre) | Australia Southeast | AARNet, Devoli, Equinix, Megaport, NEXTDC, Optus, Telstra Corporation, TPG Telecom |
| **Miami** | [Equinix MI1](https://www.equinix.com/locations/americas-colocation/united-states-colocation/miami-data-centers/mi1/) | n/a | C3ntro+, Equinix, Megaport, Neutrona Networks |
| **Montreal** | [Cologix MTL3](https://www.cologix.com/data-centers/montreal/mtl3/) | n/a | Bell Canada, Cologix, Megaport, Telus, Zayo |
| **Mumbai** | Tata Communications | West India | Global CloudXchange (GCX), Reliance Jio, Sify, Tata Communications, Verizon |
| **Mumbai2** | Airtel | West India | Airtel, Sify, Vodafone Idea |
| **New York** | [Equinix NY9](https://www.equinix.com/locations/americas-colocation/united-states-colocation/new-york-data-centers/ny9/) | n/a | CenturyLink Cloud Connect, Coresite, Equinix, InterCloud, Megaport, Packet, Zayo |
| **Newport(Wales)** | [Next Generation Data](https://www.nextgenerationdata.co.uk) | UK West | British Telecom, Colt, Level 3 Communications, Next Generation Data |
| **Osaka** | [Equinix OS1](https://www.equinix.com/locations/asia-colocation/japan-colocation/osaka-data-centers/os1/) | Japan West | Colt, Equinix, Internet Initiative Japan Inc. - IIJ, NTT Communications, NTT SmartConnect, Softbank |
| **Paris** | [Interxion PAR5](https://www.interxion.com/Locations/paris/) | France Central | CenturyLink Cloud Connect, Colt, Equinix, Intercloud, Interxion, Orange, Telia Carrier, Zayo |
| **Perth** | [NextDC P1](https://www.nextdc.com/data-centres/p1-perth-data-centre) | n/a | Megaport, NextDC |
| **Quebec City** | [Vantage](https://vantage-dc.com/data_centers/quebec-city-data-center-campus/) | Canada East | Bell Canada, Megaport |
| **San Antonio** | [CyrusOne SA1](https://cyrusone.com/locations/texas/san-antonio-texas/) | South Central US | CenturyLink Cloud Connect, Megaport |
| **Sao Paulo** | [Equinix SP2](https://www.equinix.com/locations/americas-colocation/brazil-colocation/sao-paulo-data-centers/sp2/) | Brazil South | Aryaka Networks, Ascenty Data Centers, British Telecom, Equinix, Level 3 Communications, Neutrona Networks, Orange, Tata Communications, Telefonica, UOLDIVEO |
| **Seattle** | [Equinix SE2](https://www.equinix.com/locations/americas-colocation/united-states-colocation/seattle-data-centers/se2/) | West US 2 | Aryaka Networks, Equinix, Level 3 Communications, Megaport, Telus, Zayo |
| **Seoul** | [KINX Gasan IDC](https://www.kinx.net/support/location/?lang=en) | Korea Central | KINX, LG CNS, Sejong Telecom |
| **Silicon Valley** | [Equinix SV1](https://www.equinix.com/locations/americas-colocation/united-states-colocation/silicon-valley-data-centers/sv1/) | West US | Aryaka Networks, AT&T NetBond, British Telecom, CenturyLink Cloud Connect, Comcast, Coresite, Equinix, InterCloud, Internet2, IX Reach, Packet, PacketFabric, Level 3 Communications, Megaport, Orange, Sprint, Tata Communications, Telia Carrier, Verizon, Zayo |
| **Silicon Valley2** | [Coresite SV7](https://www.coresite.com/data-centers/locations/silicon-valley/sv7) | West US | Coresite | 
| **Singapore** | [Equinix SG1](https://www.equinix.com/locations/asia-colocation/singapore-colocation/singapore-data-center/sg1/) | Southeast Asia | Aryaka Networks, AT&T NetBond, British Telecom, Epsilon Global Communications, Equinix, InterCloud, Level 3 Communications, Megaport, NTT Communications, Orange, SingTel, Tata Communications, Telstra Corporation, Verizon, Vodafone |
| **Singapore2** | [Global Switch Tai Seng](https://www.globalswitch.com/locations/singapore-data-centres/) | Southeast Asia | Colt, Epsilon Global Communications, Megaport, SingTel |
| **Stockholm** | [Equinix SK1](https://www.equinix.com/locations/europe-colocation/sweden-colocation/stockholm-data-centers/sk1/) | n/a | Telia Carrier |
| **Sydney** | [Equinix SY2](https://www.equinix.com/locations/asia-colocation/australia-colocation/sydney-data-centers/sy2/) | Australia East | AARNet, AT&T NetBond, British Telecom, Devoli, Equinix, Kordia, Megaport, NEXTDC, NTT Communications, Optus, Orange, Spark NZ, Telstra Corporation, TPG Telecom, Verizon, Vocus Group NZ |
| **Taipei** | Chief Telecom | n/a | Chief Telecom, FarEasTone |
| **Tokyo** | [Equinix TY4](https://www.equinix.com/locations/asia-colocation/japan-colocation/tokyo-data-centers/ty4/) | Japan East | Aryaka Networks, AT&T NetBond, British Telecom, CenturyLink Cloud Connect, Colt, Equinix, Internet Initiative Japan Inc. - IIJ, NTT Communications, NTT EAST, Orange, Softbank, Verizon |
| **Toronto** | [Cologix TOR1](https://www.cologix.com/data-centers/toronto/tor1/) | Canada Central | AT&T NetBond, Bell Canada, CenturyLink Cloud Connect, Cologix, Equinix, IX Reach Megaport, Telus, Verizon, Zayo |
| **Washington DC** | [Equinix DC2](https://www.equinix.com/locations/americas-colocation/united-states-colocation/washington-dc-data-centers/dc2/) | East US, East US 2 | Aryaka Networks, AT&T NetBond, British Telecom, CenturyLink Cloud Connect, Cologix, Comcast, Coresite, Equinix, Internet2, InterCloud, Level 3 Communications, Megaport, Neutrona Networks, NTT Communications, Orange, PacketFabric, Sprint, Tata Communications, Telia Carrier, Verizon, Zayo |
| **Washington DC2** | [Coresite Reston](https://www.coresite.com/data-centers/locations/northern-virginia-washington-dc/reston-campus) | East US, East US 2 |Coresite | 
| **Zurich** | [Interxion ZUR2](https://www.interxion.com/Locations/zurich/) | n/a | Intercloud, Interxion |

 **+** denotes coming soon

### National cloud environments

### US Government cloud
| **Location** | **Service providers** |
| --- | --- |
| **Chicago** |AT&T NetBond, Equinix, Level 3 Communications, Verizon |
| **Dallas** |Equinix, Megaport, Verizon |
| **New York** |Equinix, CenturyLink Cloud Connect, Verizon |
| **Phoenix** | AT&T NetBond, CenturyLink Cloud Connect, Megaport |
| **San Antonio** | CenturyLink Cloud Connect, Megaport |
| **Silicon Valley** | Equinix, Level 3 Communications, Verizon |
| **Seattle** | Equinix, Megaport |
| **Washington DC** |AT&T NetBond, CenturyLink Cloud Connect, Equinix, Level 3 Communications, Megaport, Verizon |

### China
| **Location** | **Service providers** |
| --- | --- |
| **Beijing** |China Telecom |
| **Beijing2** | China Telecom, GDS |
| **Shanghai** |China Telecom |
| **Shanghai2** | China Telecom, GDS |

To learn more, see [ExpressRoute in China](http://www.windowsazure.cn/home/features/expressroute/)

### Germany
| **Location** | **Service providers** |
| --- | --- |
| **Berlin** |e-shelter, Megaport+, T-Systems |
| **Frankfurt** |Colt, Equinix, Interxion |

## <a name="c1partners"></a>Connectivity through Exchange providers
If your connectivity provider is not listed in previous sections, you can still create a connection.

* Check with your connectivity provider to see if they are connected to any of the exchanges in the table above. You can check the following links to gather more information about services offered by exchange providers. Several connectivity providers are already connected to Ethernet exchanges.
  * [Cologix](https://www.cologix.com/)
  * [CoreSite](https://www.coresite.com/)
  * [Equinix Cloud Exchange](https://www.equinix.com/services/interconnection-connectivity/cloud-exchange/)
  * [InterXion](https://www.interxion.com/)
  * [NextDC](https://www.nextdc.com/)
  * [Megaport](https://www.megaport.com/services/microsoft-expressroute/)
  * [PacketFabric](https://www.packetfabric.com/packetcor/microsoft-azure/)
  
* Have your connectivity provider extend your network to the peering location of choice.
  * Ensure that your connectivity provider extends your connectivity in a highly available manner so that there are no single points of failure.
* Order an ExpressRoute circuit with the exchange as your connectivity provider to connect to Microsoft.
  * Follow steps in [Create an ExpressRoute circuit](expressroute-howto-circuit-classic.md) to set up connectivity.

## <a name="c1partners"></a>Connectivity through additional service providers
| **Location** | **Exchange** | **Connectivity providers** |
| --- | --- | --- |
| **Amsterdam** | Equinix, Interxion, Level 3 Communications, Telecity | BICS, CloudXpress, Eurofiber, Fastweb S.p.A, Gulf Bridge International, Kalaam Telecom Bahrain B.S.C, MainOne, Nianet, POST Telecom Luxembourg, Proximus, TDC Erhverv, Telecom Italia Sparkle, Telekom Deutschland GmbH, Telia |
| **Atlanta** | Equinix| Crown Castle
| **Cape Town** | Teraco | MTN |
| **Chicago** | Equinix| Crown Castle, Spectrum Enterprise, Windstream |
| **Dallas** | Equinix, Megaport | Axtel, C3ntro Telecom, Cox Business, Crown Castle, Data Foundry, Spectrum Enterprise, Transtelco |
| **Frankfurt** | Interxion, Telecity | BICS, Cinia, Nianet, QSC AG, Telekom Deutschland GmbH |
| **Hamburg** | Equinix | Cinia |
| **Hong Kong SAR** | Equinix | Chief, Macroview Telecom |
| **Johannesburg** | Teraco | MTN |
| **London** | BICS, Equinix, euNetworks, Telecity | Bezeq International Ltd., CoreAzure, Epsilon Telecommunications Limited, Exponential E, HSO, NexGen Networks, Proximus, Tamares Telecom, Zain |
| **Los Angeles** | Equinix |Crown Castle, Spectrum Enterprise, Transtelco |
| **Madrid** | Level3 | Zertia |
| **Montreal** | Cologix, Equinix | Airgate Technologies, Inc. Aptum Technologies, Rogers, Zirro |
| **New York** |Equinix, Megaport | Altice Business, Crown Castle, Spectrum Enterprise, Webair |
| **Paris** | Equinix | Proximus |
| **Quebec City** | Megaport | Fibrenoire |
| **Sao Paula** | Equinix | Venha Pra Nuvem |
| **Seattle** |Equinix | Alaska Communications |
| **Silicon Valley** |Coresite, Equinix | Cox Business, Spectrum Enterprise, Windstream, X2nsat Inc. |
| **Singapore** |Equinix |1CLOUDSTAR, BICS, CMC Telecom, Epsilon Telecommunications Limited, LGA Telecom, United Information Highway (UIH) |
| **Slough** | Equinix | HSO|
| **Sydney** | Megaport | Macquarie Telecom Group|
| **Tokyo** | Equinix | ARTERIA Networks Corporation, BroadBand Tower, Inc. |
| **Toronto** | Equinix, Megaport | Airgate Technologies Inc., Beanfield Metroconnect, Aptum Technologies, IVedha Inc, Rogers, Thinktel, Zirro|
| **Washington DC** |Equinix | Altice Business, BICS, Cox Business, Crown Castle, Gtt Communications Inc, Epsilon Telecommunications Limited, Masergy, Windstream |

## ExpressRoute system integrators
Enabling private connectivity to fit your needs can be challenging, based on the scale of your network. You can work with any of the system integrators listed in the following table to assist you with onboarding to ExpressRoute.

| **Continent** | **System integrators** |
| --- | --- |
| **Asia** |Avanade Inc., OneAs1a |
| **Australia** | Ensyst, IT Consultancy, MOQdigital, Vigilant.IT |
| **Europe** |Avanade Inc., Altogee, Bright Skies GmbH, Inframon, MSG Services, New Signature, Nelite, Orange Networks, sol-tec |
| **North America** |Avanade Inc., Equinix Professional Services, FlexManage, Lightstream, Perficient, Presidio |
| **South America** |Avanade Inc., Venha Pra Nuvem |
## Next steps
* For more information about ExpressRoute, see the [ExpressRoute FAQ](expressroute-faqs.md).
* Ensure that all prerequisites are met. See [ExpressRoute prerequisites](expressroute-prerequisites.md).

<!--Image References-->
[0]: ./media/expressroute-locations/expressroute-locations-map.png "Location map"
