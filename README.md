HOW TO MERGE MAPS USING VERTEX HUB (FIX COLLISION, INVISIBLE WALLS & DOORS)
🧠 GhostCore Guide – Merging Maps with Vertex Hub
❗ Problem
Maps overlapping
Flickering textures
Invisible walls or doors
Broken collision in certain areas

**💡 What is Vertex Hub?**
Paid tool (~$10/month)
Includes ~4000 coins (It will not take all your coins in one merge)
Allows merging multiple .ymap files into one
Helps reduce conflicts and improve performance

**✅ Before You Start**
Test each map individually
Make sure all maps load correctly
Identify if any map is escrowed

**⚠️ Escrow Warning (VERY IMPORTANT)**
If a map includes escrowed .ybn (collision files):
❌ You cannot edit or merge those collisions
❌ You may experience:
Falling through map
Invisible walls
Broken interiors

**👉 Workaround:**
Use custom collision props
Do NOT attempt to bypass escrow protections
🔧 How to Merge Maps

**BACKUP YOUR MAPS BFEORE YOU MERGE THEM**

Upload your .ymap files into Vertex Hub
Select all maps you want to merge
 -- create a folder [maps-to-fix]/ with all maps you are merging inside on their own folder and manifest.--

Run the merge (uses coins)

Download the generated .zip file

**📦 After Merging (IMPORTANT)**
Extract the .zip
Rename the folder:
merged_maps_gc <- (anything you like)

Place it inside your resources folder
📌 Server Load Order (CRITICAL)
Add the merged map at the bottom of your server.cfg:
ensure house_map
ensure mlo_map
ensure city_map

ensure merged_maps_gc  (make sure the merged file load AFTER the maps you merged)

**👉 This ensures:**

Base maps load first
Merged map overrides properly (to remove what is causing issues)
Reduces flickering and conflicts

**💡 Extra Tips**
Always test collision after merging
Never merge broken maps
Keep backups of original files
Some maps are visual-only (no collision included)

✍️ Author
**GhostCore Scripts**
