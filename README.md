# Revit Material Texture Relinker

A PyRevit tool that scans appearance assets in a Revit model and reconnects missing texture file paths.  
It searches for texture files by filename across one or more user-defined root folders and remembers those folders across sessions.

---

## Overview

Revit often loses texture links when projects are moved or shared.  
This tool automatically finds and reconnects those missing texture files based on their filenames within your texture library folders.

It is lightweight, safe to run, and operates inside a controlled Revit transaction.

---

## Features

- Relinks missing material textures by filename  
- Searches multiple root folders recursively  
- Remembers folders across sessions  
- Automatically includes the current project folder  
- Displays unresolved textures in the PyRevit output panel  
- Built-in help popup for quick onboarding  
- Safe and reversible transaction scope  
- Designed for the **Materials** tab in the **SwichTools** extension  

---

The bundle follows the PyRevit standard layout so it can load directly when placed in your extensions directory.

---

## Installation

### Manual Install

Copy the entire folder to:

E:\Users[username]\AppData\Roaming\pyRevit-Master\extensions\

Then restart Revit or reload extensions from the PyRevit settings window.

### Optional (for Git tracking)

You can manage the repository through Git by cloning it directly into your extensions directory if you maintain version control for your tools.

---

## Usage

1. Open your Revit model.  
2. Go to the **Materials** tab → **Repair** panel → **Relink Textures**.  
3. The menu gives you these options:  hover the cutton to Show quick help popup  
   - **r**: Run the relink process  
   - **m**: Manage or add search folders  
   - **c**: Cancel  
4. Add the top-level folders where your texture libraries live.  
5. Run the search and relink process.  
6. Check the PyRevit output panel for unresolved texture names.

---

## Requirements

- Autodesk Revit 2023 or later  
- PyRevit 5.3 or newer  
- Windows 10 or newer  

---

## License

This project is open source under the **Apache License 2.0**.  
You are free to use, modify, and distribute this software for personal or commercial purposes.  
See [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0) for full details.
Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

---

## Credits

Created by **Roi Hason**  Swich Design
Built for production-ready BIM environments using PyRevit  
Designed for the **Materials** tab in the **SwichTools** extension

---

## Summary

This tool keeps Revit projects visually consistent by fixing broken material texture links quickly and safely.  
Ideal for teams sharing models between workstations or migrating large material libraries.
