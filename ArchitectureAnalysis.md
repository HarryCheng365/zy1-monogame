# MarkDown
## Context View
### System Requirements
#### Windows
- MonoGame for Visual Studio (requires a 64bit version of Windows, VS2013, VS2015, or VS2017, and the latest DirectX Runtime)
#### Mac OS
- MonoGame for Mac (includes the Mac and iOS assemblies, the Pipeline Tool, and the installs the addin for Xamarin Studio if installed)
Stand alone installer for the MonoGame Pipeline Tool for Mac (requires Mono)
#### Linux
- MonoGame for Linux (includes assemblies, the Pipeline Tool, and the MonoDevelop addin)




## Evolve View(Change Log for latest Three Years)
### 3.6 Release - 2/28/2017
- Fixed XML deserialization of Curve type. #5494
- Fix #5498 Pipeline Tool template loading on MacOS. #5501
- Fix typo in the exclude.addins which cause warnings when installing the Addin in XS. #5500
- Added support for arbitrary defines passed to the Effect compiler. #5496
- Fixed GraphicsDevice.Present() to check for current render target. #5389
- Custom texture compression for SpriteFonts. #5299
- Performance improvements to SpriteBatch.DrawString(). #5226
- Removed the OUYA platform #5194
- Dispose of all graphical resources in unit tests. #5133
- Throw NoSuitableGraphicsDeviceException if graphics device creation fails. #5130
- Optimized and added additional constructors to Color. #5117
- Added SamplerState.TextureFilterMode to correctly support comparison filtering. #5112
- Fixed Apply3D() on stereo SoundEffect. #5099
- Fixed Effect.OnApply to return void to match XNA. #5090
- Fix crash when DynamicSoundEffectInstance not disposed. #5075
- Texture2D.FromStream now correctly throws on null arguments. #5050
- Implemented GraphicsAdapter for DirectX platforms. #5024
- Fixed initialization of GameComponent when created within another GameComponent. #5020
- Improved SoundEffect internal platform extendability. #5006
- Refactored audio processing for platform extensibility. #5001
- Refactored texture processing for platform extensibility. #4996
- Refactor ShaderProfile to allow for pipeline extensibility. #4992
- Removed unnessasary dictionary lookup for user index buffers for DirectX platforms. #4988
- New SetRenderTargets() method which allows for variable target count. #4987
- Added support for XACT reverb and filter effects. #4974
- Remove array in GamePadDPad constructor. #4970
- Updated to the latest version of Protobuild. #4964
- Fixed static VBs and IBs on UWP on XB1. #4955
- Updated to the latest version of Protobuild. #4950
- Update Xamarin Studio addin for latest platform changes. #4926
- Replace OpenTK with custom OpenGL bindings #4874
- Fix Mouse updating when moving the Window. #4924
- Fix incorrect use of startIndex in Texture2D.GetData DX. #4833
- Cleanup of AssemblyInfo for framework assembly. #4810
- New SDL2 backend for desktop GL platforms. #4428
- Two MaterialProcessor properties fixed. #4746
- Fixed thumbstick virtual buttons to always use independent axes. #4742
- Fixed back buffer MSAA on DirectX platforms. #4739
- Added new CHANGELOG.md to project. #4732
- Added obsolete attribute and updated documentation. #4731
- Fixed layout of UWP windows in VS template to ignore window chrome. #4727
- Remove support for reading raw assets through ContentManager. #4726
- Implemented DynamicSoundEffectInstance for DirectX and OpenAL platforms. #4715
- Removed unused Yeti Mp3 compressor. #4713
- MonoGame Portable Assemblies. #4712
- Fixed RGBA64 packing and added unit tests. #4683
- Fix Gamepad crash when platform doesn't support the amount. #4677
- Fixed Song stopping before they are finished on Windows. #4668
- Removed the Linux .deb installer. #4665
- OpenAssetImporter is now automatically selected for all the formats it supports. #4663
- Fixed broken unit tests under Linux. #4614
- Split out Title Container into partial classes. #4590
- Added Rider Support to Linux installer. #4589
- Implement vertexStride in VertexBuffer.SetData for OpenGL. #4568
- Performance improvement to SpriteBatch vertex generation. #4547
- Optimization of indices initialization in SpriteBatcher. #4546
- Optimized ContentReader to decode LZ4 compressed streams directly. #4522
- TitleContainer partial class cleanup. #4520
- Remove raw asset support from ContentManager. #4489
- Initial implementation of RenderTargetCube for OpenGL. #4488
- Removed unnecessary platform differences in MGFX. #4486
- SoundEffect fixes and tests. #4469
- Cleanup FX syntax for shader compiler. #4462
- General Improvements to Pipeline Gtk implementation. #4459
- ShaderProfile Refactor. #4438
- GraphicsDeviceManager partial class refactor. #4425
- Remove legacy Storage classes. #4320
- Added mipmap generation for DirectX render targets. #4189
### 3.5.1 Release - 3/30/2016
- Fixed negative values when pressing up on left thumbstick on Mac.
- Removed exception and just return empty state when requesting an invalid GamePad index.
- Fixed texture processing for 64bpp textures.
- Fixed Texture2D.SaveAsPng on Mac.
### 3.5 Release - 3/17/2016
- Content Pipeline Integration for Xamarin Studio and MonoDevleop on Mac and Linux.
- Automatic inclusion of XNBs into your final project on Mac and Linux.
- Improved Mac and Linux installers.
- Assemblies are now installed locally on Mac and Linux just like they are on Windows.
- New cross-platform �Desktop� project where same binary and content will work on Windows, Linux and Mac desktops.
- Better Support for Xamarin.Mac and Xam.Mac.
- Apple TV support (requires to be built from source at the moment).
- Various sound system fixes.
- New GraphicsMetrics API.
- Optimizations to SpriteBatch performance and garbage generation.
- Many improvements to the Pipeline tool: added toolbar, new filtered output view, new templates, drag and drop, and more.
- New GamePad support for UWP.
- Mac and Linux now support Vorbis compressed music.
- Major refactor of texture support in content pipeline.
- Added 151 new unit tests.
- Big improvements to FBX and model content processing.
- Various fixes to XML serialization.
- MediaLibrary implementation for Windows platforms.
- Removed PlayStation Mobile platform.
- Added content pipeline extension template project.
- Support for binding multiple vertex buffers in a draw call.
- Fixed deadzone issues in GamePad support.
- OcclusionQuery support for DX platforms.
- Fixed incorrect z depth in SpriteBatch.
- Lots of OpenTK backend fixes.
- Much improved font processing.
- Added new VertexPosition vertex format.
- Better VS project template installation under Windows.
### 3.4 Release - 4/29/2015
- Removed old XNA content pipeline extensions.
- Added all missing PackedVector types.
- Replacement of old SDL joystick path with OpenTK.
- Added SamplerState.ComparisonFunction feature to DX and OGL platforms.
- Fixed bug where content importers would not be autodetected on upper case file extensions.
- Fixed compatibility with XNA sound effect XNBs.
- Lots of reference doc improvements.
- Added SamplerState.BorderColor feature to DX and OGL platforms.
- Lots of improvements to the Mac, Linux and Windows versions of the Pipeline GUI tool.
- Fixes for bad key mapping on Linux.
- Support for texture arrays on DX platforms.
- Fixed broken ModelMesh.Tag
- VS templates will now only install if VS is detected on your system.
- Added Color.MonoGameOrange.
- Fixed Xact SoundBack loading bug on Android.
- Added support for a bunch of missing render states to MGFX.
- Added support for sRGB texture formats to DX and OGL platforms.
- Added RasterizerState.DepthClipEnable support for DX and OGL platforms.
- New support for the Windows 10 UAP plafform.
- Fixed bug which caused the GamePad left thumbstick to not work correctly.
- Preliminary base classed for future Joystick API.
- Performance improvement on iOS by avoiding unnessasary GL context changes.
- Fixed bug where MediaPlayer volume affected all sounds.
- New XamarinStudio/MonoDevelop Addin for Mac.
- New Mac installer packages.
