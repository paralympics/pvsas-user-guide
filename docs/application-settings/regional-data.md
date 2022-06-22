# Regional Data

Besides sport codes, another important group of entities is related to the basic organisational 
structure of PVSAS. Apart from the countries table that is derived from the IPC common codes, 
the NPC has full access to register any entity.

## Countries 

The term **‘country’** does not only consider independent states recognised by the United 
Nations but also any other overseas territories or other self-governed areas in dependency of 
an independent state. Storage of historical information requires definition of historical 
nations or territories.

In this application, countries are used in a few screens, mainly for nationality information of 
athletes and location of competitions, meetings, and events.

For a better differentiation between countries and organisations (e.g. NPCs) and due to 
missing organisation codes for some countries, the ISO-3166-1 (Alpha-3) codes are in use as 
unique country identifier of recent states and territories. Historical countries (Soviet Union, 
East Germany, Czechoslovakia) are identified by former ISO-codes, or alternatively by the 
former IOC code.

## International Federations

For the effective co-operation between the various SDMS versions, each sport and each class 
are owned by a particular international federation. As athletes are stored in a central SDMS 
database that is shared between the existing IF SDMS versions (IPC, IBSA, and World 
ParaVolley), the classification of the athlete defines who is the owner of the athlete profile. 
Ownership can be shared by several IFs if the athlete is registered in various sports, e.g. 
athletics (World Para Athletics/IPC) and volleyball (World ParaVolley). However, the access to 
classification relevant data is limited to the owner of the respective sport.

Each federation registered has two assignment tables which sports it governs and which are 
the national member federations.

World ParaVolley as owner of PVSAS can view all data sets, and additionally can amend the 
list of national members of their own federation. This list then applies to all country drop-down
menus across PVSAS.

When a new country is granted membership at World ParaVolley, or when such a member 
loses its status, search for World ParaVolley as international federation, open its detail page 
and the tab **‘Members’**. The assignment table as shown in the figure below.

Both tables are populated from the list of potential active country members as defined in the 
**‘members’** section of PVSAS, loaded from the [IPC Common Codes](https://db.ipc-services.org/centre/common-codes/index). 
The right table shows the current membership; in the left table, all potential countries exist.

<figure>
  <img src="_img/figures/3.1-assignment-grid-federation.png" alt="Assignment Grid of National Member Federations" class="screenshot">
  <figcaption>Assignment screen of national member federations to World ParaVolley</figcaption>
</figure>

To assign, find the new country on the left. Either select it and click **‘Assign’** or move it to the 
right table by drag-and-drop. To remove a country, find the country in the right table, select it 
and click **‘Remove’** or move it to the left table by drag-and-drop.

## Members

This table reflects the list of all potential member federations of international sport movements, 
both current and historical entities. Each member is identified by their IPC or IOC code that is 
the standard code for the Paralympic and Olympic Games and their environments. The IPC maintains 
that list in co-operation with the IOC when countries become independent and sooner or later 
eligible to obtain membership of any international federation.