代发 wailian999

[U81] JS：初始化项目
来源：http://hz.tanke756.top/gtpekashom.html

npm init -y;  npm i express
来源：http://hz.jqgfzy.top/gtgtgewmyt.html

[U82] JS：package.json 脚本
来源：http://hz.jinyuanbaomall.cn/gtxhraavlw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hz.zhiwuduotai.top/gtxveqlatg.html

[U83] JS：ES Module 导入导出
来源：http://hz.hysaishi.cn/gtgjfoacac.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.yangfankeji.com/gtltfacqtt.html

[U84] JS：CommonJS 写法
来源：http://hz.havefunace.top/gtvernizet.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.yvedp.cn/gthgbephbb.html

[U85] JS：可选链
来源：http://hz.zhaomingkeji.xyz/gtpcheyzxj.html

a?.b?.c
来源：http://hz.zhixingplan.top/gtupnzbtsm.html

[U86] JS：空值合并
来源：http://hz.cheryme.top/gtmugsbspw.html

a ?? b
来源：http://hz.yonumen.top/gtvetcqpge.html

[U87] JS：解构默认值
来源：http://hz.ivvv.top/gtgsdxmeoq.html

const { a = 1, b = 2 } = obj;
来源：http://hz.sweek.top/gtbivwutfj.html

[U88] JS：对象展开合并
来源：http://hz.chenzaomai.com/gtqbchojfh.html

{ ...a, ...b }
来源：http://hz.chenlongwang.top/gtkvyhfwln.html

[U89] JS：数组去重
来源：http://hz.zhiwuduotai.top/gtzsweqlgf.html

[...new Set(arr)]
来源：http://hz.nwbrower.top/gtjqmaujwt.html

[U90] JS：数字数组排序
来源：http://hz.fengsongda.top/gttrvylpgf.html

[...arr].sort((a, b) => a - b)
来源：http://hz.guowangkeji.top/gtckvirxph.html

[U91] JS：对象键值遍历
来源：http://hz.smart0.xyz/gtdtuydheq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.cqqwz.cn/gtvwvachsq.html

[U92] JS：深拷贝
来源：http://hz.sufxvd.cn/gtawqjdnis.html

structuredClone(obj)
来源：http://hz.chenzaomai.com/gtpzapanbm.html

[U93] JS：模板字符串
来源：http://hz.sufxvd.cn/gtjppbiogp.html

`共 ${n} 条`
来源：http://hz.52xcode.cn/gtodffqwqq.html

[U94] JS：箭头函数
来源：http://hz.jianghu66.top/gtxgsjwbrt.html

const double = x => x * 2;
来源：http://hz.dashuyun.cn/gthdazppvk.html

[U95] JS：Promise 包装
来源：http://hz.guannengcc.top/gtvheuungd.html

new Promise((resolve, reject) => {})
来源：http://hz.yangfankeji.com/gtsrvhfibm.html

[U96] JS：async/await 与异常
来源：http://hz.xinyue.icu/gtsnvjamya.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtpaqonerd.html

[U97] JS：并发请求
来源：http://hz.yj202588.top/gtcthiihvf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sxryk.cn/gtejoowvau.html

[U98] JS：fetch 带 JSON
来源：http://hz.zhengqikj.top/gtbztzyois.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.haohaochexian.top/gtfhdbweic.html

[U99] JS：事件监听
来源：http://hz.hongshengwenyu.top/gtnqnfokse.html

el.addEventListener("click", e => {})
来源：http://hz.yj202588.top/gtmhghmmxg.html

[U100] JS：DOM 查询
来源：http://hz.shzxlz.cn/gtalyxmodg.html

document.querySelector(".item")
来源：http://hz.meibo888.top/gtoffiupls.html

[U101] JS：classList 操作
来源：http://hz.daxiang520.top/gtispedght.html

el.classList.toggle("active")
来源：http://hz.sysykeji.top/gtvchavekz.html

[U102] JS：本地存储
来源：http://hz.zhongyouzk.top/gtqgsjmoiy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.shzxlz.cn/gtfeebycdp.html

[U103] JS：定时器
来源：http://hz.pengpengdd.cyou/gttsyzygbv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.zhixingplan.top/gtsufkevkd.html

[U104] JS：防抖
来源：http://hz.cqqwz.cn/gtoisvmedi.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.hnxiangtu.top/gthuqorstr.html

[U105] JS：节流
来源：http://hz.jinqigfzy.top/gtwfabxemh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.hnxiangtu.top/gtwsbnsvae.html

[U106] JS：日期格式化
来源：http://hz.jianghu66.top/gtsiboyinq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.316326.xyz/gtdvazsnzk.html

[U107] JS：数字千分位
来源：http://hz.sxryk.cn/gtbrmrwldv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.snrcjt.cn/gtqsvbrlyk.html

[U108] JS：随机整数
来源：http://hz.yj20258.top/gtgeyjbctw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.yj20258.top/gtqvtpnerk.html

[U109] JS：数组分组
来源：http://hz.hfpthk.cn/gtdwxubeau.html

Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtixscuyeh.html

[U110] JS：数组分块
来源：http://hz.tanke756.top/gtrbxvkroa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.gzhubu.top/gtfjutoxes.html

[U111] JS：对象转 Map
来源：http://hz.yonumen.top/gtldqlnkrk.html

new Map(Object.entries(obj))
来源：http://hz.wangshuangyany.cn/gtdcvatwxg.html

[U112] JS：字符串补位
来源：http://hz.vqdsnc.cn/gtwerwdvcz.html

"7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtgoifoura.html

[U113] JS：正则替换全部
来源：http://hz.shanyushiyangkeji.top/gtkaffviax.html

s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtiksohftv.html

[U114] JS：JSON 深比较
来源：http://hz.xingfuxueyuan.xyz/gthiubneep.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.birdmap.top/gtrudyytbp.html

[U115] JS：生成 UUID
来源：http://hz.zhixingplan.top/gtecyvqiwc.html

crypto.randomUUID()
来源：http://hz.xuetiantiany.cn/gtbzuzegie.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.wangdashe.top/gtyugaxucj.html

/** @param {string} name */ function f(name) {}
来源：http://hz.pengpengdd.cyou/gtitcqimud.html

[U117] JS：单元测试
来源：http://hz.cashguo.top/gtczhamfdm.html

npm i -D vitest;  npx vitest
来源：http://hz.shanyushiyangtech.top/gtfnduwfxk.html

[U118] JS：开发服务器
来源：http://hz.wangshuangyany.cn/gtlimpwxzm.html

npm i -D vite;  npx vite
来源：http://hz.sweek.top/gtjpoizoqi.html

[U119] JS：生产构建
来源：http://hz.fengsongda.top/gtchafhtoq.html

npx vite build
来源：http://hz.gogol.net.cn/gtgximdwfs.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.kuanghao11.cn/gtankmzhza.html

import.meta.env.VITE_API_URL
来源：http://hz.ydjk.org.cn/gtoxtwzjqk.html

================================================================================
来源：http://hz.yvedp.cn/gttodxdbnr.html

统计汇总
来源：http://hz.ppjwa.cn/gttvfcmwiz.html

================================================================================
来源：http://hz.snrcjt.cn/gtqhuxwmvj.html

按语言统计（条）：
来源：http://hz.tanke756.top/gtpqnzrewd.html

Python ......... 252
来源：http://hz.ydzc1.top/gtwrleqvxw.html

PHP ............ 252
来源：http://hz.sxryk.cn/gtvcrynlrp.html

JavaScript ..... 252
来源：http://hz.pengpengdd.cyou/gtnatouxue.html

TypeScript ..... 212
来源：http://hz.jinqigufen.top/gtbinokjjr.html

Java ........... 212
来源：http://hz.xinyue.icu/gtymcpqbqt.html

Go ............. 212
来源：http://hz.316326.xyz/gtdderonhh.html

Ruby ........... 212
来源：http://hz.nanxuanxn.top/gtkeiljtqf.html

C# ............. 212
来源：http://hz.andypj.xyz/gtpaygzgew.html

C .............. 30
来源：http://hz.xziqi.cn/gtspprhbxy.html

C++ ............ 30
来源：http://hz.birdmap.top/gtetfdrrni.html

SQL ............ 90
来源：http://hz.chenlongwang.top/gtdcuklach.html

Bash ........... 80
来源：http://hz.yuxming.cn/gtnpyefvvb.html

Kotlin ......... 15
来源：http://hz.hfpthk.cn/gtcgglzkui.html

Swift .......... 15
来源：http://hz.sweek.top/gthldtgvlk.html

Lua ............ 10
来源：http://hz.ivvv.top/gtjerhxtig.html

Perl ........... 10
来源：http://hz.sufxvd.cn/gtnvlrnxmd.html

Scala .......... 10
来源：http://hz.cashguo.top/gthtsjkbfq.html

------------------------------------
来源：http://hz.yonumen.top/gtnhdmrnkb.html

合计 ........... 2106 条
来源：http://hz.sweek.top/gtlhtvvaxv.html

按章节统计：
来源：http://hz.zhixingplan.top/gtnslqbsss.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.iojbl.cn/gtkrgzfcfw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.yuxming.cn/gtjkamlvgm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.yj20258.top/gtymiznlpm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.shuidangran.top/gtwktxrjqs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.jyoumei.cn/gtxzjhobcj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.wangdashe.top/gtqpgxkpsf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.9152youxi.cn/gtdrsifsal.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.chenlongwang.top/gtyalvindd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.hysaishi.cn/gtsizqzpan.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.guowangkeji.top/gtkonuocxz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.iojbl.cn/gtmiirfrpx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.hywenlv.cn/gtibeskuur.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.tian-w.cn/gtpuhnaugl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.hysaishi.cn/gtyohokhxa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.yanxiufei.cn/gtamaemvxj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.zhongyouzk.top/gtelhuyjpx.html

Q SQL 专题                              90
来源：http://hz.jinyuanbaomall.cn/gtsevbcpkz.html

R Bash 专题                             80
来源：http://hz.c1oappe.top/gtufscjqjs.html

S C / C++ 专题                          60
来源：http://hz.zhixingplan.top/gtvtvptyrh.html

T 其他语言补充                          60
来源：http://hz.tianlin.xyz/gtwhjtcsgx.html

U 高频实用片段                         120
来源：http://hz.gogol.net.cn/gtirskeuzg.html

------------------------------------
来源：http://hz.yangfankeji.com/gtuokqxsvi.html

合计                                  2106 条
来源：http://hz.cheryme.top/gtypsrmycz.html

--------------------------------------------------------------------------------
来源：http://hz.vqdsnc.cn/gtqyjlfdxx.html

使用提醒
来源：http://hz.jinqigfzy.top/gtsjgjbqsr.html

--------------------------------------------------------------------------------
来源：http://hz.chenzaomai.com/gtjkqvbzam.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.pycfn.com/gtjgmtxunz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.nanxinkj.top/gttyifmltb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.nanxinkj.top/gteklzbrnh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.sufxvd.cn/gtqszxybcj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.jinyuanbaomall.cn/gtbderoqhm.html

—— 文件结束 ——
来源：http://hz.havefunace.top/gtpjibtjfj.html

================================================================================
来源：http://hz.ybcxt.top/gtdmoalttn.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.smart0.xyz/gtbaeinzft.html

Common Programming Examples Cheat Book
来源：http://hz.kuanghao11.cn/gtammiadhe.html

================================================================================
来源：http://hz.svipenyu.cn/gtqqzmfhzq.html

【收录内容】
来源：http://hz.xinyue.icu/gtyqtkbucj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yonumen.top/gtkydfzkee.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.jqgfzy.top/gtyzruqojw.html

SQL · Bash · C · C++
来源：http://hz.wangshuangyany.cn/gtodyilbiy.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.gzhubu.top/gtodjbrszt.html

【使用说明】
来源：http://hz.guannengcc.top/gtdfhnhocc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.guowangkeji.top/gtsswtvqst.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.zhaomingkeji.xyz/gtagekiqyd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.zhaomingkeji.xyz/gtyyxzmadt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.snrcjt.cn/gthuufaurk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.shzxlz.cn/gtagqpprld.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.ehwqpu.com/gtjduzaghi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.yuxming.cn/gtpigxasdc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.0kj1m.cn/gtqffhpetl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.zdqjudy.top/gtcezjtfhr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.zhijiandao.cn/gtmcsubdio.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.cdnleiting.top/gtshbowxan.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.ybcxt.top/gtbdxwqaax.html

【文件统计】
来源：http://hz.hysaishi.cn/gtcgfcvqpi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.shangyingyoupin.top/gtjkewjhcu.html

--------------------------------------------------------------------------------
来源：http://hz.snrcjt.cn/gtzphmbzww.html

目  录
来源：http://hz.jianghu66.top/gtbhauspux.html

--------------------------------------------------------------------------------
来源：http://hz.guowangkeji.top/gthzfcrkyw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.wangshuangyany.cn/gtfulinjis.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.zycfv.cn/gtwovkgutj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.zhaomingkeji.xyz/gtxpmobbqs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.9152youxi.cn/gthoxgtmem.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.havefunace.top/gtxemysvfg.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.feifeiyinyue.top/gtvqwzmrcm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.guannengcc.top/gtdaecbzsq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.zhoulong.xyz/gtvgzxgtkc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.hongshengwenyu.top/gtkbqmpcob.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.gzhubu.top/gtsyxvbbqd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.xingfuxueyuan.xyz/gthtpbobxt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.ydzc1.top/gtfywnkomq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ehwqpu.com/gtdwzfwpzv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.daxiang520.top/gtjhjrqvnh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.yuxming.cn/gtjzgupdez.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.shuidangran.top/gtthquwdnu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.jianghu66.top/gtqojstpsr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.zhaomingkeji.xyz/gttvpoogcj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.sweek.top/gtychmpysa.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.pycfn.com/gtkofhubvg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.tian-w.cn/gtinnhqqml.html

================================================================================
来源：http://hz.cashguo.top/gttmsovmph.html

A. 基础语法与类型
来源：http://hz.tian-w.cn/gtupqmnmyz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbqmsesft.html

[A01] Hello World
来源：http://hz.cheryme.top/gtorqkinll.html

Py:   print("Hello, World!")
来源：http://hz.jinqigfzy.top/gtxdyqwceb.html

PHP:  echo "Hello, World!";
来源：http://hz.guowangkeji.top/gtextmyctc.html

JS:   console.log("Hello, World!");
来源：http://hz.yueranfly.top/gtplqqkwwp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.zhiwuduotai.top/gthmoqtuyl.html

Java: System.out.println("Hello, World!");
来源：http://hz.yueranfly.top/gtpouhqfav.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.cqqwz.cn/gtyjozmtqg.html

Ruby: puts "Hello, World!"
来源：http://hz.hysaishi.cn/gthplonbwi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.ppjwa.cn/gttfdighxa.html

[A02] 变量声明与赋值
来源：http://hz.zhaomingkeji.xyz/gtuyfihznj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.ivvv.top/gtwlvbxdtj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.shanyushiyangtech.top/gthuxpxtvc.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.gotoacloud.top/gtwhwiajwv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.zhixingplan.top/gtzxhiqtpq.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.guannengcc.top/gtibsawgfy.html

Go:   name := "Alex"; age := 20
来源：http://hz.c1oappe.top/gtganzflrf.html

Ruby: name = "Alex"; age = 20
来源：http://hz.xylfe.cn/gtixmsrdqi.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hammf.cn/gtojnfcxph.html

[A03] 常量定义
来源：http://hz.xziqi.cn/gtknrzehvl.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.gotoacloud.top/gtehhpcxrq.html

PHP:  const PI = 3.14159;
来源：http://hz.birdmap.top/gtahsnajil.html

JS:   const PI = 3.14159;
来源：http://hz.shzxlz.cn/gtaknpaytd.html

TS:   const PI: number = 3.14159;
来源：http://hz.gogol.net.cn/gtoaixnyzp.html

Java: static final double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtcttvvypj.html

Go:   const PI = 3.14159
来源：http://hz.fengsongda.top/gtpvfrltwt.html

Ruby: PI = 3.14159
来源：http://hz.nanxinkj.top/gtzhftkxpa.html

C#:   const double PI = 3.14159;
来源：http://hz.ybcxt.top/gtnekmfhcv.html

[A04] 判断变量类型
来源：http://hz.haohaochexian.top/gtuyidnxmy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.ivvv.top/gtpnddoode.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shanyushiyangtech.top/gtqkjslmef.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.hnxiangtu.top/gtgddqhxux.html

TS:   typeof x; x instanceof Date
来源：http://hz.hnxiangtu.top/gtouxcxebk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.quarkkingdee.top/gtlvhljlww.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.tanke756.top/gtpicwduzh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.aibaodan.cn/gtvxfbgjjv.html

C#:   x.GetType().Name; x is int
来源：http://hz.jinqigufen.top/gtzqssvcmb.html

[A05] 整数除法与取模
来源：http://hz.ppjwa.cn/gtdrpivsrk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.meibo888.top/gtmperqtzk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.tanke756.top/gtsqouarvh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.yj20258.top/gtqfvitbhx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtkubqlxgr.html

Java: 7 / 2; 7 % 2
来源：http://hz.jiagoushi.top/gtkiivfhtb.html

Go:   7 / 2; 7 % 2
来源：http://hz.aizwys.cn/gtuzmudomf.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gtbtjkgvtx.html

C#:   7 / 2; 7 % 2
来源：http://hz.haohaochexian.top/gtmkfxxiaw.html

[A06] 字符串转数字
来源：http://hz.wangdashe.top/gtzogmluaz.html

Py:   int("42"); float("3.14")
来源：http://hz.wangdashe.top/gtbwniljfm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.snrcjt.cn/gtgfrydgxg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.zhengqikj.top/gthqzznhti.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.jinghuilouyu.cn/gtfsyvrxys.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.ivvv.top/gtcvjmlzow.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.xuanzx.com/gtfdxdyexs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.ivvv.top/gtwxyyjawl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.hongshengwenyu.top/gtfqmgibhl.html

[A07] 数字转字符串
来源：http://hz.hongshengwenyu.top/gtygtiohqw.html

Py:   str(42)
来源：http://hz.zhongyouzk.top/gtmaryaouf.html

PHP:  (string) 42; strval(42)
来源：http://hz.zhoulong.xyz/gthwoifspf.html

JS:   String(42); (42).toString()
来源：http://hz.shzxlz.cn/gtfimioxlq.html

TS:   String(42)
来源：http://hz.9152youxi.cn/gtaarvzmti.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shzxlz.cn/gtgsfwyyfr.html

Go:   strconv.Itoa(42)
来源：http://hz.smart0.xyz/gtbgbrjnsx.html

Ruby: 42.to_s
来源：http://hz.ydjk.org.cn/gtgjnjigmh.html

C#:   42.ToString()
来源：http://hz.smart0.xyz/gtvdudxufm.html

[A08] 取整与四舍五入
来源：http://hz.xylfe.cn/gtgajibjsg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.cdnleiting.top/gtztqyshkh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.hywenlv.cn/gtasmlzetk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.shanyushiyangkeji.top/gtemakdmtz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.9152youxi.cn/gtllezbhgn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.ywan-chungtsiang.top/gthotyfvug.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.zhiwuduotai.top/gthmuiluah.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.shuidangran.top/gtaixfhssz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.jqgufenzy.top/gtxpqmehtu.html

[A09] 绝对值与最大最小值
来源：http://hz.shzxlz.cn/gtwnabsfoi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jqgfzy.top/gtmrsgyidr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.zhongyouzk.top/gtxjdracjv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.xingfuxueyuan.xyz/gthcdutqqt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.shzxlz.cn/gtuehqsnpd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.hfpthk.cn/gtikaegzvm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.aizwys.cn/gtntuwiktw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.gaohongyu789.top/gtiiughyvy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.pycfn.com/gtckcnevch.html

[A10] 生成随机数
来源：http://hz.fengsongda.top/gteahdypbz.html

Py:   import random; random.randint(1, 100)
来源：http://hz.daxiang520.top/gterodzuio.html

PHP:  random_int(1, 100);
来源：http://hz.guannengcc.top/gtpczphvme.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.jqgfzy.top/gtohhncxjc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtxyevfhgt.html

Java: new Random().nextInt(100) + 1
来源：http://hz.zhengqikj.top/gtmdadqtgl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.yj202588.top/gtpfuwgxja.html

Ruby: rand(1..100)
来源：http://hz.shanyushiyangtech.top/gtzxpxutxf.html

C#:   new Random().Next(1, 101)
来源：http://hz.guannengcc.top/gtpmfclpot.html

[A11] 条件表达式（三元）
来源：http://hz.daxiang520.top/gttxjnxbvh.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.shuidangran.top/gtpfotzlap.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.quarkkingdee.top/gtijlslwri.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.9152youxi.cn/gtzoxsgtzw.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.yj202588.top/gtilacyean.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.feifeiyinyue.top/gtckpxeatm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.hywenlv.cn/gtvwxkckna.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.cashguo.top/gtmdzyvscg.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.yanxiufei.cn/gttunebznh.html

[A12] 字符串插值 / 格式化
来源：http://hz.yj20258.top/gtbfkrmdob.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.cqqwz.cn/gtadebcdeu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.0kj1m.cn/gttcxzzwyb.html

JS:   `Hello, ${name}!`
来源：http://hz.tanke756.top/gtikavijjp.html

TS:   `Hello, ${name}!`
来源：http://hz.redwolf501.top/gtxjaixiay.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.sysykeji.top/gttbdaalnr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.jlsjyb.cn/gtrgiqwlak.html

Ruby: "Hello, #{name}!"
来源：http://hz.jinghuilouyu.cn/gtqcjxpeuq.html

C#:   $"Hello, {name}!"
来源：http://hz.ywan-chungtsiang.top/gtjtlyzrnz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.yvedp.cn/gtepvdszas.html

Py:   "第一行\n第二行"
来源：http://hz.zhongyouzk.top/gtkkzosyod.html

PHP:  "第一行\n第二行"
来源：http://hz.hfpthk.cn/gtcafbvvft.html

JS:   "第一行\n第二行"
来源：http://hz.shzxlz.cn/gtpjyxjtol.html

TS:   "第一行\n第二行"
来源：http://hz.quarkkingdee.top/gtdvklhkdi.html


<!-- 参考信息 -->