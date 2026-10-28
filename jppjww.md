代发 wailian999

[U81] JS：初始化项目
来源：http://hz.cheryme.top/gtnelrnrqk.html

npm init -y;  npm i express
来源：http://hz.gaohongyu789.top/gtiobkhlus.html

[U82] JS：package.json 脚本
来源：http://hz.yangfankeji.com/gtdmqugixy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.jinqigfzy.top/gtzhtncveq.html

[U83] JS：ES Module 导入导出
来源：http://hz.cucudq.cn/gtrjqbonyy.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yvedp.cn/gtpvbvfvty.html

[U84] JS：CommonJS 写法
来源：http://hz.pycfn.com/gtglczawkr.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gotoacloud.top/gtksneebai.html

[U85] JS：可选链
来源：http://hz.quarkkingdee.top/gtwoitrlcb.html

a?.b?.c
来源：http://hz.hammf.cn/gtsetzupqn.html

[U86] JS：空值合并
来源：http://hz.shuidangran.top/gtlokriytk.html

a ?? b
来源：http://hz.snrcjt.cn/gthuyxcpfx.html

[U87] JS：解构默认值
来源：http://hz.jinqigfzy.top/gtcmmdxwok.html

const { a = 1, b = 2 } = obj;
来源：http://hz.shuidangran.top/gtxbgqxruc.html

[U88] JS：对象展开合并
来源：http://hz.gotoacloud.top/gtarmbsdcz.html

{ ...a, ...b }
来源：http://hz.hfpthk.cn/gtppxqyobl.html

[U89] JS：数组去重
来源：http://hz.jqgufenzy.top/gtenjdpacm.html

[...new Set(arr)]
来源：http://hz.yj20258.top/gtzvjatgps.html

[U90] JS：数字数组排序
来源：http://hz.gzhubu.top/gtyqskcnrc.html

[...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtezjvbrov.html

[U91] JS：对象键值遍历
来源：http://hz.nwbrower.top/gtskoxxoyq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinyuanbaomall.cn/gttzxntpws.html

[U92] JS：深拷贝
来源：http://hz.daxiang520.top/gtwrxhroat.html

structuredClone(obj)
来源：http://hz.havefunace.top/gtpzcatxpo.html

[U93] JS：模板字符串
来源：http://hz.jqgufenzy.top/gttqgrsnnv.html

`共 ${n} 条`
来源：http://hz.kuanghao11.cn/gttnptnhxi.html

[U94] JS：箭头函数
来源：http://hz.sweek.top/gtzxhmmumd.html

const double = x => x * 2;
来源：http://hz.cqqwz.cn/gtfcqwaffb.html

[U95] JS：Promise 包装
来源：http://hz.shanyushiyangkeji.top/gtwbcgyari.html

new Promise((resolve, reject) => {})
来源：http://hz.vqdsnc.cn/gtgqfiqzcd.html

[U96] JS：async/await 与异常
来源：http://hz.ppjwa.cn/gtpoeuxrce.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtqrfjdmwe.html

[U97] JS：并发请求
来源：http://hz.hfpthk.cn/gthuufhiuy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtsravqsdh.html

[U98] JS：fetch 带 JSON
来源：http://hz.shzxlz.cn/gtwrtazxbf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.tian-w.cn/gtgwwqhnoy.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gthafmbtcx.html

el.addEventListener("click", e => {})
来源：http://hz.gzhubu.top/gtptaxqjlh.html

[U100] JS：DOM 查询
来源：http://hz.ydzc1.top/gtjlnarztx.html

document.querySelector(".item")
来源：http://hz.tianlin.xyz/gtnyuwbbgn.html

[U101] JS：classList 操作
来源：http://hz.hongshengwenyu.top/gtejiydmjx.html

el.classList.toggle("active")
来源：http://hz.havefunace.top/gtyfitubvu.html

[U102] JS：本地存储
来源：http://hz.havefunace.top/gtgauhqfhb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hnxiangtu.top/gtgzpfcbnl.html

[U103] JS：定时器
来源：http://hz.zhengqikj.top/gtyxbexxfp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenlongwang.top/gtfdfjwtsy.html

[U104] JS：防抖
来源：http://hz.jqgufenzy.top/gtnsnccqjq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.yj20258888.top/gtwquaisdy.html

[U105] JS：节流
来源：http://hz.aibaodan.cn/gtpegvaxur.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.cucudq.cn/gtwgilaumk.html

[U106] JS：日期格式化
来源：http://hz.gotoacloud.top/gtadjqzpmm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.fzhhl.top/gtmwclbxiz.html

[U107] JS：数字千分位
来源：http://hz.cdnleiting.top/gtxttmvngc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guowangkeji.top/gtcrqezsbe.html

[U108] JS：随机整数
来源：http://hz.andypj.xyz/gtejdwcaan.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.daxiang520.top/gtbrdqspnh.html

[U109] JS：数组分组
来源：http://hz.52xcode.cn/gthwqzaddu.html

Object.groupBy(arr, x => x.type)
来源：http://hz.smart0.xyz/gtdjbnawgw.html

[U110] JS：数组分块
来源：http://hz.cqqwz.cn/gtyelxclbp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.svipenyu.cn/gtokkmfvcu.html

[U111] JS：对象转 Map
来源：http://hz.gogol.net.cn/gtzjvhggpe.html

new Map(Object.entries(obj))
来源：http://hz.guannengcc.top/gtktztoslo.html

[U112] JS：字符串补位
来源：http://hz.ivvv.top/gthlbiabut.html

"7".padStart(3, "0")
来源：http://hz.hnqzz.top/gtpugeyfpv.html

[U113] JS：正则替换全部
来源：http://hz.yanxiufei.cn/gtexepouuy.html

s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtkrdbcrea.html

[U114] JS：JSON 深比较
来源：http://hz.yangfankeji.com/gtioxexlzf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hongshengwenyu.top/gtnbwectqq.html

[U115] JS：生成 UUID
来源：http://hz.zhoulong.xyz/gtbewvlnng.html

crypto.randomUUID()
来源：http://hz.zhongyouzk.top/gttlhxerdt.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.yj20258888.top/gtpvrsiaob.html

/** @param {string} name */ function f(name) {}
来源：http://hz.9152youxi.cn/gtyeczpdad.html

[U117] JS：单元测试
来源：http://hz.aibaodan.cn/gtmazlrucc.html

npm i -D vitest;  npx vitest
来源：http://hz.jinyuanbaomall.cn/gtdabcbrne.html

[U118] JS：开发服务器
来源：http://hz.tian-w.cn/gtspjzpglr.html

npm i -D vite;  npx vite
来源：http://hz.gotoacloud.top/gtawivuprx.html

[U119] JS：生产构建
来源：http://hz.316326.xyz/gtdnrdgqpx.html

npx vite build
来源：http://hz.nwbrower.top/gtevgsycbp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.ydjk.org.cn/gtrutwhrit.html

import.meta.env.VITE_API_URL
来源：http://hz.tanke756.top/gtrqtaybfv.html

================================================================================
来源：http://hz.chenzaomai.com/gtdgpeopxn.html

统计汇总
来源：http://hz.jyoumei.cn/gtcnobotet.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtiwdsxswa.html

按语言统计（条）：
来源：http://hz.quarkkingdee.top/gtvnctkrdg.html

Python ......... 252
来源：http://hz.nanxuanxn.top/gtijbxkbhx.html

PHP ............ 252
来源：http://hz.zhaomingkeji.xyz/gtvqfwwlqw.html

JavaScript ..... 252
来源：http://hz.xingfuxueyuan.xyz/gtvfqslyle.html

TypeScript ..... 212
来源：http://hz.jianghu66.top/gtsamypjug.html

Java ........... 212
来源：http://hz.hammf.cn/gtukccplsv.html

Go ............. 212
来源：http://hz.jianghu66.top/gtgzmfbubx.html

Ruby ........... 212
来源：http://hz.jyoumei.cn/gtmhunqszp.html

C# ............. 212
来源：http://hz.xuanzx.com/gtlvyifkga.html

C .............. 30
来源：http://hz.guowangkeji.top/gtdbwlvlqr.html

C++ ............ 30
来源：http://hz.smart0.xyz/gtpeqaljim.html

SQL ............ 90
来源：http://hz.ydzc1.top/gtoudbgjqd.html

Bash ........... 80
来源：http://hz.52xcode.cn/gtaguqtbcj.html

Kotlin ......... 15
来源：http://hz.daria6918.cn/gtdygcjzlq.html

Swift .......... 15
来源：http://hz.ywan-chungtsiang.top/gtqpjdluzr.html

Lua ............ 10
来源：http://hz.havefunace.top/gtjrewhxej.html

Perl ........... 10
来源：http://hz.ivvv.top/gthlnwzjzj.html

Scala .......... 10
来源：http://hz.xinyue.icu/gtycpwrpfa.html

------------------------------------
来源：http://hz.nwbrower.top/gtljhvugjq.html

合计 ........... 2106 条
来源：http://hz.zhijiandao.cn/gtchzbqvxr.html

按章节统计：
来源：http://hz.xinyue.icu/gtgffpugvq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.9152youxi.cn/gtufgxymkl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.zhongyouzk.top/gtpurhldxr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtrrlkjhlh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.zhengqikj.top/gtrdwcbjrs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ehwqpu.com/gtvzsetumv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.tianlin.xyz/gtecwxnlza.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jiagoushi.top/gtlnhcyleq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.zhaomingkeji.xyz/gtsqyvwhnl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.ybcxt.top/gterqihpvc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.aibaodan.cn/gttlezdeva.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtptfjbjpb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtdsxjzqzf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zycfv.cn/gtueejtnfy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.xinyue.icu/gtxsgobjjf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xziqi.cn/gtbmeekpsm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtnitlpfxg.html

Q SQL 专题                              90
来源：http://hz.hfpthk.cn/gtgnjjyvue.html

R Bash 专题                             80
来源：http://hz.jinghuilouyu.cn/gtlxuwqwgs.html

S C / C++ 专题                          60
来源：http://hz.fengsongda.top/gtkbrcvkjj.html

T 其他语言补充                          60
来源：http://hz.zhongyouzk.top/gtxjasmspg.html

U 高频实用片段                         120
来源：http://hz.ydjk.org.cn/gtyywelhww.html

------------------------------------
来源：http://hz.hongshengwenyu.top/gtlycqzwri.html

合计                                  2106 条
来源：http://hz.xuetiantiany.cn/gtftjcgjzg.html

--------------------------------------------------------------------------------
来源：http://hz.hywenlv.cn/gttxkbjrhy.html

使用提醒
来源：http://hz.zhiwuduotai.top/gtxfjcwaqy.html

--------------------------------------------------------------------------------
来源：http://hz.sweek.top/gtyjupqxvt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.fengsongda.top/gtyiavovov.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.sufxvd.cn/gtblyqecoc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.jianghu66.top/gtepbnjsof.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.zdqjudy.top/gtrvbkevzn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.tian-w.cn/gtbxguuqch.html

—— 文件结束 ——
来源：http://hz.zhongyouzk.top/gtxzxkiysd.html

================================================================================
来源：http://hz.fengsongda.top/gtpjklemqr.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.hnqzz.top/gtzujxarih.html

Common Programming Examples Cheat Book
来源：http://hz.pycfn.com/gtnypaedws.html

================================================================================
来源：http://hz.yongpay.top/gtdiuyodpx.html

【收录内容】
来源：http://hz.shanyushiyangtech.top/gtrbbwcrau.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.jinghuilouyu.cn/gtjuntxltk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ydjk.org.cn/gtwoeoimhi.html

SQL · Bash · C · C++
来源：http://hz.jinghuilouyu.cn/gtgruaievb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.9152youxi.cn/gtpxxdritb.html

【使用说明】
来源：http://hz.hnqzz.top/gtadbmxgdn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.dianchejie.cn/gtriitusyb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.iojbl.cn/gtfharjltl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.yj202588.top/gtsibqmyeh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.smart0.xyz/gtaklkthyf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.iojbl.cn/gtwuvevizs.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jqgfzy.top/gtgbxiibjt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.snrcjt.cn/gtucpgbkfw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.wangshuangyany.cn/gtomtqbuug.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zhoulong.xyz/gtffmhswpn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shanyushiyangkeji.top/gtnddwgpdr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.jianghu66.top/gtggyvsegj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.shuidangran.top/gthghfennu.html

【文件统计】
来源：http://hz.quarkkingdee.top/gtvgkeroqe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ppjwa.cn/gtntomfxkd.html

--------------------------------------------------------------------------------
来源：http://hz.jinghuilouyu.cn/gtsmervzgf.html

目  录
来源：http://hz.cucudq.cn/gtznasiqwy.html

--------------------------------------------------------------------------------
来源：http://hz.zhixingplan.top/gtrgwpdhwg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.xingfuxueyuan.xyz/gtlcgkkalz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtwzrdauka.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.jinqigfzy.top/gtyghdzerg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.cashguo.top/gtiznscpwq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.svipenyu.cn/gtjwtlzgju.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.nanxinkj.top/gtmyzpbklp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xylfe.cn/gtximeuilz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.pengpengdd.cyou/gtszvhwxsg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.jinqigufen.top/gtcpzyjnyg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.wangshuangyany.cn/gtztisktvt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.birdmap.top/gtgfznnidh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.jyoumei.cn/gtbneobpvu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.316326.xyz/gtzjjtovdd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.guannengcc.top/gtuujlyjfo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.shangyingyoupin.top/gtsqwfiiqq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jinyuanbaomall.cn/gtptxnssvm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.nanxuanxn.top/gtqdxmjgbz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.hnxiangtu.top/gtiyybjapf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.cheryme.top/gtpprgtumt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtusekgted.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.iojbl.cn/gtlpwzkqxu.html

================================================================================
来源：http://hz.jyoumei.cn/gtxeqglzmf.html

A. 基础语法与类型
来源：http://hz.aibaodan.cn/gtcfczznkd.html

================================================================================
来源：http://hz.xuanzx.com/gtgyirowmw.html

[A01] Hello World
来源：http://hz.aizwys.cn/gtmlcdszzo.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtosnfacim.html

PHP:  echo "Hello, World!";
来源：http://hz.wangshuangyany.cn/gtmeixlbgx.html

JS:   console.log("Hello, World!");
来源：http://hz.dianchejie.cn/gtrdvtffzt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.xuetiantiany.cn/gtegkjrrlj.html

Java: System.out.println("Hello, World!");
来源：http://hz.yj202588.top/gtxnryshco.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.shanyushiyangtech.top/gtyolkgbhu.html

Ruby: puts "Hello, World!"
来源：http://hz.meibo888.top/gtgmihfdoh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.hfpthk.cn/gtuoluuvle.html

[A02] 变量声明与赋值
来源：http://hz.redwolf501.top/gtqktvxjhh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.shzxlz.cn/gtovshhuey.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.vqdsnc.cn/gtrbojbdgq.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.wangdashe.top/gtbwjgyvfg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.tian-w.cn/gteygsddrm.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yj20258888.top/gtyojixmtr.html

Go:   name := "Alex"; age := 20
来源：http://hz.yangfankeji.com/gtgekcnetd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.mhx1999.top/gtcvomqqmd.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.nanxinkj.top/gtkjqdirbz.html

[A03] 常量定义
来源：http://hz.sysykeji.top/gtypgtiwuo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.meibo888.top/gtbjxitwdj.html

PHP:  const PI = 3.14159;
来源：http://hz.pycfn.com/gtwfwcbjyq.html

JS:   const PI = 3.14159;
来源：http://hz.nwbrower.top/gtcvqbnkwa.html

TS:   const PI: number = 3.14159;
来源：http://hz.cqqwz.cn/gtxsowdxxk.html

Java: static final double PI = 3.14159;
来源：http://hz.yongpay.top/gtimlhtcxc.html

Go:   const PI = 3.14159
来源：http://hz.ybcxt.top/gtjprxemog.html

Ruby: PI = 3.14159
来源：http://hz.nanxuanxn.top/gtlcejdgic.html

C#:   const double PI = 3.14159;
来源：http://hz.yueranfly.top/gtwkwqpxtq.html

[A04] 判断变量类型
来源：http://hz.xinyue.icu/gtknixruta.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.fengsongda.top/gtcogqmber.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.guannengcc.top/gttgqhsevb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.zhoulong.xyz/gtifncbzqf.html

TS:   typeof x; x instanceof Date
来源：http://hz.yongpay.top/gtouuupanu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.yonumen.top/gtxwwwfyok.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.316326.xyz/gtltpibcay.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.quarkkingdee.top/gtxyislwjr.html

C#:   x.GetType().Name; x is int
来源：http://hz.aibaodan.cn/gtnuyrrxxf.html

[A05] 整数除法与取模
来源：http://hz.bjfxy.top/gtuplbhwri.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.redwolf501.top/gtszqrdtqc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.shanyushiyangtech.top/gtchypligb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.9152youxi.cn/gtnrpjkdlz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.xuetiantiany.cn/gtodjmtteg.html

Java: 7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtvdumvttc.html

Go:   7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtqyzlugfg.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.andypj.xyz/gtcckopjga.html

C#:   7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtujmkhgdj.html

[A06] 字符串转数字
来源：http://hz.yuxming.cn/gtpzvdmrze.html

Py:   int("42"); float("3.14")
来源：http://hz.quarkkingdee.top/gtxdeezain.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.zycfv.cn/gtjjrymfge.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.chenzaomai.com/gtjhmxzjff.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.yuxming.cn/gttxlygrvq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.iojbl.cn/gtrtfmlnht.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.hnqzz.top/gteiotlpef.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.shzxlz.cn/gtfbfjrqyv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.yuanzhike.top/gtlquepdvn.html

[A07] 数字转字符串
来源：http://hz.sweek.top/gtudsjxqbc.html

Py:   str(42)
来源：http://hz.cheryme.top/gtgmeqkkih.html

PHP:  (string) 42; strval(42)
来源：http://hz.dashuyun.cn/gtysrmedld.html

JS:   String(42); (42).toString()
来源：http://hz.zhaomingkeji.xyz/gtmztfnwja.html

TS:   String(42)
来源：http://hz.ybcxt.top/gtakreolyh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sweek.top/gtraecspjh.html

Go:   strconv.Itoa(42)
来源：http://hz.tianlin.xyz/gtlhwayjxq.html

Ruby: 42.to_s
来源：http://hz.yuxming.cn/gtwgubnxou.html

C#:   42.ToString()
来源：http://hz.hammf.cn/gtbhpvryvu.html

[A08] 取整与四舍五入
来源：http://hz.ppjwa.cn/gtnodvjsrk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.jinqigfzy.top/gtnohtnomp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.jianghu66.top/gtqzulqsjv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ppjwa.cn/gttmiucnzq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.dianchejie.cn/gtgcozqlqk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.gzhubu.top/gtdwprczeo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhengqikj.top/gtwltfbgcn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.redwolf501.top/gtrodyucuo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.zhengqikj.top/gtipsgpljs.html

[A09] 绝对值与最大最小值
来源：http://hz.c1oappe.top/gtbmvjvwty.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhijiandao.cn/gttoottpth.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jqgufenzy.top/gtmnnclekm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.tanke756.top/gtsmexodta.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.xziqi.cn/gtphgemryl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.chenlongwang.top/gtrbuuvugn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.snrcjt.cn/gtaoizomvf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.shuidangran.top/gtbffjjuex.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.chenzaomai.com/gtcleicsbt.html

[A10] 生成随机数
来源：http://hz.zhaomingkeji.xyz/gtuyblrsyb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.cheryme.top/gtytroyoec.html

PHP:  random_int(1, 100);
来源：http://hz.wangdashe.top/gtwugagbbd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhongyouzk.top/gtzdaasdfo.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.guowangkeji.top/gtrdalihun.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jiagoushi.top/gtuezpjkfk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.hysaishi.cn/gtbddpvafs.html

Ruby: rand(1..100)
来源：http://hz.guannengcc.top/gturoklzbr.html

C#:   new Random().Next(1, 101)
来源：http://hz.zycfv.cn/gtjmragdek.html

[A11] 条件表达式（三元）
来源：http://hz.xziqi.cn/gtfnoehnwr.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cheryme.top/gtrlvfkvqj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gtprulqcxl.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jyoumei.cn/gtuwetumsp.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtgeakvdth.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.nanxinkj.top/gtlrmvbtgk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.shangyingyoupin.top/gtebigxfyp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.pengpengdd.cyou/gtzcdjnzbo.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.smart0.xyz/gtblatvyjr.html

[A12] 字符串插值 / 格式化
来源：http://hz.yj20258.top/gtykbungjy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.feifeiyinyue.top/gttovjgrvi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.shanyushiyangkeji.top/gtjgsqkocv.html

JS:   `Hello, ${name}!`
来源：http://hz.shangyingyoupin.top/gtiounqewv.html

TS:   `Hello, ${name}!`
来源：http://hz.ybcxt.top/gtokbdwris.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.wangdashe.top/gtrfrxmifx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.cucudq.cn/gtozxxnvsy.html

Ruby: "Hello, #{name}!"
来源：http://hz.guowangkeji.top/gtkrosrxas.html

C#:   $"Hello, {name}!"
来源：http://hz.shanyushiyangkeji.top/gtieuxrbex.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.shangyingyoupin.top/gtqzpgtkim.html

Py:   "第一行\n第二行"
来源：http://hz.zhixingplan.top/gtgptfaxyy.html

PHP:  "第一行\n第二行"
来源：http://hz.316326.xyz/gtkhbpzwzz.html

JS:   "第一行\n第二行"
来源：http://hz.316326.xyz/gtdumckgwe.html

TS:   "第一行\n第二行"
来源：http://hz.hysaishi.cn/gtqpvtnllh.html


<!-- 参考信息 -->