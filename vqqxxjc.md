代发 wailian999

[U101] JS：classList 操作
来源：http://td.chemitech.net.cn

el.classList.toggle("active")
来源：http://vj.bookmarksfly.cn

[U102] JS：本地存储
来源：http://in.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zp.haigaiapp.cn

[U103] JS：定时器
来源：http://es.hahajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qe.yuntaijiaju.cn

[U104] JS：防抖
来源：http://td.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://az.shxzukj.cn

[U105] JS：节流
来源：http://pm.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sy.panjiajie.cn

[U106] JS：日期格式化
来源：http://oq.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bh.newstarts.cn

[U107] JS：数字千分位
来源：http://tf.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nh.muxihuayi.cn

[U108] JS：随机整数
来源：http://nd.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wq.shxzukj.cn

[U109] JS：数组分组
来源：http://lp.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://de.szxytkj.cn

[U110] JS：数组分块
来源：http://yi.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nw.colortex.cn

[U111] JS：对象转 Map
来源：http://nz.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ai.shtwfgs.cn

[U112] JS：字符串补位
来源：http://hl.nicolike.cn

"7".padStart(3, "0")
来源：http://mg.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://qi.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://un.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://aq.chemitech.net.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://px.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://ft.bjjhwx.cn

crypto.randomUUID()
来源：http://pq.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://ix.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://vo.9csxet.cn

[U117] JS：单元测试
来源：http://ob.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://ky.wgjwhj.cn

[U118] JS：开发服务器
来源：http://vy.huanxung.cn

npm i -D vite;  npx vite
来源：http://kf.panjiajie.cn

[U119] JS：生产构建
来源：http://nc.asd995.cn

npx vite build
来源：http://sc.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://vt.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://ab.huanxung.cn

================================================================================
来源：http://du.wgjwhj.cn

统计汇总
来源：http://zp.hnjuh.cn

================================================================================
来源：http://pw.chemitech.net.cn

按语言统计（条）：
来源：http://vv.yuexingan06.cn

Python ......... 252
来源：http://on.szsharing.cn

PHP ............ 252
来源：http://nc.yuexingan06.cn

JavaScript ..... 252
来源：http://qv.szxytkj.cn

TypeScript ..... 212
来源：http://ne.jctech888.com.cn

Java ........... 212
来源：http://tg.muxihuayi.cn

Go ............. 212
来源：http://zi.chemitech.net.cn

Ruby ........... 212
来源：http://ky.nszjky.cn

C# ............. 212
来源：http://ql.lnxyls.cn

C .............. 30
来源：http://vp.gzmigu.cn

C++ ............ 30
来源：http://pc.hnjuh.cn

SQL ............ 90
来源：http://ey.colortex.cn

Bash ........... 80
来源：http://ef.yuntaijiaju.cn

Kotlin ......... 15
来源：http://zi.521024.cn

Swift .......... 15
来源：http://tw.huixinmuqiang.cn

Lua ............ 10
来源：http://ti.shtwfgs.cn

Perl ........... 10
来源：http://vl.szsharing.cn

Scala .......... 10
来源：http://kx.newstarts.cn

------------------------------------
来源：http://hr.gzmigu.cn

合计 ........... 2106 条
来源：http://an.nszjky.cn

按章节统计：
来源：http://ei.chemitech.net.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nj.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://en.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lm.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oj.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vx.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zx.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yo.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nm.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://si.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://kz.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bt.shxzukj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tu.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vq.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yv.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mc.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ta.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://ga.newstarts.cn

R Bash 专题                             80
来源：http://oz.muxihuayi.cn

S C / C++ 专题                          60
来源：http://az.bjjhwx.cn

T 其他语言补充                          60
来源：http://hj.shxzukj.cn

U 高频实用片段                         120
来源：http://ds.nicolike.cn

------------------------------------
来源：http://is.shxzukj.cn

合计                                  2106 条
来源：http://wr.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://vz.haigaiapp.cn

使用提醒
来源：http://wr.newstarts.cn

--------------------------------------------------------------------------------
来源：http://hw.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vn.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://at.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ta.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vo.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zp.panjiajie.cn

—— 文件结束 ——
来源：http://lf.9csxet.cn

================================================================================
来源：http://vu.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://bc.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://dn.chemitech.net.cn

================================================================================
来源：http://sk.shxzskj.cn

【收录内容】
来源：http://mb.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yh.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://es.szxytkj.cn

SQL · Bash · C · C++
来源：http://sw.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hx.bjjhwx.cn

【使用说明】
来源：http://xt.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fo.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qq.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nn.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dz.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://op.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oj.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kp.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jx.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lf.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tm.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nn.haigaiapp.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qp.bjjhwx.cn

【文件统计】
来源：http://ne.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gy.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://ob.jianghongdianzi.cn

目  录
来源：http://cn.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://im.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tf.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wy.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mg.lnxyls.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lz.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hh.chemitech.net.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ah.asd995.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://au.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hy.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gh.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yx.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://rs.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jw.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jr.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xa.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bs.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ce.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xy.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://un.521024.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xk.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zu.shtwfgs.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wf.wgjwhj.cn

================================================================================
来源：http://kz.wgjwhj.cn

A. 基础语法与类型
来源：http://zj.gzmigu.cn

================================================================================
来源：http://ip.hnjuh.cn

[A01] Hello World
来源：http://un.asd995.cn

Py:   print("Hello, World!")
来源：http://bw.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://fz.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://oo.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yg.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://tm.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://xk.panjiajie.cn

Ruby: puts "Hello, World!"
来源：http://cv.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cd.hnjuh.cn

[A02] 变量声明与赋值
来源：http://kn.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ej.shtwfgs.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oe.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://si.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bi.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://mu.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://qq.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://gl.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ut.jianghongdianzi.cn

[A03] 常量定义
来源：http://gb.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hb.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://an.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://qp.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://mu.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://wf.gzmigu.cn

Go:   const PI = 3.14159
来源：http://so.yuexingan06.cn

Ruby: PI = 3.14159
来源：http://gt.szsharing.cn

C#:   const double PI = 3.14159;
来源：http://is.hnjuh.cn

[A04] 判断变量类型
来源：http://hm.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qq.hahajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://lq.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://jd.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://ni.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://is.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jb.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://am.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://le.newstarts.cn

[A05] 整数除法与取模
来源：http://wn.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mp.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ga.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yj.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ie.szsharing.cn

Java: 7 / 2; 7 % 2
来源：http://sz.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://ow.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://mv.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://xt.jctech888.com.cn

[A06] 字符串转数字
来源：http://oz.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://ly.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rk.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bw.muxihuayi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hx.panjiajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aq.9csxet.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://eu.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vg.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fg.jctech888.com.cn

[A07] 数字转字符串
来源：http://lv.lnxyls.cn

Py:   str(42)
来源：http://kl.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://vw.521024.cn

JS:   String(42); (42).toString()
来源：http://ek.nszjky.cn

TS:   String(42)
来源：http://ui.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vb.colortex.cn

Go:   strconv.Itoa(42)
来源：http://so.huanxung.cn

Ruby: 42.to_s
来源：http://jo.jctech888.com.cn

C#:   42.ToString()
来源：http://tw.lnxyls.cn

[A08] 取整与四舍五入
来源：http://mg.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qf.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gh.panjiajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jj.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tn.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://bv.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bt.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gg.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://de.shxzskj.cn

[A09] 绝对值与最大最小值
来源：http://zt.szxytkj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ec.newstarts.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xe.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://zw.shxzskj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ls.muxihuayi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://as.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://zp.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jf.asd995.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nq.szxytkj.cn

[A10] 生成随机数
来源：http://zx.colortex.cn

Py:   import random; random.randint(1, 100)
来源：http://bw.bookmarksfly.cn

PHP:  random_int(1, 100);
来源：http://lp.huixiangedu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sb.bjjhwx.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qp.wgjwhj.cn

Java: new Random().nextInt(100) + 1
来源：http://bp.huanxung.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qe.shtwfgs.cn

Ruby: rand(1..100)
来源：http://kr.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://tc.bjjhwx.cn

[A11] 条件表达式（三元）
来源：http://nn.shxzskj.cn

Py:   "yes" if x > 0 else "no"
来源：http://zp.shxzukj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kh.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vp.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ok.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://yw.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wx.chemitech.net.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ft.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zs.szxytkj.cn

[A12] 字符串插值 / 格式化
来源：http://oe.jctech888.com.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://uu.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://dc.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://ke.bjjhwx.cn

TS:   `Hello, ${name}!`
来源：http://dw.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://aa.jianghongdianzi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://re.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://uv.shxzskj.cn

C#:   $"Hello, {name}!"
来源：http://fl.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gg.nicolike.cn

Py:   "第一行\n第二行"
来源：http://zv.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://wg.lnxyls.cn

JS:   "第一行\n第二行"
来源：http://ny.szxytkj.cn

TS:   "第一行\n第二行"
来源：http://tb.bjjhwx.cn

Java: "第一行\n第二行"
来源：http://zn.shxzukj.cn

Go:   "第一行\n第二行"
来源：http://tn.szxytkj.cn

Ruby: "第一行\n第二行"
来源：http://pt.yuexingan06.cn

C#:   "第一行\n第二行"
来源：http://nn.jctech888.com.cn

[A14] 注释写法
来源：http://xq.bookmarksfly.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wr.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://vx.huixinmuqiang.cn

JS:   // 单行；/* 多行 */
来源：http://xo.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ga.chemitech.net.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://kp.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://du.muxihuayi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fl.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://vk.hahajie.cn

[A15] 空值判断与默认值
来源：http://tn.521024.cn

Py:   value = data or "默认值"
来源：http://ge.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://iv.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://bd.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://rk.szsharing.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gx.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://ik.jctech888.com.cn

Ruby: value = data || "默认值"
来源：http://ef.yuexingan06.cn

C#:   var value = data ?? "默认值";
来源：http://yh.asd995.cn

[A16] 真假值判断规则
来源：http://jq.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://fr.nszjky.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vb.521024.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://dr.9csxet.cn

TS:   if (!x) {}
来源：http://rh.bjjhwx.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wh.newstarts.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qe.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mc.hnjuh.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yo.szsharing.cn

[A17] 位运算
来源：http://rq.jianghongdianzi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ry.szxytkj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://at.521024.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wg.nszjky.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://po.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pl.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ne.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wz.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gt.shtwfgs.cn


<!-- 参考信息 -->