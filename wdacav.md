代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.sufxvd.cn/gtvqrlggmn.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.zhengqikj.top/gtqapvnoaz.html

[U84] JS：CommonJS 写法
来源：http://hz.pengpengdd.cyou/gtteawjsui.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.wangshuangyany.cn/gtwzksasvl.html

[U85] JS：可选链
来源：http://hz.tian-w.cn/gthlergrwt.html

a?.b?.c
来源：http://hz.dianchejie.cn/gtwzzmjbni.html

[U86] JS：空值合并
来源：http://hz.xuetiantiany.cn/gtzhdybkul.html

a ?? b
来源：http://hz.redwolf501.top/gtdrvcgrfj.html

[U87] JS：解构默认值
来源：http://hz.yj20258888.top/gtuajltjdz.html

const { a = 1, b = 2 } = obj;
来源：http://hz.bjfxy.top/gtxabwakut.html

[U88] JS：对象展开合并
来源：http://hz.snrcjt.cn/gtvopmbdnq.html

{ ...a, ...b }
来源：http://hz.xziqi.cn/gtjpvcmwko.html

[U89] JS：数组去重
来源：http://hz.tianlin.xyz/gtonnanjid.html

[...new Set(arr)]
来源：http://hz.chenzaomai.com/gtoluhadga.html

[U90] JS：数字数组排序
来源：http://hz.nanxuanxn.top/gteunxgeed.html

[...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtarskpypm.html

[U91] JS：对象键值遍历
来源：http://hz.shuidangran.top/gtfhgxjotu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.daria6918.cn/gttzdbsfpg.html

[U92] JS：深拷贝
来源：http://hz.sysykeji.top/gtmgkrnxgt.html

structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtbazlugpa.html

[U93] JS：模板字符串
来源：http://hz.hnqzz.top/gteammjrvc.html

`共 ${n} 条`
来源：http://hz.yuanzhike.top/gtvhjzyknp.html

[U94] JS：箭头函数
来源：http://hz.iojbl.cn/gtsjtolcng.html

const double = x => x * 2;
来源：http://hz.yj202588.top/gthwqfwakh.html

[U95] JS：Promise 包装
来源：http://hz.xingfuxueyuan.xyz/gtipwjpjfu.html

new Promise((resolve, reject) => {})
来源：http://hz.xziqi.cn/gtktpbchmd.html

[U96] JS：async/await 与异常
来源：http://hz.ppjwa.cn/gtfpngfvxs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtjnxdrwul.html

[U97] JS：并发请求
来源：http://hz.52xcode.cn/gtyjjtltle.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gthgevyrjj.html

[U98] JS：fetch 带 JSON
来源：http://hz.kuanghao11.cn/gtuncuiesv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.zhongyouzk.top/gtnvxijjcz.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtpnblxytf.html

el.addEventListener("click", e => {})
来源：http://hz.zycfv.cn/gteksnxtqd.html

[U100] JS：DOM 查询
来源：http://hz.xingfuxueyuan.xyz/gtvicbxggj.html

document.querySelector(".item")
来源：http://hz.wangshuangyany.cn/gtinwbsmfw.html

[U101] JS：classList 操作
来源：http://hz.havefunace.top/gtgnajkrhw.html

el.classList.toggle("active")
来源：http://hz.9152youxi.cn/gtxdkcyxwi.html

[U102] JS：本地存储
来源：http://hz.hywenlv.cn/gtywtlgkie.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.svipenyu.cn/gtcbgazsex.html

[U103] JS：定时器
来源：http://hz.nwbrower.top/gtcmuascts.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.sxryk.cn/gtwacapxkn.html

[U104] JS：防抖
来源：http://hz.zhongyouzk.top/gtutquzohh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.jqgfzy.top/gtqztgbnlm.html

[U105] JS：节流
来源：http://hz.jianghu66.top/gtqbkvlzpv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.sysykeji.top/gtctfofjkf.html

[U106] JS：日期格式化
来源：http://hz.haohaochexian.top/gtnbsiqbss.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.nanxuanxn.top/gtwjkxyxgd.html

[U107] JS：数字千分位
来源：http://hz.hnqzz.top/gttkncdoaq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.shzxlz.cn/gtrtzdjijy.html

[U108] JS：随机整数
来源：http://hz.xuetiantiany.cn/gtzohbdckc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258888.top/gtyxikgdqa.html

[U109] JS：数组分组
来源：http://hz.jinghuilouyu.cn/gtrcelwaln.html

Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtlxgytrvt.html

[U110] JS：数组分块
来源：http://hz.ydjk.org.cn/gtmsrbfbxa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jinqigfzy.top/gtiylqjawc.html

[U111] JS：对象转 Map
来源：http://hz.guannengcc.top/gtxjxzxnku.html

new Map(Object.entries(obj))
来源：http://hz.xziqi.cn/gtvyfktptf.html

[U112] JS：字符串补位
来源：http://hz.zhijiandao.cn/gtdqxefwsc.html

"7".padStart(3, "0")
来源：http://hz.yonumen.top/gtpakpmvsi.html

[U113] JS：正则替换全部
来源：http://hz.ybcxt.top/gtcqnoftmj.html

s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtrwiyvpln.html

[U114] JS：JSON 深比较
来源：http://hz.jiagoushi.top/gtbnojiqeb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.zhiwuduotai.top/gtuecvnwiy.html

[U115] JS：生成 UUID
来源：http://hz.zhoulong.xyz/gtanjhqijo.html

crypto.randomUUID()
来源：http://hz.jyoumei.cn/gtbkkkvmon.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.iojbl.cn/gthyalsysr.html

/** @param {string} name */ function f(name) {}
来源：http://hz.svipenyu.cn/gtelfrfqbd.html

[U117] JS：单元测试
来源：http://hz.jinyuanbaomall.cn/gtyohvvpyq.html

npm i -D vitest;  npx vitest
来源：http://hz.hnxiangtu.top/gttzwosdhf.html

[U118] JS：开发服务器
来源：http://hz.yvedp.cn/gtdzzqukdp.html

npm i -D vite;  npx vite
来源：http://hz.birdmap.top/gtdbtnwuqh.html

[U119] JS：生产构建
来源：http://hz.meibo888.top/gtoxhgedxr.html

npx vite build
来源：http://hz.jyoumei.cn/gttnbdozrb.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.vqdsnc.cn/gtcmtuweux.html

import.meta.env.VITE_API_URL
来源：http://hz.redwolf501.top/gtjvzpxujs.html

================================================================================
来源：http://hz.andypj.xyz/gtrtiqkknu.html

统计汇总
来源：http://hz.jqgfzy.top/gtzobijiyv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtabhvlhdy.html

按语言统计（条）：
来源：http://hz.shzxlz.cn/gtoddmebyu.html

Python ......... 252
来源：http://hz.jinghuilouyu.cn/gtubwfrinl.html

PHP ............ 252
来源：http://hz.dianchejie.cn/gtfwvxhwlj.html

JavaScript ..... 252
来源：http://hz.jiagoushi.top/gtrnudsmmu.html

TypeScript ..... 212
来源：http://hz.gogol.net.cn/gtnhdbsdce.html

Java ........... 212
来源：http://hz.fzhhl.top/gtwqvjrssk.html

Go ............. 212
来源：http://hz.redwolf501.top/gtmgzwwaon.html

Ruby ........... 212
来源：http://hz.aibaodan.cn/gtzmiesdhm.html

C# ............. 212
来源：http://hz.zdqjudy.top/gtehbthuhq.html

C .............. 30
来源：http://hz.chenjidiqi.icu/gtvoxhuhll.html

C++ ............ 30
来源：http://hz.sweek.top/gtpubsyjzz.html

SQL ............ 90
来源：http://hz.ivvv.top/gtvkbcwyno.html

Bash ........... 80
来源：http://hz.jinqigfzy.top/gtqefvdcba.html

Kotlin ......... 15
来源：http://hz.bjfxy.top/gtopcglndf.html

Swift .......... 15
来源：http://hz.fengsongda.top/gtoygjkwsz.html

Lua ............ 10
来源：http://hz.zhiwuduotai.top/gtmdibbpeq.html

Perl ........... 10
来源：http://hz.yj20258888.top/gtgwrbkinl.html

Scala .......... 10
来源：http://hz.birdmap.top/gtsfbaidun.html

------------------------------------
来源：http://hz.shanyushiyangkeji.top/gtjtlyznoq.html

合计 ........... 2106 条
来源：http://hz.ywan-chungtsiang.top/gtcpqrtmmr.html

按章节统计：
来源：http://hz.gaohongyu789.top/gtxkngpgfx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.birdmap.top/gtcjgmfxgl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.dianchejie.cn/gtrmtacbgs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.iojbl.cn/gtymboqsqo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhaomingkeji.xyz/gtaqtmkmwv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.0kj1m.cn/gtviefexpf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.svipenyu.cn/gtwioskdau.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jqgfzy.top/gtzsrmjatb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ppjwa.cn/gtvvyguqmo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xziqi.cn/gthnhlkcea.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.cucudq.cn/gtzbdkidzj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtzluvlhpr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.jinqigfzy.top/gtwlakmcro.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtpnbcbvpk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gtwniaqfpf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.jlsjyb.cn/gtuhcssepx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.wangdashe.top/gtfmpwwvvv.html

Q SQL 专题                              90
来源：http://hz.ppjwa.cn/gtopvobbdg.html

R Bash 专题                             80
来源：http://hz.ppjwa.cn/gtgcslxsze.html

S C / C++ 专题                          60
来源：http://hz.pengpengdd.cyou/gtfbyhiuzy.html

T 其他语言补充                          60
来源：http://hz.sufxvd.cn/gtpuuicagc.html

U 高频实用片段                         120
来源：http://hz.hammf.cn/gtivnamzwq.html

------------------------------------
来源：http://hz.ydzc1.top/gtlecvlvdo.html

合计                                  2106 条
来源：http://hz.yj20258888.top/gtvvrkjbud.html

--------------------------------------------------------------------------------
来源：http://hz.daxiang520.top/gtsbshidws.html

使用提醒
来源：http://hz.shanyushiyangtech.top/gtoqmnskby.html

--------------------------------------------------------------------------------
来源：http://hz.9152youxi.cn/gthmdgsfih.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.chenzaomai.com/gtzehcpewg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.jinqigfzy.top/gtagdblkal.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jqgufenzy.top/gtkrwkjpaa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.birdmap.top/gtztjghfth.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.fengsongda.top/gtglmnqami.html

—— 文件结束 ——
来源：http://hz.nanxinkj.top/gtwpgvgqfu.html

================================================================================
来源：http://hz.cqqwz.cn/gtnusvcsct.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hysaishi.cn/gtllysjjvn.html

Common Programming Examples Cheat Book
来源：http://hz.pycfn.com/gtrealalcq.html

================================================================================
来源：http://hz.cheryme.top/gtuavigrkm.html

【收录内容】
来源：http://hz.zhixingplan.top/gtviflwpgr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.hongshengwenyu.top/gthnqrwirm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.svipenyu.cn/gtqxotnzam.html

SQL · Bash · C · C++
来源：http://hz.fzhhl.top/gtpxzveyql.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.cqqwz.cn/gthqcdipmg.html

【使用说明】
来源：http://hz.yueranfly.top/gtxndbjhrr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.shuidangran.top/gtkjsnyiea.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.hysaishi.cn/gteejfjxgp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ydzc1.top/gtzcxynvjb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.cdnleiting.top/gtfocnrzyg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.wangdashe.top/gtqhqpjvlf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ppjwa.cn/gtznbohkmi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.snrcjt.cn/gtarsmgzuv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.9152youxi.cn/gtjfmvouuq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.daxiang520.top/gtwbvhbsnt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.yuxming.cn/gtwbzjerkf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.sufxvd.cn/gtrktuvgrp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.tanke756.top/gtrrbqqlll.html

【文件统计】
来源：http://hz.shanyushiyangkeji.top/gtdrfwivii.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.jinghuilouyu.cn/gtouivnlwf.html

--------------------------------------------------------------------------------
来源：http://hz.feifeiyinyue.top/gtuerbnezx.html

目  录
来源：http://hz.sweek.top/gtnckprxms.html

--------------------------------------------------------------------------------
来源：http://hz.yueranfly.top/gtknwaiaqc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.yj20258888.top/gtcrubdash.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtffrslpuj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenjidiqi.icu/gtciktldby.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.birdmap.top/gtywlaldhk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.pycfn.com/gtbcjrspej.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.kuanghao11.cn/gtlxwapznl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.shangyingyoupin.top/gtdgowylxp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.sxryk.cn/gtwtumuhru.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.xziqi.cn/gtwwbgmqde.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.jinqigufen.top/gtzzpvntyw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.sxryk.cn/gtcijiltcy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtvkkmzuyt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnxiangtu.top/gtqrawmrae.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.0kj1m.cn/gtzzbvmppc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shanyushiyangtech.top/gtcisgcqre.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.chenzaomai.com/gtqftyyqru.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.0kj1m.cn/gtfowaxuhf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.smart0.xyz/gtzuvmhivi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.hongshengwenyu.top/gtqhzoyexm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shanyushiyangkeji.top/gtqkefnnat.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hnqzz.top/gtunwrqupz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrgwbohlj.html

A. 基础语法与类型
来源：http://hz.52xcode.cn/gtrwzclpuk.html

================================================================================
来源：http://hz.snrcjt.cn/gtlfmscxpp.html

[A01] Hello World
来源：http://hz.dianchejie.cn/gtyxcopmjm.html

Py:   print("Hello, World!")
来源：http://hz.yj202588.top/gtpvxbijbz.html

PHP:  echo "Hello, World!";
来源：http://hz.bjfxy.top/gtfwtzvnxe.html

JS:   console.log("Hello, World!");
来源：http://hz.mhx1999.top/gtsvhqplyg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.aibaodan.cn/gtisylqqry.html

Java: System.out.println("Hello, World!");
来源：http://hz.hammf.cn/gthtnwocxq.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhongyouzk.top/gtcsbfcuuq.html

Ruby: puts "Hello, World!"
来源：http://hz.daria6918.cn/gtnjupngru.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.tianlin.xyz/gthnvgmcxe.html

[A02] 变量声明与赋值
来源：http://hz.daxiang520.top/gtunaubbno.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shanyushiyangkeji.top/gtutaykzms.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.aizwys.cn/gthdmoalzw.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.chenlongwang.top/gtuezahrpf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.xuanzx.com/gtgmdvpsyj.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.zhoulong.xyz/gtsznplkos.html

Go:   name := "Alex"; age := 20
来源：http://hz.kuanghao11.cn/gtypzuclzx.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ybcxt.top/gtghrhgsww.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.bjfxy.top/gttbafmzqu.html

[A03] 常量定义
来源：http://hz.havefunace.top/gtcntmqjap.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hysaishi.cn/gteupstufq.html

PHP:  const PI = 3.14159;
来源：http://hz.hnqzz.top/gtnjwnnkcd.html

JS:   const PI = 3.14159;
来源：http://hz.yj20258888.top/gtgexoltop.html

TS:   const PI: number = 3.14159;
来源：http://hz.wangshuangyany.cn/gtscatkuyh.html

Java: static final double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtetgeplje.html

Go:   const PI = 3.14159
来源：http://hz.nanxuanxn.top/gteidfqwld.html

Ruby: PI = 3.14159
来源：http://hz.svipenyu.cn/gtrdqdobfs.html

C#:   const double PI = 3.14159;
来源：http://hz.dianchejie.cn/gtydqmcyvm.html

[A04] 判断变量类型
来源：http://hz.yueranfly.top/gtfxojtvga.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.gotoacloud.top/gtxavzpjtb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jlsjyb.cn/gtyxrpzrkf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hnqzz.top/gtjdsddcym.html

TS:   typeof x; x instanceof Date
来源：http://hz.tian-w.cn/gtocrzccqk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ywan-chungtsiang.top/gtxuwbders.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.shzxlz.cn/gtphyxuqki.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.52xcode.cn/gtfsliyaum.html

C#:   x.GetType().Name; x is int
来源：http://hz.daxiang520.top/gtdfkxbpnw.html

[A05] 整数除法与取模
来源：http://hz.pycfn.com/gtrmathjeg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.sysykeji.top/gtcplapjee.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yuxming.cn/gtwtigbqdq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.ydzc1.top/gttrpktbil.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.gogol.net.cn/gtlevzhyvv.html

Java: 7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtaghpxrlp.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhiwuduotai.top/gtirxzvswq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ybcxt.top/gtcrtcxmyy.html

C#:   7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtbgeumcmw.html

[A06] 字符串转数字
来源：http://hz.tianlin.xyz/gtsniwqckv.html

Py:   int("42"); float("3.14")
来源：http://hz.wangshuangyany.cn/gttfhmdmmn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.quarkkingdee.top/gtvkjanqos.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.chenjidiqi.icu/gtgnjtqvvx.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.redwolf501.top/gttwccmyur.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.jqgufenzy.top/gtohdlbkya.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.redwolf501.top/gtxwjvremk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.meibo888.top/gtwemzfpfe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yangfankeji.com/gtigvxbqul.html

[A07] 数字转字符串
来源：http://hz.havefunace.top/gtowgmnvgz.html

Py:   str(42)
来源：http://hz.xuetiantiany.cn/gtiywxnhsa.html

PHP:  (string) 42; strval(42)
来源：http://hz.hnqzz.top/gtsmyiffdl.html

JS:   String(42); (42).toString()
来源：http://hz.meibo888.top/gtchjqfoln.html

TS:   String(42)
来源：http://hz.316326.xyz/gtbjghznuh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yuanzhike.top/gtnyubrioh.html

Go:   strconv.Itoa(42)
来源：http://hz.gaohongyu789.top/gtpcepoulk.html

Ruby: 42.to_s
来源：http://hz.dashuyun.cn/gtztowyxok.html

C#:   42.ToString()
来源：http://hz.shanyushiyangkeji.top/gtcjbnnldy.html

[A08] 取整与四舍五入
来源：http://hz.tanke756.top/gtxnxsrfpg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.haohaochexian.top/gtxshfnncw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hongshengwenyu.top/gtiziunyyj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.shanyushiyangtech.top/gtbhfvltik.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.9152youxi.cn/gtlpbnohxk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.wangdashe.top/gtivewawkk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jinyuanbaomall.cn/gtyvpheaiw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.sxryk.cn/gtlnxsevim.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.cashguo.top/gtlsojpxmv.html

[A09] 绝对值与最大最小值
来源：http://hz.fzhhl.top/gtuorqgihr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.redwolf501.top/gtowapehmw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhiwuduotai.top/gtmhyuaqju.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.smart0.xyz/gtovjqrrme.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.yongpay.top/gtgomlklso.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hammf.cn/gtqbfytvds.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.zhiwuduotai.top/gtqrkwczzt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.yvedp.cn/gtvixkvvnv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.iojbl.cn/gtkpbghaga.html

[A10] 生成随机数
来源：http://hz.wangdashe.top/gtcpwiqtkl.html

Py:   import random; random.randint(1, 100)
来源：http://hz.ppjwa.cn/gtzuhmogyr.html

PHP:  random_int(1, 100);
来源：http://hz.yvedp.cn/gtcmrmzcdw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.pengpengdd.cyou/gtvybpfbvu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.wangdashe.top/gtfbnwlhkc.html

Java: new Random().nextInt(100) + 1
来源：http://hz.zhaomingkeji.xyz/gtlhezqwbr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.pengpengdd.cyou/gthksvvtiu.html

Ruby: rand(1..100)
来源：http://hz.shangyingyoupin.top/gthnxfosvf.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhixingplan.top/gtdrjuaijy.html

[A11] 条件表达式（三元）
来源：http://hz.yongpay.top/gtnugjhojv.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.hywenlv.cn/gtnjcamcdg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.chenjidiqi.icu/gtisucycrd.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtlyqovvfb.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtsrepihos.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtppddxjgb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.chenlongwang.top/gtgptqyiul.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.dianchejie.cn/gtzyaxqxdg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.andypj.xyz/gtmphyzwav.html

[A12] 字符串插值 / 格式化
来源：http://hz.xuanzx.com/gtdpfkxbxm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.shuidangran.top/gtvzfvdybn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.zhijiandao.cn/gtxynzdtjv.html

JS:   `Hello, ${name}!`
来源：http://hz.chenzaomai.com/gthatjgigz.html

TS:   `Hello, ${name}!`
来源：http://hz.xinyue.icu/gtlbnndzvq.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.xinyue.icu/gtqmznljsw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.daxiang520.top/gtlixtluie.html

Ruby: "Hello, #{name}!"
来源：http://hz.yueranfly.top/gtnomeawal.html

C#:   $"Hello, {name}!"
来源：http://hz.ivvv.top/gtheiviegw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.andypj.xyz/gtbcojwtmu.html

Py:   "第一行\n第二行"
来源：http://hz.chenjidiqi.icu/gtzbwyyphx.html

PHP:  "第一行\n第二行"
来源：http://hz.jinyuanbaomall.cn/gtskfxadlx.html

JS:   "第一行\n第二行"
来源：http://hz.ehwqpu.com/gtfpqmiwjt.html

TS:   "第一行\n第二行"
来源：http://hz.jlsjyb.cn/gtfqvykkwa.html

Java: "第一行\n第二行"
来源：http://hz.yj202588.top/gtgjablwrm.html

Go:   "第一行\n第二行"
来源：http://hz.ppjwa.cn/gtikgcuajw.html

Ruby: "第一行\n第二行"
来源：http://hz.kuanghao11.cn/gtbjpuxqky.html

C#:   "第一行\n第二行"
来源：http://hz.cqqwz.cn/gtqflmgspc.html


<!-- 参考信息 -->