# Quick Start Guide - Blender MCP Server

## 🎉 Your Blender MCP Server is Ready!

The server has been successfully installed and tested. Here's how to use it with Q CLI:

## Step 1: Configure Q CLI

Add the MCP server to your Q CLI configuration. The configuration file location depends on your setup, but typically it's in one of these locations:

- `~/.config/q/mcp.json`
- `~/.q/mcp.json`

Add this configuration:

```json
{
  "mcpServers": {
    "blender": {
      "command": "mcp-blender-server",
      "args": []
    }
  }
}
```

## Step 2: Test with Q CLI

Once configured, you can use the Blender tools through Q CLI:

```bash
q chat "Check if Blender is available and list the available templates"
```

```bash
q chat "Create a cube in Blender and then add a red material to it"
```

```bash
q chat "Create a sphere in Blender, list all objects in the scene, and render it"
```

## Available Commands

The MCP server provides these tools:

1. **blender___check_blender_status** - Check if Blender is installed and running
2. **blender___list_blender_templates** - List available script templates
3. **blender___run_blender_template** - Run predefined templates (create_cube, create_sphere, etc.)
4. **blender___execute_blender_script** - Execute custom Python scripts in Blender

## Example Conversations

### Basic Object Creation
```
You: "Create a cube in Blender"
Q: I'll create a cube in Blender for you.
[Uses blender___run_blender_template with template_name: "create_cube"]
```

### Custom Scripting
```
You: "Create 5 cubes in a line in Blender"
Q: I'll create 5 cubes arranged in a line using a custom script.
[Uses blender___execute_blender_script with custom Python code]
```

### Scene Management
```
You: "Show me what objects are in my Blender scene"
Q: Let me list all the objects in your current Blender scene.
[Uses blender___run_blender_template with template_name: "list_objects"]
```

## Troubleshooting

If you encounter issues:

1. **Server not found**: Make sure the server is installed with `pip install -e .`
2. **Blender not found**: Use `--blender-path` option or install Blender
3. **Permission issues**: Ensure Blender executable has proper permissions

## Next Steps

- Explore the predefined templates
- Create custom Blender scripts
- Combine multiple operations in single conversations
- Use with .blend files by specifying file paths

Happy 3D modeling with AI assistance! 🎨
