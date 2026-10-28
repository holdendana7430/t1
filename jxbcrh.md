代发 wailian999

[U81] JS：初始化项目
来源：http://hz.yj20258.top/gtlqtmvmuj.html

npm init -y;  npm i express
来源：http://hz.yanxiufei.cn/gtlaxmeorn.html

[U82] JS：package.json 脚本
来源：http://hz.zhoulong.xyz/gtrjlfwbuf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.ybcxt.top/gttbxgrtdf.html

[U83] JS：ES Module 导入导出
来源：http://hz.kuanghao11.cn/gtgxrdtqmc.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.jyoumei.cn/gtipgocrsn.html

[U84] JS：CommonJS 写法
来源：http://hz.gzhubu.top/gtetmqbwsw.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.guannengcc.top/gtidmudnfj.html

[U85] JS：可选链
来源：http://hz.yongpay.top/gtyscrmrzh.html

a?.b?.c
来源：http://hz.aibaodan.cn/gtwppqukbw.html

[U86] JS：空值合并
来源：http://hz.feifeiyinyue.top/gtzgrajpuh.html

a ?? b
来源：http://hz.zdqjudy.top/gtndqxffld.html

[U87] JS：解构默认值
来源：http://hz.jianghu66.top/gtspwmposb.html

const { a = 1, b = 2 } = obj;
来源：http://hz.hammf.cn/gtvpducubn.html

[U88] JS：对象展开合并
来源：http://hz.meibo888.top/gtqsfmvjxs.html

{ ...a, ...b }
来源：http://hz.gogol.net.cn/gtkcsbjgss.html

[U89] JS：数组去重
来源：http://hz.cucudq.cn/gtgratjgci.html

[...new Set(arr)]
来源：http://hz.jqgfzy.top/gtxgsyipqz.html

[U90] JS：数字数组排序
来源：http://hz.hysaishi.cn/gtvxoqesmf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtcpeeywvm.html

[U91] JS：对象键值遍历
来源：http://hz.sxryk.cn/gtcponrblg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.c1oappe.top/gtqpfzajub.html

[U92] JS：深拷贝
来源：http://hz.zhengqikj.top/gtxdccpnsf.html

structuredClone(obj)
来源：http://hz.xinyue.icu/gtlehtrjwm.html

[U93] JS：模板字符串
来源：http://hz.haohaochexian.top/gtydukhjsy.html

`共 ${n} 条`
来源：http://hz.yj20258.top/gtpgolxntp.html

[U94] JS：箭头函数
来源：http://hz.jqgufenzy.top/gtuwaqmohq.html

const double = x => x * 2;
来源：http://hz.jiagoushi.top/gtupscdedr.html

[U95] JS：Promise 包装
来源：http://hz.sxryk.cn/gtnroscutb.html

new Promise((resolve, reject) => {})
来源：http://hz.ywan-chungtsiang.top/gtyrqdwzrd.html

[U96] JS：async/await 与异常
来源：http://hz.xuetiantiany.cn/gtsrulqpin.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtghokwedo.html

[U97] JS：并发请求
来源：http://hz.ehwqpu.com/gtopfhpgrf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtgjlcmzqh.html

[U98] JS：fetch 带 JSON
来源：http://hz.pycfn.com/gtaiifrsju.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.guowangkeji.top/gtxptuwung.html

[U99] JS：事件监听
来源：http://hz.yanxiufei.cn/gtlyllnssi.html

el.addEventListener("click", e => {})
来源：http://hz.jinyuanbaomall.cn/gtbgqyvnex.html

[U100] JS：DOM 查询
来源：http://hz.vqdsnc.cn/gtbakgyaaw.html

document.querySelector(".item")
来源：http://hz.yj20258.top/gtgpaoouvw.html

[U101] JS：classList 操作
来源：http://hz.snrcjt.cn/gtsuqekwyz.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtfmuxloxy.html

[U102] JS：本地存储
来源：http://hz.cheryme.top/gtnzcmszje.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.dianchejie.cn/gtqupezkdi.html

[U103] JS：定时器
来源：http://hz.hongshengwenyu.top/gtfgiglzuj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.jqgufenzy.top/gtkgixyfqj.html

[U104] JS：防抖
来源：http://hz.sysykeji.top/gtrngtihez.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.shangyingyoupin.top/gtxmhqqcuy.html

[U105] JS：节流
来源：http://hz.0kj1m.cn/gtrgivcbgn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.chenlongwang.top/gtcloudixz.html

[U106] JS：日期格式化
来源：http://hz.zycfv.cn/gtuvpnsych.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.xingfuxueyuan.xyz/gtalcnrucu.html

[U107] JS：数字千分位
来源：http://hz.gotoacloud.top/gtuhftckyg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.yuxming.cn/gtudjsgwbb.html

[U108] JS：随机整数
来源：http://hz.0kj1m.cn/gtqxvaznhk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.ivvv.top/gtghzbcppr.html

[U109] JS：数组分组
来源：http://hz.yuanzhike.top/gtlwiwjtkz.html

Object.groupBy(arr, x => x.type)
来源：http://hz.ydzc1.top/gtjlwsrkav.html

[U110] JS：数组分块
来源：http://hz.zhijiandao.cn/gtbgrtfxyj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.snrcjt.cn/gtvdficvrz.html

[U111] JS：对象转 Map
来源：http://hz.hongshengwenyu.top/gtzsyowjnk.html

new Map(Object.entries(obj))
来源：http://hz.daria6918.cn/gtuyyuifzu.html

[U112] JS：字符串补位
来源：http://hz.yj20258.top/gtqndhgblz.html

"7".padStart(3, "0")
来源：http://hz.tanke756.top/gtzidlmatj.html

[U113] JS：正则替换全部
来源：http://hz.yangfankeji.com/gtabsclben.html

s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtrqxxejhp.html

[U114] JS：JSON 深比较
来源：http://hz.aibaodan.cn/gtobtlyylu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.smart0.xyz/gtdrlfzpsq.html

[U115] JS：生成 UUID
来源：http://hz.havefunace.top/gtpnqqhglk.html

crypto.randomUUID()
来源：http://hz.sxryk.cn/gtrjganhwe.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.xuetiantiany.cn/gtsguokmqz.html

/** @param {string} name */ function f(name) {}
来源：http://hz.daria6918.cn/gtxxfylqnw.html

[U117] JS：单元测试
来源：http://hz.snrcjt.cn/gtbkemqnat.html

npm i -D vitest;  npx vitest
来源：http://hz.9152youxi.cn/gtyvbdteee.html

[U118] JS：开发服务器
来源：http://hz.shzxlz.cn/gtotlurrzt.html

npm i -D vite;  npx vite
来源：http://hz.xingfuxueyuan.xyz/gtlhzaxldx.html

[U119] JS：生产构建
来源：http://hz.hongshengwenyu.top/gtqzkuapwa.html

npx vite build
来源：http://hz.c1oappe.top/gtwonqiwjp.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.shanyushiyangkeji.top/gtjskflhvh.html

import.meta.env.VITE_API_URL
来源：http://hz.pycfn.com/gtrlwybqzr.html

================================================================================
来源：http://hz.ivvv.top/gtxafzaqzk.html

统计汇总
来源：http://hz.zhaomingkeji.xyz/gtjfmyugmi.html

================================================================================
来源：http://hz.iojbl.cn/gtkrwbedua.html

按语言统计（条）：
来源：http://hz.sxryk.cn/gtwcampkqo.html

Python ......... 252
来源：http://hz.kuanghao11.cn/gthptrusag.html

PHP ............ 252
来源：http://hz.ehwqpu.com/gtgyadsvub.html

JavaScript ..... 252
来源：http://hz.jinqigufen.top/gtstbvblmr.html

TypeScript ..... 212
来源：http://hz.shuidangran.top/gtycyxeovk.html

Java ........... 212
来源：http://hz.cheryme.top/gtrfasqcma.html

Go ............. 212
来源：http://hz.cqqwz.cn/gtrflnkzch.html

Ruby ........... 212
来源：http://hz.ppjwa.cn/gtbqekjndz.html

C# ............. 212
来源：http://hz.zhengqikj.top/gthmcetowu.html

C .............. 30
来源：http://hz.shzxlz.cn/gtgunpecwg.html

C++ ............ 30
来源：http://hz.quarkkingdee.top/gtkzdxsfyt.html

SQL ............ 90
来源：http://hz.ybcxt.top/gtlhigfbwu.html

Bash ........... 80
来源：http://hz.52xcode.cn/gtuhncqulh.html

Kotlin ......... 15
来源：http://hz.smart0.xyz/gtrgqwxjze.html

Swift .......... 15
来源：http://hz.jyoumei.cn/gtnpcbfwpy.html

Lua ............ 10
来源：http://hz.jinqigfzy.top/gtetpvrqhs.html

Perl ........... 10
来源：http://hz.zhiwuduotai.top/gtlzdpozfe.html

Scala .......... 10
来源：http://hz.yanxiufei.cn/gtrgkskbkc.html

------------------------------------
来源：http://hz.hfpthk.cn/gtoyrylvaz.html

合计 ........... 2106 条
来源：http://hz.52xcode.cn/gtpmrfyrzu.html

按章节统计：
来源：http://hz.ybcxt.top/gtcqultgsp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.chenlongwang.top/gtpadyraif.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.daxiang520.top/gtbzpgprev.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.hfpthk.cn/gtpurnssgy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.kuanghao11.cn/gtbzhrfftc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.dashuyun.cn/gtzrurjzvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.ehwqpu.com/gttswzeuds.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.gaohongyu789.top/gtrbmuyany.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.yangfankeji.com/gttjuazbfe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.tianlin.xyz/gtuccazicc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.fzhhl.top/gtfivzsjpi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.havefunace.top/gtrfseslon.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.yuanzhike.top/gtyditskgq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.birdmap.top/gtwvydfsmx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.jlsjyb.cn/gtxxrvckbi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yanxiufei.cn/gtyaybvalt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.yuxming.cn/gtwntzavpc.html

Q SQL 专题                              90
来源：http://hz.zhiwuduotai.top/gtubbwtnhg.html

R Bash 专题                             80
来源：http://hz.sweek.top/gtrcefpqqh.html

S C / C++ 专题                          60
来源：http://hz.ydzc1.top/gtlupphufh.html

T 其他语言补充                          60
来源：http://hz.gotoacloud.top/gtnrurljna.html

U 高频实用片段                         120
来源：http://hz.yangfankeji.com/gtlbhxwaus.html

------------------------------------
来源：http://hz.tian-w.cn/gtedebkdio.html

合计                                  2106 条
来源：http://hz.tanke756.top/gtjnoqucum.html

--------------------------------------------------------------------------------
来源：http://hz.gotoacloud.top/gtvwyguikw.html

使用提醒
来源：http://hz.zhixingplan.top/gtjiicfnyl.html

--------------------------------------------------------------------------------
来源：http://hz.nwbrower.top/gtpivyhawt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.jinqigufen.top/gtotdzvbrw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.hammf.cn/gtpgmdydar.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.quarkkingdee.top/gtosvvdvnt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.redwolf501.top/gttzdowuij.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.cqqwz.cn/gtcbxvsvec.html

—— 文件结束 ——
来源：http://hz.wangshuangyany.cn/gttnajwfzj.html

================================================================================
来源：http://hz.smart0.xyz/gthgjjcwrz.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.chenlongwang.top/gtcelhofwb.html

Common Programming Examples Cheat Book
来源：http://hz.xuetiantiany.cn/gtgbqmhaqx.html

================================================================================
来源：http://hz.dashuyun.cn/gttzkggygc.html

【收录内容】
来源：http://hz.jyoumei.cn/gtmqhpewon.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.havefunace.top/gthpfgcirc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.chenzaomai.com/gtesvpplgr.html

SQL · Bash · C · C++
来源：http://hz.aibaodan.cn/gtzdohxcbp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.yj202588.top/gtsmreqouw.html

【使用说明】
来源：http://hz.zhiwuduotai.top/gtdfiyxhor.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.xingfuxueyuan.xyz/gtlncjwroa.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zdqjudy.top/gtwcdgatdy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhixingplan.top/gtdlgqmzvv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.zdqjudy.top/gtalonzyip.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.ppjwa.cn/gtrggwzawp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.wangdashe.top/gttpdsqdfb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.andypj.xyz/gtoetsslcg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.jianghu66.top/gtpbevaeam.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.hfpthk.cn/gtthafexws.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.shuidangran.top/gttpvgezzr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.zycfv.cn/gtdpbzxgqf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ydjk.org.cn/gtitesbfyw.html

【文件统计】
来源：http://hz.ppjwa.cn/gtjqnnavds.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.ehwqpu.com/gtstprkerr.html

--------------------------------------------------------------------------------
来源：http://hz.jinyuanbaomall.cn/gttxlpeyrc.html

目  录
来源：http://hz.fengsongda.top/gtnwlgibtq.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gthoqidqtt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.vqdsnc.cn/gtkwhjevrb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.yangfankeji.com/gtvwmvjymx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.yuanzhike.top/gtszsvynkh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.yonumen.top/gtblcvnztf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.daxiang520.top/gtgclpyizg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.xuanzx.com/gtlmjlklid.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.yj20258.top/gtqsvgeqau.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.fzhhl.top/gthmmhvqbd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.zhaomingkeji.xyz/gtvurwhifh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.hnqzz.top/gtxmdpzpst.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.tianlin.xyz/gtkozrsvzx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.9152youxi.cn/gttfudmkbf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.hnqzz.top/gtminnzyfx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.yueranfly.top/gtvayyvjki.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.xylfe.cn/gtfmthqfce.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.hfpthk.cn/gtwsfklbhs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cheryme.top/gtshkzvtkd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.jlsjyb.cn/gtnzettina.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.dashuyun.cn/gtlihifgyt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.aizwys.cn/gtdxzshqcw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.yj20258.top/gtsjholcbu.html

================================================================================
来源：http://hz.havefunace.top/gtsjbquulk.html

A. 基础语法与类型
来源：http://hz.smart0.xyz/gtsodhsrcz.html

================================================================================
来源：http://hz.yj202588.top/gtcjbflhlt.html

[A01] Hello World
来源：http://hz.zycfv.cn/gtcczlgrvj.html

Py:   print("Hello, World!")
来源：http://hz.chenjidiqi.icu/gtsftbpphn.html

PHP:  echo "Hello, World!";
来源：http://hz.tanke756.top/gtvtztjbek.html

JS:   console.log("Hello, World!");
来源：http://hz.xziqi.cn/gtmdcychpz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.meibo888.top/gtdqjamcay.html

Java: System.out.println("Hello, World!");
来源：http://hz.jqgufenzy.top/gtxfupxeie.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.zhiwuduotai.top/gtskxesmwp.html

Ruby: puts "Hello, World!"
来源：http://hz.chenlongwang.top/gtcncwxgki.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ybcxt.top/gtirpnbcgh.html

[A02] 变量声明与赋值
来源：http://hz.zhixingplan.top/gtwoihafed.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.0kj1m.cn/gtarygbmsi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tanke756.top/gthfshqjck.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.nwbrower.top/gtnqswxcou.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.jinyuanbaomall.cn/gtcrpbscqk.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.ydjk.org.cn/gtvclltzju.html

Go:   name := "Alex"; age := 20
来源：http://hz.yj202588.top/gtbjpehjyu.html

Ruby: name = "Alex"; age = 20
来源：http://hz.smart0.xyz/gthhqdojkm.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.birdmap.top/gtqykgfsbh.html

[A03] 常量定义
来源：http://hz.feifeiyinyue.top/gtfuvrxpxk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.sweek.top/gtfkcpsfur.html

PHP:  const PI = 3.14159;
来源：http://hz.meibo888.top/gtrbxlrhjx.html

JS:   const PI = 3.14159;
来源：http://hz.yonumen.top/gtlylcapnx.html

TS:   const PI: number = 3.14159;
来源：http://hz.sufxvd.cn/gtasvdcjop.html

Java: static final double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtkbzcqkii.html

Go:   const PI = 3.14159
来源：http://hz.zhiwuduotai.top/gtvvxcvgnm.html

Ruby: PI = 3.14159
来源：http://hz.snrcjt.cn/gtehyravmv.html

C#:   const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtgaevdiay.html

[A04] 判断变量类型
来源：http://hz.zdqjudy.top/gtfdahgagk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.jianghu66.top/gtgggvnivq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.meibo888.top/gtmhirirjw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.tanke756.top/gtfpeavoch.html

TS:   typeof x; x instanceof Date
来源：http://hz.yongpay.top/gtdqzmwlph.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.jinghuilouyu.cn/gtergddqqq.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.pycfn.com/gtcepvzlfj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xingfuxueyuan.xyz/gtlxovxrrj.html

C#:   x.GetType().Name; x is int
来源：http://hz.zhijiandao.cn/gtrtkhbade.html

[A05] 整数除法与取模
来源：http://hz.52xcode.cn/gtcfvtcmxi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.jinqigfzy.top/gtxvusljjo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.jinyuanbaomall.cn/gtegzncrnz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.havefunace.top/gtnmeasflx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jianghu66.top/gtytrsevls.html

Java: 7 / 2; 7 % 2
来源：http://hz.shangyingyoupin.top/gtizqfymjp.html

Go:   7 / 2; 7 % 2
来源：http://hz.zhoulong.xyz/gtrpgedrkq.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtlyzpsgaz.html

C#:   7 / 2; 7 % 2
来源：http://hz.hammf.cn/gtdxiqtrnk.html

[A06] 字符串转数字
来源：http://hz.iojbl.cn/gtkqjahijb.html

Py:   int("42"); float("3.14")
来源：http://hz.daxiang520.top/gtsgqruqzl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.jinyuanbaomall.cn/gtoptyifgz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.aizwys.cn/gtkirrwdwj.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.guowangkeji.top/gtfnfgmiad.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.zhixingplan.top/gtohfzdrbu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.quarkkingdee.top/gtgrorbxkx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.jqgufenzy.top/gtascbbvxq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.jyoumei.cn/gtkwboingy.html

[A07] 数字转字符串
来源：http://hz.gogol.net.cn/gtdhohtlym.html

Py:   str(42)
来源：http://hz.zdqjudy.top/gtttozgowq.html

PHP:  (string) 42; strval(42)
来源：http://hz.c1oappe.top/gtmqzhnsgi.html

JS:   String(42); (42).toString()
来源：http://hz.cheryme.top/gtyxcdjvww.html

TS:   String(42)
来源：http://hz.kuanghao11.cn/gtregnfkmw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.yongpay.top/gtokhgglyu.html

Go:   strconv.Itoa(42)
来源：http://hz.yueranfly.top/gtswvqjapb.html

Ruby: 42.to_s
来源：http://hz.sweek.top/gtytwpctzf.html

C#:   42.ToString()
来源：http://hz.chenzaomai.com/gthlmjkqgy.html

[A08] 取整与四舍五入
来源：http://hz.hnqzz.top/gtxekftefm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.dianchejie.cn/gtqrapxncm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.sweek.top/gtmdtbovgb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.hnxiangtu.top/gtjsoenaim.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xingfuxueyuan.xyz/gtnwjlwjst.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.hongshengwenyu.top/gtfqfvbfen.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.cucudq.cn/gtisjpnujq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.jiagoushi.top/gtmgrrcsii.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.fzhhl.top/gtqlhrlgif.html

[A09] 绝对值与最大最小值
来源：http://hz.yj20258.top/gtrmoitvew.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.hnqzz.top/gtuaszuids.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.havefunace.top/gtczhdalha.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.cheryme.top/gtcnfqmmnh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.guowangkeji.top/gtrzliztye.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.jiagoushi.top/gtsxekwxzc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.xuetiantiany.cn/gtvrawixrd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.smart0.xyz/gtdbjkwdxg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.shanyushiyangkeji.top/gtivnnvmuo.html

[A10] 生成随机数
来源：http://hz.zhijiandao.cn/gtbjcvuagt.html

Py:   import random; random.randint(1, 100)
来源：http://hz.xziqi.cn/gtbexnzrqe.html

PHP:  random_int(1, 100);
来源：http://hz.yj202588.top/gtshjrqpus.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.smart0.xyz/gtfduyqwej.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.sysykeji.top/gtaohhbbio.html

Java: new Random().nextInt(100) + 1
来源：http://hz.jinqigfzy.top/gtpjcenxup.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.haohaochexian.top/gtbivavhqh.html

Ruby: rand(1..100)
来源：http://hz.xuanzx.com/gtxnblvblu.html

C#:   new Random().Next(1, 101)
来源：http://hz.zhongyouzk.top/gtqtwbltvw.html

[A11] 条件表达式（三元）
来源：http://hz.cucudq.cn/gtfpkauohs.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.yangfankeji.com/gtpovzfzam.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.xylfe.cn/gtbyzuuhle.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.yonumen.top/gtogytjmtv.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.hfpthk.cn/gtgxgchjla.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtkavgvuom.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.yangfankeji.com/gtfalyjudg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.52xcode.cn/gtifzectqn.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yangfankeji.com/gtbzhquksq.html

[A12] 字符串插值 / 格式化
来源：http://hz.zhijiandao.cn/gtbbrplqfc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.tianlin.xyz/gtdwdcaocc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.birdmap.top/gtrvziyuvb.html

JS:   `Hello, ${name}!`
来源：http://hz.cheryme.top/gtnqmmhtnd.html

TS:   `Hello, ${name}!`
来源：http://hz.hywenlv.cn/gtjrvbjrne.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.shzxlz.cn/gtakfibexe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.zhengqikj.top/gtrmrsfzfr.html

Ruby: "Hello, #{name}!"
来源：http://hz.nanxinkj.top/gtmjirolqr.html

C#:   $"Hello, {name}!"
来源：http://hz.c1oappe.top/gttvmrusnc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jinqigfzy.top/gtfnnyftof.html

Py:   "第一行\n第二行"
来源：http://hz.pycfn.com/gtijtbfydq.html

PHP:  "第一行\n第二行"
来源：http://hz.zhaomingkeji.xyz/gtarqmrmxg.html

JS:   "第一行\n第二行"
来源：http://hz.sxryk.cn/gtydclfqxe.html

TS:   "第一行\n第二行"
来源：http://hz.cdnleiting.top/gtcknjqymo.html


<!-- 参考信息 -->