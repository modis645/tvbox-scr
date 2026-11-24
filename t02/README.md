# t02 · TVBox 配置与 jar（自动生成，勿手改）

配置内容：97 个实测可播站，按实测 ms 从快到慢排序；jar 只引用本目录 `spiders/`。

## 安卓（FongMi / TVBox）

任选一条填到「点播配置」：

- ghfast：`https://ghfast.top/https://raw.githubusercontent.com/modis645/tvbox-scr/main/t02/config_android_ghfast.json`
- ghproxy：`https://ghproxy.net/https://raw.githubusercontent.com/modis645/tvbox-scr/main/t02/config_android_ghproxy.json`
- ghproxy_net：`https://ghproxy.net/https://raw.githubusercontent.com/modis645/tvbox-scr/main/t02/config_android_ghproxy_net.json`
- jsdelivr：`https://cdn.jsdelivr.net/gh/modis645/tvbox-scr@main/t02/config_android_jsdelivr.json`
- raw：`https://raw.githubusercontent.com/modis645/tvbox-scr/main/t02/config_android_raw.json`
- 备用默认副本：`config_android.json`

各份的站点完全一致，只有 `jar` 地址前缀不同；哪条能通就用哪条。

## 电脑（仅直连站，无 jar）

`https://ghfast.top/https://raw.githubusercontent.com/modis645/tvbox-scr/main/t02/config_pc.json`

## 说明

- `spiders/*.jar.png` 实际是 jar 字节，只是改名为 .png 规避 raw 的 MIME 嗅探；播放器按字节加载，不影响使用。
- 更新流程：电视/网页点「生成并打包」→ 重新上传本目录的 `config_android_*.json` 与 `spiders.json` 列出的 jar。
- `links.txt` 为全部地址清单；`spiders.json` 为本次真正引用到的 jar。
