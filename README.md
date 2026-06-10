# 0-AD Mod

This is a mod implementing a Māori civilization into the game 0-AD. It was built as the big end-of-semester project for the Data Structures and Algorithms paper at Waikato. We added unique Māori models, units, buildings, and audio into the game. As it was a Māori game, we interviewed relevant Māori stakeholders to get feedback and advice to help with the mod authenticity and to make sure we were portraying the culture correctly.

<img width="640" height="400" alt="Image 10-06-2026 at 8 16 pm" src="https://github.com/user-attachments/assets/bdfd5189-5e19-487a-83df-e5d18fad1b26" />


## 🛠️ Technologies

• JavaScript

• XML

• Blender

• Visual Studio

• Paint.net

• GIMP

• Audacity

## ⚙️ Features

Here's what you can do with our 0-AD mod:

• Build 6 unique units:

  • Toa - Basic warrior
  
  • Tauira - Cheap spamable infantry
  
  • Mou Potu - Stone thrower
  
  • Mou Rakau - Javelin thrower
  
  • Rangatira - Elite tank unit
  
• Build 2 unique buildings:

  • Pa - Powerful Māori fortress that increases food production
  
  • Pou Whenua - Territorial marking pole to claim large tracks of land
  
• Unique Technologies

• Unique skins and models of buildings, UI, and units

<img width="640" height="400" alt="Image 10-06-2026 at 8 11 pm" src="https://github.com/user-attachments/assets/52da0b07-42dc-4f19-a4cb-2c491c447453" />

## 💡 Process

### Planning

The first step was figuring out how the game's mod actually worked. To do this, we downloaded an existing 0-AD mod file that added a unique the bean civ to the game.

Then we planned the project. Firstly, we decided to add unique units. We chose to make the tribe more early-game oriented, so we made a lot of cheap units like Mou Potu and Tauira to allow for an early rush. As the Māori didn't have horses and all the other civs do, we made all the Māori troops have fast movement speeds to make them competitive. We also needed siege unit replacement, so we added the Rangatira tank unit to take down buildings. For the unique buildings, we chose the Pa as it's a classic of Māori construction. For the Pou Whenua, we thought that a cheap, easy way to expand your territory would be interesting, as no other tribes have this, and it can help you grab resources just out of reach.

After the planning stage, we made some basic proof of concept unit models and reached out to the University's Māori department for feedback on our ideas. Te Taka reviewed our ideas and recommended some changes. Firstly, he recommended that we create a map of Waikato as it's rich in Māori history and it is where his iwi is from. He also recommended that we change some of the building and troop names so they would be more accurate in te reo. He also gave us valuable insights into Māori technologies that we could adapt into the game.

### Development

Next, we started to develop the Māori technologies that Te Taka gave us. We made a special effect with the Pa that increases food generation and a special tech that allows you to unlock the powerful Rangatira.

### Asset Creation

After this, we set out to create skins for the unique units. To do this, we downloaded preexisting skins for the people, and then we overlaid custom skins we made in Paint.net over them. To control the skins, we need to create unique actor XML files.

Next, we started building the models and skins for the buildings. We created the models in Blender and then exported a UV map of them and downloaded it in GIMP. Then, in GIMP, we put the textures we wanted onto the UV map. After that, we imported it into Blender and projected the texture onto the building model using an image texture in the shading window. Then, in VS Code, we created custom XML files to tie the model, building code, and image together.

After that, we started on customising the game's UI so it felt Māori. The first task was finding a symbol that represented the Māori for the map overlay, and we chose the koru. Next, we had to create icons for the unique buildings and units we created. To do this, we screenshotted the unit/building, imported it to GIMP and gave it a black background. Then we added an icon pointer in the XML files.

### Polish

Next, it was finally time for polishing. The first step was creating promotions. To do this, we used unique XML files so they could be promoted from basic to advanced to elite as they gained more XP. The final thing to polish was debugging all the errors. Most of this was just removing redundant theaban code from the old mod we built on top of.

<img width="640" height="400" alt="Image 10-06-2026 at 1 41 pm" src="https://github.com/user-attachments/assets/a30c5a2c-50b8-46d7-a043-5115ad634f4b" />

## 🧠 What We Learned

• XML

• JavaScript

• UV Mapping

• Github

• File structures

• Linking different languages and data types

• Māori culture and history

## 🎯 How it can be improved

• The first major thing that can be improved is adding unique naval units. Naval is barely ever used in 0-AD, and due to time constraints, we decided to leave unique naval units out of our mod. Adding in unique naval units for Māori would be cool, as they have a rich naval history and it would really enhance the mod.

• The second thing that would be good to improve is adding unique heroes. Most of the other civs have heroes, so it would be cool to give the Māori civilisation its own. This would add new interesting late-game strategies that would further help differentiate the civilization.

<img width="640" height="400" alt="Image 10-06-2026 at 8 06 pm" src="https://github.com/user-attachments/assets/2a596736-4959-4989-b2dc-c7bf6523ce2e" />

## 🖥️ To run the project locally:

### For the mod

Download the repository to your machine.

Move the Maori folder to your 0-AD mod folder.

That's it for the mod!

### For the map

Put Waikato_2p.xml in mods/user/maps/scenarios

Then put Waikato_2p.png in mods/user/art/textures/ui/session/icons/mappreview
