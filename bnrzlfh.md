代发 wailian999

[U101] JS：classList 操作
来源：http://ha.huixiangedu.cn

el.classList.toggle("active")
来源：http://el.yuexingan06.cn

[U102] JS：本地存储
来源：http://zv.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://gc.newstarts.cn

[U103] JS：定时器
来源：http://ns.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xn.hnjuh.cn

[U104] JS：防抖
来源：http://as.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yq.nszjky.cn

[U105] JS：节流
来源：http://bn.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mm.shxzukj.cn

[U106] JS：日期格式化
来源：http://xl.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vv.huixiangedu.cn

[U107] JS：数字千分位
来源：http://qx.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lt.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ag.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://jl.bjjhwx.cn

[U109] JS：数组分组
来源：http://sk.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://av.shxzukj.cn

[U110] JS：数组分块
来源：http://va.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://an.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ic.panjiajie.cn

new Map(Object.entries(obj))
来源：http://jf.shtwfgs.cn

[U112] JS：字符串补位
来源：http://ms.szsharing.cn

"7".padStart(3, "0")
来源：http://df.szxytkj.cn

[U113] JS：正则替换全部
来源：http://hl.szxytkj.cn

s.replaceAll("a", "b")
来源：http://xm.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://fo.shtwfgs.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cg.haigaiapp.cn

[U115] JS：生成 UUID
来源：http://wn.muxihuayi.cn

crypto.randomUUID()
来源：http://ks.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://if.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://pp.lnxyls.cn

[U117] JS：单元测试
来源：http://lj.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://yh.haigaiapp.cn

[U118] JS：开发服务器
来源：http://gv.nszjky.cn

npm i -D vite;  npx vite
来源：http://pa.szsharing.cn

[U119] JS：生产构建
来源：http://do.9csxet.cn

npx vite build
来源：http://ar.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://sz.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://oe.yuexingan06.cn

================================================================================
来源：http://ut.shtwfgs.cn

统计汇总
来源：http://hm.lnxyls.cn

================================================================================
来源：http://mh.huixinmuqiang.cn

按语言统计（条）：
来源：http://lt.huixinmuqiang.cn

Python ......... 252
来源：http://rq.lnxyls.cn

PHP ............ 252
来源：http://et.panjiajie.cn

JavaScript ..... 252
来源：http://hc.szxytkj.cn

TypeScript ..... 212
来源：http://cg.chemitech.net.cn

Java ........... 212
来源：http://hw.bookmarksfly.cn

Go ............. 212
来源：http://fk.9csxet.cn

Ruby ........... 212
来源：http://oo.panjiajie.cn

C# ............. 212
来源：http://jm.huanxung.cn

C .............. 30
来源：http://as.colortex.cn

C++ ............ 30
来源：http://yk.wgjwhj.cn

SQL ............ 90
来源：http://zq.haigaiapp.cn

Bash ........... 80
来源：http://el.521024.cn

Kotlin ......... 15
来源：http://qy.yuexingan06.cn

Swift .......... 15
来源：http://ze.gzmigu.cn

Lua ............ 10
来源：http://ww.huixiangedu.cn

Perl ........... 10
来源：http://va.wgjwhj.cn

Scala .......... 10
来源：http://mf.hnjuh.cn

------------------------------------
来源：http://sb.nszjky.cn

合计 ........... 2106 条
来源：http://us.bookmarksfly.cn

按章节统计：
来源：http://va.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://te.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://md.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jl.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lk.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yi.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zc.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mj.szsharing.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://el.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jb.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zx.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://vx.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kf.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xy.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pz.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sm.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ol.hnjuh.cn

Q SQL 专题                              90
来源：http://ba.9csxet.cn

R Bash 专题                             80
来源：http://jw.haigaiapp.cn

S C / C++ 专题                          60
来源：http://ry.colortex.cn

T 其他语言补充                          60
来源：http://my.nicolike.cn

U 高频实用片段                         120
来源：http://fm.bjjhwx.cn

------------------------------------
来源：http://qg.9csxet.cn

合计                                  2106 条
来源：http://jf.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://nx.shxzukj.cn

使用提醒
来源：http://pk.colortex.cn

--------------------------------------------------------------------------------
来源：http://gl.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ls.bjjhwx.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bw.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vc.nszjky.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://df.hnjuh.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xp.asd995.cn

—— 文件结束 ——
来源：http://zw.asd995.cn

================================================================================
来源：http://lr.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://qn.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://fk.lnxyls.cn

================================================================================
来源：http://fd.chemitech.net.cn

【收录内容】
来源：http://of.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dz.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://zd.bjjhwx.cn

SQL · Bash · C · C++
来源：http://pq.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sq.jctech888.com.cn

【使用说明】
来源：http://ea.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nn.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jy.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://of.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://lw.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dd.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://za.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fx.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pb.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ho.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://eo.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ts.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ue.szsharing.cn

【文件统计】
来源：http://bx.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://in.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://bk.nicolike.cn

目  录
来源：http://of.9csxet.cn

--------------------------------------------------------------------------------
来源：http://vu.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kl.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://aw.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ho.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://om.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ig.wgjwhj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ol.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hz.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://st.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ti.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yf.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wy.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jx.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://hb.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://iu.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://me.jctech888.com.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dh.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ge.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gu.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mk.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ik.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://js.panjiajie.cn

================================================================================
来源：http://dj.szxytkj.cn

A. 基础语法与类型
来源：http://am.bookmarksfly.cn

================================================================================
来源：http://cw.muxihuayi.cn

[A01] Hello World
来源：http://lx.huanxung.cn

Py:   print("Hello, World!")
来源：http://jt.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://cb.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://gf.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gl.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://ei.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://kn.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://lp.huanxung.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ch.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://gh.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fu.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yl.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yf.bookmarksfly.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yj.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://bv.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://ns.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://im.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rh.huixiangedu.cn

[A03] 常量定义
来源：http://tv.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qy.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://ws.asd995.cn

JS:   const PI = 3.14159;
来源：http://bf.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://mq.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://ws.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://dn.panjiajie.cn

Ruby: PI = 3.14159
来源：http://cu.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://kd.wgjwhj.cn

[A04] 判断变量类型
来源：http://ax.colortex.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kx.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cq.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vn.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://dg.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://kh.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://dp.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lc.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://ko.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://ta.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rq.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sl.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yx.colortex.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wn.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://ij.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://oh.szsharing.cn

Ruby: 7 / 2; 7 % 2
来源：http://as.521024.cn

C#:   7 / 2; 7 % 2
来源：http://nq.panjiajie.cn

[A06] 字符串转数字
来源：http://rn.colortex.cn

Py:   int("42"); float("3.14")
来源：http://wl.shxzukj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ry.bookmarksfly.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oe.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://zy.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bj.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hb.huixiangedu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ut.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ry.szxytkj.cn

[A07] 数字转字符串
来源：http://rw.szxytkj.cn

Py:   str(42)
来源：http://fz.gzmigu.cn

PHP:  (string) 42; strval(42)
来源：http://ag.bookmarksfly.cn

JS:   String(42); (42).toString()
来源：http://qb.szxytkj.cn

TS:   String(42)
来源：http://nn.shxzskj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://af.yuexingan06.cn

Go:   strconv.Itoa(42)
来源：http://ym.huixiangedu.cn

Ruby: 42.to_s
来源：http://zo.wgjwhj.cn

C#:   42.ToString()
来源：http://co.yuexingan06.cn

[A08] 取整与四舍五入
来源：http://jb.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pn.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ih.shxzskj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bg.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yr.nicolike.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://xk.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wt.gzmigu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://py.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zf.nszjky.cn

[A09] 绝对值与最大最小值
来源：http://zl.yuexingan06.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://gs.521024.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://da.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hr.szxytkj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ot.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://di.colortex.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://oj.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://jm.shxzskj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ft.newstarts.cn

[A10] 生成随机数
来源：http://mk.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://kf.gzmigu.cn

PHP:  random_int(1, 100);
来源：http://uz.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mh.huixinmuqiang.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hm.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://ji.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://tu.521024.cn

Ruby: rand(1..100)
来源：http://vo.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://gi.huanxung.cn

[A11] 条件表达式（三元）
来源：http://fn.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://cu.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://if.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yq.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ur.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://pe.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://mn.nicolike.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ee.huixinmuqiang.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nh.521024.cn

[A12] 字符串插值 / 格式化
来源：http://qi.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://gn.colortex.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hn.asd995.cn

JS:   `Hello, ${name}!`
来源：http://yr.chemitech.net.cn

TS:   `Hello, ${name}!`
来源：http://gq.wgjwhj.cn

Java: "Hello, %s!".formatted(name)
来源：http://sb.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qw.jianghongdianzi.cn

Ruby: "Hello, #{name}!"
来源：http://xp.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://xd.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fg.9csxet.cn

Py:   "第一行\n第二行"
来源：http://nn.shxzukj.cn

PHP:  "第一行\n第二行"
来源：http://vw.huixiangedu.cn

JS:   "第一行\n第二行"
来源：http://qy.521024.cn

TS:   "第一行\n第二行"
来源：http://hq.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://ka.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://bn.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://ju.shxzskj.cn

C#:   "第一行\n第二行"
来源：http://lr.newstarts.cn

[A14] 注释写法
来源：http://pk.jianghongdianzi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nu.shtwfgs.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hn.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://ns.521024.cn

TS:   // 单行；/* 多行 */
来源：http://wa.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hn.nszjky.cn

Go:   // 单行；/* 多行 */
来源：http://zg.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://gz.huixiangedu.cn

C#:   // 单行；/* 多行 */
来源：http://bf.panjiajie.cn

[A15] 空值判断与默认值
来源：http://ic.huanxung.cn

Py:   value = data or "默认值"
来源：http://ax.asd995.cn

PHP:  $value = $data ?? "默认值";
来源：http://ol.chemitech.net.cn

JS:   const value = data ?? "默认值";
来源：http://hl.shxzukj.cn

TS:   const value = data ?? "默认值";
来源：http://rz.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hl.521024.cn

Go:   if data == "" { data = "默认值" }
来源：http://lf.shxzskj.cn

Ruby: value = data || "默认值"
来源：http://cd.newstarts.cn

C#:   var value = data ?? "默认值";
来源：http://sx.hahajie.cn

[A16] 真假值判断规则
来源：http://ce.asd995.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mt.521024.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ns.chemitech.net.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ws.newstarts.cn

TS:   if (!x) {}
来源：http://sj.newstarts.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rt.gzmigu.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yk.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://eo.521024.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bw.colortex.cn

[A17] 位运算
来源：http://xs.bookmarksfly.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mn.hahajie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://os.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bj.colortex.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ct.yuntaijiaju.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://az.jianghongdianzi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://zo.panjiajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ht.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kt.bjjhwx.cn


<!-- 参考信息 -->