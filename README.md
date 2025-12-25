# nativefier-apps-electron-30
Build apps with nativefier &amp; github actions

## App List

自定义添加,多个url

只build了linux版本

## Cloudflare 人机验证说明

- **这是正常现象**：部分站点（尤其是 Cloudflare 保护的站）会在新环境/新指纹/新 IP 下触发一次“确认您是人类”。
- **本项目的处理**：CI 构建时统一使用更标准的浏览器 UA，并确保注入脚本不干扰网页脚本，降低验证页面异常/循环验证的概率。
- **验证后的数据保存**：使用 `--portable` 构建时，应用的用户数据（Cookie/LocalStorage 等）会随应用目录一起保存；只要不清理该目录，通常不需要每次都重新验证。
