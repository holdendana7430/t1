代发 wailian999

[U87] JS：解构默认值
来源：http://ix.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://to.colortex.cn

[U88] JS：对象展开合并
来源：http://gd.yuexingan06.cn

{ ...a, ...b }
来源：http://cy.521024.cn

[U89] JS：数组去重
来源：http://wv.szsharing.cn

[...new Set(arr)]
来源：http://gi.nicolike.cn

[U90] JS：数字数组排序
来源：http://nn.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://vw.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://bx.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lq.huixiangedu.cn

[U92] JS：深拷贝
来源：http://gk.nszjky.cn

structuredClone(obj)
来源：http://xw.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://xi.szxytkj.cn

`共 ${n} 条`
来源：http://ru.gzmigu.cn

[U94] JS：箭头函数
来源：http://cq.bjjhwx.cn

const double = x => x * 2;
来源：http://uj.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://ec.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://gz.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://rx.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://va.asd995.cn

[U97] JS：并发请求
来源：http://le.szsharing.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hk.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://ql.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wp.shtwfgs.cn

[U99] JS：事件监听
来源：http://me.hahajie.cn

el.addEventListener("click", e => {})
来源：http://cm.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://ly.shxzskj.cn

document.querySelector(".item")
来源：http://tl.521024.cn

[U101] JS：classList 操作
来源：http://as.szxytkj.cn

el.classList.toggle("active")
来源：http://zr.lnxyls.cn

[U102] JS：本地存储
来源：http://bc.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jc.hnjuh.cn

[U103] JS：定时器
来源：http://gj.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://rn.yuntaijiaju.cn

[U104] JS：防抖
来源：http://cx.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vg.bookmarksfly.cn

[U105] JS：节流
来源：http://pj.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vv.lnxyls.cn

[U106] JS：日期格式化
来源：http://ka.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gi.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://lk.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://np.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://nx.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ug.szsharing.cn

[U109] JS：数组分组
来源：http://it.wgjwhj.cn

Object.groupBy(arr, x => x.type)
来源：http://vq.muxihuayi.cn

[U110] JS：数组分块
来源：http://wj.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iu.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://jp.bjjhwx.cn

new Map(Object.entries(obj))
来源：http://wq.newstarts.cn

[U112] JS：字符串补位
来源：http://lf.haigaiapp.cn

"7".padStart(3, "0")
来源：http://si.asd995.cn

[U113] JS：正则替换全部
来源：http://jz.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://qy.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://dv.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lf.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://xo.hnjuh.cn

crypto.randomUUID()
来源：http://mu.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://gr.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://bk.gzmigu.cn

[U117] JS：单元测试
来源：http://gv.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://yn.wgjwhj.cn

[U118] JS：开发服务器
来源：http://mv.lnxyls.cn

npm i -D vite;  npx vite
来源：http://bl.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://zx.yuntaijiaju.cn

npx vite build
来源：http://mk.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://lj.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://be.jctech888.com.cn

================================================================================
来源：http://sm.jianghongdianzi.cn

统计汇总
来源：http://uq.szxytkj.cn

================================================================================
来源：http://ps.asd995.cn

按语言统计（条）：
来源：http://ia.yuntaijiaju.cn

Python ......... 252
来源：http://ru.panjiajie.cn

PHP ............ 252
来源：http://ha.yuntaijiaju.cn

JavaScript ..... 252
来源：http://zg.muxihuayi.cn

TypeScript ..... 212
来源：http://ry.huixiangedu.cn

Java ........... 212
来源：http://ts.huixiangedu.cn

Go ............. 212
来源：http://cw.asd995.cn

Ruby ........... 212
来源：http://up.shxzukj.cn

C# ............. 212
来源：http://ir.asd995.cn

C .............. 30
来源：http://mn.9csxet.cn

C++ ............ 30
来源：http://cb.huixiangedu.cn

SQL ............ 90
来源：http://gu.muxihuayi.cn

Bash ........... 80
来源：http://jc.jianghongdianzi.cn

Kotlin ......... 15
来源：http://wl.huixinmuqiang.cn

Swift .......... 15
来源：http://sl.bjjhwx.cn

Lua ............ 10
来源：http://iv.9csxet.cn

Perl ........... 10
来源：http://tk.wgjwhj.cn

Scala .......... 10
来源：http://nc.nicolike.cn

------------------------------------
来源：http://ps.newstarts.cn

合计 ........... 2106 条
来源：http://cd.bookmarksfly.cn

按章节统计：
来源：http://dx.shtwfgs.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cj.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ic.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ot.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ay.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wz.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://kx.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://iw.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qy.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mt.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ub.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ya.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gv.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tc.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://re.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://rd.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wg.chemitech.net.cn

Q SQL 专题                              90
来源：http://ti.hnjuh.cn

R Bash 专题                             80
来源：http://ua.9csxet.cn

S C / C++ 专题                          60
来源：http://mq.nszjky.cn

T 其他语言补充                          60
来源：http://hm.nszjky.cn

U 高频实用片段                         120
来源：http://ci.nszjky.cn

------------------------------------
来源：http://xz.jianghongdianzi.cn

合计                                  2106 条
来源：http://nk.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://an.hahajie.cn

使用提醒
来源：http://km.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://jx.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ch.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uf.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://lg.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kq.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eo.521024.cn

—— 文件结束 ——
来源：http://no.newstarts.cn

================================================================================
来源：http://vw.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://xq.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://jr.jianghongdianzi.cn

================================================================================
来源：http://fp.chemitech.net.cn

【收录内容】
来源：http://rj.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qa.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cs.chemitech.net.cn

SQL · Bash · C · C++
来源：http://sn.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cn.lnxyls.cn

【使用说明】
来源：http://pj.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://on.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xn.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vx.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jh.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kh.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ed.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fe.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ed.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ul.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gr.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ns.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pa.bookmarksfly.cn

【文件统计】
来源：http://bs.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pj.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ll.jianghongdianzi.cn

目  录
来源：http://nk.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://zy.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://om.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xp.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ci.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://km.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gl.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iq.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qr.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ex.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ae.lnxyls.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bu.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mc.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jd.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yo.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cj.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yr.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gz.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://uq.yuexingan06.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tf.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://le.yuntaijiaju.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xi.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tc.521024.cn

================================================================================
来源：http://zt.521024.cn

A. 基础语法与类型
来源：http://fu.chemitech.net.cn

================================================================================
来源：http://qp.jianghongdianzi.cn

[A01] Hello World
来源：http://ml.hahajie.cn

Py:   print("Hello, World!")
来源：http://jn.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://yp.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://fr.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xo.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://qa.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://ns.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://lr.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mw.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://my.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://aw.colortex.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xt.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://de.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fo.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://nt.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://cr.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://te.jctech888.com.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xr.bjjhwx.cn

[A03] 常量定义
来源：http://cr.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sc.colortex.cn

PHP:  const PI = 3.14159;
来源：http://go.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://gj.nicolike.cn

TS:   const PI: number = 3.14159;
来源：http://tm.haigaiapp.cn

Java: static final double PI = 3.14159;
来源：http://it.szsharing.cn

Go:   const PI = 3.14159
来源：http://zd.newstarts.cn

Ruby: PI = 3.14159
来源：http://gv.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://eu.shtwfgs.cn

[A04] 判断变量类型
来源：http://uo.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ek.shxzskj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ce.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uz.yuntaijiaju.cn

TS:   typeof x; x instanceof Date
来源：http://wv.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wp.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ji.yuexingan06.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pv.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://td.szsharing.cn

[A05] 整数除法与取模
来源：http://fz.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dc.jianghongdianzi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pw.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nd.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jl.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://lk.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://au.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://si.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://wq.panjiajie.cn

[A06] 字符串转数字
来源：http://sc.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://xr.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ug.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zb.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bd.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://le.jianghongdianzi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ir.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eu.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yi.colortex.cn

[A07] 数字转字符串
来源：http://nz.yuexingan06.cn

Py:   str(42)
来源：http://hb.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://an.huanxung.cn

JS:   String(42); (42).toString()
来源：http://ji.szsharing.cn

TS:   String(42)
来源：http://np.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://aa.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://nw.jctech888.com.cn

Ruby: 42.to_s
来源：http://vn.9csxet.cn

C#:   42.ToString()
来源：http://pg.9csxet.cn

[A08] 取整与四舍五入
来源：http://xd.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wm.nicolike.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://cf.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://qp.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tn.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ww.szsharing.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uk.huixinmuqiang.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rz.szsharing.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nx.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://iv.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ow.asd995.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://sm.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mf.gzmigu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dp.nszjky.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xt.asd995.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fj.szxytkj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ak.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bx.bjjhwx.cn

[A10] 生成随机数
来源：http://yg.szsharing.cn

Py:   import random; random.randint(1, 100)
来源：http://iz.yuntaijiaju.cn

PHP:  random_int(1, 100);
来源：http://bz.nicolike.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://bk.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ec.muxihuayi.cn

Java: new Random().nextInt(100) + 1
来源：http://bi.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://dl.521024.cn

Ruby: rand(1..100)
来源：http://mo.panjiajie.cn

C#:   new Random().Next(1, 101)
来源：http://ux.huixinmuqiang.cn

[A11] 条件表达式（三元）
来源：http://xo.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://ya.jctech888.com.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://jb.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://kc.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zp.hnjuh.cn

Java: x > 0 ? "yes" : "no"
来源：http://bn.panjiajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nr.huixiangedu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hv.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nv.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://ar.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://rp.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zu.haigaiapp.cn

JS:   `Hello, ${name}!`
来源：http://dr.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://ev.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://jf.shxzskj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vx.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://ux.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://ds.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://rj.bookmarksfly.cn

Py:   "第一行\n第二行"
来源：http://hi.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://ny.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://jq.yuntaijiaju.cn

TS:   "第一行\n第二行"
来源：http://fd.szsharing.cn

Java: "第一行\n第二行"
来源：http://fj.shxzskj.cn

Go:   "第一行\n第二行"
来源：http://mz.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://sm.nicolike.cn

C#:   "第一行\n第二行"
来源：http://aw.szsharing.cn

[A14] 注释写法
来源：http://ho.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://oy.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wq.yuntaijiaju.cn

JS:   // 单行；/* 多行 */
来源：http://jk.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://ls.hahajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://st.lnxyls.cn

Go:   // 单行；/* 多行 */
来源：http://tl.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://tg.szsharing.cn


<!-- 参考信息 -->