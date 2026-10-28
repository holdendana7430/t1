代发 wailian999

[U81] JS：初始化项目
来源：http://hz.shanyushiyangtech.top/gtpfflprvw.html

npm init -y;  npm i express
来源：http://hz.chenzaomai.com/gtfrleohos.html

[U82] JS：package.json 脚本
来源：http://hz.kuanghao11.cn/gttvgwjuly.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.hysaishi.cn/gtaxopusye.html

[U83] JS：ES Module 导入导出
来源：http://hz.andypj.xyz/gtzsdwhwng.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.shanyushiyangtech.top/gtlfohyvwy.html

[U84] JS：CommonJS 写法
来源：http://hz.shanyushiyangtech.top/gtgvrhjshu.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.c1oappe.top/gtogujmcbr.html

[U85] JS：可选链
来源：http://hz.yongpay.top/gtltlrncao.html

a?.b?.c
来源：http://hz.shanyushiyangkeji.top/gtnmdopnfz.html

[U86] JS：空值合并
来源：http://hz.sweek.top/gtwfruqerr.html

a ?? b
来源：http://hz.tian-w.cn/gtnxmrttiz.html

[U87] JS：解构默认值
来源：http://hz.gogol.net.cn/gtvxtwqrsa.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sweek.top/gtldzuljav.html

[U88] JS：对象展开合并
来源：http://hz.tian-w.cn/gtzndydmnw.html

{ ...a, ...b }
来源：http://hz.chenzaomai.com/gtqyyjkvwc.html

[U89] JS：数组去重
来源：http://hz.xuetiantiany.cn/gthzskrpzt.html

[...new Set(arr)]
来源：http://hz.fzhhl.top/gtranlxwma.html

[U90] JS：数字数组排序
来源：http://hz.yuxming.cn/gtvwjvvcuq.html

[...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtqdqwfsmy.html

[U91] JS：对象键值遍历
来源：http://hz.9152youxi.cn/gtrxgfpsgb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.jinghuilouyu.cn/gtqnjyyfhc.html

[U92] JS：深拷贝
来源：http://hz.daria6918.cn/gtntzckltb.html

structuredClone(obj)
来源：http://hz.nwbrower.top/gtximapcku.html

[U93] JS：模板字符串
来源：http://hz.iojbl.cn/gtseewucgv.html

`共 ${n} 条`
来源：http://hz.jinqigfzy.top/gtekdscywg.html

[U94] JS：箭头函数
来源：http://hz.hnxiangtu.top/gtdbfuzhoe.html

const double = x => x * 2;
来源：http://hz.havefunace.top/gtxjkwdyjj.html

[U95] JS：Promise 包装
来源：http://hz.yj20258.top/gtkqrweswh.html

new Promise((resolve, reject) => {})
来源：http://hz.vqdsnc.cn/gtozmgbmcw.html

[U96] JS：async/await 与异常
来源：http://hz.snrcjt.cn/gtyzigxrje.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtycprtccn.html

[U97] JS：并发请求
来源：http://hz.hammf.cn/gtrpplyfks.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gthgrktvsz.html

[U98] JS：fetch 带 JSON
来源：http://hz.quarkkingdee.top/gtekhzngtn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.svipenyu.cn/gtcohajmar.html

[U99] JS：事件监听
来源：http://hz.jinqigufen.top/gtfqgewejo.html

el.addEventListener("click", e => {})
来源：http://hz.jlsjyb.cn/gtgrrhfuzg.html

[U100] JS：DOM 查询
来源：http://hz.zhixingplan.top/gtdwqqvmmw.html

document.querySelector(".item")
来源：http://hz.jiagoushi.top/gtacwpsafn.html

[U101] JS：classList 操作
来源：http://hz.hysaishi.cn/gthymxjkxf.html

el.classList.toggle("active")
来源：http://hz.yanxiufei.cn/gtzzqjijab.html

[U102] JS：本地存储
来源：http://hz.yuxming.cn/gtgbixkppl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.hywenlv.cn/gthncsbqdk.html

[U103] JS：定时器
来源：http://hz.hysaishi.cn/gtunuhxkuc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.cdnleiting.top/gtsfgqhiwr.html

[U104] JS：防抖
来源：http://hz.yuxming.cn/gtrqquesqy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.iojbl.cn/gttcaqcype.html

[U105] JS：节流
来源：http://hz.svipenyu.cn/gtyajpzamw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.zhijiandao.cn/gtqqwtoprw.html

[U106] JS：日期格式化
来源：http://hz.gotoacloud.top/gthaphefmz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xinyue.icu/gtnerjcvip.html

[U107] JS：数字千分位
来源：http://hz.hywenlv.cn/gtgbppvgdi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.jianghu66.top/gtvrxoxdoo.html

[U108] JS：随机整数
来源：http://hz.jinghuilouyu.cn/gtbanwrtuz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.guannengcc.top/gtpciaupms.html

[U109] JS：数组分组
来源：http://hz.gogol.net.cn/gtpihkswnj.html

Object.groupBy(arr, x => x.type)
来源：http://hz.snrcjt.cn/gtqyoljejy.html

[U110] JS：数组分块
来源：http://hz.cdnleiting.top/gtlpyzgfrw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.jlsjyb.cn/gtmkizfdki.html

[U111] JS：对象转 Map
来源：http://hz.yanxiufei.cn/gtmebeyzdn.html

new Map(Object.entries(obj))
来源：http://hz.guowangkeji.top/gtrgidmuvi.html

[U112] JS：字符串补位
来源：http://hz.meibo888.top/gtzeikgebw.html

"7".padStart(3, "0")
来源：http://hz.birdmap.top/gtgvnlchvm.html

[U113] JS：正则替换全部
来源：http://hz.hnxiangtu.top/gtulaliqof.html

s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtmpzspjri.html

[U114] JS：JSON 深比较
来源：http://hz.jinghuilouyu.cn/gtxvhypxqz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigufen.top/gtpuqolyti.html

[U115] JS：生成 UUID
来源：http://hz.nanxuanxn.top/gthhgrncwu.html

crypto.randomUUID()
来源：http://hz.ydzc1.top/gtwnlwgtvr.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.c1oappe.top/gtqvzsqazk.html

/** @param {string} name */ function f(name) {}
来源：http://hz.nanxuanxn.top/gtfvfwuuhi.html

[U117] JS：单元测试
来源：http://hz.jiagoushi.top/gtjqkynxfj.html

npm i -D vitest;  npx vitest
来源：http://hz.hysaishi.cn/gtvawlexxo.html

[U118] JS：开发服务器
来源：http://hz.nanxinkj.top/gtalojutvj.html

npm i -D vite;  npx vite
来源：http://hz.smart0.xyz/gtwmfbpemv.html

[U119] JS：生产构建
来源：http://hz.yj20258888.top/gtfivzjyst.html

npx vite build
来源：http://hz.zycfv.cn/gtmjbdchib.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.yangfankeji.com/gtbgyoswrd.html

import.meta.env.VITE_API_URL
来源：http://hz.0kj1m.cn/gtoaarkyzj.html

================================================================================
来源：http://hz.dashuyun.cn/gtvjztxith.html

统计汇总
来源：http://hz.dianchejie.cn/gtnghunduv.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmnrdgzit.html

按语言统计（条）：
来源：http://hz.jlsjyb.cn/gtyambmmrt.html

Python ......... 252
来源：http://hz.yj20258888.top/gtjcsiujfn.html

PHP ............ 252
来源：http://hz.daria6918.cn/gtztgbemyn.html

JavaScript ..... 252
来源：http://hz.xuanzx.com/gtyjnujwrj.html

TypeScript ..... 212
来源：http://hz.tianlin.xyz/gtkazegqpj.html

Java ........... 212
来源：http://hz.tianlin.xyz/gthrjddebq.html

Go ............. 212
来源：http://hz.haohaochexian.top/gtfbhbywwp.html

Ruby ........... 212
来源：http://hz.xinyue.icu/gtrhgzebtu.html

C# ............. 212
来源：http://hz.ywan-chungtsiang.top/gttxwnousq.html

C .............. 30
来源：http://hz.chenjidiqi.icu/gtwldroedv.html

C++ ............ 30
来源：http://hz.nanxuanxn.top/gttklhubzi.html

SQL ............ 90
来源：http://hz.gzhubu.top/gtpkzwetbx.html

Bash ........... 80
来源：http://hz.hfpthk.cn/gtdacvufny.html

Kotlin ......... 15
来源：http://hz.havefunace.top/gthuanvrks.html

Swift .......... 15
来源：http://hz.dianchejie.cn/gtvefvbymt.html

Lua ............ 10
来源：http://hz.ydzc1.top/gtmycptgof.html

Perl ........... 10
来源：http://hz.aibaodan.cn/gthhiatqje.html

Scala .......... 10
来源：http://hz.ppjwa.cn/gthsipenyx.html

------------------------------------
来源：http://hz.xziqi.cn/gtfucgqbdn.html

合计 ........... 2106 条
来源：http://hz.cheryme.top/gtwulqriia.html

按章节统计：
来源：http://hz.fzhhl.top/gtbdarahng.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.xuanzx.com/gtzzyjrdlv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.pengpengdd.cyou/gtotfvlana.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.sweek.top/gtyklvzrtm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtexopfqbq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.ywan-chungtsiang.top/gtkuxorgdp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuanzhike.top/gtldbntarv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.shzxlz.cn/gtogfifpco.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.jiagoushi.top/gtjezqfzzw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.xinyue.icu/gtuqklmikk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.gotoacloud.top/gtdecqynaa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.gaohongyu789.top/gtnjoegeyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yangfankeji.com/gtmrgyzmpf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtdzwlobur.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.dianchejie.cn/gtqchbzthq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xylfe.cn/gtttkiqgsr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gttwvgvswa.html

Q SQL 专题                              90
来源：http://hz.redwolf501.top/gtopqtrqec.html

R Bash 专题                             80
来源：http://hz.hammf.cn/gtuimekuzr.html

S C / C++ 专题                          60
来源：http://hz.yuanzhike.top/gtgaurkvnc.html

T 其他语言补充                          60
来源：http://hz.jlsjyb.cn/gtffweacvh.html

U 高频实用片段                         120
来源：http://hz.cheryme.top/gtcpcgbftb.html

------------------------------------
来源：http://hz.52xcode.cn/gtrcmnqdbg.html

合计                                  2106 条
来源：http://hz.yueranfly.top/gttbelktiq.html

--------------------------------------------------------------------------------
来源：http://hz.hongshengwenyu.top/gtwdzkaoil.html

使用提醒
来源：http://hz.redwolf501.top/gtifbklkse.html

--------------------------------------------------------------------------------
来源：http://hz.52xcode.cn/gtecryxgcl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.dashuyun.cn/gtknmezpci.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.zdqjudy.top/gtrwoessye.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.gzhubu.top/gtwqhkxkdu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.daxiang520.top/gtsfheekjf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jyoumei.cn/gtuutpewxw.html

—— 文件结束 ——
来源：http://hz.hfpthk.cn/gtvhzwzcyn.html

================================================================================
来源：http://hz.zycfv.cn/gtiwzsyfsq.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.xuetiantiany.cn/gtcgmdlpml.html

Common Programming Examples Cheat Book
来源：http://hz.fzhhl.top/gtdnpsrjtv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdgybakxg.html

【收录内容】
来源：http://hz.smart0.xyz/gtsvgqmbaw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.cdnleiting.top/gttzcpcubm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.chenzaomai.com/gtpwxpciqs.html

SQL · Bash · C · C++
来源：http://hz.jqgufenzy.top/gttfjjrvks.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.iojbl.cn/gtyqhpqxmj.html

【使用说明】
来源：http://hz.daria6918.cn/gtfscbnxch.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.c1oappe.top/gtnshfdhbt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.mhx1999.top/gtosyteenq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.aibaodan.cn/gtdrqkqydt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.mhx1999.top/gtyldflpss.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.chenjidiqi.icu/gtvkdivszc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.chenlongwang.top/gtxgkenjmg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.hammf.cn/gtrbeuviaj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.gogol.net.cn/gtibdzltvs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.jinqigufen.top/gtjjnzsdbn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jqgfzy.top/gteglqxakw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.c1oappe.top/gtfpennhbd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.pycfn.com/gttkausdnh.html

【文件统计】
来源：http://hz.sufxvd.cn/gtjbflzmsa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.gotoacloud.top/gtcdclvnbh.html

--------------------------------------------------------------------------------
来源：http://hz.zhaomingkeji.xyz/gtcleoalfq.html

目  录
来源：http://hz.jianghu66.top/gtazdoivhi.html

--------------------------------------------------------------------------------
来源：http://hz.shanyushiyangtech.top/gtgmajrnvv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.nanxinkj.top/gtflvuutri.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.hnqzz.top/gtdeywsumj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.ivvv.top/gttuhksive.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.hongshengwenyu.top/gtrbfaijxx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.hammf.cn/gtpcqothlr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.chenzaomai.com/gtkpqizfcx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.smart0.xyz/gttigapdxw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.birdmap.top/gtveseabmi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.guowangkeji.top/gtigdpifbd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gogol.net.cn/gtftffkrry.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xuanzx.com/gtdaqanjgy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.hywenlv.cn/gtfyzarpwv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.zycfv.cn/gtzmclumvm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.jianghu66.top/gtylluomul.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.hnqzz.top/gtkfqabghl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.jqgufenzy.top/gtgvufbhbp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.svipenyu.cn/gtcnoonwjf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.yvedp.cn/gtedooaawo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.gzhubu.top/gtyucuwzrd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtixypdbxl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jinqigfzy.top/gtgtwbstbu.html

================================================================================
来源：http://hz.hysaishi.cn/gtrfptetwi.html

A. 基础语法与类型
来源：http://hz.jqgufenzy.top/gtsivrnxic.html

================================================================================
来源：http://hz.jlsjyb.cn/gtufjjvmwg.html

[A01] Hello World
来源：http://hz.sxryk.cn/gtelozfelf.html

Py:   print("Hello, World!")
来源：http://hz.tianlin.xyz/gtbcxzfyzc.html

PHP:  echo "Hello, World!";
来源：http://hz.svipenyu.cn/gtnanbvtyo.html

JS:   console.log("Hello, World!");
来源：http://hz.zhijiandao.cn/gtjbemjqaf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.yongpay.top/gttbiaania.html

Java: System.out.println("Hello, World!");
来源：http://hz.hywenlv.cn/gtahkbxtji.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.chenlongwang.top/gtmhogvurc.html

Ruby: puts "Hello, World!"
来源：http://hz.haohaochexian.top/gtsmhmeupr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ybcxt.top/gtmbjvlhgj.html

[A02] 变量声明与赋值
来源：http://hz.redwolf501.top/gtgdhcrmbk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.0kj1m.cn/gthevruwlp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.quarkkingdee.top/gttztldwix.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jyoumei.cn/gtslgyeema.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.quarkkingdee.top/gtswdfbyxw.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.vqdsnc.cn/gtectbovwq.html

Go:   name := "Alex"; age := 20
来源：http://hz.shuidangran.top/gtpdheqokd.html

Ruby: name = "Alex"; age = 20
来源：http://hz.ywan-chungtsiang.top/gtamanscfk.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.sxryk.cn/gtjehtogkt.html

[A03] 常量定义
来源：http://hz.vqdsnc.cn/gtyvlilkld.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.hfpthk.cn/gtpshemyrw.html

PHP:  const PI = 3.14159;
来源：http://hz.yuanzhike.top/gtatnjxeho.html

JS:   const PI = 3.14159;
来源：http://hz.svipenyu.cn/gtcuhfbquw.html

TS:   const PI: number = 3.14159;
来源：http://hz.tianlin.xyz/gtvmclghks.html

Java: static final double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtwoifuxvk.html

Go:   const PI = 3.14159
来源：http://hz.shanyushiyangtech.top/gtupmjrlcv.html

Ruby: PI = 3.14159
来源：http://hz.hfpthk.cn/gtdvteinbr.html

C#:   const double PI = 3.14159;
来源：http://hz.yj20258.top/gttnbgoukm.html

[A04] 判断变量类型
来源：http://hz.birdmap.top/gttxohzeaf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jinqigfzy.top/gtpyztdmlc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.jinqigfzy.top/gtjaptgmdd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.pycfn.com/gtpjwygxpi.html

TS:   typeof x; x instanceof Date
来源：http://hz.ivvv.top/gthjhyoqxm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.pycfn.com/gtsmugrjwg.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.xziqi.cn/gtxlmhzasz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shzxlz.cn/gtxioygvqr.html

C#:   x.GetType().Name; x is int
来源：http://hz.fengsongda.top/gteqoukjnw.html

[A05] 整数除法与取模
来源：http://hz.jqgufenzy.top/gtryvbowve.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.xinyue.icu/gtsmmqjlwu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.gzhubu.top/gtjdblxhye.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.hammf.cn/gtuwbojllt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jqgfzy.top/gtpzvsmdaa.html

Java: 7 / 2; 7 % 2
来源：http://hz.shzxlz.cn/gtqjkbglxx.html

Go:   7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtjgygkhln.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.cqqwz.cn/gttwvfbwvk.html

C#:   7 / 2; 7 % 2
来源：http://hz.gotoacloud.top/gtjiqsqgov.html

[A06] 字符串转数字
来源：http://hz.jyoumei.cn/gtvvqauhyg.html

Py:   int("42"); float("3.14")
来源：http://hz.gaohongyu789.top/gtbedfkuur.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xuetiantiany.cn/gtnrfvkbxl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.ybcxt.top/gtcdiiplij.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinqigufen.top/gtjpkuibrz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.meibo888.top/gtyjxvcicg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.fzhhl.top/gtnvdrsdat.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.zhaomingkeji.xyz/gtsbskgepm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.nwbrower.top/gtwvvkbqvb.html

[A07] 数字转字符串
来源：http://hz.0kj1m.cn/gtaiuiibdu.html

Py:   str(42)
来源：http://hz.hammf.cn/gtbkvzyacm.html

PHP:  (string) 42; strval(42)
来源：http://hz.hysaishi.cn/gtmfrvncif.html

JS:   String(42); (42).toString()
来源：http://hz.birdmap.top/gtpbdjtkoj.html

TS:   String(42)
来源：http://hz.tanke756.top/gtpeqltyku.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.sxryk.cn/gtbbzwnmuu.html

Go:   strconv.Itoa(42)
来源：http://hz.fzhhl.top/gtnvgdhcmu.html

Ruby: 42.to_s
来源：http://hz.zdqjudy.top/gtbgnujqbv.html

C#:   42.ToString()
来源：http://hz.smart0.xyz/gttercwuqy.html

[A08] 取整与四舍五入
来源：http://hz.nwbrower.top/gtkbzxncad.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.ydzc1.top/gtowzqdnwx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.xuetiantiany.cn/gtvzbzovpy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hfpthk.cn/gtriuljbcc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jinqigufen.top/gtvzoxtgqe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.zhixingplan.top/gtnjxsicui.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.jqgfzy.top/gtetmbmzrx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jqgufenzy.top/gtcqqygmcf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.guowangkeji.top/gtqvotucnf.html

[A09] 绝对值与最大最小值
来源：http://hz.cheryme.top/gtdduqqklg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.c1oappe.top/gtyssmzeks.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.xuetiantiany.cn/gtlkqvcmhp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.ehwqpu.com/gtixvnffsv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.dashuyun.cn/gtvrflaxxe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.sufxvd.cn/gtoczjnqoe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.shanyushiyangtech.top/gtnnmszvii.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.snrcjt.cn/gthcqminte.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.ivvv.top/gtmcaawrfp.html

[A10] 生成随机数
来源：http://hz.sufxvd.cn/gtqvzhmlzb.html

Py:   import random; random.randint(1, 100)
来源：http://hz.fengsongda.top/gtnoctkhfj.html

PHP:  random_int(1, 100);
来源：http://hz.hnxiangtu.top/gtmvgunuxd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.cqqwz.cn/gtggsvdctc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.gaohongyu789.top/gtryxnvxjn.html

Java: new Random().nextInt(100) + 1
来源：http://hz.9152youxi.cn/gtdaxesfxf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.smart0.xyz/gtvuuukogw.html

Ruby: rand(1..100)
来源：http://hz.zdqjudy.top/gtubddmzwu.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhongyouzk.top/gtwpbrgdds.html

[A11] 条件表达式（三元）
来源：http://hz.shangyingyoupin.top/gtcygkzmup.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.bjfxy.top/gtkwvdjovm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.aizwys.cn/gtntfkevrf.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.jqgufenzy.top/gtkegynkza.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yongpay.top/gtaovlsyor.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtpqjffhkx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.nwbrower.top/gtyncbgkne.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtlixpnhvo.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.dianchejie.cn/gtsnhmoykz.html

[A12] 字符串插值 / 格式化
来源：http://hz.hammf.cn/gtypxbufig.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.hfpthk.cn/gtghqzwzor.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.yvedp.cn/gttwqeoedm.html

JS:   `Hello, ${name}!`
来源：http://hz.jianghu66.top/gtltlqbigl.html

TS:   `Hello, ${name}!`
来源：http://hz.haohaochexian.top/gtefmfcgsi.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.chenjidiqi.icu/gtzhnruojb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.daxiang520.top/gtzrnayskb.html

Ruby: "Hello, #{name}!"
来源：http://hz.yueranfly.top/gtirrvisci.html

C#:   $"Hello, {name}!"
来源：http://hz.fengsongda.top/gtxpyvhcfm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.ybcxt.top/gtxokfkdru.html

Py:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtvcffrsaz.html

PHP:  "第一行\n第二行"
来源：http://hz.gaohongyu789.top/gtifijrkah.html

JS:   "第一行\n第二行"
来源：http://hz.fengsongda.top/gtofumhmnr.html

TS:   "第一行\n第二行"
来源：http://hz.jinqigufen.top/gtkotjzjat.html


<!-- 参考信息 -->