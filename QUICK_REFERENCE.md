# 🎮 Real Asset Creator - Quick Reference Guide

## 🚀 **Quick Start Commands**

```bash
# Launch the application
python launch_real_creator.py

# Test MCP connection (ALWAYS DO THIS FIRST)
# Select option 2 from launcher

# Launch main application
# Select option 1 from launcher
```

## 🎨 **Asset Creation Menu**

| Option | Asset Type | Creates | Time |
|--------|------------|---------|------|
| 1 | 👤 Game Character | Rigged character with skin + clothing | ~3 sec |
| 2 | 🚗 Vehicle Asset | Blue car with metallic paint + components | ~3 sec |
| 3 | 🏗️ Environment Scene | Building with props + atmospheric lighting | ~4 sec |
| 4 | 🎨 Material Showcase | 6 PBR materials (Chrome, Gold, Wood, etc.) | ~3 sec |
| 5 | ⚔️ Weapon Asset | Medieval sword with steel + brass + leather | ~3 sec |
| 6 | 🏠 Complete Scene | All assets combined in one scene | ~15 sec |

## 👁️ **Viewing Assets in Blender**

### Essential Controls
- **'Z' key** → Viewport shading menu
- **Middle Mouse** → Orbit around scene
- **Scroll Wheel** → Zoom in/out
- **Numpad 0** → Camera view

### Best Viewport Modes
- **Material Preview** ⭐ → Shows materials clearly
- **Rendered** ⭐ → Full realistic rendering

## 🎯 **Asset Details Quick Reference**

### 👤 Character Asset
- **Components:** Head, body, arms, legs
- **Rigging:** 7-bone armature
- **Materials:** Skin tone + blue clothing
- **Best View:** Material Preview mode

### 🚗 Vehicle Asset
- **Components:** Body, hood, roof, 4 wheels, windshield, headlights
- **Materials:** Metallic blue, rubber tires, glass, emissive lights
- **Best View:** Rendered mode for reflections

### 🏗️ Environment Asset
- **Components:** Building, entrance, 4 windows, roof, 8 props, terrain
- **Materials:** Stone, wood, glass, metal, ground
- **Best View:** Rendered mode for atmospheric effects

### 🎨 Material Showcase
- **Materials:** Chrome, Gold, Wood, Plastic, Ceramic, Rubber
- **Layout:** 6 spheres in circle with pedestals and labels
- **Best View:** Rendered mode (REQUIRED for PBR)

### ⚔️ Weapon Asset
- **Components:** Blade, crossguard, handle, pommel, stand
- **Materials:** Steel, brass, leather, wood
- **Best View:** Rendered mode for metal reflections

## 🔧 **Troubleshooting Quick Fixes**

| Problem | Quick Solution |
|---------|----------------|
| Can't see asset | Press 'Z' → Material Preview |
| Materials look flat | Switch to Rendered mode |
| MCP connection failed | Test connection (launcher option 2) |
| Blender running slow | Use Material Preview instead of Rendered |
| Asset outside view | Press 'A' then 'F' to frame all |

## 📊 **Session Management**

| Menu Option | Function |
|-------------|----------|
| 7 | 📊 View Created Assets - See summary of all created assets |
| 8 | 💾 Export Assets - Export functionality (coming soon) |
| 9 | 📋 Generate Report - Detailed session statistics |

## 💾 **Manual Export (Current Method)**

In Blender:
1. **Select asset** → Click on object
2. **File → Export → FBX** → For Unity/Unreal
3. **File → Export → glTF 2.0** → For web/mobile
4. **File → Export → Wavefront (.obj)** → For general use

## 🎯 **Pro Tips**

### ✅ **Do This**
- **Always test MCP connection first** (launcher option 2)
- **Use Material Preview** for editing assets
- **Use Rendered mode** for final viewing
- **Create assets one at a time** to verify each works
- **Save Blender file** after creating assets you want to keep

### ❌ **Avoid This**
- **Don't skip MCP connection test** - Always verify first
- **Don't use Solid mode** for viewing materials
- **Don't create too many assets** in one session (performance)
- **Don't close Blender** while creating multiple assets

## 📁 **File Locations**

```
blender-mcp-server/
├── real_asset_creator_app.py     # Main application
├── launch_real_creator.py        # Launcher
├── created_assets/               # Generated assets directory
│   └── real_assets_session.json # Session log
└── STEP_BY_STEP_TUTORIAL.md     # Full tutorial
```

## 🎨 **Material Properties Reference**

| Material | Metallic | Roughness | Color | Use Case |
|----------|----------|-----------|-------|----------|
| Chrome | 1.0 | 0.0 | Light Gray | Reflective metals |
| Gold | 1.0 | 0.1 | Yellow-Orange | Precious metals |
| Wood | 0.0 | 0.8 | Brown | Natural materials |
| Plastic | 0.0 | 0.3 | Various | Synthetic materials |
| Ceramic | 0.0 | 0.1 | White | Smooth surfaces |
| Rubber | 0.0 | 0.9 | Black | Matte materials |

## 🚀 **Workflow Examples**

### Quick Asset Creation
```
1. python launch_real_creator.py
2. Select 2 (Test MCP)
3. Select 1 (Launch App)
4. Select 1 (Create Character)
5. Open Blender → Press 'Z' → Material Preview
```

### Complete Scene Creation
```
1. Launch application
2. Create Environment (option 3)
3. Add Vehicle (option 2)
4. Add Character (option 1)
5. Add Weapon (option 5)
6. View complete scene in Rendered mode
```

### Material Study Session
```
1. Create Material Showcase (option 4)
2. Switch Blender to Rendered mode
3. Orbit around to study each material
4. Compare metallic vs non-metallic properties
```

---

**🎯 Need the full tutorial? See `STEP_BY_STEP_TUTORIAL.md`**

**🔧 Need integration help? See `REAL_ASSET_INTEGRATION_GUIDE.md`**

**📊 Want complete details? See `REAL_ASSET_CREATOR_SUMMARY.md`**
