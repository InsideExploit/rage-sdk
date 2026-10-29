# rage-sdk

C++ SDK of Grand Theft Auto V (RAGE), dumped from the running game with [rage-dumper](https://github.com/InsideExploit/rage-dumper).

Each folder is one game build:

| Build | Folder |
| --- | --- |
| 1.0.3889.0 (Legacy) | [`1.0.3889.0`](1.0.3889.0) |

| File | Contents |
| --- | --- |
| `Basic.hpp` | RAGE core types (`atArray`, `atString`, `atHashString`, `atMap`, `Vec3V`, ...) with their x64 sizes. |
| `Enums.hpp` | Enums used by the parser structures. |
| `Classes.hpp` | Parser structures with their members at the registered offsets. |
| `Asserts.hpp` | Size and offset checks. Include it in one translation unit. |
| `Natives.hpp` | Script natives by namespace, as `{ hash, handler, body, command }`; `"GTA5.exe"+offset` is each address. |
