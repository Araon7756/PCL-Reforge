# Plain Craft Launcher Reforge

Plain Craft Launcher Reforge (PCL Reforge) is a personal development and experimental build based on the publicly available source code of Plain Craft Launcher 2.

This is an independent personal project, not an official PCL release. It is not affiliated with or endorsed by the Plain Craft Launcher team or CurseForge. Approval for API access does not imply endorsement of the launcher.

## Current purpose and status

The project remains in development and testing. Launcher development and CurseForge integration are being tested locally. This public repository currently contains documentation only; the launcher source code and integration implementation have not yet been published here.

## API approval and integration status

CurseForge approved Plain Craft Launcher Reforge's third-party API application on **October 29, 2026**.

The maintainer has verified the following in the Windows development environment:

- The local runtime environment variable `PCL_CURSEFORGE_API_KEY` is configured.
- A real authenticated request to the official `GET /v1/games` endpoint succeeded.

This confirms API authentication in that environment. CurseForge CDN download compatibility is still under investigation; reliable end-to-end searching, downloading, and installation are not yet claimed as verified.

Planned capabilities include Minecraft mod search, version management and update checks, modpack support, and one-click installation where third-party distribution is permitted. These are development goals, not a statement of production readiness.

The integration will respect CurseForge authors' distribution settings, including the third-party distribution toggle, and comply with the applicable CurseForge API terms. It will not bypass restrictions when an author disables third-party distribution.

## API key handling

The local integration reads the CurseForge API key from the environment variable `PCL_CURSEFORGE_API_KEY` at runtime. Real keys remain local and confidential; no default or shared key is supplied by this repository.

The API key will never be:

- Hardcoded into source code or embedded in application binaries.
- Written to public source code, committed to Git history, or published in a repository.
- Included in release files or other distributed artifacts.
- Written to logs, diagnostic output, or error reports.

## Public distribution status

The authorization requirements and authentication model for publicly distributed builds are still being clarified with CurseForge. This project does not yet claim a confirmed public-distribution authentication scheme. The approved API application and successful local authentication test do not establish permission to share the maintainer's credential or embed it in distributed clients.

Public launcher distribution remains pending confirmation of the applicable CurseForge requirements, a credential-safe authentication approach, download compatibility testing, and review of the upstream permissions and requirements for distributing modified builds.

## Upstream attribution and licensing

The original Plain Craft Launcher 2 is by **LongTengMaoYue (LTCat)**. See the [upstream project](https://github.com/Meloong-Git/PCL) and [original author's sponsorship page](https://meloong.com/afd/a/LTCat).

Upstream rights are governed by the [PCL Limited Distribution License](https://shimo.im/docs/rGrd8pY8xWkt6ryW#anchor-X0bo). Its express permission to redistribute unmodified copies, subject to its restriction on charging for the software itself, must not be treated as blanket authorization to distribute modified builds. The license is non-sublicensable; separately identified third-party components retain their own license terms. This README grants no additional rights and does not relicense upstream code.

The [PCL repository usage guidelines](https://github.com/Meloong-Git/PCL/blob/main/LICENCE) are explanatory, not a legal agreement. For substantial derivatives, they call for clear third-party naming; original-author credit and sponsorship links first in the About page; source publication with the upstream guidance retained; Minecraft purchase and sponsorship prompts; and the required blue Windows visual theme. Public release requires review of the applicable permissions and clarification with the upstream rights holder where needed; compliance is not claimed as completed.
