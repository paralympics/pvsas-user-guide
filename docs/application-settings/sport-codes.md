# Sport Codes

This section extracts the IPC common codes that are relevant for the handling and registration of data in PVSAS. 
These data cannot be changed through this application with the IPC being the owner of these common codes. 
The IPC Sports IT team shall be contacted if there is any code, label or translation missing or incorrect. 
Following common codes tables are shown:

- **Sports** are usually defined as a composition of all disciplines and events governed by a 
  single International Federation (IF). For operational purposes, some exceptions might 
  have been applied. However, for PVSAS only the sport of ParaVolley (generally named as 
  Volleyball) is used.

- **Disciplines** separate a few sports into more logical entities, e.g. the sport of cycling is 
  divided into cycling road and cycling track. The term ‘discipline’ must not be mixed up with 
  the **‘event types’**. In PVSAS, four disciplines are defined.

- **Event Types** reflects a specific competition format with a discipline. The term **‘competition’** 
  shall not be mixed up with a competition which consists of the full event programme and is defined 
  by location, start/end date, and the organiser. Event types are defined by a specific set of rules, 
  distances, styles, used equipment or team size. In able-bodied sport, event types and events are 
  synonymous terms; in sports for athletes with a disability, an event is the combination of an event 
  type and specific classification. The definition of event types and events with class combinations 
  are necessary for the treatment of entries, results, records, and rankings, none of which is currently 
  supported by PVSAS. Event Types are further divided into event type categories (subdivisions with certain 
  sporting similarities, e.g. road running races and track running races are different categories), and event 
  type groups (used for classification purposes, where a class is valid for one event or several events within 
  the event type group).

- **Event Type Categories** are defined to distinctively group event types. For example, all stadium running 
  events are considered as *Track* events, jumping and throwing events are known as *Field* events. Like 
  class groups, the event type categories are used to specify the validity of an athlete’s classification. 
  Well-known example is classification in shooting. IPC Shooting consists of several rifle and pistol events 
  as well as the both classes SH1 and SH2. According to the current classification rules, an athlete is classified 
  by weapon and could have different classes for different weapons. In a real example, an athlete is classified SH1 
  [Pistol] and SH2 [Rifle]. 

- **Event Type Groups** is a set of several event types combined. Once a new event type group is created with code 
  and name, an arbitrary number of event types can be assigned to this group. Finally, in the classification screen 
  of PVSAS for an athlete, a specific class and class status can be formally limited to such a combination of event 
  types. An obvious example is the T20-classification which is distinguished between track events (400m-10000m) and 
  horizontal jumps (long and triple) so that the athlete can be have different class statuses for each group.

- **Classes** ensure fair competition between athletes with similar or even different types of disability is an additional 
  complicated dimension when one is trying to formalize the structure of sport. This entity is the basis for the entire 
  classification data storage. Each class has a class name and a class code and are further uniquely associated with an 
  international federation who is in charge of athletes in these classes on the international stage.

- **Class Groups** follow a similar concept like event type categories and are designed to allow classes to be separated 
  in a logical way in sports where athletes can have several classes for different events in the sports. Some sports like 
  athletics or swimming allow the athlete to have up to three different classes at the same time but usually only one class 
  per ‘class group’. Consequently, for these both sports, the class groups *T*, *F*, and *P* as well as *S*, *SB*, and *SM* 
  are already defined. Furthermore, it allows the specification for which class group a pseudo-class like *NE* is applied to. 
  See [Classification Details](athletes/classification.md#classification-details) for more details how to use class groups in 
  the classification. 