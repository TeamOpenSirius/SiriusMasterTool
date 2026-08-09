# SiriusMasterTool

独立的官方 MasterData 下载与更新工具。

本仓库只负责：

- 获取环境与 MasterData 清单；
- 下载、校验并更新 `mastermemory.db`；
- 按 `data/table.json` 导出 MasterData JSON；
- 输出供部署流程读取的 manifest/publication 元数据。

资产同步、Master Index、R2 发布和 Scene Index 均保留在 YmstServer 的工具子项目中。

## Build

```powershell
dotnet build Sirius.MasterTool.sln -c Release
```

## Run

```powershell
src\Sirius.MasterTool\bin\Release\net10.0\Sirius.MasterTool.exe --sync --dir output
```

运行 `Sirius.MasterTool.exe --help` 查看认证及更新选项。
