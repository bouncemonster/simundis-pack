<div align="center">

# SIMUNDIS · Client Pack

**One distribution point for the Simundis client setup.**

Modpack import · Versioned mod synchronization · Generated release artifacts

[Get the modpack](../Simundis.mrpack?raw=1) · [Sync manifest](../schema.json) · [Companion archive](../basics.zip?raw=1)

</div>

---

This repository distributes the **Simundis client pack**. It contains the packaged client setup and the manifest consumed by Simple Mod Sync; it is not the server source repository or a place to develop individual mods.

## Choose your starting point

| You need to… | Use |
| --- | --- |
| Import the packaged client setup | [`Simundis.mrpack`](../Simundis.mrpack?raw=1) with a launcher that supports the `.mrpack` format. |
| Inspect the synchronized mod list | [`schema.json`](../schema.json). Entries contain download URLs, names, versions and artifact types. |
| Obtain the companion distribution archive | [`basics.zip`](../basics.zip?raw=1). |
| Understand how these files are published | The [generated publication notice](../README.md) and the publishing workflow in the source project. |

**Keep the pack's versions together.** The checked-in manifest currently contains Fabric mod entries targeting the 26.3 line. Treat the distributed pack and manifest as the version reference; this page does not promise compatibility with a different Minecraft version, mod loader or independently upgraded mod set.

## Install without disturbing an existing world

Download the `.mrpack` artifact and import it as a **separate launcher instance**. Review the launcher's requested game and loader versions, let it obtain the declared dependencies, then launch the new instance. Keep existing saves and custom configurations backed up before replacing or migrating another instance.

A repository download is not a Minecraft account, game entitlement or server-access grant. Server connection details are deliberately not invented here.

## How the distribution is maintained

```text
Source project's publishing workflow
                  ↓
       Pack + manifest + companion archive
                  ↓
       Launcher import / mod synchronization
```

The root publication notice identifies `scripts/publish-pack.ps1` as the generator. **Do not hand-edit generated artifacts to introduce a new pack version.** Make the change in the source publishing workflow, regenerate the distribution and review the resulting artifact changes together.

This maintained landing page lives in `.github/README.md` so the generated root `README.md` remains intact. The publisher should preserve `.github/` when refreshing the distribution.

## Report a problem

Include the downloaded pack revision, launcher, operating system, game/loader versions and the relevant error excerpt. Distinguish an import failure, dependency-download failure and crash after launch. Remove access tokens, personal paths and server credentials from logs before sharing them.

## Licensing

Included mods and downloaded dependencies retain their own licenses. The presence of a pack or manifest does not replace those licenses or create a blanket redistribution grant.

---

### По-русски

Это репозиторий **клиентской сборки Simundis**, а не исходный код сервера. Для установки скачайте `Simundis.mrpack` и импортируйте его в отдельный экземпляр игры через совместимый лаунчер. `schema.json` описывает синхронизируемые моды, `basics.zip` — дополнительный архив публикации. Не смешивайте версии сборки и не заменяйте существующие сохранения без резервной копии.

Файлы сборки генерируются процессом публикации. Описание вынесено отдельно, чтобы не перезаписывать автоматически создаваемый README и не вмешиваться в состав модов.
