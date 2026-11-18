---
name: document-lifecycle-management
description: Create, revise, review, restore and export Office-style documents using one canonical editable document per deliverable; trigger for Word, Excel, PPT, online documents and revision requests.
---
# 文档生命周期管理 V1.0
## 路由
授权资料默认 Google Docs / Sheets / Slides；公司内部资料使用企业授权平台；复杂 Office 原生模板、宏、特殊公式或版式采用获准的原生 Office 方案。明确要求下载时按要求交付。
## 执行
1. 识别任务与已有主文档，先查索引及原链接，避免重复创建。记录文件 ID、链接、类型、权限边界、状态及最后核验时间；索引只能放授权私有环境。
2. 新任务建立一个主文档；修改前读取最新版本，确认目标段落、区域或页面；保留已确认内容、格式、公式及图片。
3. 原位局部修改，防止并发覆盖；有冲突则停止并报告。无原位写权限时报告阻塞，不默认另建文件。
4. 写后回读并核对同一 ID、目标改动及未触及内容。返回原链接与简短变更摘要。
5. 使用平台历史记录；能命名版本时在重要节点命名，不能则记录可核验的修订 ID；不保证平台保留每一次编辑。恢复前核对目标版本与影响，经用户确认后执行；若无恢复接口，说明手动操作路径。
6. 草稿→审核中→已确认→已交付。用户确认后按需导出 DOCX/XLSX/PPTX/PDF，核查格式、公式、版式及图片。未经确认不标终稿。
## 安全
不得把未获授权的企业资料、个人隐私、凭证或实际文档索引写入公开仓库或外部平台。不得擅自公开分享。
## 验收
用虚构材料独立验证三种文档的创建、原位修改、同 ID 回读、历史查询、恢复及导出；区分工具可用、已测试与未测试。Codex 安装和授权须在真实执行环境验证，不以写入本文件视为已安装。
## 资源
按需触发，不新增定时轮询，不重复生成文件。
