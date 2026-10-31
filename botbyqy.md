代发 wailian999

[U85] JS：可选链
来源：http://yy.wgjwhj.cn

a?.b?.c
来源：http://oi.panjiajie.cn

[U86] JS：空值合并
来源：http://rn.521024.cn

a ?? b
来源：http://tg.hahajie.cn

[U87] JS：解构默认值
来源：http://qe.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://zi.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://kn.hnjuh.cn

{ ...a, ...b }
来源：http://qj.gzmigu.cn

[U89] JS：数组去重
来源：http://hq.yuexingan06.cn

[...new Set(arr)]
来源：http://an.gzmigu.cn

[U90] JS：数字数组排序
来源：http://dj.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://si.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://we.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ao.wgjwhj.cn

[U92] JS：深拷贝
来源：http://mq.szsharing.cn

structuredClone(obj)
来源：http://yg.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ke.521024.cn

`共 ${n} 条`
来源：http://kj.colortex.cn

[U94] JS：箭头函数
来源：http://nr.chemitech.net.cn

const double = x => x * 2;
来源：http://oe.lnxyls.cn

[U95] JS：Promise 包装
来源：http://yx.bookmarksfly.cn

new Promise((resolve, reject) => {})
来源：http://ad.bjjhwx.cn

[U96] JS：async/await 与异常
来源：http://zy.panjiajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hw.hahajie.cn

[U97] JS：并发请求
来源：http://az.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jz.shxzukj.cn

[U98] JS：fetch 带 JSON
来源：http://ds.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pp.shxzskj.cn

[U99] JS：事件监听
来源：http://zo.nicolike.cn

el.addEventListener("click", e => {})
来源：http://au.nicolike.cn

[U100] JS：DOM 查询
来源：http://ds.newstarts.cn

document.querySelector(".item")
来源：http://ci.huixiangedu.cn

[U101] JS：classList 操作
来源：http://of.nszjky.cn

el.classList.toggle("active")
来源：http://ji.shtwfgs.cn

[U102] JS：本地存储
来源：http://ub.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lf.huanxung.cn

[U103] JS：定时器
来源：http://xj.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dx.huanxung.cn

[U104] JS：防抖
来源：http://rj.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gu.colortex.cn

[U105] JS：节流
来源：http://te.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://no.huanxung.cn

[U106] JS：日期格式化
来源：http://wm.hnjuh.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bb.jctech888.com.cn

[U107] JS：数字千分位
来源：http://mn.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mz.shtwfgs.cn

[U108] JS：随机整数
来源：http://zl.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://sg.521024.cn

[U109] JS：数组分组
来源：http://tw.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://tu.muxihuayi.cn

[U110] JS：数组分块
来源：http://xt.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fe.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://zg.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://ob.nszjky.cn

[U112] JS：字符串补位
来源：http://bp.panjiajie.cn

"7".padStart(3, "0")
来源：http://jb.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://qm.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://wo.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://gp.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ak.521024.cn

[U115] JS：生成 UUID
来源：http://kh.asd995.cn

crypto.randomUUID()
来源：http://mw.wgjwhj.cn

[U116] JS：类型检查（JSDoc）
来源：http://fx.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://tx.gzmigu.cn

[U117] JS：单元测试
来源：http://ee.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://td.wgjwhj.cn

[U118] JS：开发服务器
来源：http://yv.gzmigu.cn

npm i -D vite;  npx vite
来源：http://ya.hahajie.cn

[U119] JS：生产构建
来源：http://uh.yuntaijiaju.cn

npx vite build
来源：http://yk.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://lm.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://wd.9csxet.cn

================================================================================
来源：http://kg.newstarts.cn

统计汇总
来源：http://lr.lnxyls.cn

================================================================================
来源：http://gc.huixiangedu.cn

按语言统计（条）：
来源：http://pk.gzmigu.cn

Python ......... 252
来源：http://vu.yuntaijiaju.cn

PHP ............ 252
来源：http://vt.huixinmuqiang.cn

JavaScript ..... 252
来源：http://oz.shxzskj.cn

TypeScript ..... 212
来源：http://iz.panjiajie.cn

Java ........... 212
来源：http://cf.shxzskj.cn

Go ............. 212
来源：http://fu.wgjwhj.cn

Ruby ........... 212
来源：http://fu.521024.cn

C# ............. 212
来源：http://in.bjjhwx.cn

C .............. 30
来源：http://an.szxytkj.cn

C++ ............ 30
来源：http://yg.lnxyls.cn

SQL ............ 90
来源：http://fp.huanxung.cn

Bash ........... 80
来源：http://uj.521024.cn

Kotlin ......... 15
来源：http://us.nicolike.cn

Swift .......... 15
来源：http://xd.newstarts.cn

Lua ............ 10
来源：http://ph.asd995.cn

Perl ........... 10
来源：http://sj.huixinmuqiang.cn

Scala .......... 10
来源：http://fl.muxihuayi.cn

------------------------------------
来源：http://jf.wgjwhj.cn

合计 ........... 2106 条
来源：http://cb.muxihuayi.cn

按章节统计：
来源：http://td.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dr.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ch.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sj.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oi.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tm.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://es.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rb.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aa.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xo.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nn.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wf.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://op.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hv.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://cl.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://oh.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yr.colortex.cn

Q SQL 专题                              90
来源：http://uw.hnjuh.cn

R Bash 专题                             80
来源：http://da.chemitech.net.cn

S C / C++ 专题                          60
来源：http://wu.bjjhwx.cn

T 其他语言补充                          60
来源：http://oi.hnjuh.cn

U 高频实用片段                         120
来源：http://xl.chemitech.net.cn

------------------------------------
来源：http://ky.huixinmuqiang.cn

合计                                  2106 条
来源：http://yk.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://jg.hnjuh.cn

使用提醒
来源：http://uu.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://af.nicolike.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tx.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ci.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nh.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rt.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ck.gzmigu.cn

—— 文件结束 ——
来源：http://hc.bjjhwx.cn

================================================================================
来源：http://dw.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://pt.9csxet.cn

Common Programming Examples Cheat Book
来源：http://xh.muxihuayi.cn

================================================================================
来源：http://kp.huanxung.cn

【收录内容】
来源：http://wf.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fm.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dk.asd995.cn

SQL · Bash · C · C++
来源：http://qk.9csxet.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dr.bjjhwx.cn

【使用说明】
来源：http://pa.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://yu.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rm.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ce.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zs.yuntaijiaju.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pe.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://no.jianghongdianzi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xm.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lc.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eo.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iy.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yl.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ux.huixiangedu.cn

【文件统计】
来源：http://ae.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wt.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://hk.muxihuayi.cn

目  录
来源：http://uq.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://ai.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jk.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ng.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sg.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ru.jianghongdianzi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://pa.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uj.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://er.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eq.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mj.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qh.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://el.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fw.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hj.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://qt.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eg.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sa.nicolike.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://re.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vv.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zm.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yn.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rr.nicolike.cn

================================================================================
来源：http://dj.9csxet.cn

A. 基础语法与类型
来源：http://af.newstarts.cn

================================================================================
来源：http://wg.colortex.cn

[A01] Hello World
来源：http://wm.521024.cn

Py:   print("Hello, World!")
来源：http://oh.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://mp.521024.cn

JS:   console.log("Hello, World!");
来源：http://kw.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://es.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://vu.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://ur.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ku.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kb.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://hp.521024.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rk.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bb.gzmigu.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yo.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://nw.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://qd.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://jx.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://xa.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fy.szsharing.cn

[A03] 常量定义
来源：http://db.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nm.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://ej.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://ry.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://mu.yuntaijiaju.cn

Java: static final double PI = 3.14159;
来源：http://bl.nicolike.cn

Go:   const PI = 3.14159
来源：http://qy.nicolike.cn

Ruby: PI = 3.14159
来源：http://te.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://yy.huixiangedu.cn

[A04] 判断变量类型
来源：http://cg.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bf.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vy.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zb.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://io.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://is.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qw.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://kn.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://fy.nszjky.cn

[A05] 整数除法与取模
来源：http://av.newstarts.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ae.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jm.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ja.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fu.521024.cn

Java: 7 / 2; 7 % 2
来源：http://ro.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://uy.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://gb.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://ci.9csxet.cn

[A06] 字符串转数字
来源：http://kc.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://es.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hc.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pk.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ro.szsharing.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tn.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tf.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://gj.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hi.huixiangedu.cn

[A07] 数字转字符串
来源：http://di.szsharing.cn

Py:   str(42)
来源：http://wm.asd995.cn

PHP:  (string) 42; strval(42)
来源：http://hf.asd995.cn

JS:   String(42); (42).toString()
来源：http://uv.shxzskj.cn

TS:   String(42)
来源：http://ip.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://fz.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://qb.bookmarksfly.cn

Ruby: 42.to_s
来源：http://ba.newstarts.cn

C#:   42.ToString()
来源：http://px.521024.cn

[A08] 取整与四舍五入
来源：http://is.bjjhwx.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bb.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ak.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ib.shxzukj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sf.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hw.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ih.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cq.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bd.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://pp.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ey.jianghongdianzi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ge.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nh.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nf.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://oo.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qb.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wj.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://is.gzmigu.cn

[A10] 生成随机数
来源：http://hh.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://rk.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://cq.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mv.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eo.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://qd.wgjwhj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xd.huixiangedu.cn

Ruby: rand(1..100)
来源：http://cr.nszjky.cn

C#:   new Random().Next(1, 101)
来源：http://va.newstarts.cn

[A11] 条件表达式（三元）
来源：http://cc.nszjky.cn

Py:   "yes" if x > 0 else "no"
来源：http://io.nicolike.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://al.nicolike.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ui.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ld.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://mh.colortex.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wv.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qs.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://rh.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://im.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qm.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tp.hahajie.cn

JS:   `Hello, ${name}!`
来源：http://jd.muxihuayi.cn

TS:   `Hello, ${name}!`
来源：http://nw.jianghongdianzi.cn

Java: "Hello, %s!".formatted(name)
来源：http://bt.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vc.shtwfgs.cn

Ruby: "Hello, #{name}!"
来源：http://bm.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://jo.szsharing.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jc.hahajie.cn

Py:   "第一行\n第二行"
来源：http://yy.bjjhwx.cn

PHP:  "第一行\n第二行"
来源：http://qm.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://fp.hahajie.cn

TS:   "第一行\n第二行"
来源：http://mc.jctech888.com.cn

Java: "第一行\n第二行"
来源：http://vs.newstarts.cn

Go:   "第一行\n第二行"
来源：http://cx.szsharing.cn

Ruby: "第一行\n第二行"
来源：http://ex.szsharing.cn

C#:   "第一行\n第二行"
来源：http://ev.haigaiapp.cn

[A14] 注释写法
来源：http://wk.huixinmuqiang.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vc.huixiangedu.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://il.hnjuh.cn

JS:   // 单行；/* 多行 */
来源：http://xr.yuntaijiaju.cn


<!-- 参考信息 -->