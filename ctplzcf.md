代发 wailian999

[U105] JS：节流
来源：http://dz.gzmigu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gd.bjjhwx.cn

[U106] JS：日期格式化
来源：http://cn.shtwfgs.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vq.wgjwhj.cn

[U107] JS：数字千分位
来源：http://dg.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://sy.nszjky.cn

[U108] JS：随机整数
来源：http://id.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ne.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://uq.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ey.yuexingan06.cn

[U110] JS：数组分块
来源：http://rl.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wk.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://zt.nicolike.cn

new Map(Object.entries(obj))
来源：http://hx.newstarts.cn

[U112] JS：字符串补位
来源：http://vy.newstarts.cn

"7".padStart(3, "0")
来源：http://bx.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://ka.nszjky.cn

s.replaceAll("a", "b")
来源：http://du.nszjky.cn

[U114] JS：JSON 深比较
来源：http://qi.yuntaijiaju.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jf.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://oh.panjiajie.cn

crypto.randomUUID()
来源：http://av.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://nr.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://en.colortex.cn

[U117] JS：单元测试
来源：http://fx.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://zu.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://hc.521024.cn

npm i -D vite;  npx vite
来源：http://rs.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://tz.chemitech.net.cn

npx vite build
来源：http://xl.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://ja.521024.cn

import.meta.env.VITE_API_URL
来源：http://uj.szsharing.cn

================================================================================
来源：http://ld.hnjuh.cn

统计汇总
来源：http://ev.shtwfgs.cn

================================================================================
来源：http://no.gzmigu.cn

按语言统计（条）：
来源：http://fb.lnxyls.cn

Python ......... 252
来源：http://ev.bookmarksfly.cn

PHP ............ 252
来源：http://yn.hahajie.cn

JavaScript ..... 252
来源：http://vz.shxzukj.cn

TypeScript ..... 212
来源：http://ap.521024.cn

Java ........... 212
来源：http://eb.wgjwhj.cn

Go ............. 212
来源：http://ct.bookmarksfly.cn

Ruby ........... 212
来源：http://wy.9csxet.cn

C# ............. 212
来源：http://jj.colortex.cn

C .............. 30
来源：http://vk.huixiangedu.cn

C++ ............ 30
来源：http://kn.szxytkj.cn

SQL ............ 90
来源：http://uv.shxzukj.cn

Bash ........... 80
来源：http://hk.jctech888.com.cn

Kotlin ......... 15
来源：http://hw.hahajie.cn

Swift .......... 15
来源：http://la.szxytkj.cn

Lua ............ 10
来源：http://ko.bookmarksfly.cn

Perl ........... 10
来源：http://nq.huixinmuqiang.cn

Scala .......... 10
来源：http://jm.wgjwhj.cn

------------------------------------
来源：http://km.huixiangedu.cn

合计 ........... 2106 条
来源：http://gp.shxzukj.cn

按章节统计：
来源：http://id.colortex.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bj.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qj.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zn.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nt.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bs.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://df.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nx.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fo.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jz.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ts.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dw.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kq.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xs.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ax.colortex.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zx.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wu.9csxet.cn

Q SQL 专题                              90
来源：http://wk.chemitech.net.cn

R Bash 专题                             80
来源：http://lr.hahajie.cn

S C / C++ 专题                          60
来源：http://zp.hahajie.cn

T 其他语言补充                          60
来源：http://xm.gzmigu.cn

U 高频实用片段                         120
来源：http://au.huixinmuqiang.cn

------------------------------------
来源：http://vb.yuntaijiaju.cn

合计                                  2106 条
来源：http://en.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://xp.gzmigu.cn

使用提醒
来源：http://th.colortex.cn

--------------------------------------------------------------------------------
来源：http://zw.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://iw.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ya.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jr.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kp.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pt.jctech888.com.cn

—— 文件结束 ——
来源：http://ea.asd995.cn

================================================================================
来源：http://sm.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://nj.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://sj.bjjhwx.cn

================================================================================
来源：http://st.huixinmuqiang.cn

【收录内容】
来源：http://wd.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://wu.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ey.gzmigu.cn

SQL · Bash · C · C++
来源：http://ri.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gw.nicolike.cn

【使用说明】
来源：http://tk.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hf.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xr.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pg.muxihuayi.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tq.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xh.haigaiapp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dc.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wl.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dg.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lb.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://df.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jm.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lq.shxzskj.cn

【文件统计】
来源：http://el.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mr.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://qv.haigaiapp.cn

目  录
来源：http://vo.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://eq.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jf.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zu.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kt.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sg.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bk.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mb.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hr.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ax.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sn.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fd.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yc.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jf.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bf.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rv.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://zv.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ab.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wg.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://od.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kb.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://nk.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yz.szsharing.cn

================================================================================
来源：http://yh.shtwfgs.cn

A. 基础语法与类型
来源：http://mg.shtwfgs.cn

================================================================================
来源：http://rk.hnjuh.cn

[A01] Hello World
来源：http://tu.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://vi.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://ta.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://vx.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jt.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://eg.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://me.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://tz.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oy.nszjky.cn

[A02] 变量声明与赋值
来源：http://dk.haigaiapp.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ig.hnjuh.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://hj.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ev.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qw.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://ik.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://za.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://bn.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jf.gzmigu.cn

[A03] 常量定义
来源：http://kl.szxytkj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ap.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://zz.nicolike.cn

JS:   const PI = 3.14159;
来源：http://ce.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://iu.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://rb.jctech888.com.cn

Go:   const PI = 3.14159
来源：http://id.asd995.cn

Ruby: PI = 3.14159
来源：http://fb.521024.cn

C#:   const double PI = 3.14159;
来源：http://qb.huixiangedu.cn

[A04] 判断变量类型
来源：http://ck.szsharing.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://is.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zj.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vk.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://ck.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tf.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pf.lnxyls.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mg.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://ib.chemitech.net.cn

[A05] 整数除法与取模
来源：http://nq.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://eo.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qc.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ef.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://yg.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://al.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://cn.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://hz.newstarts.cn

C#:   7 / 2; 7 % 2
来源：http://cq.9csxet.cn

[A06] 字符串转数字
来源：http://tn.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://ks.wgjwhj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://oi.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yt.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jz.huixiangedu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://cq.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ov.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fq.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hd.colortex.cn

[A07] 数字转字符串
来源：http://ij.muxihuayi.cn

Py:   str(42)
来源：http://mh.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://bf.chemitech.net.cn

JS:   String(42); (42).toString()
来源：http://vc.jianghongdianzi.cn

TS:   String(42)
来源：http://bf.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rv.asd995.cn

Go:   strconv.Itoa(42)
来源：http://ds.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://lt.yuexingan06.cn

C#:   42.ToString()
来源：http://di.huixinmuqiang.cn

[A08] 取整与四舍五入
来源：http://hl.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vo.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://br.9csxet.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hi.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ob.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hk.huixiangedu.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vu.lnxyls.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ij.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://sn.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://da.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tk.shtwfgs.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://al.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yc.shxzukj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://aw.szsharing.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lo.shxzskj.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://np.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wn.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ku.wgjwhj.cn

[A10] 生成随机数
来源：http://tz.panjiajie.cn

Py:   import random; random.randint(1, 100)
来源：http://fw.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://vy.wgjwhj.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kt.wgjwhj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://au.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://th.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kc.colortex.cn

Ruby: rand(1..100)
来源：http://vs.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://xi.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://lk.szsharing.cn

Py:   "yes" if x > 0 else "no"
来源：http://zx.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://fy.nszjky.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ay.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zi.hahajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://fx.shtwfgs.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rn.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qt.haigaiapp.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bj.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://jo.haigaiapp.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hr.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ww.panjiajie.cn

JS:   `Hello, ${name}!`
来源：http://fv.9csxet.cn

TS:   `Hello, ${name}!`
来源：http://mu.panjiajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://zu.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://bl.hahajie.cn

Ruby: "Hello, #{name}!"
来源：http://pi.jianghongdianzi.cn

C#:   $"Hello, {name}!"
来源：http://vd.hahajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://zk.huixinmuqiang.cn

Py:   "第一行\n第二行"
来源：http://ci.newstarts.cn

PHP:  "第一行\n第二行"
来源：http://tu.nszjky.cn

JS:   "第一行\n第二行"
来源：http://xo.nszjky.cn

TS:   "第一行\n第二行"
来源：http://pt.nicolike.cn

Java: "第一行\n第二行"
来源：http://ld.hnjuh.cn

Go:   "第一行\n第二行"
来源：http://fg.jianghongdianzi.cn

Ruby: "第一行\n第二行"
来源：http://ir.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://zf.bjjhwx.cn

[A14] 注释写法
来源：http://tw.huanxung.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://yh.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://sp.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://ue.nszjky.cn

TS:   // 单行；/* 多行 */
来源：http://ib.szxytkj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lo.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://wg.yuexingan06.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dn.9csxet.cn

C#:   // 单行；/* 多行 */
来源：http://om.jianghongdianzi.cn

[A15] 空值判断与默认值
来源：http://wr.9csxet.cn

Py:   value = data or "默认值"
来源：http://vo.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://bf.nszjky.cn

JS:   const value = data ?? "默认值";
来源：http://ag.nicolike.cn

TS:   const value = data ?? "默认值";
来源：http://ez.colortex.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wp.yuexingan06.cn

Go:   if data == "" { data = "默认值" }
来源：http://zr.yuexingan06.cn

Ruby: value = data || "默认值"
来源：http://uf.hnjuh.cn

C#:   var value = data ?? "默认值";
来源：http://jc.szsharing.cn

[A16] 真假值判断规则
来源：http://kl.szsharing.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kn.shxzukj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://di.huixinmuqiang.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fb.huixiangedu.cn

TS:   if (!x) {}
来源：http://vk.9csxet.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bk.shxzukj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xe.haigaiapp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://nk.szsharing.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wb.szxytkj.cn

[A17] 位运算
来源：http://dp.bjjhwx.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fp.huixinmuqiang.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ky.huixiangedu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vi.szsharing.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://it.szxytkj.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sv.hahajie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bh.muxihuayi.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cx.asd995.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fn.chemitech.net.cn

[A18] 字符与 ASCII 码互转
来源：http://tb.huixinmuqiang.cn

Py:   ord("A"); chr(65)
来源：http://pc.colortex.cn

PHP:  ord("A"); chr(65)
来源：http://iy.nicolike.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xn.bjjhwx.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vk.hahajie.cn

Java: (int) 'A'; (char) 65
来源：http://js.jctech888.com.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yy.haigaiapp.cn

Ruby: "A".ord; 65.chr
来源：http://si.szsharing.cn


<!-- 参考信息 -->