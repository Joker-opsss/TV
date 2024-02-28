# TVBox 电视直播源接口自动更新

根据基础模板直播源接口文件自动获取并更新最新直播源接口链接

[English](./README-EN.md) | 中文

## 特点

- 接口效验，过滤无效接口，排序规则：日期、速度、分辨率
- 定时执行，每隔 12 小时执行更新一次
- 可设置重点关注频道，单独配置获取分页的数量
- 分页结果获取（可配置页数、总接口数量）

## 使用方法

1. Fork 此项目，开启 Action 工作流可读写权限，Settings → Actions → General → Workflow permissions → Read and write permissions → Save
2. 修改 demo.txt 模板文件，后续更新根据此文件内容进行更新
3. 修改配置 config.py(可选)：

- source_file：模板文件，默认值：demo.txt
- final_file：生成文件，默认值：result.txt
- favorite_list：关注频道名称列表
- favorite_page_num：关注频道获取分页数量，默认值：5
- default_page_num：常规频道获取分页数量，默认值：3
- urls_limit：接口数量，默认值：15
- filter_invalid_url：是否过滤无效接口，默认值：True

4. result.txt 为更新后的直播源接口文件，source.json 为数据源文件

## 免责声明

本项目是为了提供编程学习和研究的资源。项目中收集的数据来源于网络，开发者不对数据的准确性、完整性或可靠性做任何保证。

开发者不对任何可能因使用这些代码或数据而产生的任何直接或间接损失负责。使用者应自行判断其使用的合法性和风险。

本项目的代码和数据仅供学习和研究使用，不得用于任何商业用途。任何人或组织在使用时，应遵守相关法律法规，尊重并保护开发者的权益。

如果您使用了本项目的代码或数据，即表示您已了解并同意此免责声明。如果您不同意此免责声明，您应立即停止使用本项目的代码和数据。

此外，本项目的代码和数据可能会不定期进行更新，但不保证更新的及时性和准确性，也不保证代码的稳定性和功能性。

在任何情况下，因使用或无法使用本项目的代码或数据所产生的任何损害或其他责任，开发者和任何贡献者都不承担任何责任。

使用本项目的代码或数据即表示您已经了解并接受这些条款。

## 许可证

[MIT](./LICENSE) License &copy; 2024-PRESENT [Govin](https://github.com/guovin)
