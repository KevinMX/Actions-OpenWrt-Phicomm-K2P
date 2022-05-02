# Archived.

> padavan 是 ramips 最后的归宿。
> ——天灵@https://github.com/immortalwrt/immortalwrt/discussions/528

建议使用 [hanwckf/padavan-4.4](https://github.com/hanwckf/padavan-4.4), [MeIsReallyBa/padavan-4.4](https://github.com/MeIsReallyBa/padavan-4.4), [padavanonly/padavan-4.4](https://github.com/padavanonly/padavan-4.4) (在MeIsReallyBa的基础上有小改), 或者 [hiboy的DRV_V5/3.4版](https://opt.cn2qq.com/padavan/K2P_DRV_V5_3.4.3.9-099.trx). Padavan在稳定性、性能、HWNAT（无线&有线）、SFE、WiFi上都有优势，甚至你还可以在4.4内核的Padavan上用SQM QoS（会自动关闭HWNAT，对于500M以下宽带问题不大）。

并不推荐在 K2P 上运行 Project V/X 之类的网络代理工具，放过MT7621和可怜的128MiB内存吧。

> padavan is the final destination for ramips.
> --Tianling Shen@https://github.com/immortalwrt/immortalwrt/discussions/528

Please consider using [hanwckf/padavan-4.4](https://github.com/hanwckf/padavan-4.4), [MeIsReallyBa/padavan-4.4](https://github.com/MeIsReallyBa/padavan-4.4), [padavanonly/padavan-4.4](https://github.com/padavanonly/padavan-4.4) (with minor changes to MeIsReallyBa repo), or the hiboy DRV_V5 version from [here](https://opt.cn2qq.com/padavan/K2P_DRV_V5_3.4.3.9-099.trx), which are all stable, with great performance, MTK HWNAT for both ethernet and wireless, SFE support, and last but not least, better WiFi. You can even use SQM QoS on padavan 4.4 branch (HWNAT will be disabled automatically, for <500Mbps bandwidth it should be fine).

Running network proxies such as Project V/X is not recommend, due to K2P's MT7621 chipset and 128MiB RAM.

# Actions-OpenWrt

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Forks&logo=github)

Build OpenWrt using GitHub Actions

[Read the details in my blog (in Chinese) | 中文教程](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

## Usage

- Click the [Use this template](https://github.com/P3TERX/Actions-OpenWrt/generate) button to create a new repository.
- Generate `.config` files using [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) source code. ( You can change it through environment variables in the workflow file. )
- Push `.config` file to the GitHub repository.
- Select `Build OpenWrt` on the Actions page.
- Click the `Run workflow` button.
- When the build is complete, click the `Artifacts` button in the upper right corner of the Actions page to download the binaries.

## Tips

- It may take a long time to create a `.config` file and build the OpenWrt firmware. Thus, before create repository to build your own firmware, you may check out if others have already built it which meet your needs by simply [search `Actions-Openwrt` in GitHub](https://github.com/search?q=Actions-openwrt).
- Add some meta info of your built firmware (such as firmware architecture and installed packages) to your repository introduction, this will save others' time.

## Acknowledgments

- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [ActionsRML/delete-workflow-runs](https://github.com/ActionsRML/delete-workflow-runs)
- [dev-drprasad/delete-older-releases](https://github.com/dev-drprasad/delete-older-releases)
- [peter-evans/repository-dispatch](https://github.com/peter-evans/repository-dispatch)

## License

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/main/LICENSE) © P3TERX
