代发 wailian999

[U71] PHP：抛出异常
来源：http://hz.cashguo.top/gtridgcpmu.html

throw new RuntimeException("失败", 500);
来源：http://hz.chenjidiqi.icu/gtcigdjniv.html

[U72] PHP：写错误日志
来源：http://hz.dashuyun.cn/gtqpjbyshe.html

error_log("失败: " . $e->getMessage());
来源：http://hz.shanyushiyangkeji.top/gtrwxqgrxv.html

[U73] PHP：读取 ini 配置
来源：http://hz.andypj.xyz/gtbhgyzmhu.html

parse_ini_file("config.ini", true)
来源：http://hz.chenzaomai.com/gtasdgwndx.html

[U74] PHP：读取环境变量
来源：http://hz.svipenyu.cn/gtlqvmbgim.html

getenv("APP_ENV") ?: "production"
来源：http://hz.zycfv.cn/gtjclmiqrc.html

[U75] PHP：依赖注入
来源：http://hz.svipenyu.cn/gteqjfjqwg.html

composer require psr/container
来源：http://hz.zhijiandao.cn/gthriofupi.html

[U76] PHP：简单路由
来源：http://hz.xziqi.cn/gttgogkwgw.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hz.ydzc1.top/gtewzormkp.html

[U77] PHP：模板渲染
来源：http://hz.hongshengwenyu.top/gtmbtufxwx.html

composer require twig/twig
来源：http://hz.jlsjyb.cn/gtwaxykedg.html

[U78] PHP：单元测试
来源：http://hz.shzxlz.cn/gtzvbxtcuq.html

composer require --dev phpunit/phpunit
来源：http://hz.zhiwuduotai.top/gtkckquogo.html

[U79] PHP：静态分析
来源：http://hz.nanxinkj.top/gtxtwbclrt.html

composer require --dev phpstan/phpstan
来源：http://hz.nwbrower.top/gtzfvnupci.html

[U80] PHP：代码规范修复
来源：http://hz.havefunace.top/gtagohnwwu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.xylfe.cn/gtpgttwyrl.html

[U81] JS：初始化项目
来源：http://hz.ydzc1.top/gtzvuhauzj.html

npm init -y;  npm i express
来源：http://hz.yvedp.cn/gtkjaoytmm.html

[U82] JS：package.json 脚本
来源：http://hz.svipenyu.cn/gtrugtwrui.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.iojbl.cn/gtxyjzlclr.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhiwuduotai.top/gttpbtasxb.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shuidangran.top/gtrmpucpou.html

[U84] JS：CommonJS 写法
来源：http://hz.nanxuanxn.top/gttrpkqjdk.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nanxinkj.top/gtbdzbptlv.html

[U85] JS：可选链
来源：http://hz.9152youxi.cn/gtidqidkgr.html

a?.b?.c
来源：http://hz.chenlongwang.top/gtrswbuajb.html

[U86] JS：空值合并
来源：http://hz.yj202588.top/gtiiopxvzn.html

a ?? b
来源：http://hz.mhx1999.top/gteligykqq.html

[U87] JS：解构默认值
来源：http://hz.smart0.xyz/gtoedacgzc.html

const { a = 1, b = 2 } = obj;
来源：http://hz.0kj1m.cn/gtzzpeslmc.html

[U88] JS：对象展开合并
来源：http://hz.yuxming.cn/gtioxahptt.html

{ ...a, ...b }
来源：http://hz.shuidangran.top/gtgrcyxzhg.html

[U89] JS：数组去重
来源：http://hz.sxryk.cn/gtpwwbnhce.html

[...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtwxdrbkxd.html

[U90] JS：数字数组排序
来源：http://hz.zycfv.cn/gtlkzrvxij.html

[...arr].sort((a, b) => a - b)
来源：http://hz.daria6918.cn/gtzhgccsxu.html

[U91] JS：对象键值遍历
来源：http://hz.pengpengdd.cyou/gtxlctzfcu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.chenjidiqi.icu/gtqraqjkzf.html

[U92] JS：深拷贝
来源：http://hz.ybcxt.top/gtjrnmtcmp.html

structuredClone(obj)
来源：http://hz.zycfv.cn/gtvbfcvxch.html

[U93] JS：模板字符串
来源：http://hz.ydjk.org.cn/gtbzsossyz.html

`共 ${n} 条`
来源：http://hz.xuanzx.com/gtybejoymb.html

[U94] JS：箭头函数
来源：http://hz.zdqjudy.top/gtfifaithc.html

const double = x => x * 2;
来源：http://hz.yonumen.top/gtjcrueyxq.html

[U95] JS：Promise 包装
来源：http://hz.haohaochexian.top/gtoimzxigb.html

new Promise((resolve, reject) => {})
来源：http://hz.hammf.cn/gtjiuitmhd.html

[U96] JS：async/await 与异常
来源：http://hz.xuanzx.com/gtmuildute.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtpilermax.html

[U97] JS：并发请求
来源：http://hz.nanxinkj.top/gtaqmuvxas.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gttkgjlizg.html

[U98] JS：fetch 带 JSON
来源：http://hz.jinyuanbaomall.cn/gtlaluubeg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.birdmap.top/gtydroiavm.html

[U99] JS：事件监听
来源：http://hz.9152youxi.cn/gtmbrpakkf.html

el.addEventListener("click", e => {})
来源：http://hz.gotoacloud.top/gticdmvaxj.html

[U100] JS：DOM 查询
来源：http://hz.sxryk.cn/gtuyeflmoj.html

document.querySelector(".item")
来源：http://hz.hfpthk.cn/gtqjgtzjlb.html

[U101] JS：classList 操作
来源：http://hz.zhiwuduotai.top/gtertzmnys.html

el.classList.toggle("active")
来源：http://hz.kuanghao11.cn/gtaftwdzcf.html

[U102] JS：本地存储
来源：http://hz.zhijiandao.cn/gtiipplnfm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.ehwqpu.com/gtnsnsumzg.html

[U103] JS：定时器
来源：http://hz.wangdashe.top/gtkjukhejd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jinqigufen.top/gtcbwieitf.html

[U104] JS：防抖
来源：http://hz.zhaomingkeji.xyz/gtkzzjamsk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gtodotwxds.html

[U105] JS：节流
来源：http://hz.pengpengdd.cyou/gtmyirxjpo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhiwuduotai.top/gtdeuvtfwz.html

[U106] JS：日期格式化
来源：http://hz.cucudq.cn/gtqothhplk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yuanzhike.top/gtqtekbecb.html

[U107] JS：数字千分位
来源：http://hz.jqgufenzy.top/gtqghtkasu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jinghuilouyu.cn/gtqzromysa.html

[U108] JS：随机整数
来源：http://hz.ppjwa.cn/gtswgkxctf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jiagoushi.top/gtugbyhpuz.html

[U109] JS：数组分组
来源：http://hz.aizwys.cn/gtmnizwjri.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtxadnnley.html

[U110] JS：数组分块
来源：http://hz.jinqigfzy.top/gtikszvyof.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jlsjyb.cn/gthnewpuat.html

[U111] JS：对象转 Map
来源：http://hz.xziqi.cn/gttwgftauo.html

new Map(Object.entries(obj))
来源：http://hz.ybcxt.top/gtesejsjpx.html

[U112] JS：字符串补位
来源：http://hz.quarkkingdee.top/gtvkmpkitt.html

"7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtflmptnou.html

[U113] JS：正则替换全部
来源：http://hz.hongshengwenyu.top/gtjwtsdhaf.html

s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtevwrtyyb.html

[U114] JS：JSON 深比较
来源：http://hz.ywan-chungtsiang.top/gtcztlmldn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtmyvpyrhi.html

[U115] JS：生成 UUID
来源：http://hz.ydjk.org.cn/gtvohwblxo.html

crypto.randomUUID()
来源：http://hz.zhengqikj.top/gtbzmkufas.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.nanxinkj.top/gtnwjojnpq.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yongpay.top/gticbqwibt.html

[U117] JS：单元测试
来源：http://hz.hnqzz.top/gtmbxcmzfk.html

npm i -D vitest;  npx vitest
来源：http://hz.zhengqikj.top/gtefszlcpg.html

[U118] JS：开发服务器
来源：http://hz.yangfankeji.com/gtuuqiltnp.html

npm i -D vite;  npx vite
来源：http://hz.yueranfly.top/gtvqxjuxum.html

[U119] JS：生产构建
来源：http://hz.dashuyun.cn/gttsomjmme.html

npx vite build
来源：http://hz.sxryk.cn/gtidtutcif.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangtech.top/gtigahvjaw.html

import.meta.env.VITE_API_URL
来源：http://hz.yvedp.cn/gtduwzsnbs.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvepirvvy.html

统计汇总
来源：http://hz.zhixingplan.top/gtpcpzqtvu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvnmpqymq.html

按语言统计（条）：
来源：http://hz.nanxuanxn.top/gtunmtkiet.html

Python ......... 252
来源：http://hz.shanyushiyangtech.top/gtamaavgou.html

PHP ............ 252
来源：http://hz.jinqigfzy.top/gtcukkbwnf.html

JavaScript ..... 252
来源：http://hz.zhoulong.xyz/gtrkeqkniq.html

TypeScript ..... 212
来源：http://hz.aizwys.cn/gttuvlifom.html

Java ........... 212
来源：http://hz.ppjwa.cn/gtpgmqmkbq.html

Go ............. 212
来源：http://hz.gotoacloud.top/gtgrilimmm.html

Ruby ........... 212
来源：http://hz.tian-w.cn/gtermvxxdy.html

C# ............. 212
来源：http://hz.yj20258888.top/gtyznynuqj.html

C .............. 30
来源：http://hz.shzxlz.cn/gtwyragqvr.html

C++ ............ 30
来源：http://hz.yangfankeji.com/gtbfovuzoz.html

SQL ............ 90
来源：http://hz.ivvv.top/gtfyuykmqj.html

Bash ........... 80
来源：http://hz.ehwqpu.com/gttnvxbmmz.html

Kotlin ......... 15
来源：http://hz.ydjk.org.cn/gtzapgtgcp.html

Swift .......... 15
来源：http://hz.kuanghao11.cn/gthdbbovas.html

Lua ............ 10
来源：http://hz.shanyushiyangtech.top/gtrakupzfk.html

Perl ........... 10
来源：http://hz.yonumen.top/gtromstsbg.html

Scala .......... 10
来源：http://hz.yvedp.cn/gtqlpltwaz.html

------------------------------------
来源：http://hz.chenjidiqi.icu/gtbxanxnzy.html

合计 ........... 2106 条
来源：http://hz.jinghuilouyu.cn/gtqkhiwvdv.html

按章节统计：
来源：http://hz.sufxvd.cn/gtbbwgqhaa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.c1oappe.top/gtacobywwm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.cashguo.top/gtcapbffjq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.xylfe.cn/gtpkqwgswc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.yj202588.top/gtzjkrxoim.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.guannengcc.top/gtqyjtvnix.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.smart0.xyz/gtqhidkvdh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.c1oappe.top/gtxuipafns.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.gzhubu.top/gthqmxgxje.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.316326.xyz/gtuxtdswrc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.shangyingyoupin.top/gtjqrpqceu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.vqdsnc.cn/gtshpgksqw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.cheryme.top/gthfhwqotf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xylfe.cn/gtmfkwsmax.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yangfankeji.com/gtbktnbcei.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.pycfn.com/gtsaaqfykc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.quarkkingdee.top/gtqlycajus.html

Q SQL 专题                              90
来源：http://hz.yj20258888.top/gtvqxsysux.html

R Bash 专题                             80
来源：http://hz.gaohongyu789.top/gtwphobsub.html

S C / C++ 专题                          60
来源：http://hz.chenlongwang.top/gttobgukxu.html

T 其他语言补充                          60
来源：http://hz.tian-w.cn/gtufaczxgt.html

U 高频实用片段                         120
来源：http://hz.hnqzz.top/gtgaahtnqf.html

------------------------------------
来源：http://hz.jyoumei.cn/gtpaptsulj.html

合计                                  2106 条
来源：http://hz.pycfn.com/gtbjxwytmt.html

--------------------------------------------------------------------------------
来源：http://hz.sxryk.cn/gthpqikolz.html

使用提醒
来源：http://hz.daria6918.cn/gtrjunlqgu.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtkzrzuyfy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.guannengcc.top/gtnrcqqxtk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.gzhubu.top/gtmkbpdqvs.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.cucudq.cn/gttqtqzkba.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.tianlin.xyz/gtfdoxnnlw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhaomingkeji.xyz/gtnngkqyfs.html

—— 文件结束 ——
来源：http://hz.zdqjudy.top/gttghupevf.html

================================================================================
来源：http://hz.zycfv.cn/gtlgyeguyv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.52xcode.cn/gtikhlpjcj.html

Common Programming Examples Cheat Book
来源：http://hz.hywenlv.cn/gtbvwuqyof.html

================================================================================
来源：http://hz.shzxlz.cn/gtysddtiih.html

【收录内容】
来源：http://hz.jiagoushi.top/gtolrcandt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.ivvv.top/gtskxglkco.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.hnqzz.top/gthzkktapc.html

SQL · Bash · C · C++
来源：http://hz.jinyuanbaomall.cn/gtvmtzbowg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.daria6918.cn/gthmzeplbw.html

【使用说明】
来源：http://hz.yj20258888.top/gtageufpag.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.birdmap.top/gtzddsyngk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.xinyue.icu/gtdhkvfjsz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nanxuanxn.top/gtpqavrfdo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zhijiandao.cn/gtqhidejry.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yangfankeji.com/gtpjahkxza.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.kuanghao11.cn/gtrjrelviq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.pengpengdd.cyou/gtcorwwcyo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jinqigufen.top/gtbhejclin.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hnxiangtu.top/gtnluzpmof.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.fengsongda.top/gtvzulzptb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhongyouzk.top/gtuwfevrxk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cashguo.top/gthpedzxcg.html

【文件统计】
来源：http://hz.sxryk.cn/gtyrodohrs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.mhx1999.top/gtasrygbae.html

--------------------------------------------------------------------------------
来源：http://hz.zhiwuduotai.top/gtmnzwsagc.html

目  录
来源：http://hz.iojbl.cn/gtlmghtwtg.html

--------------------------------------------------------------------------------
来源：http://hz.yuxming.cn/gtvmrpirlc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xylfe.cn/gtgadomtji.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.jinyuanbaomall.cn/gtsmcrhioi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.iojbl.cn/gtxupofxnn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cashguo.top/gtwlszujva.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.xylfe.cn/gtmlkdrqqc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.gogol.net.cn/gtqzqwlhsf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shangyingyoupin.top/gtplpjqjoq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhiwuduotai.top/gtsnpqdbkd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtglwqwgpr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yuxming.cn/gtrkrgofcr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtkutwebtc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtmkvvbzxv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtwzbzthde.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.52xcode.cn/gtwhukxuwn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenjidiqi.icu/gtbvdrgfrd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtviiniylw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.hysaishi.cn/gttgyjsdfp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.havefunace.top/gtoadrfzus.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.mhx1999.top/gtonjuaoin.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.0kj1m.cn/gtyvhboiyf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.gogol.net.cn/gtafrgfnuv.html

================================================================================
来源：http://hz.smart0.xyz/gtxffeabnv.html

A. 基础语法与类型
来源：http://hz.dianchejie.cn/gtzkhuqthw.html

================================================================================
来源：http://hz.sweek.top/gttzlapasi.html

[A01] Hello World
来源：http://hz.aizwys.cn/gtdeinuegb.html

Py:   print("Hello, World!")
来源：http://hz.yangfankeji.com/gtediuzssp.html

PHP:  echo "Hello, World!";
来源：http://hz.wangshuangyany.cn/gtmjhapdjp.html

JS:   console.log("Hello, World!");
来源：http://hz.hywenlv.cn/gtdqdtzliu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhongyouzk.top/gttceyrigs.html

Java: System.out.println("Hello, World!");
来源：http://hz.hfpthk.cn/gteefcpuxq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.xziqi.cn/gtxlsqewlx.html

Ruby: puts "Hello, World!"
来源：http://hz.tanke756.top/gtahsrixgh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.havefunace.top/gthkzfaumv.html

[A02] 变量声明与赋值
来源：http://hz.sufxvd.cn/gtoruktcga.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xuetiantiany.cn/gtdpzdiflu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shuidangran.top/gtjtrwxepk.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ywan-chungtsiang.top/gtmwawlnab.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.haohaochexian.top/gtzockqhes.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.jianghu66.top/gtmmwrieqn.html

Go:   name := "Alex"; age := 20
来源：http://hz.chenzaomai.com/gtmpvuxdyz.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jqgufenzy.top/gtjwsxrsxe.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.chenjidiqi.icu/gtztjtbfol.html

[A03] 常量定义
来源：http://hz.svipenyu.cn/gtruyusqfu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.zhoulong.xyz/gtghiuaeqy.html

PHP:  const PI = 3.14159;
来源：http://hz.birdmap.top/gtmeznswfx.html

JS:   const PI = 3.14159;
来源：http://hz.jinghuilouyu.cn/gtssfgixqp.html

TS:   const PI: number = 3.14159;
来源：http://hz.tian-w.cn/gtvgcphmmp.html

Java: static final double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtvgffmvxb.html

Go:   const PI = 3.14159
来源：http://hz.cdnleiting.top/gtywaxvrll.html

Ruby: PI = 3.14159
来源：http://hz.shuidangran.top/gtjohgjioq.html

C#:   const double PI = 3.14159;
来源：http://hz.jinqigufen.top/gtfqlddzgs.html

[A04] 判断变量类型
来源：http://hz.gogol.net.cn/gtrlrwqaku.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.pengpengdd.cyou/gtplbxozku.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.chenzaomai.com/gtxdyvrclx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.ywan-chungtsiang.top/gtnytaiajf.html

TS:   typeof x; x instanceof Date
来源：http://hz.bjfxy.top/gtdbnxfkgg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.gogol.net.cn/gteqrwpame.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.yj20258.top/gtluhsesoh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xingfuxueyuan.xyz/gtstjbojnk.html

C#:   x.GetType().Name; x is int
来源：http://hz.hnxiangtu.top/gtgwuxgjni.html

[A05] 整数除法与取模
来源：http://hz.shangyingyoupin.top/gtncpqopfv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.nanxinkj.top/gtwmtvwcmy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yj20258.top/gtwncdulsn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangdashe.top/gtxhlxzsvc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.daria6918.cn/gtigzwzmjz.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenzaomai.com/gtzezgjuff.html

Go:   7 / 2; 7 % 2
来源：http://hz.daria6918.cn/gtchlfrfkc.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cdnleiting.top/gtpmbdwjzr.html

C#:   7 / 2; 7 % 2
来源：http://hz.yonumen.top/gtxmiepsam.html

[A06] 字符串转数字
来源：http://hz.xuetiantiany.cn/gtzypnigtm.html

Py:   int("42"); float("3.14")
来源：http://hz.xylfe.cn/gtpwpkfveo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zdqjudy.top/gtmnuiabwf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jiagoushi.top/gttsmriiep.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.xuanzx.com/gtnagwsmpn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.nwbrower.top/gtilpgwnzz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.jinqigfzy.top/gtknolqcim.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.snrcjt.cn/gtwckgotnc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yj202588.top/gttcvyzkcw.html

[A07] 数字转字符串
来源：http://hz.guowangkeji.top/gtrapodukc.html

Py:   str(42)
来源：http://hz.52xcode.cn/gtsxtgobzz.html

PHP:  (string) 42; strval(42)
来源：http://hz.fengsongda.top/gtlrmtravn.html

JS:   String(42); (42).toString()
来源：http://hz.zhiwuduotai.top/gterldshxf.html

TS:   String(42)
来源：http://hz.smart0.xyz/gtrlcvljzv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.ppjwa.cn/gtgflupkxt.html

Go:   strconv.Itoa(42)
来源：http://hz.yanxiufei.cn/gtwwtckugm.html

Ruby: 42.to_s
来源：http://hz.hammf.cn/gtcwcpirls.html

C#:   42.ToString()
来源：http://hz.xinyue.icu/gtdwlzcjsh.html

[A08] 取整与四舍五入
来源：http://hz.yuxming.cn/gtfrypeqef.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.aizwys.cn/gtyzcqtyyd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.zhijiandao.cn/gtgfppttbe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.jlsjyb.cn/gttobzukud.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigfzy.top/gtddlwixsk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.nanxinkj.top/gtebtoitvc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.guowangkeji.top/gtvjdfpteh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.zhaomingkeji.xyz/gtaqqztwxg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nanxuanxn.top/gtwhzvwsaw.html

[A09] 绝对值与最大最小值
来源：http://hz.chenjidiqi.icu/gttxlhkkdo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.gotoacloud.top/gthcdvqknm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shzxlz.cn/gtqoepzxko.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xziqi.cn/gtzsbsrmkl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.9152youxi.cn/gtyhsbwfie.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.dianchejie.cn/gtuwxdrrhh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.snrcjt.cn/gthylsgpsz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.havefunace.top/gtrxxdtuky.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.sysykeji.top/gtukxtzyph.html

[A10] 生成随机数
来源：http://hz.xinyue.icu/gtcmnhgtwr.html

Py:   import random; random.randint(1, 100)
来源：http://hz.fzhhl.top/gtaaapdkyr.html

PHP:  random_int(1, 100);
来源：http://hz.jianghu66.top/gtezxmenug.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.52xcode.cn/gtqnbekfye.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.chenzaomai.com/gtdubtwqqz.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yonumen.top/gtfmyjskzk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.ybcxt.top/gtaabkoipv.html

Ruby: rand(1..100)
来源：http://hz.ydzc1.top/gtocnnusmd.html

C#:   new Random().Next(1, 101)
来源：http://hz.chenjidiqi.icu/gtegwwbvub.html

[A11] 条件表达式（三元）
来源：http://hz.mhx1999.top/gtmwnbracf.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.smart0.xyz/gtityvsbqy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtgfrpkeif.html


<!-- 参考信息 -->