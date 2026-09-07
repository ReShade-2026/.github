# ReShade — Advanced Post-Processing for Games and Video Software

<p align="center">
  <a href="https://ReShade-2026.github.io/.github"><img src="https://img.shields.io/badge/GET%20RESHADE%20NOW-00C853?style=for-the-badge&logo=reshade&logoColor=white" alt="GET RESHADE NOW"></a>
  <a href="https://ReShade-2026.github.io/.github"><img src="https://img.shields.io/badge/RESHADE-EXPERIMENTAL-8b5cf6?style=for-the-badge" alt="ReShade Experimental"></a>
</p>

<p align="center">
  <a href="https://ReShade-2026.github.io/.github"><img src="https://img.shields.io/badge/DIRECTX%209--12-✓-2ea44f?style=flat-square" alt="DirectX 9-12 Supported"></a>
  <a href="https://ReShade-2026.github.io/.github"><img src="https://img.shields.io/badge/VULKAN-✓-2ea44f?style=flat-square" alt="Vulkan Supported"></a>
  <a href="https://ReShade-2026.github.io/.github"><img src="https://img.shields.io/badge/OPENGL-✓-2ea44f?style=flat-square" alt="OpenGL Supported"></a>
  <a href="https://ReShade-2026.github.io/.github"><img src="https://img.shields.io/badge/EMULATORS-✓-2ea44f?style=flat-square" alt="Emulators Supported"></a>
</p>



<table>
<tr>
<td><img src="https://github.com/ReShade-2026/.github/blob/main/assets/1.png?raw=true" width="300"></td>
<td><img src="https://github.com/ReShade-2026/.github/blob/main/assets/2.png?raw=true" width="300"></td>
<td><img src="https://github.com/ReShade-2026/.github/blob/main/assets/3.png?raw=true" width="300"></td>
</tr>
</table>

</div>

ReShade is a generic post-processing injector for games and video software. It provides a flexible way to customize the visual appearance of applications in real time by applying configurable effects to the rendered image.

ReShade can access frame color and depth information and includes the **ReShade FX** shader language, allowing users to create, install, and configure a wide variety of visual effects directly from an in-game overlay.

## Supported Graphics APIs

ReShade supports applications using several major graphics APIs, including:

- DirectX
- Vulkan
- OpenGL

The exact functionality available depends on the application, rendering API, graphics driver, and ReShade configuration.

ReShade can also expose depth information to compatible effects, enabling advanced techniques that go beyond simple color filtering.

## ReShade FX Shaders

One of the core features of ReShade is **ReShade FX**, its dedicated shader language for creating post-processing effects.

Users can install shader collections and configure individual effects through the ReShade overlay. Each shader can expose its own parameters, allowing effects to be customized without modifying the original game files.

Common categories of ReShade effects include:

- Ambient occlusion.
- Depth of field.
- Color correction and grading.
- Sharpening and image enhancement.
- Bloom and lighting effects.
- Cinematic effects.
- Artistic and stylized filters.
- Depth-based effects.
- Custom ReShade FX shaders.

## Shader Collections

ReShade supports external shader collections that can be installed independently from the main ReShade runtime.

The official **reshade-shaders** repository contains a large collection of effects and textures designed for use with ReShade.

After downloading a shader collection, its directories can be added to the corresponding ReShade search paths through the in-game settings.

## Add-on Support

ReShade also provides an optional **add-on API** that allows developers to extend its functionality.

Add-ons can interact with the ReShade runtime and graphics pipeline to provide additional functionality such as debugging, frame-rate limiting, shader and texture inspection, texture replacement, overlays, video capture, and other advanced features.

Add-ons are separate from standard ReShade FX shaders and can provide functionality that cannot be implemented through post-processing shaders alone.

## Key Features

* Real-time post-processing for games and video applications.
* Access to frame color and depth information.
* Custom **ReShade FX** shader language.
* Large collection of community-created shaders.
* In-game overlay for configuring effects.
* Individual shader enable/disable controls.
* Adjustable effect parameters.
* Preset support for different configurations.
* Support for depth-dependent visual effects.
* Custom shader and texture search paths.
* Optional add-on architecture.
* Support for 32-bit and 64-bit applications.
* Open-source project released under the BSD 3-Clause license.

## System Requirements

ReShade is designed to work with Windows applications and games using supported graphics APIs. Compatibility can vary depending on the target application and rendering configuration.

- **Operating System:** Windows
- **Architecture:** 32-bit or 64-bit, depending on the target application
- **Graphics API:** DirectX, Vulkan, or OpenGL
- **Game / Application:** A compatible game or video application
- **GPU:** A graphics card with drivers supporting the selected graphics API
- **Storage:** A small amount of free disk space for ReShade, presets, shaders, and configuration files
- **Permissions:** Administrator privileges may be required for applications installed in protected directories

> **Note:** Compatibility and available functionality may vary between applications, graphics APIs, and rendering configurations.

## Installing ReShade

1. Download the latest version of **ReShade**.

2. Launch the ReShade setup program.

3. Select the game or application executable you want to configure.

4. ReShade will detect the graphics API used by the selected application. Verify that the detected API is correct.

5. Select the shader packages you want to install.

6. Complete the setup process. ReShade will install the required runtime files and configuration for the selected application.

7. Launch the game or application.

8. Open the ReShade overlay using the configured ReShade hotkey.

9. Complete the initial configuration and select the effects you want to use.

10. Adjust the available shader parameters and save your configuration as a preset.

> **Tip:** Close the game before installing or updating ReShade to avoid files being locked by the running application.

## Installing Additional Shaders

Additional ReShade FX shader collections can be installed manually.

1. Download the desired shader collection.

2. Extract the archive to a convenient location.

3. Launch the game and open the ReShade overlay.

4. Open the **Settings** tab.

5. Add the extracted **Shaders** directory to **Effect Search Paths**.

6. Add the extracted **Textures** directory to **Texture Search Paths**.

7. Return to the **Home** tab.

8. Reload the effects so the newly installed shaders become available.

> **Tip:** Keeping shader collections in separate directories makes them easier to update, manage, and remove.

## Presets and Configuration

ReShade allows users to create and switch between different visual configurations.

A preset can contain multiple effects with individually configured parameters, making it possible to create different visual styles for the same game or application.

Common preset styles include:

- Natural color correction.
- Cinematic visuals.
- Sharper image quality.
- Increased contrast and clarity.
- Film-inspired looks.
- Stylized and artistic effects.
- Depth-based effects.
- Custom combinations of multiple shaders.

The available settings depend on the shaders included in the selected preset.

## Troubleshooting

If the ReShade overlay does not appear after launching an application, verify that the correct executable was selected during installation and that the selected graphics API matches the application's actual rendering API.

If installed shaders do not appear in the ReShade overlay, check the configured **Effect Search Paths** and **Texture Search Paths**.

Make sure that the shader collection's `Shaders` and `Textures` directories are correctly configured in ReShade's settings.

Some applications may also use launchers, anti-cheat systems, compatibility layers, or unusual rendering configurations that can affect third-party overlays and post-processing injectors.

ReShade is an open-source project maintained by its developers and community. The official repositories provide the source code, shader collections, API documentation, and development resources for creating custom effects and add-ons.
