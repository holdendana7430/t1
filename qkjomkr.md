代发 wailian999

[U103] JS：定时器
来源：http://kx.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dy.shxzskj.cn

[U104] JS：防抖
来源：http://uc.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fg.nszjky.cn

[U105] JS：节流
来源：http://fm.shxzukj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ts.lnxyls.cn

[U106] JS：日期格式化
来源：http://nt.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ix.lnxyls.cn

[U107] JS：数字千分位
来源：http://ay.gzmigu.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ep.szsharing.cn

[U108] JS：随机整数
来源：http://pa.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xy.colortex.cn

[U109] JS：数组分组
来源：http://px.chemitech.net.cn

Object.groupBy(arr, x => x.type)
来源：http://rd.yuexingan06.cn

[U110] JS：数组分块
来源：http://vx.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ed.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://ie.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://xa.shtwfgs.cn

[U112] JS：字符串补位
来源：http://vf.colortex.cn

"7".padStart(3, "0")
来源：http://lg.hahajie.cn

[U113] JS：正则替换全部
来源：http://ts.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://dn.nszjky.cn

[U114] JS：JSON 深比较
来源：http://fv.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jz.hnjuh.cn

[U115] JS：生成 UUID
来源：http://gr.szxytkj.cn

crypto.randomUUID()
来源：http://cf.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://kr.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://gl.shxzskj.cn

[U117] JS：单元测试
来源：http://zd.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://jt.jctech888.com.cn

[U118] JS：开发服务器
来源：http://iq.9csxet.cn

npm i -D vite;  npx vite
来源：http://np.yuexingan06.cn

[U119] JS：生产构建
来源：http://bb.asd995.cn

npx vite build
来源：http://uc.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://td.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://ma.nszjky.cn

================================================================================
来源：http://cd.yuexingan06.cn

统计汇总
来源：http://bd.9csxet.cn

================================================================================
来源：http://si.huanxung.cn

按语言统计（条）：
来源：http://hm.shxzukj.cn

Python ......... 252
来源：http://ck.huixiangedu.cn

PHP ............ 252
来源：http://om.colortex.cn

JavaScript ..... 252
来源：http://jb.huixiangedu.cn

TypeScript ..... 212
来源：http://md.huixiangedu.cn

Java ........... 212
来源：http://qo.muxihuayi.cn

Go ............. 212
来源：http://wo.huixiangedu.cn

Ruby ........... 212
来源：http://jh.521024.cn

C# ............. 212
来源：http://pp.muxihuayi.cn

C .............. 30
来源：http://ot.huixiangedu.cn

C++ ............ 30
来源：http://sv.huixinmuqiang.cn

SQL ............ 90
来源：http://ta.huixiangedu.cn

Bash ........... 80
来源：http://qs.huixiangedu.cn

Kotlin ......... 15
来源：http://cr.haigaiapp.cn

Swift .......... 15
来源：http://oa.jctech888.com.cn

Lua ............ 10
来源：http://gb.nicolike.cn

Perl ........... 10
来源：http://ew.huixiangedu.cn

Scala .......... 10
来源：http://uw.521024.cn

------------------------------------
来源：http://hx.gzmigu.cn

合计 ........... 2106 条
来源：http://yj.shxzskj.cn

按章节统计：
来源：http://zm.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://uv.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://lk.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gp.gzmigu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://yo.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jh.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qy.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yo.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aj.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://iy.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lk.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pt.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gm.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://me.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hj.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vx.newstarts.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ng.jctech888.com.cn

Q SQL 专题                              90
来源：http://ni.9csxet.cn

R Bash 专题                             80
来源：http://ap.huanxung.cn

S C / C++ 专题                          60
来源：http://nr.gzmigu.cn

T 其他语言补充                          60
来源：http://qz.bjjhwx.cn

U 高频实用片段                         120
来源：http://de.521024.cn

------------------------------------
来源：http://fl.hnjuh.cn

合计                                  2106 条
来源：http://gb.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://pk.panjiajie.cn

使用提醒
来源：http://kf.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://aj.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fi.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tn.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://od.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dg.huixiangedu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nh.huixiangedu.cn

—— 文件结束 ——
来源：http://jc.hahajie.cn

================================================================================
来源：http://ok.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://ku.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://ei.huanxung.cn

================================================================================
来源：http://ew.nszjky.cn

【收录内容】
来源：http://nv.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://no.newstarts.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qr.chemitech.net.cn

SQL · Bash · C · C++
来源：http://bc.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ai.huanxung.cn

【使用说明】
来源：http://vt.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sv.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://he.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fh.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sf.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mh.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ky.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hl.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qh.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://at.lnxyls.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bo.nszjky.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oi.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cj.asd995.cn

【文件统计】
来源：http://ll.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cl.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://nu.huanxung.cn

目  录
来源：http://hj.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://dy.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mx.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hj.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ye.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://iv.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gy.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://by.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nb.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nd.shxzukj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ce.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nf.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wd.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wq.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jl.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://lj.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pc.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://id.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hl.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jf.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jx.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ej.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wd.shxzskj.cn

================================================================================
来源：http://xu.lnxyls.cn

A. 基础语法与类型
来源：http://gt.hahajie.cn

================================================================================
来源：http://qr.bjjhwx.cn

[A01] Hello World
来源：http://lp.colortex.cn

Py:   print("Hello, World!")
来源：http://df.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://cj.521024.cn

JS:   console.log("Hello, World!");
来源：http://ei.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aq.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://uz.chemitech.net.cn

Go:   fmt.Println("Hello, World!")
来源：http://ws.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://mg.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://mj.nszjky.cn

[A02] 变量声明与赋值
来源：http://cv.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://as.huanxung.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bb.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cy.newstarts.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hl.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://oa.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://bu.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://wm.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sk.huanxung.cn

[A03] 常量定义
来源：http://ic.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bz.colortex.cn

PHP:  const PI = 3.14159;
来源：http://lu.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://wu.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://rd.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://ot.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://li.asd995.cn

Ruby: PI = 3.14159
来源：http://mh.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://nc.9csxet.cn

[A04] 判断变量类型
来源：http://vd.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dc.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://iq.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tn.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://wu.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ff.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dx.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://zi.9csxet.cn

C#:   x.GetType().Name; x is int
来源：http://gt.jctech888.com.cn

[A05] 整数除法与取模
来源：http://rt.hnjuh.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ix.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://wh.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jj.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hk.newstarts.cn

Java: 7 / 2; 7 % 2
来源：http://bn.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://md.colortex.cn

Ruby: 7 / 2; 7 % 2
来源：http://cn.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://kx.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://je.nszjky.cn

Py:   int("42"); float("3.14")
来源：http://rj.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dt.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cw.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tq.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gp.chemitech.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rq.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tf.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pq.lnxyls.cn

[A07] 数字转字符串
来源：http://fp.jctech888.com.cn

Py:   str(42)
来源：http://nu.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://ri.jianghongdianzi.cn

JS:   String(42); (42).toString()
来源：http://sp.nicolike.cn

TS:   String(42)
来源：http://ub.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vn.newstarts.cn

Go:   strconv.Itoa(42)
来源：http://vs.hahajie.cn

Ruby: 42.to_s
来源：http://ub.haigaiapp.cn

C#:   42.ToString()
来源：http://ux.9csxet.cn

[A08] 取整与四舍五入
来源：http://vj.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ic.yuntaijiaju.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mc.bjjhwx.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ld.hnjuh.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://dr.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zi.521024.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mx.nicolike.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cs.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qy.hnjuh.cn

[A09] 绝对值与最大最小值
来源：http://np.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rs.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ei.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cq.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ra.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yx.shxzukj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hr.jctech888.com.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ao.newstarts.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://rs.colortex.cn

[A10] 生成随机数
来源：http://sp.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://zk.nszjky.cn

PHP:  random_int(1, 100);
来源：http://cs.yuexingan06.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zi.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xn.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://iw.haigaiapp.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://xg.muxihuayi.cn

Ruby: rand(1..100)
来源：http://zs.yuexingan06.cn

C#:   new Random().Next(1, 101)
来源：http://eu.colortex.cn

[A11] 条件表达式（三元）
来源：http://wx.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://bi.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dv.shtwfgs.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qd.shxzukj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qk.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://ys.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lj.huixinmuqiang.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ux.9csxet.cn

C#:   x > 0 ? "yes" : "no"
来源：http://be.yuexingan06.cn

[A12] 字符串插值 / 格式化
来源：http://zm.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mq.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://st.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://gk.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://uh.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://wr.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ew.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://ba.huanxung.cn

C#:   $"Hello, {name}!"
来源：http://yx.asd995.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://if.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://mb.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://se.huanxung.cn

JS:   "第一行\n第二行"
来源：http://di.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://cd.nszjky.cn

Java: "第一行\n第二行"
来源：http://dg.9csxet.cn

Go:   "第一行\n第二行"
来源：http://ex.hahajie.cn

Ruby: "第一行\n第二行"
来源：http://at.jctech888.com.cn

C#:   "第一行\n第二行"
来源：http://cd.shtwfgs.cn

[A14] 注释写法
来源：http://ou.wgjwhj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://rv.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://uv.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://oc.shtwfgs.cn

TS:   // 单行；/* 多行 */
来源：http://ki.wgjwhj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bv.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://sd.szsharing.cn

Ruby: # 单行；=begin 多行 =end
来源：http://vn.shxzskj.cn

C#:   // 单行；/* 多行 */
来源：http://eo.haigaiapp.cn

[A15] 空值判断与默认值
来源：http://ir.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://ph.hahajie.cn

PHP:  $value = $data ?? "默认值";
来源：http://qo.yuexingan06.cn

JS:   const value = data ?? "默认值";
来源：http://of.panjiajie.cn

TS:   const value = data ?? "默认值";
来源：http://pq.shtwfgs.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mq.bjjhwx.cn

Go:   if data == "" { data = "默认值" }
来源：http://ki.nszjky.cn

Ruby: value = data || "默认值"
来源：http://rh.colortex.cn

C#:   var value = data ?? "默认值";
来源：http://ma.szxytkj.cn

[A16] 真假值判断规则
来源：http://vl.huixinmuqiang.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hv.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mp.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xe.wgjwhj.cn

TS:   if (!x) {}
来源：http://er.521024.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ad.panjiajie.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gd.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oy.nicolike.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iv.huixinmuqiang.cn

[A17] 位运算
来源：http://tc.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sa.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kl.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uh.jctech888.com.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gf.asd995.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gs.shxzukj.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hv.9csxet.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ya.hnjuh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wj.huanxung.cn

[A18] 字符与 ASCII 码互转
来源：http://ze.huanxung.cn

Py:   ord("A"); chr(65)
来源：http://xa.jctech888.com.cn

PHP:  ord("A"); chr(65)
来源：http://xx.yuntaijiaju.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bw.huanxung.cn


<!-- 参考信息 -->