---
author: Sabertazimi
authorTitle: Web Developer
authorURL: https://github.com/sabertazimi
authorImageURL: https://github.com/sabertazimi.png
tags: [CS, Math]
---

# Math Basic Notes

## 牌效策略

基于 **向听数** 与 **进张数**, 适当考虑 **打点**:

- 摸入后可以减少向听数的牌称为**进张**.
- 摸入后可以增加进张数的牌称为**改良**.
- **进张**与**改良**合称为**有效牌**.

### 单张牌效

#### 单张切牌顺序

- 客风牌:
  - 一般情况, 按`东南西北`顺序切客风牌.
  - 考虑场况, 优先切`直接竞争家`客风牌.
- `14`/`69` 中的 `1` 与 `9`:
  - 客风牌 -> `1`/`9`: 不暴露 `4`/`6`.
  - `1`/`9` -> 客风牌: 保留客风安全牌.
  - 无固定雀头时, `14`/`69` 强于客风牌.
  - 有固定雀头时, `14`/`69` 弱于客风牌.
- `1` `9`.
- 役牌: 场风牌 -> 三元牌 -> 自风牌 -> 双风牌.
- `2` `8`.
- `3` `4` `5` `6` `7`.

#### 单张切牌技巧

- 相同进张: 搭子直接模切, 面子**空切**:
  - Slide: 使对手误以为面子靠张危险. 同时存在**改良打点**可能 (宝牌靠张/断幺九/三色同顺).
  - Reset: 重置对手安全牌判断.
- 尽早切掉连筋孤张:
  - 有效牌重复效应.
  - 中晚巡易放铳.
- 靠近顺子的浮牌价值上升, 靠近搭子的浮牌价值下降.
- 搭子**足够** + 打点**足够** (不需要宝牌/三色靠张) 时,
  优先切**高危险度**孤张 (宝牌/中张靠张/生张字牌):
  - 优先切**场风/三元牌**， 保留**客风牌**, 防止他人鸣役牌, 保留安全牌与平和可能.
  - 优先切中张靠张, 保留高威胁对手现物, 增强手牌防守力.

### 对子牌效

#### 对子基本牌效

- **早巡**不应固定雀头, 应该把雀头拆开和其他牌组成搭子, **中晚巡**自然进张形成雀头或切牌固定雀头.
- 愚型复合型包含**唯一雀头**时, 可以考虑固定雀头 (e.g `112`).
- 役牌为**唯一雀头**时, 若牌型较好(一向听), 且立直门清打点显著高于役牌打点, 则不急于鸣役牌.
- 客风对子:
  - 攻可作雀头听平和, 守可作安牌防一发.
  - 若对子或搭子超载, 可以优先切掉客风对子作断幺九手役.
- 非现物中张对子进张十分困难, 高概率**牌山 0 枚残** (对手手牌有一组对子).
- 绝张对子: 没有双碰进张只能作雀头, 搭子超载时可以优先切掉绝张对子.
- 对子超载二择:
  - 偏向门清的手牌, 保留中张对子, 最大化改良可能.
  - 偏向副露的手牌, 保留幺九对子, 最大化副露可能.
  - e.g 门清断幺九手牌 `44` 优于 `22`, `44` 存在 `34` / `45` 两种改良.
  - e.g 副露断幺九手牌 `22` 优于 `44`, `22` 更容易鸣牌.

#### 两对子牌效

- 两对子存在双碰进张, 是快速听牌的诀窍.
- 存在愚型与两对子时, 优先保留两对子改良好型可能.

#### 三对子牌效

- 三对子相比于两对子, 仅增加 2 张刻子进张.
- 有役时 (役牌, 断幺九, 对对和):
  - 考虑保留三组对子, 可将**碰**作为进张手段, 三对子可作为**快速听牌**手段.
- 两向听时:
  - **一向听顶峰理论**: 最大化**一向听进张**数, 在两向听时可考虑保留三组对子, 切掉较弱三牌复合型.
- 门清时 (立直或平和):
  - 考虑切掉一组对子 (同时保证不退向): 切两面对 -> 切坎张对 -> 切边张对.
  - 考虑**向内靠拢**, 切幺九对.

#### 四对子牌效

四对子: 进张较差时, 可考虑七对子手役.

### 搭子牌效

#### 搭子基本牌效

- 搭子强度: 两面 > 两坎 > 坎张 > 边张.
- 副露手牌, 双碰进张优于两坎进张, **碰**的几率远大于**吃**.
- **高向听**时, 禁止切掉唯一一组雀头 (切掉后会导致退向).
- **奇数**枚有利: 3/5/7 张同色牌比偶数枚更优.
- 四连型, 中膨型, 亚两面型混合时, **切掉亚两面型**, 高概率是正解.
- 多种复合型混合成复杂形状时, **保留复杂形状, 切牌固定两面搭子或完整面子**, 高概率是正解.
- 早巡重视改良数与速度, 中巡重视进张数与安全度.
- 中巡好型搭子足够时, 可考虑**保留安全牌**进行防守, 亦可用安全牌进行追立:
  完全一向听时, 上张熟张字牌, 可以考虑切掉两面对中的对子补强牌 (仅损失 2 枚非平和进张),
  保留熟张字牌 (**安全牌**), 切掉**危险两面对** (牌河较少同色牌) 中的对子补强牌,
  攻可切字牌安全立直, 守可作安牌防止一发.

**有效牌重复**效应:

- 筋牌: `147`, `258`, `369` 同一筋上存在有效牌重复效应.
- 边张: `14` / `69` 存在时, `1` `9` 价值甚至低于客风牌.
- 存在二度进张的边张搭子, 切掉边张搭子保留浮牌比较有利.
- `14` 进 `2`/`3`, 形成 `124`/`134`, 仍然切 `1`, 所以可以在 `14` 时就切 `1`.

#### 五搭子理论

**五搭子理论** - 五搭子饱和, 六搭子不利:

- 五搭子型基本上只要切掉价值最低的浮牌.
- 打点足够时重视好型搭子, 保留浮牌寻求**好型改良**, 最大化进张数.
- 打点不足时重视手役搭子, 保留浮牌寻求**打点改良**, 提升手牌打点.
- 六搭子 (6 Block):
  保留用于形状改良 (存在愚型搭子) 与打点改良 (断平三色可能)
  的孤张浮牌或超载搭子,
  防止手牌形成低打点愚型听牌.
- **低效率二度进张**:
  考虑有效牌重复效应, 可以切掉同色超载搭子 (进张数损失最小).
  如 `1245` 二度进张 `3`, `3467` 二度进张 `5`.

搭子超载时, 优先切掉弱搭子:

- **搭子评价标准**:
  - 进张枚数.
  - 形状改良枚数.
  - 打点改良枚数.
  - 和牌难易度.
  - 和牌残枚数.
- 强搭子:
  **复合型**,
  两面搭,
  两坎搭,
  **宝牌搭**,
  役牌搭,
  **三色搭**,
  染手搭.
- 弱搭子:
  坎张搭 (中张坎 > 尖张坎 > 边张坎, e.g `35` > `13` > `24`),
  边张搭,
  损失手役牌 (幺九牌),
  **绝张搭** (e.g 损失四枚 `2` 的 `34` 两面搭, 损失两枚的双碰进张).
- 全好型时, 优先**切掉中张浮张** (降低手牌危险度), 然后切掉超载搭子.
- 存在愚型时, 优先切掉最弱搭子, **保留中张浮张**, 后续形成好型搭子后, 继续切掉最弱搭子, 直至剩下至多五组搭子.
- 存在愚型与**两对子**时, 可以切掉愚型搭子, 保留中张对子形成好型搭子后, 另一组对子可作雀头.
- 存在复合型时, 可以先切边张: 价值低.
- 不存在复合型时, 可以先切中张: 危险度高.

**超载对子**二择:

- 两对子二择: 切中张对子退回浮牌, 保留中张浮牌周边改良.
- 三对子二择: 切幺九对子退回浮牌, 保留中张对子周边改良, 保留幺九安全牌.

### 三牌复合型

- 两面对: `233`.
- 坎张对: `244`.
- 边张对: `122`.
- 两坎型: `246`.
  - 两面两坎型: `2` + `456` + `67` -> `246` + `567`.
  - 长两坎型: `134568`, 进 `2` 或 `7` 都可形成两面子.
  - 弱于两面搭子: 需要 3 张牌, 听牌型为坎张听.
- 坎张对利于副露鸣牌, 两坎型利于门清平和.

搭子进张成为搭子 + 对子复合型, 称该进张为**补强牌**:

- 两对子双碰:
  当出现两组复合型二择时,
  切掉**搭子部位较弱**的复合型的**搭子**,
  固定两对子双碰牌型.
- 三对子不利:
  当出现三对子不利时,
  切掉**搭子部位较强**的复合型的**对子** (e.g 两面对),
  **让补强牌辅助较弱的搭子**,
  固定强搭子牌型 (两面对 - 对子补强牌 = 两面搭),
  即**固定好型**.

`13345667m` + `123788s`:

先根据五块理论与中膨复合型, 将手牌分为 `133m` + `456m` + `67m` + `123s` + `788s`.
可以此时已经形成了有效的五块搭子, 需要切掉两个三牌复合型中的一个, 保持张数的正收益.
对于`对子` + `搭子`的复合型, 可以采取固定好型的策略, 切掉 `8s`, 固定 `78s` 两面型.
显然切掉 `3m` 去固定 `13m` 坎张是低效率的切法.

### 四牌复合型

#### 四连型

又称延伸单骑, 具有良好**延展性**:

- 好型: `3456` -> `34` + `56`, 常常将其视为**两面 + 两面**, 而不是单骑进张.
- 次好型: `1234` -> `123` + `4`, 常常将其视为单骑进张, 而不是**边张 + 两面**.
- `3456` 与 `4567` 8 种 28 枚进张, 进张数最多的四牌复合型.
- 缺少搭子或**存在愚型**时, 四连型具有良好**延展性**, 容易形成新的**两面搭**, `4567` -> `34567` / `45667`.
- 缺少对子时, 四连型具有良好**延展性**, 容易形成新的**雀头**, `4567` -> `44 567`.

#### 中膨型

- 进张: 五种进张, `3445` 存在 `23456` 进张.
- 好型: `3445` -> `34` + `45`, 两面 + 一杯口, **好型进张 + 一杯口进张**.
- 缺少搭子或**存在愚型**时, 中膨具有良好**延展性**, 容易形成新的**两面搭**, `4556` -> `34556` / `45566`.
- **恶型**: `1223` -> `123` + `2`, 价值较低, 接近于单张 `2`, 不存在连续型时, 可优先切掉 `2`.

#### 亚两面型

- `3345` -> `34` + `35` / `33` + `45` / `3` + `345`.
- 缺少对子时, `3345` 有一定价值, 稍稍高于单张 `3`.
- 不缺对子时, `3345` 价值较低, 接近于单张 `3`, 可优先切掉 `3`, 保留其他复合型.
- **恶型**: `1123` 价值接近于单张 `1`, `7899` 价值接近于单张 `9`.
- 总体来说, 亚两面型作两面能力**与孤张无太大区别**.
- `3345` -> `34` + `35`, 可以通过鸣牌改良成 `34` 两面.
- 亚两面型可以直接用于听牌, 存在转二杯口可能性, 可以形成 `33345` 暗刻复合型.

| 复合型          | 靠张 | 两面 | 坎张 | 双碰 (雀头) |
| --------------- | ---- | ---- | ---- | ----------- |
| 四连型 `3456`   | 1~8  | 2457 | 18   | 36          |
| 中膨型 `3445`   | 2~6  | 2356 |      | 4           |
| 亚两面型 `3345` | 1~6  | 24   | 15   | 36          |

| 复合型   | 进张数 | 好型率 | 雀头固定型 | 雀头流动型 |
| -------- | ------ | ------ | ---------- | ---------- |
| 四连型   | S      | A      | A          | S          |
| 中膨型   | B      | S      | S          | B          |
| 亚两面型 | A      | B      | B          | A          |

#### 跳一型

- `3567` -> `35` + `67`.
- `1235`/`5789` 接近于孤张 `5`.
- `1345`/`5679` 中的 `1`/`9` 比孤张 `1`/`2`/`8`/`9` **强**.
- `5679`: `9` **不再**受制于重复牌效应, 进 `8` 可以形成五连型好型, 形成 `56` 两面搭.
- `3457` 可以形成好型 `34567`, 利用**吃**可以形成两面子.
- 靠张一向听时, **暗刻跳一型**牌效差 (e.g `1113s` 切 `3s`, 保留其他两张浮牌).
- 各种形状的跳一型 (三连跳一型, 两面对跳一型, 四连跳一型, 中膨跳一型, 亚两面跳一型, 暗刻跳一型, 五连跳一型)
  在搭子不足时可以形成新的好型搭子, 当搭子足够时牌效较差, 切掉跳一**浮张**进张损失较小.

#### 暗刻复合型

- `3334` -> `33` + `34`, 容易形成`面子` + `雀头`:
  - 无其他雀头时靠张价值较高, 可作雀头, 存在**三面进张**.
  - 有其他雀头时靠张价值较低, 可固定暗刻, 天然损失三枚.
  - 可以形成平和型, 提升手牌打点.
- **一向听**同时存在**两种四牌复合型**时, **复合型切牌顺序**:
  - 跳一型: 牌效最差.
  - 亚两面型.
  - 中膨型.
  - 四连型: 保留三面听牌可能.
  - 暗刻复合型: 保留平和可能, 保留三面听牌可能.

#### 二度进张复合型

- `3556` -> `35` + `56`: 存在二度进张 `4`, 当搭子超载时, 优先切掉 `3`.
- `3467`: 坎张二度进张.
- `3344`: 完全二度进张, 只有存在其他复合型 (一杯口) 或双碰听时有价值.
- **恶型**`6889`: 边张二度进张, `69` 连筋恶型, 当搭子超载时, 优先切掉 `9`.

#### 四牌复合型强度

- 四牌复合型**强度**: 四连型 > 中膨型 >> 亚两面型 > 跳一型 > 二度进张恶型.

`1234p` 与 `1123s`:

当手牌缺少对子时, 四连型中的 `1p` 可以解放 `4p`, 进张下一个 `4p` 时, 可以形成面子 + 雀头,
即 `1p` + `234p` -> `123p` + `4p`, 使得 `1p` 价值约等于 `4p`.

亚两面型中的 `1s` + `123s` 无法解放 `3s`, 使得 `1s` 价值约等于 `1s`.
比较 `4p` 与 `1s` 价值, 可以得出此时应该切 `1s`, 保留 `1p`.

### 多牌复合型

- 五连型: 进张超好型, 且容易形成雀头.
- 五连复合型: `234556`, 进张 `1457`.
- 暗刻复合型:
  - 暗刻可作面子, 可作对子, 扩大进张面.
  - `333` + `45` -> `33` + `345`, 容易形成`面子` + `雀头`, 缺少对子时, 价值上升.
  - `344457`: 两坎暗刻型, 进张 `46`.
  - `355567`: 坎张对暗刻型, 进张 `458`.
  - `344456`/`345556`: 两面对暗刻型, 进张 `2457`.
  - `334445`/`344455`: 中膨暗刻型, 进张 `2345`/`3456`.
  - `334555`/`333455`: 中凹暗刻型, 进张 `2345`/`3456`.
  - `344555`/`333445`: 阶梯暗刻型, 进张 `23456`.
  - `2345666`: 进张 `25`/`147`.
- 暗刻跳一型: `333` + `5`, **暗刻**旁边的**浮牌不适合靠张一向听**.
- 两顺子型:
  - `344556` -> `345` + `456`.
  - `2344556` 切 `2` 形成 `344556`, 存在一杯口改良可能.
  - 门清时, 向一杯口方向 (内卷) 前进.
  - 副露时, 向五连型方向 (外扩) 前进.
- 连续两面对型: `566788`
  - `5` + `66788`: 切 `5` 固定一杯口.
  - `56` + `6788`: 切 `8` 固定两面.
  - `5667` + `88`: 切 `6` 固定雀头.
- 两面一杯口型: `34455` -> `345` + `45`.
- 坎张一杯口型: `33455` -> `345` + `35`
  - 存在靠张时: `133455` 进张 `2` -> `123` + `345` + `5` / `123` + `34` + `55`.
  - 存在靠张时, 形成隐藏的两坎型后, 可转化成**两面两坎型**.
- 两面中坎型: `23578` 切 `5` (有效牌重复).
- 两坎预备型:
  - `24579`: 进张 `3` -> `234579`, `68` 两坎进张.
  - `24679`: 进张 `5` -> `245679`, `38` 两坎进张.
  - `24679`: 进张 `8` -> `246789`, `35` 两坎进张.
- 相离两坎型: `245679` 进张 `3` / `8`.
- **两面两坎**预备型:
  - `2356778` 切 `2`.
  - `3356778` 切 `3`.
  - `3556778` 切 `5`.
- **两面两坎型**: `455679` -> `456` + `579`, 进张 `368`.
  - 当追求进张数时, 保留 `455679` 形成 `456` + `579`.
  - 当**缺少雀头**或追求**好型率**时, `455679` 切 `9` 形成 `45` + `567`, 损失进张 `8`.
- 宝牌连续型: `11234` (`4` 为宝牌), 用筋牌 `1` 作雀头, 摸入 `4` 时可切 `1` 极具迷惑性.
- 跳对子型: `335577`, **跳对子型切中间对子**, 一般选择切 `5`, 固定中间**两坎好型**, 保留**边张雀头**可能,
  `33577` 进张能力很强, 是一组强力复合型.
- 双雀头天平型:
  - `23345667`: `33`/`66` 作雀头, 进张 `14`/`58`, 两面 + 两面.
  - `13345667`: `33`/`66` 作雀头, 进张 `2`/`58`, 坎张 + 两面.
  - `12234556`: `22`/`55` 作雀头, 进张 `3`/`47`, 边张 + 两面.
  - `22334556`: `22`/`33`/`55` 作雀头, 进张 `14`/`2`/`3`/`47`, 两面 + 双碰 + 两面.
  - `22334557`:`22`/`55` 作雀头, 进张 `14`/`6`, 两面 + 坎张.
- **好型** 八枚翼对称型 (两组中膨型): `34456778` -> 顺子 + 两坎型 + 对子, 保留此复合型.
- **好型** 九枚翼对称型 (两组中膨型 + 中张): `233456778`, 两组顺子 + 两坎型, 进张 `1469`, 保留此复合型.

## 向听策略

### 两向听策略

- `面子` + `雀头` + 3 `搭子` + 孤张 (**五搭子**):
  - 全好型时, 优先切掉最弱孤张.
  - 存在愚型时, 可以切掉最弱搭子, 保留孤张改良可能.
- `面子` + 3 `对子`搭 + 孤张 (**四搭子**):
  - 愚型较少时, 可以切掉两面对补强牌, 固定两面好型, 保留孤张改良可能.
  - 愚型过多时, 重视七对子/对对和进张.
- `面子` + `雀头` + 4 `搭子` (**六搭子**):
  - 全好型时, 可以切掉两面对补强牌, 固定两面好型, 保留六搭子型.
  - 存在愚型时, 优先切掉最弱搭子.
- 2 `面子` + **无雀头**两向听:
  - 全好型时, 重视雀头进张, 重视易形成雀头的复合型 (如四连型与亚两面型).
  - 存在愚型时, 重视改良进张, 保留孤张改良可能,
- 一向听顶峰理论:
  全好型低向听时, 可考虑切掉多余四牌复合型 (固定面子),
  保留三牌复合型, 最大化一向听到听牌的进张数.
- 存在愚型搭子时 (容易形成愚型听牌), 可以考虑暂时保留四牌复合型 (不急于固定面子), 寻求**好型搭子改良**.
- 多牌复合型的价值在缺少搭子的情况下价值较高 (进张面广, 进张数多), 在不缺搭子的情况下只能用于改良牌型与打点.

### 一向听策略

- 一向听类别: 愚型一向听, 完全一向听, 靠张一向听, 无头一向听.
- 全牌效策略.
- 听牌型重视策略 (愚型轻视策略).
- 和牌率重视策略 (愚型轻视策略).
- 速度重视策略:
  - 役牌双碰副露: 可以保留 3 组对子 (役牌 + 幺九 + 中张对子).
  - 断幺副露.
- 符数重视策略: 重视幺九刻子.
- 打点重视策略.
- 宝牌进张重视策略:
  - 重视宝牌靠张延展性.
  - 重视宝牌复合型延展性
  - 重视宝牌搭子转换宝牌对子可能性 (**不固定非宝牌雀头**).
- 赤宝牌进张重视策略:
  - 重视内侧 Slide.
  - 重视 `34` 与 `67` 搭子.
  - 赤宝牌进张优先于不确定三色进张.
- 平和重视策略 (好型重视策略).
  - 四牌复合型延展性.
  - 面子 + 搭子 (对子/两面/坎张/跳一) 五牌复合型延展性.
- 断幺重视策略:
  - 重视内侧 Slide.
- 三色重视策略.

#### 早巡一向听策略

早巡时可以考虑**高打点**进行退向:

- 宝牌靠张.
- 断幺九/平和: 切**边张**搭子/对子, 追求断幺九或平和好型.
- 染手: 切同色搭子 (甚至面子).
- 三色同顺.
- 多愚型高向听手牌, 早巡退向寻求形状与打点改良, 保留立直 Nomi 变成立断平三色的可能.
- 早巡低打点愚型一向听应退回两向听寻求形状与打点改良:
  - 保留四连型与中膨型, 切掉愚型搭子, 退回两向听, 寻求形状改良.
  - 保留手役靠张, 切掉愚型搭子, 退回两向听, 寻求打点改良.
- 存在复合型的低向听手牌, 早巡退向可以带来至少 2 番打点改良时, 应选择退向甚至拒听:
  e.g 立直 Nomi 边坎听牌 -> 立断平好型听牌.
- 中晚巡进行改良时 (无法改变打点) **禁止退向**.

#### 两面一向听策略

- 2 `面子` + `两面对` + 2 `两面`.
- 一组两面搭子进张补强牌形成两面对后, 可以将一组两面对固定为雀头, 转为完全一向听.
- 含有唯一雀头的两面对进张形成面子后, 转为全好型无雀头一向听.

#### 完全一向听策略

- 2 `面子` + `雀头` + `两面对` + `两面`.
- 6 种 20 枚进张 (4 种 16 枚两面进张 + 2 种 4 枚双碰进张).
- 不要双碰进张, **保留安全牌或改良牌**, 切掉两面对补强牌:
  - 双碰进张枚数数不理想 (只有 1~2 枚).
  - 双碰进张严重影响手牌打点: e.g 双碰进张是宝牌靠张时, 平和 + 宝牌 -> Nomi.
  - 场况危险, 对手速度较快, 需要安全牌防止一发.

#### 无头一向听策略

三面子一向听:

- 无头暗刻一向听:
  - **不固定雀头**进张数更多 (拆开雀头形成面子与搭子).
  - 非单骑听牌确定, 其中一组搭子进张听牌时可以切掉暗刻作雀头.
- 无头非暗刻一向听:
  - 当两组搭子均为两面搭子时,
    进张数多于完全一向听 (28 > 20), 好型率均为 100%,
    应选择无头一向听 (不考虑打点).
  - 当一组搭子为愚型搭子时,
    进张数多于完全一向听 (24 > 20), 好型率仅为 42%,
    应选择完全一向听.
  - 当重视其中一个搭子进张时, 可以切掉另一组搭子:
    e.g `34s` + `24m` (`2s` 为宝牌) 无头一向听,
    `34s` **好型**搭子进张均为**宝牌**,
    可以切 `2m` 固定 `34s` 搭子.
  - 存在**单骑听牌**可能, 损失平和打点, 和牌率低, 可以考虑默听改良或拒听.
- 无头愚型一向听: 考虑形状和打点改良可以切掉愚型搭子, 考虑听牌速度可以保留无头愚型一向听.
- 两组搭子与面子形成复合型后, 进张数进一步增加.
- 3 `面子` + 1 `搭子` 一向听, 优先考虑改良和听牌型.

#### 靠张一向听策略

**撞头一向听**:

- 3 `面子` + `雀头` + 2 `单张`: e.g `1223455568p7s555m` 切 `2p` 成为撞头一向听 (`8p` `7s` 靠张).
- 靠张一向听进张数一般为 30+~40+ 枚:
  - 优先考虑听牌形状和手牌打点, 选择**好型听牌**/**高打点**浮牌靠张.
  - 两张浮牌与面子/雀头形成复合型后, 进张数进一步增加.
- 进张数大于完全一向听, 可能形成**愚型听牌**, 优先考虑**听牌好型率**进行切牌.
- 中张四连型 (进张) > 中张中膨型 (好型) > 中张亚两面型 >
  `37` > `46` > `5` >
  边张四连型 > 边张中膨型 > 边张亚两面型 >
  `28` > `19`.

#### 改良一向听策略

- 进张数差别不大时, 优先考虑形状与打点改良:
  - 最终听牌**面数**.
  - 最终听牌**打点**.
  - 切掉愚型可以最大化**平和**可能.
  - e.g `56m123p67p2345666s` 切 `6m`/`2s` 进张数均为 28 枚, 应切 `6m` 最大化平和可能.
- 早巡/不含复合型/需要打点时, 固定雀头形成两面两面一向听, 提升手牌打点.
- 中晚巡/包含复合型时, 固定面子形成无雀头一向听, 最大化进张数.
- 早巡寻求改良时, `坎张对+两面+中张雀头`略优于`两坎+两面+中张雀头` (**两雀头有利**),
  雀头部分进张形成两面对时, 可以改良成完全一向听, 同时保留双碰进张与副露可能.

下一巡听牌概率 = `听牌枚数 * 5/6`:

- 完全一向听下一巡听牌概率为 10 %.
- 无头/靠张一向听下一巡听牌概率为 20 %.
- 存在四/五牌复合型时下一巡听牌概率可提升至 30~50 %.

### 听牌策略

#### 基本听牌形式

- 两面听.
- 双碰听: 听牌枚数小于 2 (e.g 一组对子 0 枚残) 时, 双碰听和牌率较低.
- 坎张听: 中张坎张听和率较低.
- 边张听.
- 单骑听:
  - 存在换听两面可能, 不急于立直.
  - 早巡听多枚数单骑, 晚巡可以考虑听 1 枚地狱单骑.
  - 存在暗刻时, 单骑向复合型靠近, 保留换听两面可能:
    e.g 单骑听中膨型中间牌, 进张后暗刻改雀头换听两面.
  - 不存在暗刻时, 可以直接选择听字牌, 也可以默听保留亚两面听牌或两面单骑听牌可能.
- 听牌数: 两面听 > 双碰听 > 坎张听 > 边张听 > 单骑听.
  - 两面听优势明显, 听牌数为 8.
  - 单骑听变化多, 难以防守, 特别是听熟张字牌容易荣和.

#### 复合听牌形式

- 四连型与亚两面型听牌数都为 6.
- 暗刻复合型:
  - `1222`: 边张单骑, `1` + `222` / `12` + `22`, 听牌数为 7.
  - `3555`: 坎张单骑, `3` + `555` / `35` + `55`, 听牌数为 7.
  - `3444`: 两面单骑, `3` + `444` / `34` + `44`, 听牌数为 11.
- 三面听:
  - 听三种牌.
  - 基本三面听: `34567` -> `34` + `567` / `345` + `67`, 听牌数为 11.
  - 单骑三面听: `1234567`, `2234567`, `4566789`, 听牌数为 9.
  - 混合三面听: `23445566`, 可以形成一杯口.
  - 多面听时, 三暗刻也可看作`雀头`+`单张`.
- 不规则多面听:
  - 基本策略:
    - 顺子延伸性: 两面/三面单骑听牌, 五连三面听牌.
    - 暗刻复合性: 暗刻型既可作`面子`, 又可作`对子+单张`, 形成多面听牌.
  - 一杯口单骑型: `2233344` 听 `234`, 双碰 + 单骑.
  - 一杯口双碰型: `33445566m99p` 听 `369`, 双碰.
  - 暗刻双碰型: `44456m99p` 听 `479`, 两面 + 双碰.
  - 暗刻亚两面型: `1112234` 听 `235`, 两面 + 边张.
  - 暗刻中膨型: `5667888` 听 `467`, 两面 + 单骑.
  - 暗刻四连型: `2224567` 听 `347`, 坎张 + 单骑.
  - 暗刻跳一型: `4445679` 听 `89`, 坎张 + 单骑.
  - 暗刻单骑型: `3335777` 听 `456`, 坎张 + 单骑.

#### 听牌技巧

- 满贯以下听高点, 满贯以上听张数.
- 和牌率: 熟张字牌 > 幺九牌 > (外) 壁引挂 > (边) 筋引挂.
- 骗筋: 听牌河 (现物/立直宣言牌) 筋牌.
- 偷现: 听`立直家`/`副露家`/`亲家`现物.
- 当听牌枚数过少 (e.g 2 枚) 或听牌场况过差 (e.g 愚型听牌且牌河同色牌过少) 时, 可以选择**拒听**寻求改良:
  - 无头一向听 (3 面子 + 2 搭子) 进张形成中张雀头 (`344`), 听牌型为边张听时 (`12`),
    可以选择切掉雀头 (`4`) 拒听, 寻求改良 `12` 边张搭子.

## 鸣牌策略

- 鸣牌是赤牌麻将中非常重要的技术.
- 鸣牌要点: 鸣牌形状 (役牌/愚型), 手牌形状, 手牌打点.
- 鸣牌优点: **速度上升**.
- 鸣牌的缺点: **打点下降**, **防御力下降**.
- 可副露时三牌/四牌复合型价值上升: 鸣牌加速和牌, 食延消解愚型.

### 鸣牌选择

- **两张以上宝牌**时候要重视速度与和牌的容易度,
  把鸣牌作为做牌的前提.
- 远而大副露: 高打点形状极差手牌, 积极寻找手役, 副露鸣牌加速和牌.
- 小牌速攻副露: 阻止对手高打点和牌, 亲家保持连庄, 子家快速过庄.
- 对子较多 (3~4 对) 且形状不佳时, 门清作牌难度较大,
  可以考虑断幺九/染手副露加速和牌.
- 可以考虑鸣牌:
  - 满贯手牌: e.g 多宝牌/染手.
  - 消除愚型 (坎张吃, 边张吃, 绝张吃/碰): 愚型过多, **门清立直速度过慢**.
    - e.g `46` 吃 `5`, 消除愚型搭子.
    - e.g `7789` 吃 `8`, 留下 `78` 两面好型搭子, 切掉另一组愚型搭子.
    - e.g `4678` 吃 `5`, 留下 `78` 两面好型搭子, 切掉另一组愚型搭子.
  - 断幺九副露基准: **3900** 点, 序盘从**愚型**开始鸣牌.
  - 两副露基准: **5200** 点, 好型一向/两向听 (防止过度鸣牌).
  - 三副露基准: **7700** 点, 好型听牌/一向听 (防止过度鸣牌).
  - 晚巡低向听 (急于听牌).
  - 破除一发.
  - 速攻阻止对手和牌.
- 不建议鸣牌:
  - 远而小副露: 牌型差, 打点低, 鸣牌加速收益较低, 不鸣牌可保持高打点和防御力.
  - 损打点副露:
    - **早巡**牌型好, 打点低: 全好型手牌可以作门清手役, 提升打点.
    - 鸣牌降低一半以上打点.
  - 无意义副露: 向听数不变, 没有形状或打点改良.
  - 鸣牌**过早**或副露**过多**都会导致他家提高警惕性, 使得**和牌率降低**:
    - e.g 若 `68s` 先于 `双东对子` 鸣牌, 则 `双东对子` 鸣牌难度大幅度提升.
    - e.g 若 `13s` 先于 `宝牌中对子` 鸣牌, 则 `宝牌中对子` 鸣牌难度大幅度提升.

### 吃牌策略

- 吃牌时尽量选择坎张/边张吃, 进张数最大化.
- 食延:
  - `12333`: `13` 吃 `2` 切 `3` 听 `14`.
  - `13345` `35` 吃 `4` 切 `1` 听 `25`.
  - `57789`: `79` 吃 `8` 切 `5` 听 `69`.
  - `234456`: `46` 吃 `0` 切 `2`.
- 在食替限制下, 作出能够**自由吃宝牌/赤宝牌**的听牌型.

### 碰牌策略

役牌为**唯一雀头**时, 若牌型较好(一向听), 且立直门清打点显著高于役牌打点, 则不急于鸣役牌:

- 唯一雀头鸣牌不能降低向听数.
- 胡一番役牌意义不大, 副露降低防守能力.

### 杠牌策略

- 幺九牌暗杠 32 符, 相当于 1 番.
- **加杠**/**暗杠**增加一次摸牌机会.
- 建议杠牌:
  - 低打点一向听/听牌.
  - 危险牌暗杠.
- 不建议杠牌:
  - 牌型差, 多愚型, 高向听.
  - 进张减少 (甚至退向): e.g 中张暗刻不开杠, 保留作搭子 (暗刻复合型).
  - 他人立直, 自己和牌率较低.
  - 手牌打点足够, 无需杠宝牌.

## 手役策略

### 常见手役

| Rank | Type     | Ratio (%) |
| ---- | -------- | --------- |
| A    | 立直     | 42.6      |
| A    | 役牌     | 38.7      |
| A    | 平和     | 22.5      |
| A    | 断幺九   | 21.2      |
| B    | 混一色   | 6.1       |
| B    | 一杯口   | 5.0       |
| B    | 三色同顺 | 4.3       |
| B    | 七对子   | 3.0       |
| B    | 对对和   | 2.9       |
| C    | 一气贯通 | 1.7       |
| C    | 全带幺   | 1.2       |
| C    | 三暗刻   | 0.8       |
| C    | 清一色   | 0.8       |
| F    | 其他     | < 0.5     |

- 打点 (番数) 相同时, 确定的手役比不确定的手役更有利:
  - 断幺九接近成型, 可以选择切掉役牌对子 (未成型), 保留其他中张的对子或搭子, 选择断幺九手役.
  - 断幺九并未成型, 可以选择保留役牌对子, 切掉其他超载的对子或搭子, 选择役牌手役.
- 不损失或较小损失牌效时, 应在**充分考虑高打点手役**的前提下进行切牌:
  - 宝牌: **早巡**保留宝牌及其靠张.
  - 平和手役: 一向听顶峰理论.
  - 断幺九手役: 切幺九牌向内靠拢.
  - 三色同顺手役: 切牌考虑三色可能.
  - 一气贯通手役: 保留多牌复合型.
  - 染手手役: 切牌考虑染手可能, 同色牌较多时积极鸣牌.
- 当配牌同色牌多/幺九搭子多/对子多/愚型多/牌型极散时:
  **不应按牌效直线作牌**, 应采取**防守反击**策略,
  可以考虑混一色/七对子/全带/国士无双等幺九手役,
  手牌多为幺九边张, 弃和时拥有足够安全牌.
- 领先时, 速攻 (役牌副露/断幺九副露/默听) 局消化是保持一位的有效手段.
- 低打点时, 不应盲目和亲家对攻 (放铳代价极大).
- 手役**和牌素点**: 立直一发 > 副露对对和 > 副露混一色 > 立直非一发 > 副露断幺九 > 副露役牌.
- 手役会限制牌形 (防守 ↓), **作手役追求打点**切牌高概率不是进张数最大化的切牌 (速度 ↓), 是其不可忽视的两大缺点.

### 立直手役

- 立直可视为 1.5 番.
- 立直有威吓力, 迫使对手防守, 破坏对手和牌, 增加自摸可能性.

#### 默听选择

- 默听基本准则:
  - 打点足够, 无需立直打点, 更重视和率:
    e.g 3 番 50 符, 听现物满贯, 跳满.
  - 形状太差, 立直和率过低:
    e.g 2 枚残听牌, 456 愚型 Nomi 听牌.
  - 存在好型高打点改良 (大于 2 种):
    可以在早中巡默听改良,
    在其他家手牌进展时 (副露/切宝牌/切搭子/连续切中张) 及时先制立直进行压制.
- 好型立直与默听基本准则:
  - 打点: **7700** 以上默听.
  - 巡目: **12** 巡后默听.
- 愚型立直与默听基本准则:
  - 打点: **1300** 以下拒听, **5200** 以上默听.
  - 巡目: **8** 巡后默听.
- AL + TOP + 有役, 选择默听**局消化**.
- **愚型**听牌时, 默听有**改良**与**弃和**机会:
  - 亲家**早巡愚型**听牌, 可以先制立直.
  - 子家**早巡愚型**听牌, 当改良枚数是和牌枚数两倍以上时, 可以默听寻求改良.
- **早巡** `1` ~ `2` 番牌:
  - 可以考虑拒听, 切愚型搭子提升打点:
    - e.g **早巡**手牌含复合型 + 平和可能, 切愚型搭子拒听, 退回好型一向听, 作平和手役.
    - e.g **早巡**手牌含复合型 + 断幺可能, 切幺九搭子拒听, 退回好型一向听, 作断幺手役.
  - 平和/断幺 NOMI:
    - 一般情况下可以先制立直.
    - TOP/对手打点过高时选择默听, 摸到危险张时弃和, 同时提高和率进行局消化.
  - 低打点手牌存在**两番以上**打点改良时, 可以选择默听等待改良.
- **愚型默听**和牌率 ~= **好型立直**和牌率.

#### 立直选择

- **两面**立直, **字牌双碰**立直, **NC 壁外数牌双碰**立直, 均为**好型听牌**.
- 两面立直 > 振听三面立直 > 愚型立直 = 振听两面立直.
- **早中巡好型**听牌应先制立直.
- **无役多宝牌愚型**听牌应先制立直.
- **平场**或**亲家**时, 低打点好型听牌立直 > 高打点愚型听牌立直 > 默听.
- **非平场**或**子家**时, 立直 `Nomi` 时需要考虑立直风险, 不可激进对攻.
- **早中巡**两面立直与字牌双碰立直和率相近, 选择高打点立直.
- 平和里宝率约为 `30%`, 七对子里宝率约为 `20%`.
- 四暗刻:
  - 多面听立直率大于 50%:
    - 立直可以提升打点, 立直逼迫对手防守, 延长巡目提升自摸率 (`15%` -> `20%`).
    - 中张双碰听牌可以默听, 边张幺九双碰听牌应该立直.
  - 一面听立直率小于 1%: 役满确定, 无需提升打点, 存在换听可能.

#### 门清选择

- 亲家愚型搭子过多, 且有确定手役 (役牌/断幺九) 时,
  应**积极鸣牌**, **放弃门清**, 加速和牌.

### 平和手役

- 作两面是作平和手役要点.
- **早巡**手牌打点较低, 牌型较好可作平和时,
  可以切掉役牌对子, 保留断幺平和可能.

### 一发手役

- 鸣牌破一发:
  - 手牌安全牌充足.
  - 立直家是直接竞争对手.
- 防止破一发: 容易被鸣牌不立直, 下一巡摸切立直.

### 断幺九手役

- 断幺九**可鸣牌 + 赤宝牌**可以做到速攻多番.
- 早中巡**二向听**手牌, 通常是**鸣牌断幺九** (鸣牌后切幺九牌) 的好开始点:
  - **一向听**手牌可以追求门清.
  - **高向听无宝牌**恶型手牌不急于鸣牌: 鸣牌对于高向听帮助不大, 反而降低打点与防御力.
- **多张宝牌**: 和牌速度至关重要, **鸣牌断幺九**可以加速和牌.
- **亲家**愚型搭子过多时, **愚型搭吃牌** + **断幺九**可以加速和牌.
- 断幺九容易作成, 容易与其他役复合, 摸切过程中需要**时刻考虑断幺九**可能性.
- 断幺九副露基准: **3900** 点, 序盘从**愚型**开始鸣牌.
- 切边张两面对固定边张两面搭子时 (`788` 切 `8`), 容易形成偏听断幺九 (进张 `9` 失去断幺九手役),
  可以考虑暂时保留边张两面对 (或者固定雀头) 保留完全断幺九可能.

### 役牌手役

- 三枚役牌进张数约等于两坎型.
- 好型搭子超载时, 优先切掉单张役牌.
- 愚型搭子超载时, 可以保留单张役牌, 等待役牌对子, 寻求快速和牌.
- 宝牌多 + 牌型极散, 保留单张役牌, 等待役牌对子, 寻求快速和牌.
- 切役牌对子: 牺牲速度, 提升打点. e.g 役牌 Nomi -> 立断平一杯口
- 当打点提升不大时, 保留役牌对子, 寻求快速和牌.
- 手牌有役牌对子或刻子 (特别是两番役牌对子) 时,
  可以保留其他孤张字牌, 保留混一色或对对和满贯可能.
- 后付役牌: 可以优先消除愚型鸣牌, 后付役牌鸣牌难度不大, 且可以作安全牌.
- 役牌价值低:
  - 全好型`平和`/`断幺`手牌: 门前清提升打点.
  - 多愚型役牌 Nomi 手牌: 门前清保持防御力.
- `3077s66z`: 切 `3s` 保留役牌双碰进张, **速度**优于切 `7s` 固定赤宝牌 (役牌与赤宝牌**均为一番**).
- **绞杀**策略: 弃和或配弃时, 扣住**对手字牌**, 扣住**下家关键牌**, 阻碍对手作牌, 阻止后附和牌.

### 宝牌策略

- 宝牌: **早巡**保留宝牌及其靠张.
- **多张**宝牌:
  - 重视速度: 好型足够时可考虑门清立直, 一般情况下积极鸣牌速攻.
  - 多宝牌门清手牌最大化进张, 多宝牌副露手牌寻找手役加速和牌.
- 宝牌靠张 (特别是愚型靠张) 会降低和牌速度, 降低手牌防御力, 存在提升打点可能性.
- 孤张宝牌 (宝牌靠张) 切出时机:
  - 一般情况下, 手牌基本成型时, 切出孤张宝牌 (靠张).
  - 其余牌均对手牌速度/形状/打点有更大作用时, 切出孤张宝牌 (靠张).
  - 场况危险, 保留安全牌有更大作用时, 切出孤张宝牌 (靠张).
  - 一位/打点足够时更早切出孤张宝牌 (靠张).
  - 四位/打点不足时更晚切出孤张宝牌 (靠张).
- 处理浮牌与复合型时, 时刻考虑**宝牌进张**的影响.
  - 宝牌搭子: **不固定非宝牌雀头**, 保留宝牌搭子形成宝牌对子可能性 (1 番 -> 2 番).
  - 宝牌对子:
    重视宝牌双碰进张, 保留至少 2 组对子 (包括两面补强牌),
    保留宝牌对子形成宝牌刻子可能性 (2 番 -> 3 番).
  - 宝牌四连型: `3456` (`3` 为宝牌), 进 `3` 时可形成 `33` + `456`, 尽量保留四连型.
  - 宝牌连续型: `11234` (`4` 为宝牌), 用筋牌 `1` 作雀头, 进 `4` 时可切 `1` 极具迷惑性.
  - 宝牌复合型: `345566` (`3` 为宝牌), 保留 `6`, 进 `3` 时可形成 `45566` 一杯口复合型, 宝牌对子作**雀头**.
  - 重视宝牌复合型**延展性**:
    - 最大化宝牌进张期望, 充分利用**后续宝牌进张**: 优先固定**非宝牌复合型**, 保证宝牌复合型延展性.
    - 宝牌**靠边**时延展性最好.

### 三色同顺手役

- 可以考虑三色同顺手役: 1 组面子 + 至少 6 牌.
- 同等牌效切牌时, **时刻注意三色同顺**手役的自然形成.
- 打点不足时重视三色靠张, 打点足够时重视好型与速度.
- 愚型较多时, 三色副露可以加快速度, 三色确定愚型搭子价值高于两面搭子.
- 三色同顺作牌天平:
  - Slide 天平: 空切 Slide 成型面子, 最大化三色可能.
  - 两天平: `34m2345p34s` 保留四连型, 保留 `234`/`345` 三色可能.
  - 浮牌天平: `245m234p234s` 保留浮牌 `2m`, 保留三色可能.
- 三色同顺处于当中位置的牌作为浮牌稍差: `234` 中 `3` 稍差.
  - `1234w3p122334s` 切 `4w`, 进张 `124p` 均有役, 存在 **3 种**改良.
  - `1234w3p122334s` 切 `1w`, 进张 `1p` 无役, 存在 **2 种**改良.
  - 不同位置的三色浮牌, 对于**拒听 / 即立**二择有重大影响 (**改良数差异**).
- 不考虑三色同顺手役:
  - 三色部分含有唯一雀头, 三色同顺手役作成难度较高.
  - 三色部分以外已有**两组**成型**面子**, 三色同顺手役作成难度较高.

### 一气贯通手役

- 可以考虑一气贯通手役: 1 组面子 + 至少 6 牌.
- 打点不足时重视一气靠张, 打点足够时重视好型与速度.
- 愚型较多时, 一气副露可以加快速度, 一气确定愚型搭子价值高于两面搭子.
- 1~2 枚宝牌时, 平和 > 一气贯通.
- 多组断幺搭子时, 断幺九 > 一气贯通.
- 对手吃 `9s` 形成 `789s` 副露, 对于防守一气贯通手役, `14s` 比 `23s` 安全.

### 染手手役

- 具有`立直`(**多好型**)/`断幺`/`三色`/`一气`等其他可能手役时, 不要强行染手.
- 中巡后染手手役未成型, 转牌效切牌, 不要强行染手.
- 可以考虑染手手役:
  - 混一色: 4 组搭子 + 至少 3 番.
  - 清一色: 至少 10 牌.
  - 3 组同色搭子 + 正常面子手最终型为愚型立直 Nomi: 强行染手追求满贯.
- 牌型较差的混一色手役要**重视防守**:
  - 高向听时不要轻易鸣牌.
  - 优先切中张给对手读牌压力, 保留**字牌**作为后续安全牌 (他人立直或听牌).
    (染手手役中的字牌在弃和后可用于防守).
- 牌型较好的混一色手役切牌时适当隐藏染手倾向 (e.g 优先切边张), 降低字牌鸣牌难度.

### 全带幺手役

- 五组以上幺九搭子 + 对子时可以考虑全带幺手役, 优先切中张牌.
- 赤五规则中全带幺手役价值较低, 除特殊情况基本不考虑副露全带幺手役.
- 全带系手役自身价值不高 (作牌难度大 + 听牌多愚型 + 副露降番),
  全带三色/全带役牌/全带宝牌等满贯复合手役 (门清/副露) 才有作牌价值:
  - 手牌较差有至少 4 组幺九愚型搭子, 门清和率较低时, 中巡可以考虑全带副露加速和牌.
  - 混老头/清老头 = 对对和 + 全带幺.

### 七对子手役

- 四对子: **牌型与进张较差**时, 可考虑七对子手役.
- 五对子: 早巡七对子一向听, 可考虑转对对和手役.
- 六对子: 中晚巡七对子听牌, 禁止转对对和手役.
- 亲家作七对子优先考虑和牌率 (保留**幺九对子**), 子家作七对子可考虑打点 (**断幺七对子/门混七对子**).
- 早巡 3 对子 + 0/1 面子 + 多愚型, 可以考虑七对子手役:
  - 在此种情况下, 普通面子手役**速度过慢, 打点过低**.
  - 七对子手役手牌灵活, 可以保留现物/幺九牌, 保证弃和时**拥有足够安全牌**.
- 七对子**平衡**:
  - 好型多向面子手前进, 愚型多向对子手前进.
  - 优先保留对子复合型, 保留面子手可能.
  - 4 对子 1 暗刻保留对对和/三暗刻/四暗刻面子手可能.
  - 山确枚数.
  - 对子筋容易成对.
- 七对子和率: 七对子进张数少, 听牌数少, 需要注重牌河作成 (引挂), 提升和率.
  - 壁筋引挂: `58` / `69` 前三巡早切 `5` / `6`, 提升 `8` / `9` 和率.
  - 单骑引挂: 听熟张/绝张字牌, 提升和率.
  - 早外引挂: `79` / `89` 前三巡早切 `7` / `8`, 提升 `9` 和率.
  - 幺九字牌立直与默听和率相近.
  - 早巡生张字牌, 中巡一枚现字牌, 晚巡两枚现字牌和率相近.
  - 8 巡目七对子一向听和率仅为 `11%`.
  - 在手牌条件允许下, 早巡按照字牌-幺九-中张顺序切若干张牌, 隐藏七对子手役, 提升和率.
- 七对子**对攻能力较弱**:
  - 追立需谨慎, 可考虑**兜牌或弃和**.
  - 避四规则平场场况, 七对子**一向听**一般选择**完全弃和**.
  - 避四规则南场四位, 七对子可以作成跳满进行对攻 (立直七对宝牌里宝牌).
- 七对子**宝牌二立直**有 55% 跳满机会.

### 对对和手役

- 提高和率 (对对和只能双碰听牌):
  - 牌河迷彩: 断幺/染手/全带.
  - 牌河手顺: 对子足够时, 尽早切掉对子周边牌, 防止被读牌.
  - 幺九牌容易鸣牌, 中张数牌不容易鸣牌.
- 多副露对对和 Nomi 收益低,
  需复合其他手役 (宝牌/役牌/混一色/全带幺/三暗刻/混老头) 作满贯.
- 可以考虑对对和手役 (七对子转对对和):
  - 早巡多对幺九对子 + **3900 / 5200** 点.
  - **8000** 点: 积极鸣牌.
  - 1 组 `刻子` + 4 组 `对子` (尽可能保留**幺九对子**).
- 基本不考虑对对和手役:
  - 两组 3-7 中张对子 + 低于 **5200** 点.

### 三暗刻手役

- 手牌打点低且有两组暗刻时, 可以损失一定牌效, 保留三暗刻可能.
- 手牌处于两暗刻一向听时, 可以保留两面补强牌与至少两组对子, 保留三暗刻可能.

### 国士无双手役

- 十种九牌可考虑国士无双手役.
- 九中九牌一般选择推牌流局.

### 役满手役

除天和/地和/国士无双外所有役满都是通常役的上位手役:

- 对对和 -> 四暗刻/四杠子.
- 小三元 -> 大三元.
- 混一色 -> 绿一色.
- 混一色 -> 清一色 -> 九莲宝灯.
- 混一色/对对和 -> 字一色/小四喜/大四喜.
- 全带幺/对对和 -> 混老头 -> 清老头.

## 振听规则

处在振听状态下, 无法荣和, 只能自摸.

### 捨牌振听

- 曾打出过当前听牌 (胡牌型, 不考虑手役), 进入捨牌振听, 所有听牌都无法荣和, 只能自摸.
- 解除方法: 换听其他没有振听的牌.
- 意味着可以**安全打出**其他三家**河牌与副露**,
  通过看牌避免放铳, 强调立直麻将的防守性.

### 同巡振听

- 听牌时, 没有荣和他人的牌, 进入同巡振听.
- 解除方法: 下一次自己打出任何牌.
- 意味着在一巡中可以**安全打出**上家打出过的牌,
  通过看牌避免放铳, 强调立直麻将的防守性.

### 立直振听

- 立直听牌时, 若出现可以胡的牌, 但没有进行胡牌, 进入立直后振听.
- 一直持续到此局结束, 意味着此局只能自摸.

:::tip 竞技麻将
振听规则是奠定立直麻将防守战术的基石.
:::

## 防守策略

### 安全牌

- 三家现物.
- 熟张字牌.
- 完全 NO CHANCE 牌.

#### 留安策略

在**搭子足够**前提下, 损失一定牌效 (一般为 2 张左右),
保留`熟张字牌`/`NC 边张`/高威胁对手`现物`作为安全牌:

- 切安全牌进行立直, 稳健进攻.
- 切安全牌进行兜牌, 不损牌效.
- 防止一发.
- 保留安全牌的同时, 可以优先切掉高威胁对手的`可能听牌` (**危险牌**), 保证自己**听牌时不放铳**.
- 当对手手牌速度较快时 (牌河宝牌/牌河异色中张/积极副露), 优先保留安全牌, 放弃改良浮牌, 保持手牌安定度.
- 一般情况下, 手牌 N 向听保留 N 张安全牌.
- 副露后手牌价值低 (形状/打点), 注重保留安全牌, 严格遵循 N 向听保留**至少** N 张安全牌准则.
- 积极观察牌河, 用**高效安全牌**代替字牌安全牌, 降低留安带来的**牌效损失**.
  **高效安全牌** (牌效损失小): `现物数牌`/`壁外数牌`/`暗刻字牌`.
- 手牌价值较高或点棒较少 (满贯或四位) 时, 可以不保留安全牌, 全速进攻.

### 壁牌

- 壁牌: 四枚可见, 对应 NO CHANCE 牌.
- 薄壁牌: 三枚可见, 对应 ONE CHANCE 牌.
- 壁牌/薄壁牌外侧牌相对安全, 内侧牌仍有放铳可能.

### 筋牌

表筋 `147`, `258`, `369`:

- 满筋 (**安全**): 现物有 `1` `7`, 则 `4` 是满筋牌.
- 边筋 (**安全**): 现物有 `4` `6`, 则 `1` `9` 是边筋牌.
- 半筋: 现物只有 `1`, 则 `4` 是半筋牌, 不太安全 (e.g `156` 切 `1` 听 `47`).

### 早巡外侧牌

早巡手切边张, 外侧牌安全.

### 弃和

安全度:

- 安全牌: 现物 > 熟字.
- 壁牌: NO CHANCE > Double ONE CHANCE > ONE CHANCE .
- 筋牌: 边筋 `19` >> 边筋 `28` = 满筋 `456` > 筋牌 `37`
- 早外牌: 早巡 `2378` 外侧牌放铳率降低 30%.
- ONE CHANCE 危险度: (筋牌, 无筋牌).
  中晚巡, OC 危险度急剧上升.
  晚巡 OC 不可信, 立直家持有最后一张概率极大.
- 中晚巡**生张/一枚现**役牌比`筋 28`危险.
- 边张 > 生张 > 宝牌生张.
- 宝牌筋 > 宝牌边 > 宝牌.
- 立直宣言牌的所在筋牌存在**骗筋听牌**可能, 危险度接近无筋牌.
- 立直宣言牌的另外两条筋牌存在**好型听牌**可能, 危险度上升.
- 引挂安全度: 后引挂 > 前引挂 > 立直宣言牌引挂.
- **变则手筋牌不可信**:
  - 染手手役 (混一色/清一色) 没有筋牌防守理论, 同色牌都是**危险牌**.
  - 对子手役 (对对和/七对子) 没有筋牌防守理论, `NO CHANCE`/`役牌`/`生张`都是**超危险牌**.

| 安全度 | 种类              | 注解                           |
| ------ | ----------------- | ------------------------------ |
| SSS    | 现物              | 绝对安全                       |
| SS     | 单骑字牌          |                                |
| S      | Side NO CHANCE    |                                |
| A+     | 边筋 `19`         | 双碰听, 单骑听                 |
| A      | 客风牌            | 双碰听, 单骑听 (高概率)        |
| A-     | NO CHANCE         |                                |
| B+     | Double ONE CHANCE |                                |
| B      | 边筋 `28`         |                                |
|        | 满筋 `456`        | 双碰听, 坎张听, 单骑听         |
| B-     | 筋牌 `37`         | 双碰听, 坎张听, 边张听, 单骑听 |
| C+     | 早外牌            |                                |
| C      | 役牌              |                                |
| C-     | ONE CHANCE        |                                |
| D      | 无筋 `19`         |                                |
|        | 半筋 `456`        |                                |
| E      | 无筋 `2378`       |                                |
| F      | 无筋 `456`        |                                |

:::tip 宝牌安全度
幺九宝牌下调 3 级, 非幺九宝牌下调 2 级, 宝牌跨筋下调 1 级.
:::

#### 弃和选择

- 某一家牌河有高打点迹象, 另外两家仍直线进攻, 自家手牌高向听, 应切掉危险牌留好安全牌, 随时作弃和准备.
- 他人立直或多副露听高打点牌, 且自己和牌困难 (e.g `23456` 向听/愚型搭子多且进张少) 时,
  除非情况特殊, 应完全弃和.

#### 弃和策略

- 未有人听牌 (早巡) 时, 优先打危险牌; 有人听牌后, 顺序打安全牌.
- 尽量保留**多家共同安全牌**, 优先切立直家特有现物, 警惕他家突然进攻.
- 不要过度依赖筋牌, 要结合壁牌/熟张/场况进行判断.
- 跟打策略 (同巡振听): 优先**跟着上家**出牌, 在对手直接摸切时才可跟着对家或下家出牌.
- 两家立直防守策略:
  - 优先防守亲家.
  - 优先防守追立家.
  - 优先防守竞争对手 (e.g 1 位防 2 位, 3 位防 4 位).
- 配牌极差, 和牌困难, **不应按牌效直线作牌**, 应该注重防守:
  - 可以损失一定牌效保留危险对手 (e.g 亲家) 现物, 同时尝试向听牌前进.
  - **防守反击**策略:
    可以考虑混一色/七对子/全带/国士无双等幺九手役,
    手牌多为幺九边张, 弃和时拥有足够安全牌.
  - **配牌弃和**策略:
    可以**优先切中张**, **保留幺九牌**,
    既可切掉危险牌保留安全牌, 又可制造染手/国士无双等高打点假象.
- 子家对亲家立直全弃与亲家对子家立直全弃的局收支均为 **-1700**:
  **东场自亲与高点差顺位自亲**面对子家先制立直, 不应盲目对攻连庄,
  应采取**子家面对亲家先制立直**相近攻守选择.

### 兜牌

扣住危险牌的同时, 向听牌前进:

- 以减少无筋孤张的前提进行切牌.
- 拆对子/复合型是兜牌的有效手段.
- 拆暗刻.
- 拆搭子.
- 拆面子会产生 2 张无筋孤张, 最终只能弃和.
- 七对子: 最强防守牌型.

### 牌山读牌

- 对手**染手**花色**场况差**, 牌山残余枚数少.
- **早巡对手捨牌**的**靠张**进张更容易, **场况好**:
  - 进张可能: 靠张高概率**牌山确**.
  - 鸣牌可能: 对手后续摸到早巡捨牌的靠张 (孤张废张), 高概率会**直接摸切**.
  - 听牌可能: 对手放铳率增加.
  - 早巡愚型听对手捨牌及其靠张, 可以考虑立即立直 (不寻求改良).
- **中晚巡对手捨牌**的**靠张**进张更困难, **场况差**.
- 生张字牌山确概率最高.
- 壁外数牌山确概率较高:
  e.g 可见 4 枚 `5m`, `5m` 靠张 (`3467m`) 山确概率较高.
- 边张数牌山确概率大于中张数牌.
- 中巡 1 枚现字牌山确概率大于生张字牌.
- 多家弃和时, 立直家现物山确概率大于非现物.

### 副露读牌

- 听牌可能:
  - 三副露.
  - 二副露 + 若干巡手切.
  - 一副露 + 切好型 + 多巡摸切.
  - 晚巡一副露.
  - 染手副露 + 切同色牌.
  - 断幺九副露 + 切中张宝牌.
  - 对对和副露 + 切中张好型.
  - 小三元副露.
- 宝牌副露: 不应盲目对攻.
- 小牌副露: 不应直接弃和.
- 早巡固定愚型存在作三色/一气/全带可能.
- 碰幺九宝牌存在役牌后附/对对和可能.
- 早巡两面吃牌: 存在高打点可能.
- 三副露 + 拆搭子: 单骑听牌可能.

副露线索牌:

- 副露捨牌.
- 手切安全牌.
- 手切宝牌.
- 手切搭子.
- 副露上家捨牌 (副露家未鸣牌).

副露安全牌:

- 手切安全牌前捨牌跨筋.
- 非最后副露捨牌跨筋.
- 两坎副露同色牌.

副露危险牌:

- 最后副露捨牌跨筋:
  - 两面听牌.
  - 吃牌跨筋危险度高于碰牌跨筋, 碰牌后捨牌周边可能存在雀头.
- 最后副露捨牌里筋: 食延换听.
- 副露捨牌未覆盖区域:
  - 暗刻作雀头.
  - 食延换听.
  - 复合型.
- 生牌.

6-10 巡听牌率:

- 一副露: 15%.
- 二副露: 34%.
- 三副露: 71%.

13 巡后听牌率:

- 一副露: 53%.
- 二副露: 70%.
- 三副露: 87%.

### 宝牌读牌

- 手切宝牌存在两种可能：
  - 满贯以上高打点 (放弃宝牌).
  - 好型一向听/听牌 (孤张宝牌).
- 早巡手切宝牌, 手牌速度较快.
- 早巡手切客风宝牌, 一般没有役牌对子, 存在断幺/平和可能.
- 早巡手切役牌, 一般没有客风宝牌, 存在断幺/平和可能.
- 手切宝牌靠张 (e.g `3p` 为宝牌时手切 `12p`): 固定宝牌对子/刻子.
- 通过**牌河宝牌**个数推测对手手牌打点.

### 手摸切读牌

- **摸切**: 存在靠张可能性下降.
- **手切**: 存在靠张可能性上升.
  - **跨筋**: `-2/+1` 与 `-1/+2` 两面听.
  - **里筋**: `23457` 进张或副露 `14` 后, 手切 `7` 形成 `36` 两面听.
- 空切可能 (Reset / Slide):
  - 面子手切捨牌: e.g 手切 `35s`, 多巡后手切 `4s`.
  - 重复手切捨牌: e.g 手切 `8s`, 多巡后手切 `8s`.
- 早巡多次摸切: 超好型或进张极差.
- 早巡切牌多为**断幺牌**, 后切**生张字牌**:
  高概率非常规手役 (染手/对子/全带/国士无双), 壁筋理论失效, 手牌速度不确定 (一般慢于正常顺子手役).
- 早巡手切 (两番) 自风牌, 手牌无孤张字牌, 手牌速度较快.
- 逆序手切: 后切的边张周围存在搭子/面子/手役的可能性上升.
  - e.g 切 `中9s`: `9s` 周围以及 `s` 上段存在搭子/面子/手役的可能性上升.
  - e.g 切 `3p8p`: `8p` 周围以及 `p` 上段存在搭子/面子/手役的可能性上升.
  - e.g 切 `8m1p`: `1p` 周围以及 `p` 下段存在搭子/面子/手役的可能性上升.
  - e.g 切 `4p -> XX -> 2p 立直`: `1p` 危险度上升 (`1124` -> `112` -> `11`).
  - e.g 切 `8m1p7p2s`: 下段存在三色同顺手役的可能性上升.
  - e.g 切 `8s -> 2p -> 字牌`: 存在字牌对子, 较高副露可能.
  - e.g 切 `5s -> 3s -> 字牌`: 染手手役可能性上升 (字牌价值 > 非同色数牌), 手牌**速度较快**.
  - e.g 早巡切 `役牌 -> 客风牌`: 轻视役牌, 手牌**速度较快**, **打点较高** (存在立断平可能).
  - e.g 前五巡切 `3p2w` / `7s2p`: 早出尖张牌 `37`, 手牌**速度较快**.
- `高价值浮牌早切`/`低价值浮牌晚切`: 留有特定形状的可能性变高, 特定牌的危险度上升.
  - e.g 早切 `5`, 里筋 `1469` 危险度上升: `235`, `578`.
  - e.g 晚切 `5`, 里筋/跨筋危险度基本不变, 存在多种情况: `235`, `556`, 靠张一向听.
  - e.g 早切 `8`, 里筋/跨筋危险度基本不变, 存在多种情况:孤张 `8`, `568`, `788`, `899`.
  - e.g 晚切 `8`, 跨筋 `69` 危险度上升: `788`, `899`.
- 手切**好型搭子** (e.g `56` 两面搭):
  - 好型搭子超载, 手牌**速度较快**.
  - 好型听牌可能, 可用**筋壁理论**防守.
  - 受`宝牌`/`手役`(三色/一气/全带/七对)/`枚数`影响, 存在**更弱好型搭子**/**愚型搭子**听牌可能.
- 手切**愚型搭子** (e.g `75` 坎张搭): 愚型搭子超载, 手牌**速度较快**.
- 手切对子:
  - 对子跨筋危险度下降.
  - 手牌至少一组对子, 无头一向听可能性较小, 完全一向听可能性较大.
- 手切**幺九对子**: 作断幺九手役, 手牌**速度较快**.
- 手切**字牌对子**: 断幺手役/两面听牌可能.
- 手切**役牌对子**: 平和/断幺/清一色手役可能, 手牌**速度较快**, **打点较高**.
- 手切**两番役牌对子**: 超高打点手牌可能.

### 立直读牌

- 立直宣言牌一般为以下三种:
  - 安全牌.
  - 改良浮牌.
  - 改良靠张: e.g 两面对补强牌.
- 好型放铳率: 1 / (18 - N), `123789` + 1, `456` + 2.
- 愚型放铳率:
  - 立直前手切 2 枚以上中张数牌, 数牌周边存在愚型可能大幅度降低:
    - e.g `2mX7mX4m` 万字数牌可能全好型.
    - e.g `9mXXXX4m` 听边 `7m` 概率大幅下降.
    - e.g `9m8mXX4m` 听坎 `7m` 概率大幅下降.
  - 立直前手切 1 枚中张数牌, 未切一张远端边张牌, 存在前筋引挂可能:
    - e.g `1mxx4mxx`, 未切过 `89m`, 存在听边 `7m` 可能.
- 手切生张役牌立直: **双碰/单骑字牌**听牌可能.
- 手切熟张字牌 (安全牌) 立直: **好型**听牌可能.
- 手切壁外数牌立直: **壁外愚型**听牌可能.
- 早中巡手切 `19` 立直: 高概率双碰/单骑听牌 (`122`/`133` -> `22`/`33`), 存在七对子立直可能.
- 早中巡手切 `5XXX2` / `5XXX8` 立直:
  - 高概率双碰/边张听牌: `112` / `122` -> `11` / `12`.
  - 存在两面听牌可能: `2235` -> `223` -> `23` / `5788` -> `788` -> `78`.
- 早中巡手切 `37` 立直: 高概率两面听牌.
- 早中巡手切 `46` 立直且切过远段牌 (`789` / `123`): 高概率两面听牌.
- 早中巡手切 `5` 立直:
  - 一般情况下, 切 `5` 立直两面听 `36` 或 `47`, 即立直宣言牌周围可能存在靠张.
  - 存在坎张听牌骗筋可能 (`135`/`579` 切 `5`), 立直宣言牌的筋牌 `2` 与 `8` 危险度上升.
  - `0` 立直: `230` / `078` 切 `0`, `1469` 危险度大大上升.
- 立直前晚切 `1` / `9`: `1` / `9` 里筋危险度上升.
  e.g `13` 进张 `4` 手切 `1`.
- 摸切立直:
  - 改良数变少.
  - 改良巡目过晚.
  - 他家手牌进度加快.
  - 待牌场况变好: e.g 壁筋引挂.
- 逆切立直 (`5` -> `2`), 听立直宣言牌周边概率约为 50 %, 远远高于普通场景听立直宣言牌周边概率.
- 非靠张一向听 (读入目与里目):
  - 逆切数牌, 立直前切宝牌, 手切字牌立直: 靠张一向听优先保留靠张能力强的浮牌.
  - 立直前切两面搭: 靠张一向听缺少搭子, 不太可能拆好型搭子.
  - 立直前切 MPS 多枚中张牌: 没有靠张空间 (大部分靠张可能产生振听).
- 立直若干巡后, 其他家未切的**立直家现物**高概率**牌山确**.
- 立直若干巡后, **未通过筋牌**的危险度: 牌河中枚数越少的筋牌 (e.g 0 或 1 枚), 危险度越高.
- 立直若干巡后, **未通过暗刻**的危险度: 手牌中枚数越多的筋牌 (e.g 暗刻 `22555p`), 危险度越高.
- 亲家早巡立直, 存在愚型听牌与低打点的可能:
  - 亲家牌河: 立直前手切对子/搭子/宝牌靠张, 亲家手牌速度快, 打点高, 优先考虑弃和.
  - 手牌价值: 立直 `Nomi` / 愚型听牌, 优先考虑弃和.
  - 当前场况: 其他子家仍在进攻, 可以考虑弃和, 期待点棒横移.

### 手役读牌

- 役牌:
  - 前三巡未切字牌, 三-六巡开始手切字牌: 手牌高概率役牌对子 + 其他字牌.
  - 逆序手切 `中张数牌` -> `字牌`: 手牌高概率役牌对子 + 其他字牌.
  - 逆序手切 `中张数牌` -> `幺九数牌`: 手牌存在役牌对子可能.
- 断幺九:
  - 手切幺九对子.
  - 牌河均为幺九牌及其靠张.
  - 早巡切边张搭子.
- 平和:
  - 早巡手切 `字牌 -> 19 -> 28 -> 34567`.
  - 幺九数牌及其靠张切牌顺序晚于断幺九手役.
  - 中巡手切边张搭子.
- 三色同顺:
  - 早巡手切三色 `456`, 切掉赤宝牌靠张, 存在下/上段三色同顺手役可能.
  - 逆序手切周边存在三色同顺手役可能.
  - (赤) 宝牌周边存在三色同顺手役可能.
- 一气贯通:
  - 牌河接近混一色, 字牌切牌顺序早于染手手役.
- 染手:
  - 早巡只切两色数牌, 包括切对子/搭子.
  - 连续手切熟张字牌, 高概率一向听, 鸣牌后听牌可能.
  - 手切生张字牌, 高概率好型一向听, 鸣牌后听牌可能.
  - 连续手切染手牌 (染手溢出), 高概率听牌.
- 全带:
  - 早巡手切 `46 -> 2378`.
  - 逆序手切 `52` / `58`.
  - 前三巡不切字牌.
- 七对子:
  - 起手一般不会选择七对子手役, 后续进张多组不靠张对子才会转为七对子手役.
  - 早巡手切中张牌.
  - 可能手切两面搭子.
  - 中巡手切熟张幺九牌/边张牌 (一向听).
  - 重视幺九对子 (包括役牌对子).
- 对对和:
  - 明刻副露.
  - 可能手切两面搭子.
  - 手牌选择不如七对子灵活, 边张切牌顺序早于七对子.
  - 中巡手切熟张役牌.
  - 重视役牌对子 (包括幺九对子).

### 进攻信号

- 逆序切牌.
- 切宝牌及其靠张.
- 变则手切生张字牌.
- 先切安全牌后切危险牌.
- 摸切安全牌.
- 连续进张后手切安全牌: 听牌可能.
- 亲家鸣牌同巡 (听牌可能), 子家切危险中张: 子家选择与亲家对攻.
- 切立直/副露家危险牌.
- 晚巡切生张.

**手牌速度快**信号:

- 早巡连续切生张役牌.
- 早巡手切尖张牌 `37`.
- 早巡手切宝牌及其靠张.
- 早巡手切对子/搭子.
- 早巡手切三枚不同色中张数牌: MPS 法则.

### 防守信号

- 跟打现物.
- 切面子.
- 先切危险牌后切安全牌.

### 防守实例

`9p1z5z4p` 长考立直: 高概率 `68p` 听 `7p`.

先 `9p` 后字牌, 说明 `p` 上段存在靠张.
`4p` 长考立直, 说明愚型听牌.
`69p` 切 `9p`, `468p` 切 `4p` 骗筋听 `7p`.

`1pXXXX1pXXXX3p` 先制立直:
可能存在 `355p` 切 `3p` 立直,
若此时一向听进张后坎张听 `5p`, 则和牌率很低 (中张 `5p` 仅两枚残),
不可盲目追立, 可以拒听改良/兜牌默听/直接弃和.

## 场况策略

### 一位策略

保守策略:

- 不盲目对攻, 不盲目立直, 尽量默听.
- 手牌价值低时, 不盲目与三四位对攻.
- 可与二位对攻, 阻止二位和牌.
- 避免开杠.
- 保留安全牌.
- 南风局和牌局消化, 追求和率, 不追求打点.
  - 速攻结束牌局.
  - 速攻抢庄.
- 电报完场: 处于大 TOP ALL LAST 状态, 必要时可以帮助三/四位 (争二) 副露和牌结束牌局.

### 四位策略

激进策略:

- 积极进攻, 不保留安全牌.
- 手牌价值低时, 不盲目与一二位对攻.
- 积极与三位对攻, 阻止三位和牌.
- 南风局亲家连庄延长对战局数, 保留避四机会.

### 东场策略

- 重视打点, 争取领先进入南场.
- 东一局不执着于高打点:
  - 东一局子家和 2000 点, TOP 率上升 (`29.6%`).
  - 东一局子家铳 8000 点, LAST 率上升 (`46.0%`).

### 南场策略

- 一位重视和率, 四位重视打点.

### 亲家策略

- 积极对攻: 给予子家压力, 延长自摸巡目, 防止被自摸炸庄, 争取自家唯一形听.
- 亲家进攻威慑力大 (立直 > 默听).
- 目标不是**强行**连庄, 优先当前局收支最大化 (高打点).
- 首亲重视打点, 尾亲重视和率.
- TOP 时无需**强行**连庄, 优先保证安全下庄.

### 子家策略

- 立直追求满贯.
- 副露追求宝牌/染手/对对和.

### 早巡策略

- 当牌型较好时, 可以损失一定牌效去追求打点 (平和/断幺/三色/染手).

## 攻守策略

- 确认所持点数.
- 确认宝牌.
- 确认序盘战略.
- 确认有效牌损失枚数.
- 确认字牌损失枚数.
- 确认 NC/OC 牌.
- 读手摸切.
- 读他家手牌速度.
- 读他家手牌打点.
- 读他家手牌形状.
- 数筋牌.
- 确认安全牌.
- 手牌速度.
- 手牌打点.
- 手牌形状.

### 攻守原则

- 点棒状况: 落后激进, 领先保守.
- 手牌价值 (打点): 打点越高, 越激进.
  - 打点越高, 留安必要性下降, 优先最大化进张数.
  - 打点越低, 留安必要性上升, 优先保留安全牌 (e.g 切掉两面对补强牌, 不要双碰进张).
- 手牌形状 (和率):
  - 向听数越低, 越激进.
  - 最终形状越好, 越激进.
- 放铳危险度:
  - 捨牌危险度: 现物, 熟张字牌, 筋 `19`, NC/OC 牌, 筋 `2378`, 无筋 `2378`, 无筋 `456`.
  - 对手打点: 亲家/子家, 副露打点, 牌河**宝牌**出现枚数.
    - 立直.
    - 染手.
    - 对对和.
    - 满贯副露 (e.g 2~3 枚宝牌).
  - 巡目越晚, **半筋/无筋牌**放铳概率越高.
  - 局数越晚, **放铳吃四**概率越高.
  - 两家对攻, 放铳概率高: e.g 子家立直, 亲家对攻时, 手牌打点低或形状差时应完全弃和.
- 弃和成功率.

:::tip 对攻原则
**打点**是对攻的准入资格, **形状**是对攻的胜率保障, **放铳危险度**是对攻与否的参考依据.
:::

### 序盘策略

- `配牌向听数` = `8` - `2 * 面子数` - `1.5 * 役牌对子数` - `1 * 搭子/对子数` - `0.5 * 宝牌数`:
  - 配牌向听数 <= **3.5** 向听, 积极作牌.
  - 配牌向听数 > **3.5** 向听, 消极作牌.
- 低打点, 速度快: 牺牲速度, 提升打点.
  - e.g 早巡立直 Nomi 听牌: 可以默听或拒听, 考虑宝牌/平和/断幺九/三色同顺打点改良可能.
- 高打点, 速度慢: 寻找手役, 提升速度.
  - e.g 早巡宝牌刻子: 考虑役牌/断幺等可**鸣牌**手役, 提升速度.
- 低打点, 速度慢: 考虑非常规手役 (染手/对子/全带/国士无双), 以满贯为目标作牌, 同时保持手牌防御力.

### 对攻策略

- 追立时, 应优先考虑和率 (对攻成功率).
- 追立两家时, 保证好型 3 番/愚型 4 番打点.

#### 好型听牌对攻策略

- **两面听牌追立**局收支基本为正数, 可以**合理对攻**:
  - 一发巡切安全牌 + **1300** 以上打点.
  - 非一发巡切 `10%` 牌 + **2600** 以上打点.
  - 对攻亲家满贯 + **5200** 以上打点.
  - 一般情况下, 追立优于默听.
  - 听立直家现物 + 高打点手牌, 可以考虑默听追求和率.
- **两面副露听牌**局收支基本高于完全弃和 (-1100), 可以**合理对攻**:
  - **2600** 以上打点.
  - 切安全牌.
  - 切 `10%` 牌.
- 子家:
  - 8 巡: 打点 > `对手 * 1/3`.
  - 12 巡: 打点 > `对手 * 1/2`.
- 亲家
  - 8 巡: 全攻.
  - 14 巡后: 两番.

#### 愚型听牌对攻策略

- **愚型听牌**和率与放铳率相近, 需要**高打点对攻**:
  - **3900** 以上打点.
  - 切安全牌.
  - 切 `10%` 牌.
- 子家:
  - 6 巡: 打点 > `对手 * 2/3`.
  - 12 巡: 打点 ~= 对手.
- 亲家:
  - 6 巡: 全攻.
  - 8-15 巡: 两番.
  - 15 巡后: 三番.

## 点数计算

- 基本符数: 20 符.
- 幺九刻子符数:
  32 (暗杠) -> 16 (明杠) -> 8 (暗刻) -> 4 (明刻),
  断幺刻子符数**减半**.
- 役牌雀头/坎张听/边张听/单骑听 2 符, 自摸 2 符, 门清荣和 10 符.
- 七对子 25 符, 平和自摸 20 符, 平和荣和 30 符.
- 自摸/鸣牌荣和至少 30 符, 门清荣和至少 40 符.

| 番数       | 称呼   | 基本点                  |
| ---------- | ------ | ----------------------- |
| < 2000     |        | `2 ^ (番数 + 2) * 符数` |
| 5 番       | 满贯   | 2000                    |
| 6 - 7 番   | 跳满   | 3000                    |
| 8 - 10 番  | 倍满   | 4000                    |
| 11 - 12 番 | 三倍满 | 6000                    |
| 13 番      | 役满   | 8000                    |

|      | 荣和         | 自摸                                     |
| ---- | ------------ | ---------------------------------------- |
| 子家 | `基本点 * 4` | 亲家赔`基本点 * 2`, 子家各赔`基本点 * 1` |
| 亲家 | `基本点 * 6` | 子家各赔`基本点 * 2`                     |

## Mahjong Reference

- [Beginner's Luck](http://beginners.biz/kihon)
- [魔女ブログ](https://puyokururu.medium.com)
- [おしえて！科学する麻雀](https://book.douban.com/subject/20390543)
- [Li, Junjie, et al. "Suphx: Mastering mahjong with deep reinforcement learning." arXiv preprint arXiv:2003.13590 (2020)](https://arxiv.org/pdf/2003.13590.pdf)
- [天鳳牌理好形表示](https://greasyfork.org/zh-CN/scripts/435111-%E5%A4%A9%E9%B3%B3%E7%89%8C%E7%90%86%E5%A5%BD%E5%BD%A2%E8%A1%A8%E7%A4%BA)
