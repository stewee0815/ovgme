----------------------------------------------------------------------------------------
OvGME
Enhanced Generic Mod Enabler and manager.
----------------------------------------------------------------------------------------
**Version: 1.8.0, May 2022**
- increased repository download speed (limited only(?) by the repo server and your ISP)
- no installer anymore, sorry.
- based on the last version released some years ago

----------------------------------------------------------------------------------------

Home page: https://github.com/VNAO-Solid/ovgme

Credits:
----------------------------------------------------------------------------------------
All credits to Sedenion (Eri M.?). He created this wonderful tool afaik.

He is working on a new mod manager called "Open Mod Manager" (https://github.com/sedenion/OpenModMan).
Check it out regularly in order not to miss switching from OvGME to this new tool!

Presentation
----------------------------------------------------------------------------------------
OvGME is a Mod manager based on the idea and concept of JSGME, it take the GME acronym
from JSGME which stands for Generic Mod Enabler. The main purpose of OvGME is to provide an
easy way to import and enable mods for games then restore original files when disabling mods.
OvGME works by comparing the destination folder file tree with the given mod file tree,
then identifies what files to replace, create and save as backup.

OvGME implements the following key features:

- Support for multiple destination folder (game, software, etc.) through the main GUI.
- Custom Mods and Backup folder for each destination folder.
- Destination folder file tree snapshot and comparison based on xxHash.
- Zipped Mods files (Mod-Archives).
- Mods description (readme.txt).
- Mods versioning.
- Mods enabling profile for each destination folder.
- Mods network repositories.
- Mods online updating and downloading.
- Zip Mod-Archive creation tool.
- XML repository creation tool.
- Detailed embedded Help.


If you already use JSGME
Please read carefully the "OvGME and JSGME" chapter in the embedded help before doing
anything.

Screenshots
----------------------------------------------------------------------------------------
![OvGME Screenshot](snaps/screenshot.png)

Third party libraries
----------------------------------------------------------------------------------------


OvGME >=v1.8.0 uses curl to download files:

CURL COPYRIGHT AND PERMISSION NOTICE

Copyright (c) 1996 - 2022, Daniel Stenberg, daniel@haxx.se, and many contributors, see
the THANKS file.

All rights reserved.

Permission to use, copy, modify, and distribute this software for any purpose with or
without fee is hereby granted, provided that the above copyright notice and this permission
notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING
BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT OF THIRD PARTY RIGHTS. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
IN THE SOFTWARE.

Except as contained in this notice, the name of a copyright holder shall not be used in
advertising or otherwise to promote the sale, use or other dealings in this Software
without prior written authorization of the copyright holder.

