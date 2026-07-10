# 🎮 Minecraft Clone - Mobile Optimized

A high-quality, single-file Minecraft clone built with HTML, CSS, and JavaScript using Three.js. Designed specifically for mobile devices with touch controls while also supporting desktop play.

## 🌟 Features

### Graphics & Visual Quality
- **Realistic lighting** with dynamic day/night cycle
- **Smooth shadows** using PCF soft shadow mapping
- **Procedural terrain generation** with multi-octave noise
- **Water with realistic reflections** and normal mapping
- **Texture atlas** for efficient rendering
- **Block breaking animations** with progressive cracks
- **Particle effects** when mining blocks
- **Dynamic sky colors** transitioning through day, sunset, and night
- **Underwater fog effects**

### Mobile Controls
- **Virtual Joystick** (left side) - Movement control
- **Look Control** (right side swipe) - Camera rotation
- **JUMP Button** - Jump action
- **MINE Button** (red) - Break blocks
- **PLACE Button** (green) - Place blocks
- **INV Button** - Open/close inventory

### Desktop Controls
- **WASD** - Move around
- **Mouse** - Look around (when pointer locked)
- **Left Click** - Mine blocks
- **Right Click** - Place blocks
- **Space** - Jump
- **1-6 Keys** - Select hotbar slot
- **E Key** - Toggle inventory

### Game Mechanics
- **Multiple block types**: Grass, Dirt, Stone, Sand, Wood, Leaves, Ores, and more
- **Tool system**: Hand, Sword, Pickaxe, Axe, Shovel with different efficiencies
- **Mining system**: Progressive breaking with visual feedback
- **Block placement**: With collision detection to prevent placing inside player
- **Item drops**: Blocks drop as collectible items
- **Health & Hunger bars**: Classic Minecraft-style HUD
- **Hotbar selection**: Quick tool/block switching

### Performance Optimizations
- **Chunk-based world** with dynamic loading/unloading
- **Adaptive render distance** based on device capability
- **Efficient mesh building** with face culling
- **Instanced geometry** for better performance
- **Mobile-specific optimizations** for lower-end devices

## 📁 Files

- `minecraft_clone.html` - The complete game in a single HTML file
- `README.md` - This documentation file

## 🚀 How to Play

1. **Open the HTML file** in any modern web browser
2. **Wait for world generation** (loading bar will show progress)
3. **Use the on-screen controls** (mobile) or keyboard/mouse (desktop)
4. **Explore, mine, and build** in your infinite voxel world!

## 🎯 Technical Details

### Technologies Used
- **Three.js** (r160) - 3D graphics library
- **Simplex Noise** - Procedural terrain generation
- **Canvas API** - Texture generation
- **WebGL** - Hardware-accelerated graphics

### Block Types Included
- Grass, Dirt, Stone, Sand
- Oak Wood, Oak Leaves
- Birch Wood, Birch Leaves
- Planks, Cobblestone, Brick, Glass
- Coal Ore, Iron Ore, Gold Ore, Diamond Ore
- Bedrock, Gravel

### Tool Efficiencies
| Tool | Best For | Multiplier |
|------|----------|------------|
| Pickaxe | Stone, Ores | 15-30x |
| Axe | Wood, Planks | 8-10x |
| Shovel | Dirt, Sand, Gravel | 8-10x |
| Sword | Leaves | 3x |
| Hand | Everything else | 1x |

## 📱 Mobile Compatibility

Tested and optimized for:
- iOS Safari
- Android Chrome
- iPadOS
- Mobile Firefox

The game automatically detects mobile devices and:
- Reduces render distance
- Adjusts pixel ratio
- Shows touch controls
- Optimizes shadow quality

## 🎨 Customization

You can easily customize:
- **Colors** - Edit the CSS variables and texture generation
- **Controls** - Modify button positions in CSS
- **World generation** - Adjust noise parameters in `generateChunkData()`
- **Performance** - Change `RENDER_DIST` variable

## ⚠️ Notes

- Requires an internet connection to load Three.js from CDN
- Best experienced on devices with WebGL support
- World is infinite but chunks unload as you move away
- No saving functionality (world resets on refresh)

## 📄 License

This is a fan-made project for educational purposes. Minecraft is a trademark of Mojang Synergies AB.

---

**Enjoy building in your infinite voxel world!** 🏗️⛏️🌲
