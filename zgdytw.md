代发 wailian999

[U81] JS：初始化项目
来源：http://hz.chenjidiqi.icu/gtatrcghoj.html

npm init -y;  npm i express
来源：http://hz.jyoumei.cn/gtbvsmzlqn.html

[U82] JS：package.json 脚本
来源：http://hz.daria6918.cn/gtkfqtilwm.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.shangyingyoupin.top/gtrpvxemgt.html

[U83] JS：ES Module 导入导出
来源：http://hz.zhaomingkeji.xyz/gtnkmtofhl.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.hammf.cn/gtqakqbkot.html

[U84] JS：CommonJS 写法
来源：http://hz.zhixingplan.top/gtsdurcvvw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.nwbrower.top/gtfzhhcozu.html

[U85] JS：可选链
来源：http://hz.yj20258888.top/gtilboclll.html

a?.b?.c
来源：http://hz.xziqi.cn/gtjkbzvsyz.html

[U86] JS：空值合并
来源：http://hz.chenlongwang.top/gtmnuoyeid.html

a ?? b
来源：http://hz.feifeiyinyue.top/gtwgkkskym.html

[U87] JS：解构默认值
来源：http://hz.ivvv.top/gtbpzwkpzx.html

const { a = 1, b = 2 } = obj;
来源：http://hz.cucudq.cn/gtyeyxqplv.html

[U88] JS：对象展开合并
来源：http://hz.ydzc1.top/gtqxyqeplx.html

{ ...a, ...b }
来源：http://hz.mhx1999.top/gtevdmyivl.html

[U89] JS：数组去重
来源：http://hz.feifeiyinyue.top/gtzeuflxul.html

[...new Set(arr)]
来源：http://hz.cdnleiting.top/gtpbovezdi.html

[U90] JS：数字数组排序
来源：http://hz.zhijiandao.cn/gtytxneolg.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tian-w.cn/gtgvhjtqha.html

[U91] JS：对象键值遍历
来源：http://hz.zhiwuduotai.top/gtitwobvjy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangshuangyany.cn/gtnfkaxnlr.html

[U92] JS：深拷贝
来源：http://hz.zhijiandao.cn/gthnrsultd.html

structuredClone(obj)
来源：http://hz.hywenlv.cn/gtaabqwmxz.html

[U93] JS：模板字符串
来源：http://hz.ppjwa.cn/gtrzmemgje.html

`共 ${n} 条`
来源：http://hz.sysykeji.top/gttadwpiha.html

[U94] JS：箭头函数
来源：http://hz.xziqi.cn/gtsxfnhwvf.html

const double = x => x * 2;
来源：http://hz.hammf.cn/gtrdktvnvu.html

[U95] JS：Promise 包装
来源：http://hz.316326.xyz/gtncrllnrr.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gtfzwqvdbk.html

[U96] JS：async/await 与异常
来源：http://hz.yuanzhike.top/gtinzwivhc.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtqvmmqiyh.html

[U97] JS：并发请求
来源：http://hz.gzhubu.top/gtlguesyuy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtmagptuuc.html

[U98] JS：fetch 带 JSON
来源：http://hz.cashguo.top/gtjrllolle.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.vqdsnc.cn/gtnfzdhfsh.html

[U99] JS：事件监听
来源：http://hz.xuanzx.com/gtenrracyx.html

el.addEventListener("click", e => {})
来源：http://hz.yj20258888.top/gttjwzbice.html

[U100] JS：DOM 查询
来源：http://hz.wangshuangyany.cn/gtjbcgfbwc.html

document.querySelector(".item")
来源：http://hz.cdnleiting.top/gtxlgvaera.html

[U101] JS：classList 操作
来源：http://hz.nanxuanxn.top/gttacsoagm.html

el.classList.toggle("active")
来源：http://hz.andypj.xyz/gtsdchlzqm.html

[U102] JS：本地存储
来源：http://hz.jlsjyb.cn/gtkcexnmax.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.wangshuangyany.cn/gtvfngdatt.html

[U103] JS：定时器
来源：http://hz.zycfv.cn/gtqvjwujkt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.xylfe.cn/gtubwlidft.html

[U104] JS：防抖
来源：http://hz.jlsjyb.cn/gtfoqgydmh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.52xcode.cn/gtlvsjxyzn.html

[U105] JS：节流
来源：http://hz.andypj.xyz/gtqugwleof.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.andypj.xyz/gtuifnzefj.html

[U106] JS：日期格式化
来源：http://hz.guowangkeji.top/gtqhcqbvrj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.sxryk.cn/gtmdrnsmrh.html

[U107] JS：数字千分位
来源：http://hz.hnqzz.top/gtyrzyrlcs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.hywenlv.cn/gtwkgamdqr.html

[U108] JS：随机整数
来源：http://hz.zhiwuduotai.top/gtdsyibgaq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.shangyingyoupin.top/gtntefbubi.html

[U109] JS：数组分组
来源：http://hz.316326.xyz/gtqeezpvmp.html

Object.groupBy(arr, x => x.type)
来源：http://hz.iojbl.cn/gthtyksdyd.html

[U110] JS：数组分块
来源：http://hz.redwolf501.top/gtbriqximg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jiagoushi.top/gtbcappmmv.html

[U111] JS：对象转 Map
来源：http://hz.feifeiyinyue.top/gtjvesewzj.html

new Map(Object.entries(obj))
来源：http://hz.hywenlv.cn/gtzvcqyeqb.html

[U112] JS：字符串补位
来源：http://hz.sxryk.cn/gtymcsjegc.html

"7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtotlyscus.html

[U113] JS：正则替换全部
来源：http://hz.chenzaomai.com/gtkpmunwns.html

s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtmabzimia.html

[U114] JS：JSON 深比较
来源：http://hz.yj202588.top/gttllkgudi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.wangshuangyany.cn/gtqpdkxqsr.html

[U115] JS：生成 UUID
来源：http://hz.zhengqikj.top/gtbmpqncqj.html

crypto.randomUUID()
来源：http://hz.redwolf501.top/gtrdetzojw.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jiagoushi.top/gtiwlpwzty.html

/** @param {string} name */ function f(name) {}
来源：http://hz.havefunace.top/gtyryoexwc.html

[U117] JS：单元测试
来源：http://hz.ydzc1.top/gtdvojfafl.html

npm i -D vitest;  npx vitest
来源：http://hz.quarkkingdee.top/gtobrxebbi.html

[U118] JS：开发服务器
来源：http://hz.gzhubu.top/gtndjnyfpn.html

npm i -D vite;  npx vite
来源：http://hz.vqdsnc.cn/gtpkpqljrw.html

[U119] JS：生产构建
来源：http://hz.yonumen.top/gtaqumkssn.html

npx vite build
来源：http://hz.gogol.net.cn/gtsqwnzcqp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.hammf.cn/gtfmljrflx.html

import.meta.env.VITE_API_URL
来源：http://hz.xziqi.cn/gtvjlxxkae.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfpmzklde.html

统计汇总
来源：http://hz.guannengcc.top/gtdvezneod.html

================================================================================
来源：http://hz.ppjwa.cn/gtyqqfzsln.html

按语言统计（条）：
来源：http://hz.jqgfzy.top/gtyrqivliw.html

Python ......... 252
来源：http://hz.yj202588.top/gtdqeucnbj.html

PHP ............ 252
来源：http://hz.ywan-chungtsiang.top/gtovhfjquw.html

JavaScript ..... 252
来源：http://hz.yj20258.top/gtnatzclfq.html

TypeScript ..... 212
来源：http://hz.yj20258888.top/gtmycbbrjh.html

Java ........... 212
来源：http://hz.xuanzx.com/gtiflpgkkv.html

Go ............. 212
来源：http://hz.yongpay.top/gtkztmeudy.html

Ruby ........... 212
来源：http://hz.yj202588.top/gtpyorwkov.html

C# ............. 212
来源：http://hz.sxryk.cn/gtdfqsoell.html

C .............. 30
来源：http://hz.yanxiufei.cn/gtxkqxiqsd.html

C++ ............ 30
来源：http://hz.xuetiantiany.cn/gttampmpuw.html

SQL ............ 90
来源：http://hz.hongshengwenyu.top/gtocusvogw.html

Bash ........... 80
来源：http://hz.zhoulong.xyz/gtdsszwuqs.html

Kotlin ......... 15
来源：http://hz.zhaomingkeji.xyz/gtuuhtwptf.html

Swift .......... 15
来源：http://hz.feifeiyinyue.top/gtgnlwcxbi.html

Lua ............ 10
来源：http://hz.kuanghao11.cn/gtcfnwjxmc.html

Perl ........... 10
来源：http://hz.zhijiandao.cn/gtgyifdlcq.html

Scala .......... 10
来源：http://hz.mhx1999.top/gthajxrkxe.html

------------------------------------
来源：http://hz.zhengqikj.top/gtprsogvad.html

合计 ........... 2106 条
来源：http://hz.tanke756.top/gtaduwopth.html

按章节统计：
来源：http://hz.jianghu66.top/gtegaroply.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.redwolf501.top/gtpzhxcopt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yueranfly.top/gtkiwrqkzt.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.dashuyun.cn/gtvmqbyeyu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhiwuduotai.top/gtpdrwmdab.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jinqigufen.top/gtcrddnjrc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yanxiufei.cn/gtzcpfzhwq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.chenzaomai.com/gtwehmqccb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.nwbrower.top/gtqeqymvwh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nwbrower.top/gtsnidubqz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.andypj.xyz/gtczgvehpa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtqhaazfqf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.xingfuxueyuan.xyz/gtvwzcgxbm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.hfpthk.cn/gtvrydsapv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.shzxlz.cn/gtnsbgmoqm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xuetiantiany.cn/gtrvfzqqba.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.dashuyun.cn/gtnguquuut.html

Q SQL 专题                              90
来源：http://hz.jqgufenzy.top/gtbqmamyzx.html

R Bash 专题                             80
来源：http://hz.gotoacloud.top/gtsvgvnupj.html

S C / C++ 专题                          60
来源：http://hz.fengsongda.top/gtgcvedqbz.html

T 其他语言补充                          60
来源：http://hz.vqdsnc.cn/gtwzlkszlz.html

U 高频实用片段                         120
来源：http://hz.ydzc1.top/gtaispksvv.html

------------------------------------
来源：http://hz.nanxinkj.top/gtvkyahdgb.html

合计                                  2106 条
来源：http://hz.meibo888.top/gtzjtvdwlc.html

--------------------------------------------------------------------------------
来源：http://hz.aibaodan.cn/gtlgldbxls.html

使用提醒
来源：http://hz.cashguo.top/gtwmuysivf.html

--------------------------------------------------------------------------------
来源：http://hz.shuidangran.top/gtzgyjbhqz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.cdnleiting.top/gtnyoiiqmi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.fengsongda.top/gtwseuwrcg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.quarkkingdee.top/gtybjgtpaw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.xziqi.cn/gtglmqszke.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.quarkkingdee.top/gtaeiwtdmp.html

—— 文件结束 ——
来源：http://hz.cdnleiting.top/gtqcnyngeg.html

================================================================================
来源：http://hz.aizwys.cn/gttoexsbvq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.nanxuanxn.top/gtwitnqnmv.html

Common Programming Examples Cheat Book
来源：http://hz.c1oappe.top/gtxpfxjcys.html

================================================================================
来源：http://hz.smart0.xyz/gtfflefvum.html

【收录内容】
来源：http://hz.hnqzz.top/gtyezylgwj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.tianlin.xyz/gtqzqbicjy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.fengsongda.top/gtjcwcbbyz.html

SQL · Bash · C · C++
来源：http://hz.bjfxy.top/gtbrutlzas.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.guowangkeji.top/gthmlasnpo.html

【使用说明】
来源：http://hz.hywenlv.cn/gtstgytzqt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.gzhubu.top/gtqnhocrqa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.wangdashe.top/gtnaugvqii.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.nanxuanxn.top/gtqrojclso.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.ydzc1.top/gtrvmiaxeu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.nwbrower.top/gtpiymrikp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.tianlin.xyz/gtmpsxgxab.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.vqdsnc.cn/gtpyltvdzo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.aibaodan.cn/gtubealytu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.fengsongda.top/gtacbkfoqs.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zycfv.cn/gtkhmcvokw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.haohaochexian.top/gtuwturgqw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.cashguo.top/gtmjfntzjd.html

【文件统计】
来源：http://hz.cucudq.cn/gtwqnwqbuw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jianghu66.top/gtabagomtp.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtacgljbol.html

目  录
来源：http://hz.xuanzx.com/gtchwjyrmh.html

--------------------------------------------------------------------------------
来源：http://hz.cqqwz.cn/gtykjwtmmu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.jqgufenzy.top/gtdeypzoyb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.wangshuangyany.cn/gtwfacwdbv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.hywenlv.cn/gtczyxezll.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yj202588.top/gtpusihlyx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.nanxinkj.top/gtguwrbrzx.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.cucudq.cn/gtffainvpg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.c1oappe.top/gtsngtrmkg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.ivvv.top/gtncvawmzp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.ydjk.org.cn/gtunwsobys.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtspswytlt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.feifeiyinyue.top/gttcyefqot.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtypbwarhb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zhoulong.xyz/gtlzwycdft.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.havefunace.top/gtiktpfthh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.zhaomingkeji.xyz/gtaqtdtkbk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.xinyue.icu/gtryuikbxi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.yuxming.cn/gtbmlxbujh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenlongwang.top/gtzngqgbaa.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xylfe.cn/gtewcsbarj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj20258.top/gtnbudjfor.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtmzsqhcqj.html

================================================================================
来源：http://hz.yj20258.top/gthsicswes.html

A. 基础语法与类型
来源：http://hz.iojbl.cn/gtijlevpzw.html

================================================================================
来源：http://hz.0kj1m.cn/gtywvsugkh.html

[A01] Hello World
来源：http://hz.pycfn.com/gtuxmdzsbq.html

Py:   print("Hello, World!")
来源：http://hz.svipenyu.cn/gtcpaprudy.html

PHP:  echo "Hello, World!";
来源：http://hz.zhengqikj.top/gtlohixklr.html

JS:   console.log("Hello, World!");
来源：http://hz.svipenyu.cn/gtybkfxmnf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.sufxvd.cn/gtzozwvbpt.html

Java: System.out.println("Hello, World!");
来源：http://hz.chenlongwang.top/gtjgpvzfub.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhijiandao.cn/gtitktttwi.html

Ruby: puts "Hello, World!"
来源：http://hz.hnqzz.top/gtkmvcvndy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.9152youxi.cn/gthulbdzrg.html

[A02] 变量声明与赋值
来源：http://hz.shzxlz.cn/gtxfghdmwe.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yvedp.cn/gtepkvgiev.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.ivvv.top/gtelsrcohi.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.ybcxt.top/gtbhaaugsu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.0kj1m.cn/gtlwazeuxd.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.hfpthk.cn/gtjiwemmbe.html

Go:   name := "Alex"; age := 20
来源：http://hz.cqqwz.cn/gtphohrffa.html

Ruby: name = "Alex"; age = 20
来源：http://hz.mhx1999.top/gtvquijrsy.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hnqzz.top/gtkoimhqqd.html

[A03] 常量定义
来源：http://hz.guowangkeji.top/gtknfuukph.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sxryk.cn/gtekjffnbx.html

PHP:  const PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtwbjrbfbi.html

JS:   const PI = 3.14159;
来源：http://hz.fengsongda.top/gtmgkjunjh.html

TS:   const PI: number = 3.14159;
来源：http://hz.gaohongyu789.top/gtqqryskij.html

Java: static final double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtrhvykqbg.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangtech.top/gtgontwtwn.html

Ruby: PI = 3.14159
来源：http://hz.cdnleiting.top/gtdqpvhqay.html

C#:   const double PI = 3.14159;
来源：http://hz.xuetiantiany.cn/gtnselwbof.html

[A04] 判断变量类型
来源：http://hz.dashuyun.cn/gtopnhbdqh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.chenzaomai.com/gtwiwuyppq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.nanxinkj.top/gtuvllwysm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.sufxvd.cn/gtxnoycdce.html

TS:   typeof x; x instanceof Date
来源：http://hz.gogol.net.cn/gtmstwflqj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.zhoulong.xyz/gtamfknvss.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.zhongyouzk.top/gteiqwxxfy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tian-w.cn/gtkndifpvs.html

C#:   x.GetType().Name; x is int
来源：http://hz.cheryme.top/gtdxfbhhet.html

[A05] 整数除法与取模
来源：http://hz.jinghuilouyu.cn/gtigdhvmnr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jianghu66.top/gtlyxpoawe.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.cheryme.top/gtgljlyyoh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hammf.cn/gtzkmafpxg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.wangshuangyany.cn/gtuxsvfpkk.html

Java: 7 / 2; 7 % 2
来源：http://hz.jyoumei.cn/gthbjnntuq.html

Go:   7 / 2; 7 % 2
来源：http://hz.gaohongyu789.top/gtizmrorkq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtzpnvwbna.html

C#:   7 / 2; 7 % 2
来源：http://hz.cheryme.top/gtknwqzrjw.html

[A06] 字符串转数字
来源：http://hz.snrcjt.cn/gtyesrfuro.html

Py:   int("42"); float("3.14")
来源：http://hz.xziqi.cn/gtfgjuboad.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xuetiantiany.cn/gtwajmxhrz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.jinyuanbaomall.cn/gtxlajvjuf.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.daria6918.cn/gtyueeraon.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhengqikj.top/gtskfcprie.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.cheryme.top/gtmvktdcbk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.snrcjt.cn/gtuuoygtra.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.kuanghao11.cn/gtmrqjpzkt.html

[A07] 数字转字符串
来源：http://hz.hfpthk.cn/gtjfyloyhw.html

Py:   str(42)
来源：http://hz.gotoacloud.top/gtpmbthwiu.html

PHP:  (string) 42; strval(42)
来源：http://hz.svipenyu.cn/gtuljigxhr.html

JS:   String(42); (42).toString()
来源：http://hz.hnxiangtu.top/gtqwrbiqey.html

TS:   String(42)
来源：http://hz.xylfe.cn/gtzdhrouon.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.guowangkeji.top/gtbqloczby.html

Go:   strconv.Itoa(42)
来源：http://hz.ydjk.org.cn/gtbcrwcvkv.html

Ruby: 42.to_s
来源：http://hz.sysykeji.top/gtjufzkfqn.html

C#:   42.ToString()
来源：http://hz.yonumen.top/gtfyboohxe.html

[A08] 取整与四舍五入
来源：http://hz.zhiwuduotai.top/gtkatrcsfb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.yvedp.cn/gtwhxqggqh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.shuidangran.top/gtgbsslueo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.yj20258888.top/gtelepaklr.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.meibo888.top/gtofdzqxwj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.fengsongda.top/gtspwppjfo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.hammf.cn/gtgyfpemhm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.mhx1999.top/gtaflzcqmb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.gaohongyu789.top/gtmjsyeqkf.html

[A09] 绝对值与最大最小值
来源：http://hz.ybcxt.top/gtoalltjku.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tian-w.cn/gtsyokahpj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhiwuduotai.top/gtuwazsfbp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.yuanzhike.top/gtaolregpk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxinkj.top/gtqfeciczv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.shanyushiyangtech.top/gthurpowdw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.cucudq.cn/gtjtevbajy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.xziqi.cn/gtejyldhil.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.jinghuilouyu.cn/gtirwddcnb.html

[A10] 生成随机数
来源：http://hz.yueranfly.top/gthhagdhtz.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ywan-chungtsiang.top/gtrtutkubg.html

PHP:  random_int(1, 100);
来源：http://hz.yangfankeji.com/gtvigufeqa.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shzxlz.cn/gtmamkssqk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.shanyushiyangtech.top/gtouhgmbxe.html

Java: new Random().nextInt(100) + 1
来源：http://hz.ivvv.top/gtcilpxtqt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.zycfv.cn/gtmlxeptou.html

Ruby: rand(1..100)
来源：http://hz.hfpthk.cn/gtbhxjigvr.html

C#:   new Random().Next(1, 101)
来源：http://hz.ybcxt.top/gtarnnhjth.html

[A11] 条件表达式（三元）
来源：http://hz.zhoulong.xyz/gtxsjazmiv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.wangshuangyany.cn/gttuuctovw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.sysykeji.top/gtexyxhgrk.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jlsjyb.cn/gtpnmjssxy.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yueranfly.top/gtkgtrlwpb.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.pycfn.com/gtvqjavsmi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.birdmap.top/gtsnazkolg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.sufxvd.cn/gthmysagre.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.fengsongda.top/gtuzguzcfq.html

[A12] 字符串插值 / 格式化
来源：http://hz.yj20258.top/gtoqpbixbe.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.vqdsnc.cn/gtrxpctcrx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sufxvd.cn/gtftphmvrv.html

JS:   `Hello, ${name}!`
来源：http://hz.pycfn.com/gtzviyxvma.html

TS:   `Hello, ${name}!`
来源：http://hz.dashuyun.cn/gteswrhydz.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.xuetiantiany.cn/gtjdgmmapx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.xziqi.cn/gtujenvtuo.html

Ruby: "Hello, #{name}!"
来源：http://hz.316326.xyz/gtwkwtiigg.html

C#:   $"Hello, {name}!"
来源：http://hz.xylfe.cn/gttlczhkbz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.wangshuangyany.cn/gtflldxodo.html

Py:   "第一行\n第二行"
来源：http://hz.gotoacloud.top/gtdklxguze.html

PHP:  "第一行\n第二行"
来源：http://hz.svipenyu.cn/gtuntrorwz.html

JS:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtdancynud.html

TS:   "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtxlppfnob.html


<!-- 参考信息 -->