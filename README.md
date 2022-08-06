# CS offsets<img title="Counter-Strike" align="right" height="128" src="https://user-images.githubusercontent.com/103336115/183117198-abe1b7d3-a250-41f0-a269-2310984d7b30.png#gh-dark-mode-only"/><img align="right" height="128" src="https://user-images.githubusercontent.com/103336115/183117297-ba53f869-1206-4e11-8188-cfce5b48b954.png#gh-light-mode-only"/>
Counter-Strike offsets.

## Supported OS
For now, Windows only.

## Supported builds
Should support **all versions** (1.0 - 1.6). Builds reverse-engineered:
- 1460
- 1600
- 1712
- 1786
- 2006
- 2056
- 2511
- 2603
- 2771
- 2834
- 3213
- 3248
- 3266
- 4156
- 4554
- 4617
- 5944
- 6027
- 6153
- 7561
- 8196
- 8308
- 8684

## Client
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"ScreenFade" + 0x13 // 1460
```

## Server<img title="Server-side" align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183138951-575f59b3-92b7-4bba-9615-bc729748d91a.png#gh-dark-mode-only"/><img align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183138945-64629698-35fd-4b48-920b-fb837dea0d88.png#gh-light-mode-only"/>
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"Server shutting down" - 0x36 // 6027
"Server shutting down" - 0x37 // 1460
```

## Engine
Located in `CLIENT` module or loaded in app in pre-SteamPipe builds.
```cpp
"sprites/%s.spr" + 0x12 // 1460
```
```cpp
g_pClient->Initialize + 0x1D // 5944
g_pClient->Initialize + 0x1C // 4554
g_pClient->Initialize + 0x22 // 2006
g_pClient->Initialize + 0x14 // 1786
g_pClient->Initialize + 0xE // 1460
```

## Studio
Located in `CLIENT` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pClient->HUD_GetStudioModelInterface + 0x1A // 4554
g_pClient->HUD_GetStudioModelInterface + 0x30 // 2006
g_pClient->HUD_GetStudioModelInterface + 0x1A // 1460
```

## StudioAPI
Located in `CLIENT` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pClient->HUD_GetStudioModelInterface + 0x20 // 4554
g_pClient->HUD_GetStudioModelInterface + 0x36 // 2006
g_pClient->HUD_GetStudioModelInterface + 0x20 // 1460
```

## StudioModelRenderer<img title="Read-only" align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183142733-147a896b-15bc-4e08-8940-2e370bfbc344.png#gh-dark-mode-only"/><img align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183142736-e366d334-5ed3-45a5-a1e2-30080c1da8b4.png#gh-light-mode-only"/>
Located in `CLIENT` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pStudioAPI->StudioDrawModel + 0x5 // 1460
```

## Commands
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pEngine->pfnGetCmdList() // 1460
```

## Events
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"CL_HookEvent:  Must provide a valid event name\n" - 0x7 // 6027
"CL_HookEvent:  Must provide a valid event name\n" - 0x6 // 2006
"CL_HookEvent:  Must provide a valid event name\n" - 0x8 // 1460
```

## UserMsgs
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"UserMsg: Not Present on Client %d\n" - 0x14 // 1460
```

## ClientMsgs<img title="Server-side" align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183138951-575f59b3-92b7-4bba-9615-bc729748d91a.png#gh-dark-mode-only"/><img align="right" height="32" src="https://user-images.githubusercontent.com/103336115/183138945-64629698-35fd-4b48-920b-fb837dea0d88.png#gh-light-mode-only"/>
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"SV_ReadClientMessage: badread\n" - 0xD // 6027
"SV_ReadClientMessage: badread\n" - 0xE // 5944
"SV_ReadClientMessage: badread\n" - 0x10 // 4156
"SV_ReadClientMessage: badread\n" - 0xE // 3266
"SV_ReadClientMessage: badread\n" - 0xD // 1786
"SV_ReadClientMessage: badread\n" - 0xC // 1460
```
Note: points to `function` (subtract 8 bytes).

## ServerMsgs
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"-------- Message Load ---------\n" + 0x12 // 1460
```
Note: points to `name` (subtract 4 bytes).

## GlobalVars
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"Too many DLLs, ignoring remainder\n" - 0x15 // 1460
```

## KeyButtons
Located in `CLIENT` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pClient->KB_Find + 0x3 // 4554
g_pClient->KB_Find + 0x11 // 2006
g_pClient->KB_Find + 0x3 // 1460
```

## ClientState
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pEngine->GetEntityByIndex + 0x19 // 6027
g_pEngine->GetEntityByIndex + 0x18 // 2006
g_pEngine->GetEntityByIndex + 0xA // 1460
```

## ClientStatic
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
g_pEngine->pfnGetLevelName + 0x7 // 2006
g_pEngine->pfnGetLevelName + 0x1 // 1460
```

## ClientSpeed<img title="Read-only" align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183142733-147a896b-15bc-4e08-8940-2e370bfbc344.png#gh-dark-mode-only"/><img align="right" width="32" height="32" src="https://user-images.githubusercontent.com/103336115/183142736-e366d334-5ed3-45a5-a1e2-30080c1da8b4.png#gh-light-mode-only"/>
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"Texture load: %6.1fms\n" - 0x7 // 1460
```

## Realtime
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"Searching for local servers...\n" + 0xC // 1460
```

## COM_BuildNumber
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"Half-Life %i/%s (hw build %d)" - 0xC // 1460
```
Note: points to `relative` address.

## Steam_GSInitiateGameConnection
Located in `ENGINE` module or loaded in app in pre-SteamPipe builds.
```cpp
"%c%c%c%cconnect %i %i \"%s\" \"%s\"\n" - 0x48 // 6027
"%c%c%c%cconnect %i %i \"%s\" \"%s\"\n" - 0x49 // 4554
"%c%c%c%cconnect %i %i \"%s\" \"%s\"\n" - 0x6F // 4156
```
Note: points to `relative` address and available only on builds with `STEAMAPI` module.

## Contributing
If there's something you want to add, submit an [issue](https://github.com/rollangles/cs-offsets/issues).