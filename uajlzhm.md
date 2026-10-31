代发 wailian999

[U97] JS：并发请求
来源：http://zk.asd995.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cq.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://yh.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bg.shxzskj.cn

[U99] JS：事件监听
来源：http://up.nszjky.cn

el.addEventListener("click", e => {})
来源：http://yk.colortex.cn

[U100] JS：DOM 查询
来源：http://uq.shxzskj.cn

document.querySelector(".item")
来源：http://vo.bjjhwx.cn

[U101] JS：classList 操作
来源：http://bd.colortex.cn

el.classList.toggle("active")
来源：http://pb.muxihuayi.cn

[U102] JS：本地存储
来源：http://sd.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ah.shxzukj.cn

[U103] JS：定时器
来源：http://mn.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pv.jianghongdianzi.cn

[U104] JS：防抖
来源：http://og.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xt.shxzukj.cn

[U105] JS：节流
来源：http://sj.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rc.wgjwhj.cn

[U106] JS：日期格式化
来源：http://py.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://eg.asd995.cn

[U107] JS：数字千分位
来源：http://jd.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vb.szxytkj.cn

[U108] JS：随机整数
来源：http://xo.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yd.shxzskj.cn

[U109] JS：数组分组
来源：http://rh.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://lt.bjjhwx.cn

[U110] JS：数组分块
来源：http://gg.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pu.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ly.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://pd.jctech888.com.cn

[U112] JS：字符串补位
来源：http://md.huixiangedu.cn

"7".padStart(3, "0")
来源：http://xk.wgjwhj.cn

[U113] JS：正则替换全部
来源：http://pm.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://nb.asd995.cn

[U114] JS：JSON 深比较
来源：http://li.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qj.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://kp.szsharing.cn

crypto.randomUUID()
来源：http://ar.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://xk.chemitech.net.cn

/** @param {string} name */ function f(name) {}
来源：http://dw.shxzukj.cn

[U117] JS：单元测试
来源：http://ys.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://rm.bjjhwx.cn

[U118] JS：开发服务器
来源：http://sd.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://fj.9csxet.cn

[U119] JS：生产构建
来源：http://hz.nicolike.cn

npx vite build
来源：http://mz.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://mw.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://gx.521024.cn

================================================================================
来源：http://gi.colortex.cn

统计汇总
来源：http://ix.colortex.cn

================================================================================
来源：http://wp.haigaiapp.cn

按语言统计（条）：
来源：http://zt.asd995.cn

Python ......... 252
来源：http://ux.wgjwhj.cn

PHP ............ 252
来源：http://ej.shxzukj.cn

JavaScript ..... 252
来源：http://lc.jianghongdianzi.cn

TypeScript ..... 212
来源：http://tb.hnjuh.cn

Java ........... 212
来源：http://bg.shxzskj.cn

Go ............. 212
来源：http://rm.nicolike.cn

Ruby ........... 212
来源：http://oc.jctech888.com.cn

C# ............. 212
来源：http://xx.521024.cn

C .............. 30
来源：http://za.asd995.cn

C++ ............ 30
来源：http://vg.colortex.cn

SQL ............ 90
来源：http://yv.gzmigu.cn

Bash ........... 80
来源：http://om.huixiangedu.cn

Kotlin ......... 15
来源：http://jx.haigaiapp.cn

Swift .......... 15
来源：http://xi.wgjwhj.cn

Lua ............ 10
来源：http://ov.jianghongdianzi.cn

Perl ........... 10
来源：http://sl.shtwfgs.cn

Scala .......... 10
来源：http://lg.huanxung.cn

------------------------------------
来源：http://dg.newstarts.cn

合计 ........... 2106 条
来源：http://gg.bjjhwx.cn

按章节统计：
来源：http://tc.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://io.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ov.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gb.jctech888.com.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fe.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ci.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mv.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://lh.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hd.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nf.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wy.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://md.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://io.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yr.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://an.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qt.yuexingan06.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://su.szxytkj.cn

Q SQL 专题                              90
来源：http://ve.colortex.cn

R Bash 专题                             80
来源：http://lt.panjiajie.cn

S C / C++ 专题                          60
来源：http://ee.nszjky.cn

T 其他语言补充                          60
来源：http://wu.huanxung.cn

U 高频实用片段                         120
来源：http://kj.jctech888.com.cn

------------------------------------
来源：http://qc.huixinmuqiang.cn

合计                                  2106 条
来源：http://xc.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://hz.panjiajie.cn

使用提醒
来源：http://eo.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bs.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ny.panjiajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tm.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yw.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://et.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://on.nicolike.cn

—— 文件结束 ——
来源：http://uk.9csxet.cn

================================================================================
来源：http://mm.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://nj.huixiangedu.cn

Common Programming Examples Cheat Book
来源：http://rn.shtwfgs.cn

================================================================================
来源：http://gh.huixinmuqiang.cn

【收录内容】
来源：http://se.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wm.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wh.shxzukj.cn

SQL · Bash · C · C++
来源：http://dg.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zp.521024.cn

【使用说明】
来源：http://pl.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qg.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rs.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wa.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sa.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jb.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://me.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wp.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jw.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mf.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xd.hahajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tz.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dj.szsharing.cn

【文件统计】
来源：http://no.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://we.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ty.asd995.cn

目  录
来源：http://lc.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://hr.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://md.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ph.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pn.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rc.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nh.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zx.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://it.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lc.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://uv.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://sf.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tb.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yl.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ew.bjjhwx.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://md.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ev.haigaiapp.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zx.huixiangedu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://tq.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://by.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jh.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ik.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ft.chemitech.net.cn

================================================================================
来源：http://de.jctech888.com.cn

A. 基础语法与类型
来源：http://sh.huanxung.cn

================================================================================
来源：http://wg.shxzukj.cn

[A01] Hello World
来源：http://ni.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://gu.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://ur.huixiangedu.cn

JS:   console.log("Hello, World!");
来源：http://wi.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ku.521024.cn

Java: System.out.println("Hello, World!");
来源：http://ha.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://go.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://fj.haigaiapp.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gy.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://qv.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bj.gzmigu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://im.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ch.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ep.newstarts.cn

Java: String name = "Alex"; int age = 20;
来源：http://zm.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://oz.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://xr.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sd.newstarts.cn

[A03] 常量定义
来源：http://vw.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vd.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://uu.9csxet.cn

JS:   const PI = 3.14159;
来源：http://mh.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://fk.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://zd.nicolike.cn

Go:   const PI = 3.14159
来源：http://jw.shxzskj.cn

Ruby: PI = 3.14159
来源：http://lc.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://sz.panjiajie.cn

[A04] 判断变量类型
来源：http://kp.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lt.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ku.newstarts.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kj.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://nn.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xj.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uo.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ld.521024.cn

C#:   x.GetType().Name; x is int
来源：http://ib.jctech888.com.cn

[A05] 整数除法与取模
来源：http://cj.521024.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jh.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hv.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dr.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eo.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://da.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://ic.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://qp.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://kp.panjiajie.cn

[A06] 字符串转数字
来源：http://sz.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://jr.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mc.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jn.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ar.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jc.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tu.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rc.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ik.9csxet.cn

[A07] 数字转字符串
来源：http://dy.szsharing.cn

Py:   str(42)
来源：http://hg.521024.cn

PHP:  (string) 42; strval(42)
来源：http://qp.521024.cn

JS:   String(42); (42).toString()
来源：http://nc.haigaiapp.cn

TS:   String(42)
来源：http://kw.nicolike.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xd.shxzskj.cn

Go:   strconv.Itoa(42)
来源：http://ut.yuexingan06.cn

Ruby: 42.to_s
来源：http://bo.yuntaijiaju.cn

C#:   42.ToString()
来源：http://tl.szsharing.cn

[A08] 取整与四舍五入
来源：http://lb.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ud.gzmigu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xd.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vr.huixiangedu.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://db.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wv.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lk.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qy.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://au.hahajie.cn

[A09] 绝对值与最大最小值
来源：http://mg.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ap.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yb.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fs.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://si.szxytkj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ft.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://qr.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ak.chemitech.net.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zt.huixiangedu.cn

[A10] 生成随机数
来源：http://ua.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://fs.muxihuayi.cn

PHP:  random_int(1, 100);
来源：http://pv.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://in.huanxung.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mx.newstarts.cn

Java: new Random().nextInt(100) + 1
来源：http://dq.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jy.yuntaijiaju.cn

Ruby: rand(1..100)
来源：http://oe.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://pc.huanxung.cn

[A11] 条件表达式（三元）
来源：http://nx.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://ak.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ry.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://he.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zr.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://aq.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://hg.nszjky.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uh.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://sa.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://ul.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://dj.asd995.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ay.newstarts.cn

JS:   `Hello, ${name}!`
来源：http://vg.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://gk.521024.cn

Java: "Hello, %s!".formatted(name)
来源：http://nm.521024.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ka.chemitech.net.cn

Ruby: "Hello, #{name}!"
来源：http://va.wgjwhj.cn

C#:   $"Hello, {name}!"
来源：http://nv.shtwfgs.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ss.newstarts.cn

Py:   "第一行\n第二行"
来源：http://xr.9csxet.cn

PHP:  "第一行\n第二行"
来源：http://wk.521024.cn

JS:   "第一行\n第二行"
来源：http://la.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://mo.nicolike.cn

Java: "第一行\n第二行"
来源：http://kb.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://uh.asd995.cn

Ruby: "第一行\n第二行"
来源：http://zw.9csxet.cn

C#:   "第一行\n第二行"
来源：http://id.hnjuh.cn

[A14] 注释写法
来源：http://zr.lnxyls.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ik.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ui.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://nr.huixiangedu.cn

TS:   // 单行；/* 多行 */
来源：http://tn.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aa.hahajie.cn

Go:   // 单行；/* 多行 */
来源：http://sq.haigaiapp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://rc.haigaiapp.cn

C#:   // 单行；/* 多行 */
来源：http://qv.asd995.cn

[A15] 空值判断与默认值
来源：http://hb.bookmarksfly.cn

Py:   value = data or "默认值"
来源：http://us.colortex.cn

PHP:  $value = $data ?? "默认值";
来源：http://tk.haigaiapp.cn

JS:   const value = data ?? "默认值";
来源：http://qh.bjjhwx.cn

TS:   const value = data ?? "默认值";
来源：http://qc.szxytkj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zk.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://gl.gzmigu.cn

Ruby: value = data || "默认值"
来源：http://xj.bjjhwx.cn

C#:   var value = data ?? "默认值";
来源：http://qa.shxzskj.cn

[A16] 真假值判断规则
来源：http://rg.hahajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://md.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hy.colortex.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cs.muxihuayi.cn

TS:   if (!x) {}
来源：http://bh.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ce.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wt.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ur.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bq.szxytkj.cn

[A17] 位运算
来源：http://lg.shtwfgs.cn


<!-- 参考信息 -->