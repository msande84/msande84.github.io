---
title: Component Selection
---

## Components

*Table 1: Shift Register Options*

**8-Bit Parallel in Serial out (PISO) Shift Register**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| ![](74HC165-Q100.png)<br>\* Option 1.<br>\* 74HC165-Q100 surface mount shift register<br>\* $0.24/each<br>\* [link to product](https://www.mouser.com/ProductDetail/Nexperia/74HC165D-Q100118?qs=sGAEpiMZZMutXGli8Ay4kD1Rik6g2cV%252B%252BQvCmhxAH0s%3D)                 | \* Inexpensive<br>\* Directly outputs serial<br>\* Meets surface mount constraint of project                                               | \* Slow shipping speed<br>\* Needs special PCB layout |
| ![](74HC595D.png)<br>\* Option 2. <br>\* 74HC595D surface mount shift register <br>\* $0.63/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/Toshiba/74HC595DBJ?qs=T%2FywbITssnTkqd02WdSNRg%3D%3D) | \* Meets surface mount constraint of project <br>\* High noise immunity <br> \* Directly outputs serial | * Exceeding absolute max ratings, even briefly lead to deterioration <br>\* Slow shipping speed                                                         |
| ![](SN74HCS165.png)<br>\* Option 3. <br>\* SN74HCS165 surface mount shift register <br>\* $1.52/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/Texas-Instruments/SN74HCS165DRG4?qs=vOcB1WHNNXLF%2FP4%252BuTSdXQ%3D%3D) | \* Meets surface mount constraint of project <br>\* Wide operating voltage range 2V to 6V <br> \* Directly outputs serial | * More expensive <br>\* Slow shipping speed                                                         |

**Choice:** Option 1: 74HC165-Q100 surface mount shift register

**Rationale:** This shift register is the cheapest option and is not missing any needed features. The added benefits of the more expensive options do not add anything ciritical for this project so do not make sense to choose.

*Table 2: Push Button Options*

**Push Button**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| ![](pts645_switch.png)<br>\* Option 1.<br>\* The PTS645 switch series are 6mm tactile switches <br>\* $0.28/each<br>\* [link to product](https://www.mouser.com/ProductDetail/CK/PTS645SL50-2-LFS?qs=rqnA19JZHeTZYaJU%252B5olWA%3D%3D)                 | \* Inexpensive<br>\* Long life expectancy<br>\* Taller button                                               | \* Slow shipping speed |
| ![](WS-TASV_switch.png)<br>\* Option 2. <br>\* WS-TASV SMT Tact Switch <br>\* $0.21/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/Wurth-Elektronik/435151014824?qs=OlC7AqGiEDkCCtReGm3ZVw%3D%3D) | \* Meets surface mount constraint of project <br>\* Long life expectancy <br> \* High quality | * Not impact resistant <br>\* Slow shipping speed <br>\* Difficult to mount                                                        |
| ![](TS34-62-25-switch.png)<br>\* Option 3. <br>\* TS34-62-25-BK-100-SMT-TR Tactile Switch <br>\* $0.26/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/Same-Sky/TS34-62-25-BK-100-SMT-TR?qs=efUn273yAhdJc%2FOpc3t49g%3D%3D) | \* Inexpensive <br>\* Long life expectancy <br> \* Wide power range | * Small button <br>\* Slow shipping speed                                                         |

*Table 3: Voltage Regulator Options*

**Voltage Regulator**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| ![](AOT2618-MOSFET.png)<br>\* Option 1.<br>\* AOT2618L TO-220 MOSFET <br>\* $1.66/each<br>\* [link to product](https://www.digikey.com/en/products/detail/alpha-omega-semiconductor-inc/AOT2618L/3603378)                 | \* Inexpensive<br>\* Meets voltage requirements of project <br>\* Inexpensive <br>\* Low power loss when switching                                              | \* Slow shipping speed |
| ![](IPP038N15NM6AKSA1_MOSFET.png)<br>\* Option 2. <br>\* IPP038N15NM6AKSA1 PG-TO220-3 MOSFET <br>\* $5.16/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/Infineon-Technologies/IPP038N15NM6AKSA1?qs=7%2F6SraaimPQ1Q6UGpNL1jg%3D%3D) | \* Meets voltage requirements of project <br>\* Superior thermal resistance <br> \* Lead free | * More expensive <br>\* Slow shipping speed                                                         |
| ![](LM7805-MOSFET.png)<br>\* Option 3. <br>\* LM7805C TO-220 MOSFET <br>\* $1.80/each <br>\* [Link to product](https://www.mouser.com/ProductDetail/Texas-Instruments/LM7805CT-NOPB?qs=OYMYEaN9QmBS2GvaX6GSkQ%3D%3D) | \* Meets voltage requirements of project <br>\* Easy to use <br> \* Internal thermal overload protection | * Slow shipping speed                                                         |
