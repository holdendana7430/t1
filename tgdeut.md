代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://hz.mhx1999.top/gtcsejndon.html

export const a = 1;  import { a } from "./m.js";
来源：http://hz.cdnleiting.top/gtacbudrcz.html

[U84] JS：CommonJS 写法
来源：http://hz.chenjidiqi.icu/gtrqpqnuzt.html

module.exports = { a };  const { a } = require("./m");
来源：http://hz.gotoacloud.top/gtzyowxtxi.html

[U85] JS：可选链
来源：http://hz.vqdsnc.cn/gtwgiflyxf.html

a?.b?.c
来源：http://hz.sweek.top/gtrthafiow.html

[U86] JS：空值合并
来源：http://hz.tian-w.cn/gtbohrryze.html

a ?? b
来源：http://hz.meibo888.top/gtyfmlglfv.html

[U87] JS：解构默认值
来源：http://hz.c1oappe.top/gtwqmwtsdy.html

const { a = 1, b = 2 } = obj;
来源：http://hz.jinghuilouyu.cn/gtbwxddtwx.html

[U88] JS：对象展开合并
来源：http://hz.hysaishi.cn/gtknzjefhe.html

{ ...a, ...b }
来源：http://hz.guannengcc.top/gtbppdqbeo.html

[U89] JS：数组去重
来源：http://hz.dashuyun.cn/gtcmmoqobk.html

[...new Set(arr)]
来源：http://hz.ydzc1.top/gthzgpfkas.html

[U90] JS：数字数组排序
来源：http://hz.hywenlv.cn/gtvqlzduwi.html

[...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtyzacpytw.html

[U91] JS：对象键值遍历
来源：http://hz.mhx1999.top/gtbxxbeyjo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hz.xinyue.icu/gtwfovyzsh.html

[U92] JS：深拷贝
来源：http://hz.xuetiantiany.cn/gtzjopsmzu.html

structuredClone(obj)
来源：http://hz.c1oappe.top/gtwymolmgo.html

[U93] JS：模板字符串
来源：http://hz.xinyue.icu/gttasuotdb.html

`共 ${n} 条`
来源：http://hz.meibo888.top/gtvotfndhz.html

[U94] JS：箭头函数
来源：http://hz.snrcjt.cn/gtifkqfrqg.html

const double = x => x * 2;
来源：http://hz.jqgfzy.top/gtfosbvhmm.html

[U95] JS：Promise 包装
来源：http://hz.316326.xyz/gtwechwfcm.html

new Promise((resolve, reject) => {})
来源：http://hz.tianlin.xyz/gtzobfutzv.html

[U96] JS：async/await 与异常
来源：http://hz.yongpay.top/gtsbkhgicl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigufen.top/gtojfrjwrt.html

[U97] JS：并发请求
来源：http://hz.hongshengwenyu.top/gtwxtipwkh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtndekqhmm.html

[U98] JS：fetch 带 JSON
来源：http://hz.9152youxi.cn/gtcxiarcvb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hz.cqqwz.cn/gtzitwvcov.html

[U99] JS：事件监听
来源：http://hz.yanxiufei.cn/gtrnbgikhv.html

el.addEventListener("click", e => {})
来源：http://hz.yanxiufei.cn/gthjbhdwhj.html

[U100] JS：DOM 查询
来源：http://hz.chenzaomai.com/gtubqqmkzb.html

document.querySelector(".item")
来源：http://hz.ivvv.top/gtaokfqbzx.html

[U101] JS：classList 操作
来源：http://hz.jinghuilouyu.cn/gtfcvyxwit.html

el.classList.toggle("active")
来源：http://hz.sufxvd.cn/gtoxybokev.html

[U102] JS：本地存储
来源：http://hz.pycfn.com/gtchppgilr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://hz.chenzaomai.com/gtnvpivzkl.html

[U103] JS：定时器
来源：http://hz.sxryk.cn/gtlfhwnoro.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hz.chenjidiqi.icu/gtpwabingj.html

[U104] JS：防抖
来源：http://hz.xingfuxueyuan.xyz/gtmpqulqfc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hz.daria6918.cn/gtkitjlygx.html

[U105] JS：节流
来源：http://hz.shuidangran.top/gtsygomeiw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hz.dianchejie.cn/gtmkoffpxp.html

[U106] JS：日期格式化
来源：http://hz.sweek.top/gthhimtoat.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://hz.bjfxy.top/gtkpaluyqt.html

[U107] JS：数字千分位
来源：http://hz.daria6918.cn/gtjhbkciak.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hz.tanke756.top/gtcgzilvmu.html

[U108] JS：随机整数
来源：http://hz.sweek.top/gtkarzjhdf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hz.jqgufenzy.top/gthbhatjzv.html

[U109] JS：数组分组
来源：http://hz.cucudq.cn/gtrobumuls.html

Object.groupBy(arr, x => x.type)
来源：http://hz.xziqi.cn/gtxkmldmlh.html

[U110] JS：数组分块
来源：http://hz.tian-w.cn/gttqswiyme.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hz.bjfxy.top/gthlnennhl.html

[U111] JS：对象转 Map
来源：http://hz.hnqzz.top/gtmjkczzna.html

new Map(Object.entries(obj))
来源：http://hz.yj20258888.top/gtfdfgusta.html

[U112] JS：字符串补位
来源：http://hz.ydjk.org.cn/gtpmlyvubc.html

"7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtulxmbnzn.html

[U113] JS：正则替换全部
来源：http://hz.xinyue.icu/gtkrxhzrer.html

s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtaaionqny.html

[U114] JS：JSON 深比较
来源：http://hz.fengsongda.top/gtsbfvuhds.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.jinqigfzy.top/gtbhgnqbrj.html

[U115] JS：生成 UUID
来源：http://hz.yj20258888.top/gthaprdokn.html

crypto.randomUUID()
来源：http://hz.sufxvd.cn/gtgxoqhkay.html

[U116] JS：类型检查（JSDoc）
来源：http://hz.kuanghao11.cn/gtjqmjjryl.html

/** @param {string} name */ function f(name) {}
来源：http://hz.yj202588.top/gtaxovkqnp.html

[U117] JS：单元测试
来源：http://hz.yangfankeji.com/gtfyyahamk.html

npm i -D vitest;  npx vitest
来源：http://hz.gogol.net.cn/gtzkpqcttr.html

[U118] JS：开发服务器
来源：http://hz.sweek.top/gtmerpfkyz.html

npm i -D vite;  npx vite
来源：http://hz.yj20258888.top/gthfnelyxb.html

[U119] JS：生产构建
来源：http://hz.zdqjudy.top/gthmcyzeju.html

npx vite build
来源：http://hz.xingfuxueyuan.xyz/gtavduevbd.html

[U120] JS：读取环境变量（Vite）
来源：http://hz.zhiwuduotai.top/gtmvmbqpsk.html

import.meta.env.VITE_API_URL
来源：http://hz.hnqzz.top/gtgxfgqsxn.html

================================================================================
来源：http://hz.sysykeji.top/gtqewpcfxh.html

统计汇总
来源：http://hz.hysaishi.cn/gtlgenljtf.html

================================================================================
来源：http://hz.guowangkeji.top/gtkxxqgmlu.html

按语言统计（条）：
来源：http://hz.cqqwz.cn/gthsogkbij.html

Python ......... 252
来源：http://hz.ywan-chungtsiang.top/gttucdlzrj.html

PHP ............ 252
来源：http://hz.zhixingplan.top/gtoopeqtrc.html

JavaScript ..... 252
来源：http://hz.zhijiandao.cn/gtisqfdnvs.html

TypeScript ..... 212
来源：http://hz.cucudq.cn/gtivjtdwze.html

Java ........... 212
来源：http://hz.nwbrower.top/gtyfvjdtfs.html

Go ............. 212
来源：http://hz.ydzc1.top/gthnpwtcfk.html

Ruby ........... 212
来源：http://hz.jyoumei.cn/gturbtolvw.html

C# ............. 212
来源：http://hz.dianchejie.cn/gtrdvlyhxf.html

C .............. 30
来源：http://hz.jlsjyb.cn/gtsgsqkjdh.html

C++ ............ 30
来源：http://hz.yuxming.cn/gtmngnplss.html

SQL ............ 90
来源：http://hz.shangyingyoupin.top/gttrmubwzz.html

Bash ........... 80
来源：http://hz.fzhhl.top/gtrwcwksbo.html

Kotlin ......... 15
来源：http://hz.cqqwz.cn/gteqmsrqna.html

Swift .......... 15
来源：http://hz.tian-w.cn/gtohnitctw.html

Lua ............ 10
来源：http://hz.zhengqikj.top/gtzfopfcnk.html

Perl ........... 10
来源：http://hz.aizwys.cn/gtwhfecajb.html

Scala .......... 10
来源：http://hz.shanyushiyangkeji.top/gttcwebjae.html

------------------------------------
来源：http://hz.shzxlz.cn/gtskgbsfmz.html

合计 ........... 2106 条
来源：http://hz.zhengqikj.top/gtxqdwxtnw.html

按章节统计：
来源：http://hz.jqgfzy.top/gtabfzekyy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hz.gogol.net.cn/gtxetntcnp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hz.meibo888.top/gtknjcmnwz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hz.fengsongda.top/gtvtqsnuwq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hz.haohaochexian.top/gtczajrosy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://hz.zdqjudy.top/gtqjxgdxph.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hz.yuxming.cn/gtmjejqjvz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hz.jinyuanbaomall.cn/gtjgawxlwr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hz.sufxvd.cn/gtakzgbomy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hz.nanxinkj.top/gtrkkrwhmz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hz.tanke756.top/gtyabzezxd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://hz.hnqzz.top/gtkuofpesj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hz.zhijiandao.cn/gtmgvmqejs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hz.redwolf501.top/gtjdeszfae.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hz.cucudq.cn/gtrhvdeluy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hz.zhiwuduotai.top/gtoqdjydfa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hz.nanxuanxn.top/gtnzkfwprm.html

Q SQL 专题                              90
来源：http://hz.quarkkingdee.top/gtszlztleu.html

R Bash 专题                             80
来源：http://hz.hfpthk.cn/gtepxsildj.html

S C / C++ 专题                          60
来源：http://hz.jiagoushi.top/gtnhjtkjjs.html

T 其他语言补充                          60
来源：http://hz.ywan-chungtsiang.top/gtkxpgezzk.html

U 高频实用片段                         120
来源：http://hz.smart0.xyz/gtwyzfxalt.html

------------------------------------
来源：http://hz.yanxiufei.cn/gtotjnvjfi.html

合计                                  2106 条
来源：http://hz.hysaishi.cn/gtllipscmo.html

--------------------------------------------------------------------------------
来源：http://hz.cdnleiting.top/gtvqqasnpf.html

使用提醒
来源：http://hz.shangyingyoupin.top/gtoftjream.html

--------------------------------------------------------------------------------
来源：http://hz.xuetiantiany.cn/gtruoebmyn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hz.yonumen.top/gtvrfqccki.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hz.chenjidiqi.icu/gtyckhlqth.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hz.yueranfly.top/gtvbuvcaok.html

在旧版本上使用前请先确认语法支持情况。
来源：http://hz.yonumen.top/gtqccdpqov.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hz.birdmap.top/gtvchzfagc.html

—— 文件结束 ——
来源：http://hz.ybcxt.top/gtlurxdyxl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtrguwljao.html

程序语言常见例子速查手册（2024 版）
来源：http://hz.fzhhl.top/gtnvdjnhuu.html

Common Programming Examples Cheat Book
来源：http://hz.ybcxt.top/gtabxeoxwv.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtfqgbhahs.html

【收录内容】
来源：http://hz.cashguo.top/gtdpgccyvz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://hz.yuxming.cn/gthejizebm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hz.aibaodan.cn/gtljvgiunf.html

SQL · Bash · C · C++
来源：http://hz.hfpthk.cn/gtlnrxjqgs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hz.zycfv.cn/gtwqsyqkbu.html

【使用说明】
来源：http://hz.zhixingplan.top/gtidlstecy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hz.yonumen.top/gtnhcbylrd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hz.nanxuanxn.top/gtnouliurq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hz.ybcxt.top/gtkayxwxti.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hz.tanke756.top/gtibztqzor.html

Bash:  Shell         C:     C             C++:   C++
来源：http://hz.yanxiufei.cn/gtkxodtafc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hz.jiagoushi.top/gtitgtivzx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hz.shanyushiyangkeji.top/gthsdortub.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hz.hywenlv.cn/gtgiqshsop.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hz.52xcode.cn/gttzixvgjr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hz.jqgufenzy.top/gtbuotcuao.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.ehwqpu.com/gttzozuwed.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hz.mhx1999.top/gtiqvhjiis.html

【文件统计】
来源：http://hz.dashuyun.cn/gtoydhcwol.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hz.haohaochexian.top/gtwxebzboc.html

--------------------------------------------------------------------------------
来源：http://hz.yj20258888.top/gtuatprmtl.html

目  录
来源：http://hz.snrcjt.cn/gtcwyxhwlu.html

--------------------------------------------------------------------------------
来源：http://hz.svipenyu.cn/gtwzhozyba.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hz.fzhhl.top/gtlakcgghq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hz.tianlin.xyz/gtwxygmkii.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hz.chenlongwang.top/gtaemynayx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hz.sysykeji.top/gtxirpbudh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hz.aibaodan.cn/gtidlkweaa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.zhoulong.xyz/gttnnezrir.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.xuanzx.com/gtcivahfgs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.daxiang520.top/gtpqsmtwqg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hz.shzxlz.cn/gtownvuvaj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hz.tanke756.top/gteotvrudo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hz.yj20258888.top/gtxpxdqexo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hz.svipenyu.cn/gtgibphqoa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hz.ivvv.top/gtlukezdos.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hz.zhaomingkeji.xyz/gtjxtznupe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hz.chenzaomai.com/gtsikiiaiq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hz.guannengcc.top/gthnlkzhid.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.cdnleiting.top/gtdxwwinen.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://hz.chenlongwang.top/gtafonvaof.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hz.xuanzx.com/gtpnqcxnoc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtxfuqwzom.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hz.jianghu66.top/gtgwxbhgwi.html

================================================================================
来源：http://hz.c1oappe.top/gtyvwjjbrg.html

A. 基础语法与类型
来源：http://hz.ehwqpu.com/gtkxohrops.html

================================================================================
来源：http://hz.meibo888.top/gttfcecgoe.html

[A01] Hello World
来源：http://hz.zhiwuduotai.top/gtlowpsllg.html

Py:   print("Hello, World!")
来源：http://hz.hfpthk.cn/gtojcbkqil.html

PHP:  echo "Hello, World!";
来源：http://hz.dianchejie.cn/gtyepnuhma.html

JS:   console.log("Hello, World!");
来源：http://hz.wangshuangyany.cn/gtessliiok.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hz.feifeiyinyue.top/gtlazuqraa.html

Java: System.out.println("Hello, World!");
来源：http://hz.316326.xyz/gtdhvfpwqb.html

Go:   fmt.Println("Hello, World!")
来源：http://hz.ydzc1.top/gtsqqleopl.html

Ruby: puts "Hello, World!"
来源：http://hz.zycfv.cn/gtiogntedk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://hz.chenzaomai.com/gtyqarsbzl.html

[A02] 变量声明与赋值
来源：http://hz.xziqi.cn/gtmvhcbxzf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hz.xylfe.cn/gtsdapklyz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://hz.tian-w.cn/gtpmkhizst.html

JS:   let name = "Alex"; const age = 20;
来源：http://hz.sxryk.cn/gtqotmslgs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hz.nanxuanxn.top/gtdmzqcyjh.html

Java: String name = "Alex"; int age = 20;
来源：http://hz.shzxlz.cn/gtwtbyiexi.html

Go:   name := "Alex"; age := 20
来源：http://hz.xylfe.cn/gtwnytpywo.html

Ruby: name = "Alex"; age = 20
来源：http://hz.jinqigufen.top/gtdooizfus.html

C#:   string name = "Alex"; int age = 20;
来源：http://hz.hnxiangtu.top/gtnbnswblc.html

[A03] 常量定义
来源：http://hz.zhijiandao.cn/gtkaqxiyiw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hz.feifeiyinyue.top/gtckdpbvtr.html

PHP:  const PI = 3.14159;
来源：http://hz.shuidangran.top/gtmoaepssm.html

JS:   const PI = 3.14159;
来源：http://hz.daxiang520.top/gtfhmgnbal.html

TS:   const PI: number = 3.14159;
来源：http://hz.tanke756.top/gtjiswvwcb.html

Java: static final double PI = 3.14159;
来源：http://hz.zycfv.cn/gtoqcnfgfw.html

Go:   const PI = 3.14159
来源：http://hz.bjfxy.top/gtlaueuldp.html

Ruby: PI = 3.14159
来源：http://hz.aibaodan.cn/gtwuaiitio.html

C#:   const double PI = 3.14159;
来源：http://hz.guowangkeji.top/gtlbewppvs.html

[A04] 判断变量类型
来源：http://hz.xinyue.icu/gtwgkundgh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://hz.dashuyun.cn/gtizfvvcnl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hz.shanyushiyangkeji.top/gtgvslgyto.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hz.yvedp.cn/gtryzxfyhq.html

TS:   typeof x; x instanceof Date
来源：http://hz.hywenlv.cn/gtqlofirxh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hz.ppjwa.cn/gtzwdelibt.html

Go:   reflect.TypeOf(x).Name()
来源：http://hz.hnxiangtu.top/gtmdutmdun.html

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.xziqi.cn/gtonfmohxu.html

C#:   x.GetType().Name; x is int
来源：http://hz.gaohongyu789.top/gthuvphcdi.html

[A05] 整数除法与取模
来源：http://hz.zdqjudy.top/gteuwizeqd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hz.shuidangran.top/gtbcjazbqi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://hz.yueranfly.top/gtlsnxoidl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.svipenyu.cn/gtewghhlms.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.jinghuilouyu.cn/gtigficbbj.html

Java: 7 / 2; 7 % 2
来源：http://hz.nanxinkj.top/gtzpaalzbo.html

Go:   7 / 2; 7 % 2
来源：http://hz.hongshengwenyu.top/gtiyykpejb.html

Ruby: 7 / 2; 7 % 2
来源：http://hz.shanyushiyangtech.top/gthdrruqde.html

C#:   7 / 2; 7 % 2
来源：http://hz.zycfv.cn/gtobpkrofc.html

[A06] 字符串转数字
来源：http://hz.jlsjyb.cn/gtswvzewly.html

Py:   int("42"); float("3.14")
来源：http://hz.svipenyu.cn/gtqspteqho.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hz.xuetiantiany.cn/gtxosfwsut.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hz.pengpengdd.cyou/gtstnbwqgx.html

TS:   parseInt("42", 10); Number("42")
来源：http://hz.pycfn.com/gtnzcubbvv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hz.vqdsnc.cn/gtjxsnfuuv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hz.meibo888.top/gtghpfhbyf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://hz.feifeiyinyue.top/gtdhjdimiw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.shzxlz.cn/gtqqxavkyr.html

[A07] 数字转字符串
来源：http://hz.daxiang520.top/gtenqvuhdq.html

Py:   str(42)
来源：http://hz.ydjk.org.cn/gtyyzhvbdx.html

PHP:  (string) 42; strval(42)
来源：http://hz.haohaochexian.top/gtofepdhnm.html

JS:   String(42); (42).toString()
来源：http://hz.xziqi.cn/gtvcfboulj.html

TS:   String(42)
来源：http://hz.snrcjt.cn/gtuoossyux.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.shanyushiyangkeji.top/gtcdlczoxe.html

Go:   strconv.Itoa(42)
来源：http://hz.hywenlv.cn/gtoujouojq.html

Ruby: 42.to_s
来源：http://hz.zycfv.cn/gttsrwmcyp.html

C#:   42.ToString()
来源：http://hz.xziqi.cn/gtdnyvkxpw.html

[A08] 取整与四舍五入
来源：http://hz.xinyue.icu/gtgtfmzvfr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.zhongyouzk.top/gtmyvdpehd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.mhx1999.top/gtzwbgtrbd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.redwolf501.top/gtnwcuijqy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.xingfuxueyuan.xyz/gtmquxhrae.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.cqqwz.cn/gtkjbydism.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.daxiang520.top/gttlhiudne.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.zhoulong.xyz/gtvzqnfytr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.iojbl.cn/gtzrvgxoov.html

[A09] 绝对值与最大最小值
来源：http://hz.cheryme.top/gthfyofgly.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jyoumei.cn/gtnzoturto.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.ehwqpu.com/gtyhtgsrfx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.hywenlv.cn/gtqqcfvray.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.cdnleiting.top/gtzeecisls.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.cdnleiting.top/gtrivfrisl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.jlsjyb.cn/gtefszrwmw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.aibaodan.cn/gtctiuvhre.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.zhengqikj.top/gttcvetwfa.html

[A10] 生成随机数
来源：http://hz.jinyuanbaomall.cn/gtknffhwxk.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hysaishi.cn/gtryfihsvl.html

PHP:  random_int(1, 100);
来源：http://hz.vqdsnc.cn/gtdnhoeydw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.xingfuxueyuan.xyz/gtmiyubbie.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.redwolf501.top/gtiggmbzwg.html

Java: new Random().nextInt(100) + 1
来源：http://hz.tianlin.xyz/gtnlmpfojl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.snrcjt.cn/gtqmgiaijj.html

Ruby: rand(1..100)
来源：http://hz.nanxuanxn.top/gtuilfzejy.html

C#:   new Random().Next(1, 101)
来源：http://hz.sufxvd.cn/gtkvnzozmv.html

[A11] 条件表达式（三元）
来源：http://hz.ehwqpu.com/gtqynhyfoc.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.zdqjudy.top/gtnbwtcesh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.hongshengwenyu.top/gtrtoiiswt.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.hnqzz.top/gtcgtsbwka.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.zhixingplan.top/gttartvvfc.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.tianlin.xyz/gtsfxlsehy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.hammf.cn/gtrgvorofv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.ehwqpu.com/gtfloltktd.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.sxryk.cn/gthopbhzrs.html

[A12] 字符串插值 / 格式化
来源：http://hz.shangyingyoupin.top/gtzdmjwgtx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.yueranfly.top/gtnyrvuvlh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.sweek.top/gtbuhbbhgu.html

JS:   `Hello, ${name}!`
来源：http://hz.yvedp.cn/gtpvmjwull.html

TS:   `Hello, ${name}!`
来源：http://hz.kuanghao11.cn/gtdhcibfwe.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.mhx1999.top/gtthmltncj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.dianchejie.cn/gtbfegdftf.html

Ruby: "Hello, #{name}!"
来源：http://hz.wangdashe.top/gtohmcwlcv.html

C#:   $"Hello, {name}!"
来源：http://hz.daria6918.cn/gtwkfmqpka.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.jianghu66.top/gtgfktokbj.html

Py:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtryrytime.html

PHP:  "第一行\n第二行"
来源：http://hz.jinqigfzy.top/gtmcbyjrvy.html

JS:   "第一行\n第二行"
来源：http://hz.shangyingyoupin.top/gtasdtxygw.html

TS:   "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtyjzgsfjr.html

Java: "第一行\n第二行"
来源：http://hz.pengpengdd.cyou/gtgbpittdk.html

Go:   "第一行\n第二行"
来源：http://hz.sysykeji.top/gtazrlfear.html

Ruby: "第一行\n第二行"
来源：http://hz.chenzaomai.com/gtrnhfvuai.html

C#:   "第一行\n第二行"
来源：http://hz.cucudq.cn/gtlotficfv.html


<!-- 参考信息 -->