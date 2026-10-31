代发 wailian999

[U85] JS：可选链
来源：http://ri.yuexingan06.cn

a?.b?.c
来源：http://az.shxzskj.cn

[U86] JS：空值合并
来源：http://no.muxihuayi.cn

a ?? b
来源：http://ux.colortex.cn

[U87] JS：解构默认值
来源：http://jw.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://qz.9csxet.cn

[U88] JS：对象展开合并
来源：http://tg.szsharing.cn

{ ...a, ...b }
来源：http://az.haigaiapp.cn

[U89] JS：数组去重
来源：http://nt.panjiajie.cn

[...new Set(arr)]
来源：http://js.asd995.cn

[U90] JS：数字数组排序
来源：http://rk.nszjky.cn

[...arr].sort((a, b) => a - b)
来源：http://df.newstarts.cn

[U91] JS：对象键值遍历
来源：http://wn.huixinmuqiang.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xk.huanxung.cn

[U92] JS：深拷贝
来源：http://cm.hahajie.cn

structuredClone(obj)
来源：http://sc.szsharing.cn

[U93] JS：模板字符串
来源：http://ie.lnxyls.cn

`共 ${n} 条`
来源：http://in.szxytkj.cn

[U94] JS：箭头函数
来源：http://bl.huixiangedu.cn

const double = x => x * 2;
来源：http://dk.521024.cn

[U95] JS：Promise 包装
来源：http://jv.haigaiapp.cn

new Promise((resolve, reject) => {})
来源：http://sh.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://pi.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yo.yuexingan06.cn

[U97] JS：并发请求
来源：http://ii.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cj.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://fp.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tw.szxytkj.cn

[U99] JS：事件监听
来源：http://wp.huanxung.cn

el.addEventListener("click", e => {})
来源：http://mu.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://vv.lnxyls.cn

document.querySelector(".item")
来源：http://ya.huixiangedu.cn

[U101] JS：classList 操作
来源：http://cp.colortex.cn

el.classList.toggle("active")
来源：http://rh.gzmigu.cn

[U102] JS：本地存储
来源：http://pc.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://em.huixiangedu.cn

[U103] JS：定时器
来源：http://yh.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fu.521024.cn

[U104] JS：防抖
来源：http://gd.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cu.bjjhwx.cn

[U105] JS：节流
来源：http://jo.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ws.shxzskj.cn

[U106] JS：日期格式化
来源：http://pu.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pd.jianghongdianzi.cn

[U107] JS：数字千分位
来源：http://yu.huixiangedu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ee.9csxet.cn

[U108] JS：随机整数
来源：http://om.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://oz.gzmigu.cn

[U109] JS：数组分组
来源：http://sz.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://zj.szsharing.cn

[U110] JS：数组分块
来源：http://zo.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qo.shxzukj.cn

[U111] JS：对象转 Map
来源：http://hf.szxytkj.cn

new Map(Object.entries(obj))
来源：http://pc.lnxyls.cn

[U112] JS：字符串补位
来源：http://ij.haigaiapp.cn

"7".padStart(3, "0")
来源：http://hp.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://wr.huanxung.cn

s.replaceAll("a", "b")
来源：http://um.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://ve.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mo.hnjuh.cn

[U115] JS：生成 UUID
来源：http://pf.nszjky.cn

crypto.randomUUID()
来源：http://ru.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://vg.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://yf.newstarts.cn

[U117] JS：单元测试
来源：http://kj.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://da.shtwfgs.cn

[U118] JS：开发服务器
来源：http://pq.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://ds.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://ol.shxzskj.cn

npx vite build
来源：http://fx.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://rd.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://lj.huixinmuqiang.cn

================================================================================
来源：http://ve.lnxyls.cn

统计汇总
来源：http://iv.hnjuh.cn

================================================================================
来源：http://rt.colortex.cn

按语言统计（条）：
来源：http://cq.hnjuh.cn

Python ......... 252
来源：http://ng.hahajie.cn

PHP ............ 252
来源：http://uk.hahajie.cn

JavaScript ..... 252
来源：http://rk.haigaiapp.cn

TypeScript ..... 212
来源：http://vv.shxzukj.cn

Java ........... 212
来源：http://rz.nszjky.cn

Go ............. 212
来源：http://uu.nszjky.cn

Ruby ........... 212
来源：http://lz.jianghongdianzi.cn

C# ............. 212
来源：http://xz.yuexingan06.cn

C .............. 30
来源：http://xd.huixiangedu.cn

C++ ............ 30
来源：http://lg.chemitech.net.cn

SQL ............ 90
来源：http://ba.asd995.cn

Bash ........... 80
来源：http://wp.huixiangedu.cn

Kotlin ......... 15
来源：http://yx.yuntaijiaju.cn

Swift .......... 15
来源：http://pw.huixinmuqiang.cn

Lua ............ 10
来源：http://qh.yuntaijiaju.cn

Perl ........... 10
来源：http://dy.haigaiapp.cn

Scala .......... 10
来源：http://bo.panjiajie.cn

------------------------------------
来源：http://pr.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://hb.huixiangedu.cn

按章节统计：
来源：http://ha.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qf.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kn.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ko.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ga.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ft.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ax.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hr.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nv.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uf.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cs.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yd.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rg.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zm.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nw.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dz.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zl.jctech888.com.cn

Q SQL 专题                              90
来源：http://cm.yuntaijiaju.cn

R Bash 专题                             80
来源：http://pu.panjiajie.cn

S C / C++ 专题                          60
来源：http://yt.haigaiapp.cn

T 其他语言补充                          60
来源：http://lp.bjjhwx.cn

U 高频实用片段                         120
来源：http://mb.jctech888.com.cn

------------------------------------
来源：http://lt.haigaiapp.cn

合计                                  2106 条
来源：http://vs.nszjky.cn

--------------------------------------------------------------------------------
来源：http://yl.muxihuayi.cn

使用提醒
来源：http://nh.nicolike.cn

--------------------------------------------------------------------------------
来源：http://fb.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yg.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vd.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mo.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://nt.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qy.521024.cn

—— 文件结束 ——
来源：http://gy.asd995.cn

================================================================================
来源：http://wp.colortex.cn

程序语言常见例子速查手册（2024 版）
来源：http://es.hahajie.cn

Common Programming Examples Cheat Book
来源：http://rm.huanxung.cn

================================================================================
来源：http://uu.szsharing.cn

【收录内容】
来源：http://se.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lu.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jv.szsharing.cn

SQL · Bash · C · C++
来源：http://tc.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dj.huixiangedu.cn

【使用说明】
来源：http://od.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rm.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://fm.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://lp.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://nu.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ex.huixinmuqiang.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://fd.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ck.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mc.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yh.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pj.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://iv.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qz.lnxyls.cn

【文件统计】
来源：http://xx.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nt.huanxung.cn

--------------------------------------------------------------------------------
来源：http://ax.huixiangedu.cn

目  录
来源：http://lv.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://bg.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://de.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rk.521024.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ie.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yh.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ui.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mv.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jc.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://as.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lf.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xy.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ok.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ce.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eg.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oy.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ms.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zh.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://vj.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qn.lnxyls.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://if.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ac.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ug.hnjuh.cn

================================================================================
来源：http://vv.jctech888.com.cn

A. 基础语法与类型
来源：http://si.huanxung.cn

================================================================================
来源：http://rm.shxzskj.cn

[A01] Hello World
来源：http://pn.colortex.cn

Py:   print("Hello, World!")
来源：http://ce.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://no.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://ld.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fu.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://kd.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://fk.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://fw.huixiangedu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jr.521024.cn

[A02] 变量声明与赋值
来源：http://rg.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ae.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://cc.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://eo.szsharing.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ww.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://ql.521024.cn

Go:   name := "Alex"; age := 20
来源：http://cq.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://hm.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tj.yuexingan06.cn

[A03] 常量定义
来源：http://ib.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qj.asd995.cn

PHP:  const PI = 3.14159;
来源：http://in.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://ms.huixinmuqiang.cn

TS:   const PI: number = 3.14159;
来源：http://rd.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://gr.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://ga.shxzskj.cn

Ruby: PI = 3.14159
来源：http://nu.gzmigu.cn

C#:   const double PI = 3.14159;
来源：http://uq.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://og.szxytkj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://iw.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aj.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://cm.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://uh.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mw.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lj.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vw.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://mu.hahajie.cn

[A05] 整数除法与取模
来源：http://ld.9csxet.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vu.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yf.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://qe.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nn.521024.cn

Java: 7 / 2; 7 % 2
来源：http://pd.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://fd.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://nt.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://tr.chemitech.net.cn

[A06] 字符串转数字
来源：http://kg.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://jr.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ee.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lm.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yt.szxytkj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wi.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cf.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vw.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fl.nicolike.cn

[A07] 数字转字符串
来源：http://cb.newstarts.cn

Py:   str(42)
来源：http://vh.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://ty.panjiajie.cn

JS:   String(42); (42).toString()
来源：http://qu.muxihuayi.cn

TS:   String(42)
来源：http://an.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rw.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://nx.panjiajie.cn

Ruby: 42.to_s
来源：http://gs.lnxyls.cn

C#:   42.ToString()
来源：http://hl.hnjuh.cn

[A08] 取整与四舍五入
来源：http://ty.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qe.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kg.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://td.chemitech.net.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ht.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xs.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ff.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zh.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://si.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://wa.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://au.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rb.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://dv.huanxung.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://uk.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wq.521024.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://pz.gzmigu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xt.shxzukj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xn.haigaiapp.cn

[A10] 生成随机数
来源：http://om.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://yq.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://aj.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://yq.chemitech.net.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ik.yuexingan06.cn

Java: new Random().nextInt(100) + 1
来源：http://uk.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fn.lnxyls.cn

Ruby: rand(1..100)
来源：http://ki.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://ka.huixiangedu.cn

[A11] 条件表达式（三元）
来源：http://sy.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://fn.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tx.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qz.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ub.jianghongdianzi.cn

Java: x > 0 ? "yes" : "no"
来源：http://jp.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://pg.wgjwhj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ed.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://pw.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://jf.bookmarksfly.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://pa.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://rl.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://ux.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://cw.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://xt.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://nr.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://ha.shtwfgs.cn

C#:   $"Hello, {name}!"
来源：http://cw.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xw.bjjhwx.cn

Py:   "第一行\n第二行"
来源：http://vb.jctech888.com.cn

PHP:  "第一行\n第二行"
来源：http://oj.nszjky.cn

JS:   "第一行\n第二行"
来源：http://ir.asd995.cn

TS:   "第一行\n第二行"
来源：http://gy.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://lv.muxihuayi.cn

Go:   "第一行\n第二行"
来源：http://ip.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://uk.huixinmuqiang.cn

C#:   "第一行\n第二行"
来源：http://ra.jctech888.com.cn

[A14] 注释写法
来源：http://zv.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://at.jianghongdianzi.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rd.521024.cn

JS:   // 单行；/* 多行 */
来源：http://ox.bookmarksfly.cn


<!-- 参考信息 -->