# Frequency Response Configuration

This sample demonstrates how to customize the frequency response measurement.

If in the current workspace, in the folder `Settings`, there is a `FrequencyResponseConfig.xml` file, this file will be used in favor
of the inbuilt definition.

You can find your current workspace with the TAM System Explorer via `File > Open Workspace Folder`.
You can also create new workspaces with their own settings via `File > New > Workspace`.

Adapting the `FrequencyResponseConfig.xml` allows you for example to record different signals represented in the registers.

In order to modify the configuration, we propose to use Visual Studio. For this sake, the sample contains the FrequencyResponseConfig
solution under `Projects`.
You get full Intellisense support for the configuration format, including help tooltips. This works by virtue of
the `FrequencyResponseConfig.xsd` file linked into the Visual Studio project.

Known Limitations

- Only the first four measurement points will be shown in the GUI. For the others, no maximum can be specified, and the
  signal is not plotted during measurement. However, the frequency response will be shown in the result.

- Frequency response tuning only works correctly if the first three frequency response vectors are similar to the Open Loop
  measurement method.

- Prior to TAM Software 7.25.0, the file was named `BodeConfig.xml`.
