# Optimizing-Satisfactory  
My personal project to optimize the game Satisfactory and discover the maximum quantity and quality of produced items based on the limited supply of resources in the game.  

## Process:  
- Record the maximum yields of all resources in the Satisfactory world  
- Record the base recipies for all items and machines in the game  
- Assign values to all items based on the complexity of the base recipies  
- Utilizing as much of the limited resources as possible, maximize the produced yeild based on assigned complexity values  

### Considerations:  
- This project will only consider recipies that can be automated in a machine and does not include seasonal recipies or recipies that use resources gathered by hand (ex: leaves or animal remains)  
- All rates are items produced per minute

### Assigned Item Values (AIV):  
In order to ensure that the items produced for this project are as complex as possible, items will be assigned a value based on how intricate and advanced they are.  
This will take the form of a number starting from a base AIV of 1 for the raw resource (ex: iron ore = 1), adding 1 for the current machine processing, summing the AIVs of inputs needed to produce 1 item, and finally, multiplying by the technology tier level needed to produce the item  
Ex: Produced Item AIV = (Machine Processing (1) + (Input 1 AIV + Input 2 AIV + ...) ) x Technology Tier / Output Rate  

- Items unlocked in Tier 0 (Onboarding/Tutorial) will be collapsed into Tier 1 since many people skip this tier.  
- Items unlocked in the MAM will be assigned to Technology Tier 1.5 since their actual technology tier unlock is usually much later than players will usually unlock them through the MAM, while also needing to put in extra work to gather materials to research the MAM recipies  
- Base resources will have an Input AIV of 1

## Potential Future Additions:  
- Alternate recipies that are unlocked using hard drives  
- Power consumption and production  
- Resourced needed to create the machines used  
- Overclocking and production amplification of machines  

## Acknoledgements:  
I would like to thank Dylan and Drew Mahosky who first got me into playing Satisfactory and inspired me to start this project.  
I would also like to thank Coffee Stain Studios for creating such an amazing and fun game.  

## Resources & Links:  
https://satisfactory.wiki.gg/  
https://www.satisfactorygame.com/  