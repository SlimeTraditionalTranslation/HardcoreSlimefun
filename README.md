# :skull_and_crossbones:硬核版 - 黏液科技

這個附加的目的就是盡可能讓黏液科技更加的困難.<br>
我甚至不知道你為甚麼要安裝這個, 請對你的玩家好一點.


還在這裡? 那好吧, 讓我向你展示如何讓你的伺服器變成真正的硬核.
* [如何設置這個插件](#wrench-setting-up-your-hardcore-server)

> 此為**非官方**版本, 請勿在該作者問題追蹤內回報! <br>
> [原作連結](https://github.com/Slimefun-Addon-Community/HardcoreSlimefun) | [非官方Discord](https://discord.gg/GF4CwjFXT9)

| 非官方繁體中文版 | 官方英文版 |
| -------- | -------- |
| 點下方圖片下載 | 點下方圖片下載 |
| [![Build Status](https://xMikux.github.io/builds/SlimeTraditionalTranslation/HardcoreSlimefun/main/badge.svg)](https://xMikux.github.io/builds/SlimeTraditionalTranslation/HardcoreSlimefun/main) | [![Build Status](https://thebusybiscuit.github.io/builds/Slimefun-Addon-Community/HardcoreSlimefun/main/badge.svg)](https://thebusybiscuit.github.io/builds/Slimefun-Addon-Community/HardcoreSlimefun/main) |

## :headphones: Discord 伺服器
你可以在 Discord 上找到 Slimefun 的社群, 並與來自社區中的數千名成員聯繫.<br>
Slimefun Addon Community (附加社群) 也有自己的 Discord 伺服器! 供我們任何專案使用.

<p align="center">
  <a href="https://discord.gg/slimefun">
    <img src="https://discordapp.com/api/guilds/565557184348422174/widget.png?style=banner2" alt="Discord Invite"/>
  </a>
  <a href="https://discord.gg/SqD3gg5SAU">
    <img src="https://discordapp.com/api/guilds/809178621424041997/widget.png?style=banner2" alt="Discord Invite"/>
  </a>
</p>

# :wrench: 設置你的硬核伺服器
當你安裝好此附加之後, 你將需要對其進行配置<br>
導航至 `/plugins/HardcoreSlimefun/config.yml`, 在這裡:

```yaml
# If the plugin should auto-update
auto-update: true
on-death:
  # 如果設定為 true, 玩家將會在死亡後隨機遺失一項研究
  reset-random-research: true
  # 在死亡時有機率會重置所有研究. 百分比率 0 至 100.
  # 100 將會始終遺失, 0 將永遠不會遺失
  chance-to-reset-all-researches: 5

on-research:
  # 研究失敗的機率. 百分比率 0 至 100.
  # 100 將始終失敗, 0 將永遠不失敗.
  chance-of-failure: 10

android:
  # 機器人出現故障的機率. 百分比率 0 至 100.
  # 100 將始終故障, 0 將永遠不故障.
  chance-to-malfunction: 10
  # 故障持續時間 (以秒為單位)
  malfunction-duration: 30

messages:
  lost-random-research: '&c你遺忘了隨機的研究!'
  lost-all-research: '&c喔不... 你遺忘了所有的研究!'
  research-failed: '&c研究失敗! 你需要再研究一次 :^)'
  android-malfunctioned: '&c你的機器人出現故障! 讓它冷卻並重新啟動'
```
