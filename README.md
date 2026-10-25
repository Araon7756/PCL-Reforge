# Plain Craft Launcher Reforge

Plain Craft Launcher Reforge (PCL Reforge) is a personal development and experimental build based on the publicly available source code of Plain Craft Launcher 2.

This is an independent personal project. It is not an official PCL release and is not affiliated with or endorsed by the Plain Craft Launcher team.

## Current purpose and status

The project is currently intended for personal development, learning, and testing. This repository currently contains the project documentation; the launcher source code and the planned API integration have not been added yet.

## Planned CurseForge API integration

The project plans to integrate the official CurseForge API to search Minecraft mods and modpacks, retrieve project and file metadata, check for updates, and obtain download information where third-party distribution is permitted.

The integration will respect CurseForge authors' distribution settings, including the third-party distribution toggle, and comply with the applicable CurseForge API terms. It will not bypass restrictions when an author disables third-party distribution.

## API key handling

The planned integration will read the CurseForge API key from the local environment variable `PCL_CURSEFORGE_API_KEY` at runtime.

The API key will never be:

- Hardcoded into source code or embedded in application binaries.
- Committed to Git or published in a repository.
- Included in release files or other distributed artifacts.
- Written to logs, diagnostic output, or error reports.

Any real key must remain local and confidential. This repository currently contains no real CurseForge API key.
