代发 wailian999

[U81] JS：初始化项目
来源：http://hz.mhx1999.top/gtbsotupcb.html

npm init -y;  npm i express
来源：http://hz.shzxlz.cn/gtnyvxxshw.html

[U82] JS：package.json 脚本
来源：http://hz.ydzc1.top/gtdakoemlw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.0kj1m.cn/gtpnabkhob.html

[U83] JS：ES Module 导入导出
来源：http://hz.sweek.top/gthakjzfhs.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yj202588.top/gtyrtzwbei.html

[U84] JS：CommonJS 写法
来源：http://hz.hysaishi.cn/gtrinbxmpk.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.guannengcc.top/gtjfnzlzau.html

[U85] JS：可选链
来源：http://hz.yonumen.top/gtdxwttcha.html

a?.b?.c
来源：http://hz.316326.xyz/gtudhvfuch.html

[U86] JS：空值合并
来源：http://hz.hfpthk.cn/gtnysfqydc.html

a ?? b
来源：http://hz.aizwys.cn/gtijyuenyl.html

[U87] JS：解构默认值
来源：http://hz.hnqzz.top/gtdkghtjjq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.xziqi.cn/gtqqurwcnl.html

[U88] JS：对象展开合并
来源：http://hz.haohaochexian.top/gtfsxkungg.html

{ ...a, ...b }
来源：http://hz.jiagoushi.top/gteqoxoplq.html

[U89] JS：数组去重
来源：http://hz.andypj.xyz/gtaozuescm.html

[...new Set(arr)]
来源：http://hz.aizwys.cn/gtqmvvhbok.html

[U90] JS：数字数组排序
来源：http://hz.fengsongda.top/gtdcdeuava.html

[...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtnoxwejtu.html

[U91] JS：对象键值遍历
来源：http://hz.zhiwuduotai.top/gtcqdsxdhp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.wangshuangyany.cn/gtajbxdpoy.html

[U92] JS：深拷贝
来源：http://hz.shzxlz.cn/gtnphoswet.html

structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gtejdlxfwt.html

[U93] JS：模板字符串
来源：http://hz.jlsjyb.cn/gtmbfwfqyo.html

`共 ${n} 条`
来源：http://hz.yanxiufei.cn/gtcbkwgbxg.html

[U94] JS：箭头函数
来源：http://hz.52xcode.cn/gthwpybzjf.html

const double = x => x * 2;
来源：http://hz.tianlin.xyz/gtbdxdmdqe.html

[U95] JS：Promise 包装
来源：http://hz.jinyuanbaomall.cn/gtrjotbpoy.html

new Promise((resolve, reject) => {})
来源：http://hz.gzhubu.top/gttpcdxhlm.html

[U96] JS：async/await 与异常
来源：http://hz.cqqwz.cn/gtugonxefw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gtpovxjnbn.html

[U97] JS：并发请求
来源：http://hz.nanxinkj.top/gtqpwbxtdy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhiwuduotai.top/gtrhupyltc.html

[U98] JS：fetch 带 JSON
来源：http://hz.aibaodan.cn/gtekdmadhd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.hywenlv.cn/gtkhwmeash.html

[U99] JS：事件监听
来源：http://hz.dashuyun.cn/gtdonxqunq.html

el.addEventListener("click", e => {})
来源：http://hz.shanyushiyangtech.top/gtbdmpuovu.html

[U100] JS：DOM 查询
来源：http://hz.yuxming.cn/gtiganfsys.html

document.querySelector(".item")
来源：http://hz.xuetiantiany.cn/gttmiejlwy.html

[U101] JS：classList 操作
来源：http://hz.hnxiangtu.top/gtkdtepzwn.html

el.classList.toggle("active")
来源：http://hz.hysaishi.cn/gtwrfnsemd.html

[U102] JS：本地存储
来源：http://hz.xylfe.cn/gtlzjsrxuk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.cucudq.cn/gtzwmyafrl.html

[U103] JS：定时器
来源：http://hz.nanxinkj.top/gtkndovrvu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.0kj1m.cn/gtnqeymxhz.html

[U104] JS：防抖
来源：http://hz.yj20258888.top/gtteahncdy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.gogol.net.cn/gtzzwsyxrs.html

[U105] JS：节流
来源：http://hz.daria6918.cn/gtekyugstp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.wangdashe.top/gtdifsfbzd.html

[U106] JS：日期格式化
来源：http://hz.hnxiangtu.top/gtxxymcjsk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.52xcode.cn/gthbeelfqo.html

[U107] JS：数字千分位
来源：http://hz.pengpengdd.cyou/gtlkywcysn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.guannengcc.top/gtqnxtdook.html

[U108] JS：随机整数
来源：http://hz.9152youxi.cn/gttwznotge.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.sweek.top/gtosrdmbnk.html

[U109] JS：数组分组
来源：http://hz.yvedp.cn/gtofqadsef.html

Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtofldsyht.html

[U110] JS：数组分块
来源：http://hz.jqgufenzy.top/gtvxsofyeh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.tanke756.top/gtohnuatck.html

[U111] JS：对象转 Map
来源：http://hz.pycfn.com/gtzefvxmkh.html

new Map(Object.entries(obj))
来源：http://hz.jiagoushi.top/gtdzybmtod.html

[U112] JS：字符串补位
来源：http://hz.yj20258.top/gtqtpeollk.html

"7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtxxtvejmo.html

[U113] JS：正则替换全部
来源：http://hz.shanyushiyangkeji.top/gtwcbbycok.html

s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtyzvopdev.html

[U114] JS：JSON 深比较
来源：http://hz.smart0.xyz/gtjyhtviru.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.ehwqpu.com/gtfsfiffdn.html

[U115] JS：生成 UUID
来源：http://hz.ivvv.top/gtglxdbjhn.html

crypto.randomUUID()
来源：http://hz.yj202588.top/gtajyatwom.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.jinqigufen.top/gtgchdyzmy.html

/** @param {string} name */ function f(name) {}
来源：http://hz.aibaodan.cn/gtfhlmpokl.html

[U117] JS：单元测试
来源：http://hz.shanyushiyangtech.top/gtslgmmssf.html

npm i -D vitest;  npx vitest
来源：http://hz.xylfe.cn/gtvopzltzo.html

[U118] JS：开发服务器
来源：http://hz.shangyingyoupin.top/gtdelqjyty.html

npm i -D vite;  npx vite
来源：http://hz.shangyingyoupin.top/gtzzrcqpmr.html

[U119] JS：生产构建
来源：http://hz.zhaomingkeji.xyz/gttmmuiyvg.html

npx vite build
来源：http://hz.xuetiantiany.cn/gtljkdibrw.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.xuanzx.com/gtdzzncmna.html

import.meta.env.VITE_API_URL
来源：http://hz.jiagoushi.top/gtubxjxqez.html

================================================================================
来源：http://hz.jqgfzy.top/gtsdctazxt.html

统计汇总
来源：http://hz.wangdashe.top/gtyhjcoxfl.html

================================================================================
来源：http://hz.snrcjt.cn/gtrkflctik.html

按语言统计（条）：
来源：http://hz.xuanzx.com/gthecblciq.html

Python ......... 252
来源：http://hz.iojbl.cn/gtkcqjbiha.html

PHP ............ 252
来源：http://hz.ydjk.org.cn/gtokaqtnlt.html

JavaScript ..... 252
来源：http://hz.zhongyouzk.top/gtktppcxrb.html

TypeScript ..... 212
来源：http://hz.redwolf501.top/gtmpgxespl.html

Java ........... 212
来源：http://hz.tianlin.xyz/gtswdjjspw.html

Go ............. 212
来源：http://hz.jinyuanbaomall.cn/gtogkairic.html

Ruby ........... 212
来源：http://hz.iojbl.cn/gtyvdibgdx.html

C# ............. 212
来源：http://hz.zycfv.cn/gtogxauhxp.html

C .............. 30
来源：http://hz.0kj1m.cn/gtgdzlfddz.html

C++ ............ 30
来源：http://hz.xuetiantiany.cn/gtggftbkrz.html

SQL ............ 90
来源：http://hz.0kj1m.cn/gtzbvnlhcf.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtugczpoti.html

Kotlin ......... 15
来源：http://hz.ywan-chungtsiang.top/gtwgeudutm.html

Swift .......... 15
来源：http://hz.yuanzhike.top/gtryrrpesd.html

Lua ............ 10
来源：http://hz.zhijiandao.cn/gtcrzbdxmc.html

Perl ........... 10
来源：http://hz.shanyushiyangtech.top/gtyrfxqbvz.html

Scala .......... 10
来源：http://hz.xuetiantiany.cn/gtykvpggbs.html

------------------------------------
来源：http://hz.xylfe.cn/gttxpogzis.html

合计 ........... 2106 条
来源：http://hz.9152youxi.cn/gttdaycevk.html

按章节统计：
来源：http://hz.jyoumei.cn/gtoetsvati.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.shanyushiyangtech.top/gtsjkmnkml.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.quarkkingdee.top/gtaxivoyul.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.zhaomingkeji.xyz/gtjvbnhvgy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.gogol.net.cn/gtuthegkuf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.kuanghao11.cn/gtyxgvkzaf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gttlmbkmtf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.redwolf501.top/gtogiufnck.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.ydzc1.top/gtskxioxgq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.andypj.xyz/gtmqqbxlyp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.jinghuilouyu.cn/gthchzstbc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.ydzc1.top/gtfwjrmiwj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtosmkbvrd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.wangshuangyany.cn/gtywpoumxp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.yonumen.top/gtzsoxsdvt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.xziqi.cn/gtltyincmc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.daria6918.cn/gtmpupwvbv.html

Q SQL 专题                              90
来源：http://hz.gzhubu.top/gtfgwbymvf.html

R Bash 专题                             80
来源：http://hz.redwolf501.top/gtfozwyrya.html

S C / C++ 专题                          60
来源：http://hz.ydzc1.top/gtwfenotcs.html

T 其他语言补充                          60
来源：http://hz.jinghuilouyu.cn/gtqbonhijp.html

U 高频实用片段                         120
来源：http://hz.nanxinkj.top/gtlbobzmtk.html

------------------------------------
来源：http://hz.shanyushiyangtech.top/gtnhntjzaa.html

合计                                  2106 条
来源：http://hz.svipenyu.cn/gtkmetubmh.html

--------------------------------------------------------------------------------
来源：http://hz.mhx1999.top/gtgwwxstfp.html

使用提醒
来源：http://hz.shuidangran.top/gtaswmindk.html

--------------------------------------------------------------------------------
来源：http://hz.dianchejie.cn/gtytbktlch.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.zhongyouzk.top/gtgvcuamdl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.iojbl.cn/gtccznzanp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.zhixingplan.top/gtbgvclbkg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.havefunace.top/gtylxxrktw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.zhengqikj.top/gtdyhlcyyj.html

—— 文件结束 ——
来源：http://hz.jqgfzy.top/gtlthmxbeu.html

================================================================================
来源：http://hz.pycfn.com/gtlhdxxgtf.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.tian-w.cn/gtvcddesbc.html

Common Programming Examples Cheat Book
来源：http://hz.ppjwa.cn/gtrqpukoxp.html

================================================================================
来源：http://hz.aizwys.cn/gttdchkfzl.html

【收录内容】
来源：http://hz.tanke756.top/gthpcrzhox.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.zycfv.cn/gtghcyozuy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.ivvv.top/gtccxoqovf.html

SQL · Bash · C · C++
来源：http://hz.yj202588.top/gtyvvncwqk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.havefunace.top/gtpihrkqku.html

【使用说明】
来源：http://hz.quarkkingdee.top/gtmgdmegjc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.hnqzz.top/gtyxayixib.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.chenzaomai.com/gtyqawifoc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.jlsjyb.cn/gtiszhuxwo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.dashuyun.cn/gtkvjcqnjo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yvedp.cn/gtjrvoarrn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.nwbrower.top/gtbkvmfwwm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.52xcode.cn/gtymsqoeor.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.andypj.xyz/gtzwjveeyb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.cheryme.top/gtfhycwahi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhijiandao.cn/gtmhxyqvtd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zhoulong.xyz/gtuqlrybbd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.vqdsnc.cn/gtnixepqhy.html

【文件统计】
来源：http://hz.chenjidiqi.icu/gtylkcrcwu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.quarkkingdee.top/gtfltvpndi.html

--------------------------------------------------------------------------------
来源：http://hz.birdmap.top/gtlmwfqibi.html

目  录
来源：http://hz.ehwqpu.com/gtvgiddmbi.html

--------------------------------------------------------------------------------
来源：http://hz.xziqi.cn/gtksarapmw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.cucudq.cn/gtnptzxlar.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.ydjk.org.cn/gtgutskshq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtnisnview.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sxryk.cn/gtlqdxkhav.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.quarkkingdee.top/gtkeixkkza.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.svipenyu.cn/gtmzhauvlj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.aizwys.cn/gtoasaleft.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.bjfxy.top/gtejmxgows.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.yongpay.top/gtpqzbsjla.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.yuanzhike.top/gtxqlueolb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.gotoacloud.top/gtzfhmbynv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.zdqjudy.top/gtjlqvnjxa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.daria6918.cn/gtzpwawuvw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yuxming.cn/gtmiftfsyo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.sysykeji.top/gtpxhpcwib.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.quarkkingdee.top/gtjfdfetnw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.ydzc1.top/gtgjmwkoti.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.tanke756.top/gtvpudcakx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.pengpengdd.cyou/gtzsomdbab.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ywan-chungtsiang.top/gtxwgotacd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.hfpthk.cn/gtcmqpgtvv.html

================================================================================
来源：http://hz.cdnleiting.top/gtaahdszxy.html

A. 基础语法与类型
来源：http://hz.daria6918.cn/gtegwgkbzf.html

================================================================================
来源：http://hz.smart0.xyz/gtyaaaipyy.html

[A01] Hello World
来源：http://hz.meibo888.top/gtqetcytto.html

Py:   print("Hello, World!")
来源：http://hz.kuanghao11.cn/gtszummylx.html

PHP:  echo "Hello, World!";
来源：http://hz.chenjidiqi.icu/gtsgomgeno.html

JS:   console.log("Hello, World!");
来源：http://hz.shanyushiyangtech.top/gtmrgkgudf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.quarkkingdee.top/gtoywdipzl.html

Java: System.out.println("Hello, World!");
来源：http://hz.bjfxy.top/gtzaipakms.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.wangshuangyany.cn/gtzlycdsfs.html

Ruby: puts "Hello, World!"
来源：http://hz.cheryme.top/gtndkghzrh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.cdnleiting.top/gtdbypfnlq.html

[A02] 变量声明与赋值
来源：http://hz.hfpthk.cn/gtnqejyoau.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.yonumen.top/gtiwqvgvvr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.jianghu66.top/gtczqbjgno.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.jyoumei.cn/gtkkpbatok.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jqgufenzy.top/gtckejsgda.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.yongpay.top/gtsfsdlgny.html

Go:   name := "Alex"; age := 20
来源：http://hz.sufxvd.cn/gtsdnldnsi.html

Ruby: name = "Alex"; age = 20
来源：http://hz.gogol.net.cn/gtzfckqtxi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.havefunace.top/gtanbcqpxp.html

[A03] 常量定义
来源：http://hz.birdmap.top/gtjradxfkl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.ppjwa.cn/gthaiacqtg.html

PHP:  const PI = 3.14159;
来源：http://hz.xuanzx.com/gtoqfgjhvx.html

JS:   const PI = 3.14159;
来源：http://hz.cucudq.cn/gtozbkmusi.html

TS:   const PI: number = 3.14159;
来源：http://hz.zhaomingkeji.xyz/gttddkenzg.html

Java: static final double PI = 3.14159;
来源：http://hz.cheryme.top/gtlevvzeru.html

Go:   const PI = 3.14159
来源：http://hz.yvedp.cn/gtwxwdmkho.html

Ruby: PI = 3.14159
来源：http://hz.kuanghao11.cn/gtuywckiug.html

C#:   const double PI = 3.14159;
来源：http://hz.sxryk.cn/gtiwfooynz.html

[A04] 判断变量类型
来源：http://hz.sufxvd.cn/gtslydysgd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.yonumen.top/gticfuafwq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.redwolf501.top/gtgizwlvoi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.birdmap.top/gtqrqscjzp.html

TS:   typeof x; x instanceof Date
来源：http://hz.sysykeji.top/gtscnnjzsm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.pycfn.com/gtnmvzcgwu.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.jinqigufen.top/gtmpdhyult.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.tian-w.cn/gtmydhdcky.html

C#:   x.GetType().Name; x is int
来源：http://hz.yj20258888.top/gtcgqtbbvl.html

[A05] 整数除法与取模
来源：http://hz.jqgufenzy.top/gtveuyecom.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shanyushiyangtech.top/gtsdqtwvqh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.nanxinkj.top/gtaijltuyh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.cheryme.top/gtasfeweel.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258.top/gticzmidlk.html

Java: 7 / 2; 7 % 2
来源：http://hz.xingfuxueyuan.xyz/gtydwgqsky.html

Go:   7 / 2; 7 % 2
来源：http://hz.jinqigufen.top/gtekpjgymb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.ydzc1.top/gtfndzcrwm.html

C#:   7 / 2; 7 % 2
来源：http://hz.chenlongwang.top/gtcdhcihbq.html

[A06] 字符串转数字
来源：http://hz.aizwys.cn/gtksccofli.html

Py:   int("42"); float("3.14")
来源：http://hz.yj20258888.top/gtliedoacn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.hfpthk.cn/gtrtsixooh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.xinyue.icu/gtjvttkozl.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.ybcxt.top/gtyhpowtnu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.yuanzhike.top/gtfhmrzprq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.gaohongyu789.top/gtgunfhije.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jinyuanbaomall.cn/gtnacbiupe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.guowangkeji.top/gtlvqzrzay.html

[A07] 数字转字符串
来源：http://hz.kuanghao11.cn/gtvselycch.html

Py:   str(42)
来源：http://hz.nanxinkj.top/gtwntqtwsz.html

PHP:  (string) 42; strval(42)
来源：http://hz.tanke756.top/gtewnroubx.html

JS:   String(42); (42).toString()
来源：http://hz.ivvv.top/gtgsjrvyyv.html

TS:   String(42)
来源：http://hz.zhixingplan.top/gttodfsgxi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.zhoulong.xyz/gtdcrxjzpt.html

Go:   strconv.Itoa(42)
来源：http://hz.shuidangran.top/gtanqxmkhk.html

Ruby: 42.to_s
来源：http://hz.hnqzz.top/gteyhrycai.html

C#:   42.ToString()
来源：http://hz.hysaishi.cn/gtgqpspbug.html

[A08] 取整与四舍五入
来源：http://hz.vqdsnc.cn/gttqlrinav.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.xingfuxueyuan.xyz/gtecoorwaz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.yuanzhike.top/gtwtrvesut.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.cashguo.top/gtxzmnzuxl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.jyoumei.cn/gtuamhdfqz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hnxiangtu.top/gtjzrlyioz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cucudq.cn/gtljuxesec.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.tianlin.xyz/gtmhelajrq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.feifeiyinyue.top/gtjkmqqbmo.html

[A09] 绝对值与最大最小值
来源：http://hz.tian-w.cn/gtmvsemlot.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.shzxlz.cn/gtifxnsbms.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.tianlin.xyz/gtwkhxqaek.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.bjfxy.top/gtcztmkvhx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.ywan-chungtsiang.top/gtkkyvkdop.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.nanxuanxn.top/gtcgidzzhy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.hammf.cn/gtpuzssqam.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.316326.xyz/gtfchzyjdp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.yj20258.top/gtftgxbyhe.html

[A10] 生成随机数
来源：http://hz.hysaishi.cn/gtdfjwdnhh.html

Py:   import random; random.randint(1, 100)
来源：http://hz.chenjidiqi.icu/gtixgrziax.html

PHP:  random_int(1, 100);
来源：http://hz.pengpengdd.cyou/gtkznmmikr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.guannengcc.top/gtasqexysn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.ydjk.org.cn/gtrnccloiy.html

Java: new Random().nextInt(100) + 1
来源：http://hz.gotoacloud.top/gtuogepoed.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.xziqi.cn/gtlfwwdrfa.html

Ruby: rand(1..100)
来源：http://hz.yueranfly.top/gtwwltqnwq.html

C#:   new Random().Next(1, 101)
来源：http://hz.jqgufenzy.top/gtizukjjhi.html

[A11] 条件表达式（三元）
来源：http://hz.sweek.top/gtmvhfrlri.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shanyushiyangkeji.top/gtbfukltwq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hnqzz.top/gtvttirawr.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtrhesnjxb.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.smart0.xyz/gtuiewcjfm.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.zhoulong.xyz/gtjlbxdygc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jiagoushi.top/gtulqqgvab.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.iojbl.cn/gtycayybmn.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.jinyuanbaomall.cn/gtzqyesttm.html

[A12] 字符串插值 / 格式化
来源：http://hz.quarkkingdee.top/gtgropahhe.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.jyoumei.cn/gtyjiwvhpd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.tanke756.top/gtddhsiqrc.html

JS:   `Hello, ${name}!`
来源：http://hz.zycfv.cn/gtshmfnflh.html

TS:   `Hello, ${name}!`
来源：http://hz.ywan-chungtsiang.top/gtrilpwnzh.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.hongshengwenyu.top/gtlzyaclvk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.gaohongyu789.top/gtgnyvveuj.html

Ruby: "Hello, #{name}!"
来源：http://hz.yangfankeji.com/gtcwysthfn.html

C#:   $"Hello, {name}!"
来源：http://hz.dashuyun.cn/gtglglcpum.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.sweek.top/gtvmvfmvfj.html

Py:   "第一行\n第二行"
来源：http://hz.sysykeji.top/gtngxkpaph.html

PHP:  "第一行\n第二行"
来源：http://hz.tianlin.xyz/gtkfkeloqt.html

JS:   "第一行\n第二行"
来源：http://hz.jyoumei.cn/gtiwkdzskr.html

TS:   "第一行\n第二行"
来源：http://hz.yuxming.cn/gtlcwzfyxx.html


<!-- 参考信息 -->