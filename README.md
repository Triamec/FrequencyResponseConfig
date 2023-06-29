# BodeConfig

This sample demonstrates how to customize the Bode measurement.

If in the current workspace, in the folder TAM\Settings, there is a `BodeConfig.xml` file, this file will be used in favor
of the inbuilt definition.

You can find your current workspace whith the TAM System Explorer via `File > Open Workspace Folder`.\
You can also create new workspaces with their own settings via `File > New > Workspace`

Adapting the `BodeConfig.xml` allows you for example to record different signals represented in the Registers.

In order to modify the configuration, we propose to use Visual Studio. For this sake, the sample contains the BodeConfig
solution under Projects.
You get full Intellisense support for the Bode configuration format, including help tooltips. This works by virtue of
the BodeConfig.xsd file linked into the Visual Studio project.

Known Limitations

- Only the first four measurement points will be shown in the GUI. For the others, no maximum can be specified, and the
  signal is not plotted during measurement. However, the frequency response will be shown in the result.

- Bode tuning only works correctly if the first three frequency response vectors are similar to the Open Loop Bode
  measurement method.
