代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.shangyingyoupin.top/gtorzfgrgl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.dashuyun.cn/gtplzvnxai.html

[U84] JS：CommonJS 写法
来源：http://hz.hnxiangtu.top/gtpahibxav.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.zdqjudy.top/gtpwikrgtf.html

[U85] JS：可选链
来源：http://hz.tian-w.cn/gtoewbznor.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtwrrwfpxi.html

[U86] JS：空值合并
来源：http://hz.zhaomingkeji.xyz/gtpzumgwty.html

a ?? b
来源：http://hz.fengsongda.top/gtbvgygqfk.html

[U87] JS：解构默认值
来源：http://hz.ehwqpu.com/gtxlfdlncp.html

const { a = 1, b = 2 } = obj;
来源：http://hz.zhiwuduotai.top/gtfbdvtnju.html

[U88] JS：对象展开合并
来源：http://hz.iojbl.cn/gtlcnjtmih.html

{ ...a, ...b }
来源：http://hz.9152youxi.cn/gtalzuriwm.html

[U89] JS：数组去重
来源：http://hz.zhaomingkeji.xyz/gtdupreuii.html

[...new Set(arr)]
来源：http://hz.wangdashe.top/gtpgmhyrmo.html

[U90] JS：数字数组排序
来源：http://hz.havefunace.top/gtutdeirxd.html

[...arr].sort((a, b) => a - b)
来源：http://hz.ydzc1.top/gtreobasvs.html

[U91] JS：对象键值遍历
来源：http://hz.kuanghao11.cn/gttmzdkmqc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.hnqzz.top/gtjwblsjay.html

[U92] JS：深拷贝
来源：http://hz.sufxvd.cn/gtfrdotxgm.html

structuredClone(obj)
来源：http://hz.xziqi.cn/gtnlixsoyl.html

[U93] JS：模板字符串
来源：http://hz.nwbrower.top/gtjsjmwyua.html

`共 ${n} 条`
来源：http://hz.meibo888.top/gtgcwfmazt.html

[U94] JS：箭头函数
来源：http://hz.ydzc1.top/gtmcxvvxdx.html

const double = x => x * 2;
来源：http://hz.zdqjudy.top/gttxbunksw.html

[U95] JS：Promise 包装
来源：http://hz.yj20258.top/gtfmayxchh.html

new Promise((resolve, reject) => {})
来源：http://hz.hnqzz.top/gtuprymxvp.html

[U96] JS：async/await 与异常
来源：http://hz.jinghuilouyu.cn/gtsasygbob.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtewevqrfx.html

[U97] JS：并发请求
来源：http://hz.zhengqikj.top/gtvsrblyof.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nanxinkj.top/gtrytvatvg.html

[U98] JS：fetch 带 JSON
来源：http://hz.yanxiufei.cn/gtqfbqnjdn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.gzhubu.top/gtjdnozmof.html

[U99] JS：事件监听
来源：http://hz.xziqi.cn/gtcosxtmku.html

el.addEventListener("click", e => {})
来源：http://hz.bjfxy.top/gttxtiqqty.html

[U100] JS：DOM 查询
来源：http://hz.9152youxi.cn/gtanytmlax.html

document.querySelector(".item")
来源：http://hz.hfpthk.cn/gtlzyjifoi.html

[U101] JS：classList 操作
来源：http://hz.chenlongwang.top/gtavbsveds.html

el.classList.toggle("active")
来源：http://hz.52xcode.cn/gtpldmcbyh.html

[U102] JS：本地存储
来源：http://hz.ydzc1.top/gtowxcpqzk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.zdqjudy.top/gthtgmvyud.html

[U103] JS：定时器
来源：http://hz.jqgfzy.top/gttbegrzde.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.aibaodan.cn/gtitvbqzhg.html

[U104] JS：防抖
来源：http://hz.shuidangran.top/gtpwwaxxkw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtmpmgmqfu.html

[U105] JS：节流
来源：http://hz.xuanzx.com/gtkejivlnl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.shanyushiyangkeji.top/gtpfumsolp.html

[U106] JS：日期格式化
来源：http://hz.nanxinkj.top/gtpieavrhw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.yuxming.cn/gtsmsraiiq.html

[U107] JS：数字千分位
来源：http://hz.sufxvd.cn/gtmikechdo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtklpartsk.html

[U108] JS：随机整数
来源：http://hz.yvedp.cn/gtpkopcaxp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.dashuyun.cn/gtaiyeaxnm.html

[U109] JS：数组分组
来源：http://hz.yuxming.cn/gtgihlqxnn.html

Object.groupBy(arr, x => x.type)
来源：http://hz.jqgufenzy.top/gtwocqihfv.html

[U110] JS：数组分块
来源：http://hz.ivvv.top/gtfqpuxnsj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.hnqzz.top/gtmobhriow.html

[U111] JS：对象转 Map
来源：http://hz.ydzc1.top/gtpzyfaqjd.html

new Map(Object.entries(obj))
来源：http://hz.zhoulong.xyz/gtkrmnrfel.html

[U112] JS：字符串补位
来源：http://hz.hywenlv.cn/gttohtgvxn.html

"7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtunzonfip.html

[U113] JS：正则替换全部
来源：http://hz.cucudq.cn/gtifjzqahi.html

s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtmynamzmi.html

[U114] JS：JSON 深比较
来源：http://hz.quarkkingdee.top/gtdvgvxskb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhixingplan.top/gtmssrhpwk.html

[U115] JS：生成 UUID
来源：http://hz.tanke756.top/gtnnqohhol.html

crypto.randomUUID()
来源：http://hz.yuanzhike.top/gtcaxdkfaf.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.0kj1m.cn/gtfsuwcano.html

/** @param {string} name */ function f(name) {}
来源：http://hz.xingfuxueyuan.xyz/gtkfhqorje.html

[U117] JS：单元测试
来源：http://hz.yj20258888.top/gtbmwcvibm.html

npm i -D vitest;  npx vitest
来源：http://hz.cucudq.cn/gtrxqsowko.html

[U118] JS：开发服务器
来源：http://hz.dianchejie.cn/gtufydmnwt.html

npm i -D vite;  npx vite
来源：http://hz.yonumen.top/gtziyxejav.html

[U119] JS：生产构建
来源：http://hz.cashguo.top/gtnlnevfnk.html

npx vite build
来源：http://hz.jyoumei.cn/gtdcgkuyyd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.meibo888.top/gtujwphnzc.html

import.meta.env.VITE_API_URL
来源：http://hz.xingfuxueyuan.xyz/gtkfknsbtm.html

================================================================================
来源：http://hz.iojbl.cn/gtaindvsvi.html

统计汇总
来源：http://hz.fzhhl.top/gtxmkhvrru.html

================================================================================
来源：http://hz.316326.xyz/gthjuuicmu.html

按语言统计（条）：
来源：http://hz.shuidangran.top/gtstgyolzb.html

Python ......... 252
来源：http://hz.jqgufenzy.top/gtskemtiri.html

PHP ............ 252
来源：http://hz.iojbl.cn/gttqfnrgew.html

JavaScript ..... 252
来源：http://hz.chenjidiqi.icu/gteobfyrur.html

TypeScript ..... 212
来源：http://hz.zhiwuduotai.top/gtaklpcwwv.html

Java ........... 212
来源：http://hz.gotoacloud.top/gtmcznabsd.html

Go ............. 212
来源：http://hz.zhijiandao.cn/gtqgeokpzp.html

Ruby ........... 212
来源：http://hz.jinqigufen.top/gtizyhgzfd.html

C# ............. 212
来源：http://hz.zhoulong.xyz/gtdthhpzrd.html

C .............. 30
来源：http://hz.ehwqpu.com/gtprbmdslp.html

C++ ............ 30
来源：http://hz.aibaodan.cn/gtczxxdeql.html

SQL ............ 90
来源：http://hz.aibaodan.cn/gtmglfbdmg.html

Bash ........... 80
来源：http://hz.yongpay.top/gtdqemhluy.html

Kotlin ......... 15
来源：http://hz.jinqigfzy.top/gtlcudqqlu.html

Swift .......... 15
来源：http://hz.ivvv.top/gtnqsuqaus.html

Lua ............ 10
来源：http://hz.mhx1999.top/gtravqgkzl.html

Perl ........... 10
来源：http://hz.xingfuxueyuan.xyz/gtsfopgltu.html

Scala .......... 10
来源：http://hz.havefunace.top/gtondnnpge.html

------------------------------------
来源：http://hz.nanxinkj.top/gtaicnzpgq.html

合计 ........... 2106 条
来源：http://hz.yj20258.top/gtsddbtnai.html

按章节统计：
来源：http://hz.gotoacloud.top/gttddpisxy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.smart0.xyz/gtfxkoaynq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.52xcode.cn/gttclgojns.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.cucudq.cn/gtrqixncln.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.sysykeji.top/gtpvaawskn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.daxiang520.top/gtglwrampo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.shanyushiyangtech.top/gtzlamawux.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.sxryk.cn/gtbkoxdgjg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.cashguo.top/gtbayirqjj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xuetiantiany.cn/gtfgrfeauq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.haohaochexian.top/gtmnmxmyme.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.dianchejie.cn/gtzwnlhjst.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhiwuduotai.top/gtsztavkba.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtpocadcmj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jqgufenzy.top/gtadiftxys.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.daxiang520.top/gtwudslwyw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.kuanghao11.cn/gtrudoavwe.html

Q SQL 专题                              90
来源：http://hz.yuxming.cn/gtfuvbieyk.html

R Bash 专题                             80
来源：http://hz.aizwys.cn/gtdsabmtvd.html

S C / C++ 专题                          60
来源：http://hz.zhiwuduotai.top/gtxoqsubgb.html

T 其他语言补充                          60
来源：http://hz.jqgfzy.top/gtqythulgh.html

U 高频实用片段                         120
来源：http://hz.sufxvd.cn/gtpughgcqv.html

------------------------------------
来源：http://hz.daxiang520.top/gtkfwvmivt.html

合计                                  2106 条
来源：http://hz.dianchejie.cn/gtxskmryio.html

--------------------------------------------------------------------------------
来源：http://hz.jlsjyb.cn/gtviybhdwj.html

使用提醒
来源：http://hz.ivvv.top/gtjgsrhcnx.html

--------------------------------------------------------------------------------
来源：http://hz.quarkkingdee.top/gtnyweaewu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.feifeiyinyue.top/gtpbblhprq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sysykeji.top/gtopmojerb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nwbrower.top/gtvszrertq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yuxming.cn/gtpkiurvhq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fengsongda.top/gtnxttdslz.html

—— 文件结束 ——
来源：http://hz.yuanzhike.top/gtmclxcnaj.html

================================================================================
来源：http://hz.snrcjt.cn/gtdzglyeqv.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.birdmap.top/gtkhbywbht.html

Common Programming Examples Cheat Book
来源：http://hz.hongshengwenyu.top/gtkyzefkgt.html

================================================================================
来源：http://hz.wangdashe.top/gtbllwlalx.html

【收录内容】
来源：http://hz.zycfv.cn/gtrmixqhaq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yj20258888.top/gtcdjxsspw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.gogol.net.cn/gtsqqmwbel.html

SQL · Bash · C · C++
来源：http://hz.shuidangran.top/gturwfqvmt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.wangdashe.top/gtczkwkvdt.html

【使用说明】
来源：http://hz.ppjwa.cn/gtgyfkcjdp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.zhengqikj.top/gtdgoorsdf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenzaomai.com/gtgjutmvmg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.cucudq.cn/gtupjlvycn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.andypj.xyz/gtlfcvytsg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.jiagoushi.top/gtqxqhxiny.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.shuidangran.top/gthfqautvg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.svipenyu.cn/gtqtaggiph.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.ydjk.org.cn/gtgnbsddiv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigufen.top/gttvpzzzem.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.xuetiantiany.cn/gtxyjjbfdu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.vqdsnc.cn/gtkwnervny.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.xuanzx.com/gtdciwigor.html

【文件统计】
来源：http://hz.meibo888.top/gtfrudlxjc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jlsjyb.cn/gtmkdzcqwl.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtmycmfexn.html

目  录
来源：http://hz.gaohongyu789.top/gtppcgoiec.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtwkqocwsr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.zhaomingkeji.xyz/gtbnctapny.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.pengpengdd.cyou/gthrdxkvdg.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.cqqwz.cn/gtyrfkqian.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sufxvd.cn/gtzawethrb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.sysykeji.top/gtooewtlzz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.yonumen.top/gtkuwphivv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.daria6918.cn/gtpzwatyaa.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.smart0.xyz/gtpyupioeu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtfmfkbvwd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinghuilouyu.cn/gtndfsphqw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yonumen.top/gtlqvyrdmm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtveqizwky.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.shangyingyoupin.top/gtpcfrxdvc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhijiandao.cn/gtokaaxcfi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.meibo888.top/gttacfaiul.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtwmtfdigj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxinkj.top/gtpfwulsnz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jlsjyb.cn/gtfexrietw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sweek.top/gtxdjzpsza.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtuakkkmzl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.zhaomingkeji.xyz/gtcwiirngg.html

================================================================================
来源：http://hz.nanxinkj.top/gtznjizmbn.html

A. 基础语法与类型
来源：http://hz.aizwys.cn/gtcmoeyjcn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtcbvzltnb.html

[A01] Hello World
来源：http://hz.quarkkingdee.top/gtvjhpahrf.html

Py:   print("Hello, World!")
来源：http://hz.jyoumei.cn/gtrzrhbduf.html

PHP:  echo "Hello, World!";
来源：http://hz.aizwys.cn/gtjdhgxijd.html

JS:   console.log("Hello, World!");
来源：http://hz.sweek.top/gtjlnmhwfx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.kuanghao11.cn/gteeykpvpt.html

Java: System.out.println("Hello, World!");
来源：http://hz.tianlin.xyz/gthjetlskw.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ivvv.top/gtzcfdlxqy.html

Ruby: puts "Hello, World!"
来源：http://hz.xingfuxueyuan.xyz/gtrhicsdhd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.316326.xyz/gtqswjjgkp.html

[A02] 变量声明与赋值
来源：http://hz.gaohongyu789.top/gtcdbbmqjc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ydjk.org.cn/gtpbqbrxms.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.gotoacloud.top/gtjvuxcomb.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.hammf.cn/gtftfajkft.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhiwuduotai.top/gtcisrcpwa.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.meibo888.top/gttvbrhmgg.html

Go:   name := "Alex"; age := 20
来源：http://hz.jinghuilouyu.cn/gtwjvasdpi.html

Ruby: name = "Alex"; age = 20
来源：http://hz.cashguo.top/gtrqiqvnpg.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.jlsjyb.cn/gtxophospm.html

[A03] 常量定义
来源：http://hz.yvedp.cn/gtdqzttvvy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.tanke756.top/gtznywitpp.html

PHP:  const PI = 3.14159;
来源：http://hz.quarkkingdee.top/gtyploraxb.html

JS:   const PI = 3.14159;
来源：http://hz.sufxvd.cn/gtguiznvqc.html

TS:   const PI: number = 3.14159;
来源：http://hz.hnqzz.top/gtkorvwdqk.html

Java: static final double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtbmklezzz.html

Go:   const PI = 3.14159
来源：http://hz.316326.xyz/gtfoqcuzyb.html

Ruby: PI = 3.14159
来源：http://hz.snrcjt.cn/gtnieqkztc.html

C#:   const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtjazkwosb.html

[A04] 判断变量类型
来源：http://hz.0kj1m.cn/gtzqfczmzk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ybcxt.top/gtdztzxxvp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.yj20258888.top/gtcbkshqus.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.wangshuangyany.cn/gtokuqmbqb.html

TS:   typeof x; x instanceof Date
来源：http://hz.zhaomingkeji.xyz/gtsnxmcubm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.snrcjt.cn/gtfgwqmlzs.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.tanke756.top/gtusxsmxso.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.sweek.top/gtjjdytawm.html

C#:   x.GetType().Name; x is int
来源：http://hz.guowangkeji.top/gtrggjkpgz.html

[A05] 整数除法与取模
来源：http://hz.pengpengdd.cyou/gtejlgpjet.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.gotoacloud.top/gtztruxjay.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.zhongyouzk.top/gtwupocxjw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hfpthk.cn/gtiugaztac.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.fengsongda.top/gtdtgopksx.html

Java: 7 / 2; 7 % 2
来源：http://hz.meibo888.top/gtbozopzku.html

Go:   7 / 2; 7 % 2
来源：http://hz.ydjk.org.cn/gtqnwwoltj.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.daxiang520.top/gtrhthbfbr.html

C#:   7 / 2; 7 % 2
来源：http://hz.tanke756.top/gtgswthneo.html

[A06] 字符串转数字
来源：http://hz.chenzaomai.com/gthicttatu.html

Py:   int("42"); float("3.14")
来源：http://hz.ppjwa.cn/gtefwzllmp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jqgufenzy.top/gtrbeudqvg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.shangyingyoupin.top/gtoarhwgwk.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.cheryme.top/gtwmsvlcjg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.nwbrower.top/gtxykhbrdb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.c1oappe.top/gtfaizxxps.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.316326.xyz/gtaavvnqwc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.ybcxt.top/gtesnslbts.html

[A07] 数字转字符串
来源：http://hz.xuetiantiany.cn/gttymtqavv.html

Py:   str(42)
来源：http://hz.iojbl.cn/gtyvvvswjk.html

PHP:  (string) 42; strval(42)
来源：http://hz.cheryme.top/gtfmoojhwe.html

JS:   String(42); (42).toString()
来源：http://hz.jinqigufen.top/gtchymoulb.html

TS:   String(42)
来源：http://hz.vqdsnc.cn/gtgnixoevc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.hongshengwenyu.top/gtggawqucl.html

Go:   strconv.Itoa(42)
来源：http://hz.yuxming.cn/gtekcvsthx.html

Ruby: 42.to_s
来源：http://hz.xziqi.cn/gtvllhxnis.html

C#:   42.ToString()
来源：http://hz.hysaishi.cn/gtplcmrdlu.html

[A08] 取整与四舍五入
来源：http://hz.sufxvd.cn/gtftnylxlf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.hysaishi.cn/gtuibjnywx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.52xcode.cn/gtoiugopta.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.zhijiandao.cn/gtaaorgrhj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.gaohongyu789.top/gtzrwrmjal.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhongyouzk.top/gtexwagkdt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zycfv.cn/gtzjyhnjbk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.haohaochexian.top/gtbmnpymsh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.zhoulong.xyz/gtsoofjxbn.html

[A09] 绝对值与最大最小值
来源：http://hz.gaohongyu789.top/gtiodcylsf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tianlin.xyz/gtelfkhemq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hfpthk.cn/gttujfslcb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yanxiufei.cn/gtkundlwmc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.guowangkeji.top/gtdfhqvyut.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnqzz.top/gthskwyvtb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jqgufenzy.top/gtfrtkhfrx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.sufxvd.cn/gtowbnmalw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.guowangkeji.top/gthpytweao.html

[A10] 生成随机数
来源：http://hz.nanxinkj.top/gtsouqmice.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hysaishi.cn/gtldtufzgj.html

PHP:  random_int(1, 100);
来源：http://hz.iojbl.cn/gtlgcotumf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtqcjwpanj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shzxlz.cn/gtiamhpref.html

Java: new Random().nextInt(100) + 1
来源：http://hz.yanxiufei.cn/gtmrocxnol.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yuxming.cn/gtxejwfdcj.html

Ruby: rand(1..100)
来源：http://hz.ydjk.org.cn/gtvjutacnc.html

C#:   new Random().Next(1, 101)
来源：http://hz.ppjwa.cn/gtywyhocua.html

[A11] 条件表达式（三元）
来源：http://hz.guowangkeji.top/gtoxsuitgd.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yj20258888.top/gtevpluyrt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.cucudq.cn/gtyeyytael.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.guowangkeji.top/gtovncjzym.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.tanke756.top/gtwdxgsuxg.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.cheryme.top/gtnclosdhv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.xziqi.cn/gtawqaygmv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.xingfuxueyuan.xyz/gtdjceonax.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.guannengcc.top/gtkvhfgdbk.html

[A12] 字符串插值 / 格式化
来源：http://hz.jianghu66.top/gtsjawobop.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.bjfxy.top/gtegykhajs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.hnxiangtu.top/gtjmzdslda.html

JS:   `Hello, ${name}!`
来源：http://hz.sxryk.cn/gtyvxlxfbb.html

TS:   `Hello, ${name}!`
来源：http://hz.tanke756.top/gtgjrzkrec.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.jianghu66.top/gtixnpvjxc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.yuxming.cn/gtvevanzgb.html

Ruby: "Hello, #{name}!"
来源：http://hz.snrcjt.cn/gtxkmsbgtb.html

C#:   $"Hello, {name}!"
来源：http://hz.birdmap.top/gtqmlhizsw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.hnxiangtu.top/gtyvezyvtz.html

Py:   "第一行\n第二行"
来源：http://hz.xuanzx.com/gtmbfwuldh.html

PHP:  "第一行\n第二行"
来源：http://hz.xylfe.cn/gtsgwruhod.html

JS:   "第一行\n第二行"
来源：http://hz.jinyuanbaomall.cn/gtjbvcdchb.html

TS:   "第一行\n第二行"
来源：http://hz.guowangkeji.top/gtuwvhoubz.html

Java: "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtbklzzwfv.html

Go:   "第一行\n第二行"
来源：http://hz.bjfxy.top/gtjpuxzxib.html

Ruby: "第一行\n第二行"
来源：http://hz.ppjwa.cn/gtildwsqft.html

C#:   "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gtddumpurl.html


<!-- 参考信息 -->