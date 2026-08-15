Hi there. If you found this and would like to adapt it to your own project, edit the Device Name + version number field in "./Core/Src/Dev_Inf.c"
Make sure to verify your Quad-SPI pin out in STM32CubeMX by opening audio_external_loader.ioc. Regenerate the code if you end up changing the pin locations.
Finally, disable "discard unused sections" in the linker options.

The output .elf binary extention must be renamed .stldr and placed here to appear in STM32CubeProgrammer:

```
C:\Program Files\STMicroelectronics\STM32Cube\STM32CubeProgrammer\bin\ExternalLoader
```