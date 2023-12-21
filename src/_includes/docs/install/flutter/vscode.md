### Use VS Code to install Flutter
{:.no_toc}

#### Start Flutter install
{:.no_toc}

1. Open VS Code.

1. To open the Command Palette,
   press <kbd>Control</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>.

1. In the Command Palette, type `flutter`.

1. Select **Flutter: New Project**.

1. VS Code prompts you to locate the Flutter SDK on your computer.

   {:type="a"}
   1. If you have the Flutter SDK installed, click **Locate SDK**.

   1. If you do not have the Flutter SDK installed, click **Download SDK**.

      This option sends you the Flutter install page if you have not installed
      Git for Windows as directed in the [development tools prerequisites][].

1. When prompted **Which Flutter template?**, ignore it.
   Press <kbd>Esc</kbd>.
   You can create a test project after checking your development setup.

#### Download the Flutter SDK
{:.no_toc}

1. Choose which folder to install Flutter
   using the **Select Folder for Flutter SDK** dialog.

   VS Code places you in your user profile to start.
   Choose a different location.

   Consider `%USERPROFILE%` or `D:\dev`.

   {% include docs/install/admonitions/install-paths.md %}

1. Click **Clone Flutter**.

   While downloading Flutter, a notification displays:

   ```terminal
   Downloading the Flutter SDK. This may take a few minutes.
   ```

   This download takes a few minutes.
   If you suspect that the download has hung, click **Cancel** then
   start the installation again.

1. Once it finishes downloading Flutter, the **Output** panel displays.

   ```terminal
   Checking Dart SDK version...
   Downloading Dart SDK from the Flutter engine ...
   Expanding downloaded archive...
   ```

   When successful, a notification displays:

   ```terminal
   Initializing the Flutter SDK. This may take a few minutes.
   ```

   While initializing, the **Output** panel displays the following:

   ```terminal
   Building flutter tool...
   Running pub upgrade...
   Resolving dependencies...
   Got dependencies.
   Downloading Material fonts...
   Downloading Gradle Wrapper...
   Downloading package sky_engine...
   Downloading flutter_patched_sdk tools...
   Downloading flutter_patched_sdk_product tools...
   Downloading windows-x64 tools...
   Downloading windows-x64/font-subset tools...
   ```

   This process also runs `flutter doctor -v`.
   At this point in the procedure, _ignore this output._
   Flutter Doctor might show errors that don't apply to this quick start.

   When the Flutter install succeeds, a notification displays:

   ```terminal
   Do you want to add the Flutter SDK to PATH so it's accessible
   in external terminals?
   ```

1. Click **Add SDK to PATH**.

   When successful, a notification displays:

   ```terminal
   The Flutter SDK was added to your PATH
   ```

1. The notification displays the Google Analytics notice.

   If you agree, click **OK**.

1. To enable `flutter` in all terminal windows:

   {:type="a"}
   1. Close, then reopen all Powershell windows.
   1. Restart VS Code.

[development tools prerequisites]: #development-tools