代发 wailian999

[U101] JS：classList 操作
来源：http://lp.huixinmuqiang.cn

el.classList.toggle("active")
来源：http://ws.jctech888.com.cn

[U102] JS：本地存储
来源：http://yj.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://vn.shtwfgs.cn

[U103] JS：定时器
来源：http://wq.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wm.gzmigu.cn

[U104] JS：防抖
来源：http://yr.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oe.yuntaijiaju.cn

[U105] JS：节流
来源：http://lz.szsharing.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qa.szsharing.cn

[U106] JS：日期格式化
来源：http://ib.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xt.shtwfgs.cn

[U107] JS：数字千分位
来源：http://jw.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bc.bookmarksfly.cn

[U108] JS：随机整数
来源：http://ut.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bw.chemitech.net.cn

[U109] JS：数组分组
来源：http://ve.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ua.bjjhwx.cn

[U110] JS：数组分块
来源：http://gf.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mi.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://cy.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://zk.shxzukj.cn

[U112] JS：字符串补位
来源：http://zc.hahajie.cn

"7".padStart(3, "0")
来源：http://hu.nszjky.cn

[U113] JS：正则替换全部
来源：http://bw.asd995.cn

s.replaceAll("a", "b")
来源：http://wl.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://om.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vs.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://ii.hahajie.cn

crypto.randomUUID()
来源：http://mx.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://xu.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://ns.colortex.cn

[U117] JS：单元测试
来源：http://mn.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://my.hnjuh.cn

[U118] JS：开发服务器
来源：http://td.9csxet.cn

npm i -D vite;  npx vite
来源：http://xq.colortex.cn

[U119] JS：生产构建
来源：http://hb.szsharing.cn

npx vite build
来源：http://lg.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://hq.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://cu.chemitech.net.cn

================================================================================
来源：http://yf.newstarts.cn

统计汇总
来源：http://rg.nszjky.cn

================================================================================
来源：http://nk.yuntaijiaju.cn

按语言统计（条）：
来源：http://ug.shxzskj.cn

Python ......... 252
来源：http://zq.huixiangedu.cn

PHP ............ 252
来源：http://lj.huixiangedu.cn

JavaScript ..... 252
来源：http://re.huixinmuqiang.cn

TypeScript ..... 212
来源：http://jj.panjiajie.cn

Java ........... 212
来源：http://pi.bjjhwx.cn

Go ............. 212
来源：http://qq.wgjwhj.cn

Ruby ........... 212
来源：http://jx.colortex.cn

C# ............. 212
来源：http://fi.lnxyls.cn

C .............. 30
来源：http://ga.9csxet.cn

C++ ............ 30
来源：http://pc.szxytkj.cn

SQL ............ 90
来源：http://cg.hahajie.cn

Bash ........... 80
来源：http://ky.lnxyls.cn

Kotlin ......... 15
来源：http://jj.newstarts.cn

Swift .......... 15
来源：http://qg.jianghongdianzi.cn

Lua ............ 10
来源：http://hv.wgjwhj.cn

Perl ........... 10
来源：http://wq.shxzskj.cn

Scala .......... 10
来源：http://zu.bookmarksfly.cn

------------------------------------
来源：http://vc.bjjhwx.cn

合计 ........... 2106 条
来源：http://ya.bjjhwx.cn

按章节统计：
来源：http://nh.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kj.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://if.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kp.colortex.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pf.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kr.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://px.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sg.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hl.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xp.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dh.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uv.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rx.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sk.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mg.huixinmuqiang.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://km.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dp.colortex.cn

Q SQL 专题                              90
来源：http://jv.nszjky.cn

R Bash 专题                             80
来源：http://lb.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://ad.muxihuayi.cn

T 其他语言补充                          60
来源：http://sm.huixiangedu.cn

U 高频实用片段                         120
来源：http://cv.bookmarksfly.cn

------------------------------------
来源：http://ro.huanxung.cn

合计                                  2106 条
来源：http://zi.huanxung.cn

--------------------------------------------------------------------------------
来源：http://qh.huixinmuqiang.cn

使用提醒
来源：http://yh.szsharing.cn

--------------------------------------------------------------------------------
来源：http://bw.szxytkj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lw.bookmarksfly.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gl.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sg.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gl.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ah.chemitech.net.cn

—— 文件结束 ——
来源：http://qh.9csxet.cn

================================================================================
来源：http://bo.newstarts.cn

程序语言常见例子速查手册（2024 版）
来源：http://fq.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://sk.gzmigu.cn

================================================================================
来源：http://wm.nszjky.cn

【收录内容】
来源：http://xa.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vk.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nn.521024.cn

SQL · Bash · C · C++
来源：http://kr.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ct.szxytkj.cn

【使用说明】
来源：http://bu.shtwfgs.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kq.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ad.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://qi.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bw.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zt.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xi.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bz.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dq.haigaiapp.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eq.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bd.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zc.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cu.huixiangedu.cn

【文件统计】
来源：http://uc.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ub.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://em.jctech888.com.cn

目  录
来源：http://vv.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ug.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tg.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ij.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mt.jctech888.com.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bg.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://no.colortex.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tc.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uy.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qx.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zt.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qd.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oc.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gb.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qr.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://id.9csxet.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ze.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://iy.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fd.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://jj.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ed.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hg.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://te.wgjwhj.cn

================================================================================
来源：http://os.nszjky.cn

A. 基础语法与类型
来源：http://fd.shxzukj.cn

================================================================================
来源：http://ew.yuntaijiaju.cn

[A01] Hello World
来源：http://yv.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://wa.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://gk.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://nv.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tf.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://dc.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://hy.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://si.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://nh.colortex.cn

[A02] 变量声明与赋值
来源：http://ze.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cj.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://oe.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kx.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ii.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://lm.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://ba.gzmigu.cn

Ruby: name = "Alex"; age = 20
来源：http://uw.muxihuayi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://aa.colortex.cn

[A03] 常量定义
来源：http://ur.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ze.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://hr.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://em.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://du.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://mf.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://xg.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://iu.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ym.hahajie.cn

[A04] 判断变量类型
来源：http://sc.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://hq.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fz.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sv.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://uj.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yc.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vc.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://hp.521024.cn

[A05] 整数除法与取模
来源：http://zp.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gp.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://dq.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kr.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rd.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://yo.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://eo.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://mc.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://yj.huixiangedu.cn

[A06] 字符串转数字
来源：http://zn.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://by.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jc.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nz.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dq.wgjwhj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qf.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yi.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wk.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ky.muxihuayi.cn

[A07] 数字转字符串
来源：http://lo.bookmarksfly.cn

Py:   str(42)
来源：http://yk.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://lc.hahajie.cn

JS:   String(42); (42).toString()
来源：http://gm.yuntaijiaju.cn

TS:   String(42)
来源：http://bk.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ji.bookmarksfly.cn

Go:   strconv.Itoa(42)
来源：http://ah.jctech888.com.cn

Ruby: 42.to_s
来源：http://fm.shtwfgs.cn

C#:   42.ToString()
来源：http://ub.hahajie.cn

[A08] 取整与四舍五入
来源：http://ob.hahajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xw.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://et.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://kx.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oj.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cw.panjiajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xq.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://go.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bv.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://pr.shtwfgs.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kd.muxihuayi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://kw.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ht.huixiangedu.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qf.asd995.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bh.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://eq.szsharing.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://zv.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tv.jctech888.com.cn

[A10] 生成随机数
来源：http://np.shxzskj.cn

Py:   import random; random.randint(1, 100)
来源：http://as.panjiajie.cn

PHP:  random_int(1, 100);
来源：http://lu.shtwfgs.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ln.nicolike.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://oa.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://eh.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://td.szxytkj.cn

Ruby: rand(1..100)
来源：http://ur.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://un.hahajie.cn

[A11] 条件表达式（三元）
来源：http://hs.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://th.huixiangedu.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://tw.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://po.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qo.shtwfgs.cn

Java: x > 0 ? "yes" : "no"
来源：http://lt.lnxyls.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bf.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ik.szsharing.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mq.shtwfgs.cn

[A12] 字符串插值 / 格式化
来源：http://kl.huixinmuqiang.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wh.haigaiapp.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ak.huixiangedu.cn

JS:   `Hello, ${name}!`
来源：http://px.colortex.cn

TS:   `Hello, ${name}!`
来源：http://oh.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://qy.lnxyls.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://gh.wgjwhj.cn

Ruby: "Hello, #{name}!"
来源：http://vv.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://pg.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wh.huixiangedu.cn

Py:   "第一行\n第二行"
来源：http://qu.colortex.cn

PHP:  "第一行\n第二行"
来源：http://lo.panjiajie.cn

JS:   "第一行\n第二行"
来源：http://wg.shxzukj.cn

TS:   "第一行\n第二行"
来源：http://hi.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://lu.newstarts.cn

Go:   "第一行\n第二行"
来源：http://yg.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://my.shxzukj.cn

C#:   "第一行\n第二行"
来源：http://us.lnxyls.cn

[A14] 注释写法
来源：http://lz.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://gj.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wn.jctech888.com.cn

JS:   // 单行；/* 多行 */
来源：http://qk.chemitech.net.cn

TS:   // 单行；/* 多行 */
来源：http://sp.muxihuayi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ph.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://xk.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://fl.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://un.bjjhwx.cn

[A15] 空值判断与默认值
来源：http://hh.muxihuayi.cn

Py:   value = data or "默认值"
来源：http://ak.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://yr.colortex.cn

JS:   const value = data ?? "默认值";
来源：http://bn.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://of.gzmigu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yf.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://sb.hnjuh.cn

Ruby: value = data || "默认值"
来源：http://hb.9csxet.cn

C#:   var value = data ?? "默认值";
来源：http://fc.asd995.cn

[A16] 真假值判断规则
来源：http://qd.colortex.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wa.szsharing.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://be.szxytkj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://sp.nszjky.cn

TS:   if (!x) {}
来源：http://to.hahajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uj.yuexingan06.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qx.gzmigu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tv.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ks.jctech888.com.cn

[A17] 位运算
来源：http://no.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zq.shxzskj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ec.jctech888.com.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xc.shxzskj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://it.huanxung.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://at.chemitech.net.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://aq.hahajie.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sg.nicolike.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zu.yuexingan06.cn


<!-- 参考信息 -->