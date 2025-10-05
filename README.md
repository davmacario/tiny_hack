<img src="https://github.com/davmacario/tiny_hack/blob/main/img/logo.png?raw=true" width="400">


# MoodSip - Sip Your Stress Away 🌟

**MoodSip** is a smart water bottle developed by **[@pitadagosti](https://github.com/pitdagosti), [@davmacario](https://github.com/davmacario), and [@FrigaZzz](https://github.com/frigazzz)**.  
It integrates an **Arduino Nicla Vision** to adapt your hydration rhythm to your needs, combining **water tracking** and **emotion detection** 💆.  

Studies show that even mild dehydration can reduce concentration, cause fatigue, and irritability [1]. Proper hydration can reduce cortisol spikes under stress [2] and improve physical and mental well-being.  

MoodSip helps you **drink smarter and manage stress**, promoting both physical and mental health.

## Hydration Matters 💧

Fluid loss negatively affects the body:

- **Common symptoms:** fatigue, confusion, reduced physical and mental performance 🪫 [3]  
- **Elderly:** dehydration is widespread, increasing mortality and healthcare costs 🧑‍🦳 [4]  
- **Stress:** even mild water deprivation amplifies stress response with higher cortisol peaks 💹 [5]  

Benefits of proper hydration [6]:

- Prevents headaches  
- Reduces fatigue  
- Improves skin and cognitive performance  

Technology can support regular hydration habits. Current smart bottles remind you to drink and track intake, but rarely consider **emotional state**. MoodSip fills this gap with a **holistic daily wellness approach**.

## Existing Solutions 🤖

**[HidrateSpark PRO](https://hidratespark.com/products/hidratespark-pro-32oz-smart-water-bottle?srsltid=AfmBOoqLxbZMkuoIMlOLmEquyeIBkWmz_JHxx7YUNcmM67cucT_ZqbWG)**  

- SipSense sensors weigh the bottle and track every sip  
- Bluetooth app with personalized goals  
- Bottle lights up when it’s time to drink  
- Focus: quantitative hydration tracking  

**[REBO SMART](https://www.rebo-bottle.com/?srsltid=AfmBOoqhUXy9-czE509IICU5Ty_-udnFqgqxLnc0WFIuFZnrFpd2PKXt)**  

- Tracks personalized hydration via Bluetooth and app  
- Environmental impact: "1 REBO drank = 1 plastic bottle collected from oceans"  
- Digital reminders and hydration plans based on activity and body

**[Other solutions](https://www.goodhousekeeping.com/home-products/g37094301/best-smart-water-bottles/)**

- Recent articles on smart bottles note that these devices “can remind you to drink enough water and record how much you drink.”
- Some models even include speakers, UV sterilization, or fitness connectivity. However, most remain focused on apps, level (or weight) sensors, and notifications.

**Limitations:**  

- Existing products mainly track **water intake** and send **reminders**  
- They lack a real link between **hydration and emotional state**  

**MoodSip** bridges this gap by combining **smart hydration tracking** with **emotion-aware feedback**, creating a more holistic and personalized experience.

## How MoodSip Works 🌡️😊

MoodSip runs an **adaptive timer** based on:

### 1. Facial Expressions (Stress)  
- **Nicla Vision camera** captures the user’s face  
- ML model (FocoosAI) detects signs of stress (e.g., furrowed brows, tired eyes)  
- If stress is detected, the LED turns **red 🔴** and the drinking reminder accelerates  

### 2. Ambient Temperature  
- Sensor measures temperature and humidity  
- In hot or humid conditions, the timer shortens to encourage more frequent drinking  

### 3. Drinking Duration  
- LED turns **blue 🔵** when it’s time to drink  
- Proximity and gyroscope sensors estimate water intake  
- If intake is low, the next timer is shortened to encourage proper hydration  

**Summary:** MoodSip continuously adapts drinking reminders based on stress, temperature, and actual water intake. Everything runs on **Arduino Nicla Vision**, completely offline.

## Quick Start :on:

## Technologies ⚙️

- **[Arduino Nicla Vision](https://docs.arduino.cc/hardware/nicla-vision/):** 2MP camera, proximity sensors, 6-axis gyroscope/accelerometer, Wi-Fi/BLE  
- **[FocoosAI](https://focoos.ai):** computer vision library for facial expression recognition  
- **[Z-Ant](https://github.com/ZantFoundation/Z-Ant):** open-source framework to optimize neural models on microcontrollers  

**Advantage:** onboard intelligence, portable, and fully offline.

## Impact & Benefits 👍🏼

MoodSip is more than a gadget—it’s a tool for **public health and social impact**:

- **Promotes hydration and stress management**, especially for elderly people, who are highly vulnerable to dehydration and its serious health consequences [7].    
- Raises awareness of the **mind-body connection**: drinking water can help reduce mental tension and improve overall well-being.  

By integrating **mood detection**, MoodSip goes beyond counting milliliters—it “understands” the user and adapts to their emotional and physical needs.  

**Social impact:** Proper hydration can reduce hospital visits, lower healthcare costs, and improve quality of life, particularly for older adults who are disproportionately affected by dehydration. In this way, MoodSip contributes to a meaningful societal goal while providing a fun and engaging user experience.

## Alcoholic games? Yes please!! 🍹🎲

MoodSip can turn into a **party drinking game**:

- Everyone keeps a poker face  
- Camera detects smiles or other emotions  
- **Red LED 🔴** lights up for the “caught” person → that player must drink

Uses the same emotion detection mechanism for fun and social interaction.

## References 📚

[1]. [Dehydration: the enemy of our body](https://medimutua.org/disidratazione-il-nemico-del-nostro-organismo/)  
[2]. [This Simple Everyday Health Tweak Can Help Reduce Anxiety And Future Health Problems](https://www.womenshealthmag.com/health/a68130438/hydration-stress-anxiety-study/)  
[3]. [Hydratation](https://www.my-personaltrainer.it/disidratazione-sintomi.html)  
[4]. [Trends in Dehydration in Older People](https://www.mdpi.com/2072-6643/17/2/204)  
[5]. [Relationship between fluid intake, hydration status and cortisol dynamics in healthy, young adult males](https://www.sciencedirect.com/science/article/pii/S2666497624000572)  
[6]. [The Science of Nano-Enhanced Hydration in Sports Nutrition](https://link.springer.com/chapter/10.1007/978-981-96-5471-0_3)  
[7]. [Hydration Strategies in Older Adults](https://www.mdpi.com/2072-6643/17/14/2256)  

