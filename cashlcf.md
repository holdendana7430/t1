代发 wailian999

[U105] JS：节流
来源：http://sj.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fi.wgjwhj.cn

[U106] JS：日期格式化
来源：http://xu.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nx.521024.cn

[U107] JS：数字千分位
来源：http://fg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hf.jctech888.com.cn

[U108] JS：随机整数
来源：http://xg.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://rn.9csxet.cn

[U109] JS：数组分组
来源：http://sx.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://ea.lnxyls.cn

[U110] JS：数组分块
来源：http://is.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sa.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://oz.yuexingan06.cn

new Map(Object.entries(obj))
来源：http://kr.shtwfgs.cn

[U112] JS：字符串补位
来源：http://uo.shxzukj.cn

"7".padStart(3, "0")
来源：http://dq.panjiajie.cn

[U113] JS：正则替换全部
来源：http://yj.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://nn.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://mp.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hu.shxzskj.cn

[U115] JS：生成 UUID
来源：http://vw.hnjuh.cn

crypto.randomUUID()
来源：http://az.huixinmuqiang.cn

[U116] JS：类型检查（JSDoc）
来源：http://sl.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://qf.chemitech.net.cn

[U117] JS：单元测试
来源：http://ix.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://br.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://tc.szxytkj.cn

npm i -D vite;  npx vite
来源：http://ph.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://lo.jianghongdianzi.cn

npx vite build
来源：http://eg.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://al.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://ed.lnxyls.cn

================================================================================
来源：http://ny.hnjuh.cn

统计汇总
来源：http://ab.hnjuh.cn

================================================================================
来源：http://qa.muxihuayi.cn

按语言统计（条）：
来源：http://ku.jianghongdianzi.cn

Python ......... 252
来源：http://ln.bjjhwx.cn

PHP ............ 252
来源：http://sz.521024.cn

JavaScript ..... 252
来源：http://oz.bjjhwx.cn

TypeScript ..... 212
来源：http://vd.gzmigu.cn

Java ........... 212
来源：http://oc.muxihuayi.cn

Go ............. 212
来源：http://zq.wgjwhj.cn

Ruby ........... 212
来源：http://jy.szxytkj.cn

C# ............. 212
来源：http://fn.szxytkj.cn

C .............. 30
来源：http://fd.bjjhwx.cn

C++ ............ 30
来源：http://ek.chemitech.net.cn

SQL ............ 90
来源：http://fo.shtwfgs.cn

Bash ........... 80
来源：http://ub.yuntaijiaju.cn

Kotlin ......... 15
来源：http://rk.panjiajie.cn

Swift .......... 15
来源：http://oc.wgjwhj.cn

Lua ............ 10
来源：http://nc.asd995.cn

Perl ........... 10
来源：http://vk.huixinmuqiang.cn

Scala .......... 10
来源：http://jj.hnjuh.cn

------------------------------------
来源：http://da.jctech888.com.cn

合计 ........... 2106 条
来源：http://zj.jctech888.com.cn

按章节统计：
来源：http://hk.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zl.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vi.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sp.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gq.shxzukj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ci.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://cz.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vh.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cc.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ck.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pp.hahajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cu.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jc.hahajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://pz.panjiajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://el.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cc.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dj.newstarts.cn

Q SQL 专题                              90
来源：http://sk.huixinmuqiang.cn

R Bash 专题                             80
来源：http://tz.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://be.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://ta.yuexingan06.cn

U 高频实用片段                         120
来源：http://af.521024.cn

------------------------------------
来源：http://cw.newstarts.cn

合计                                  2106 条
来源：http://rh.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://yt.lnxyls.cn

使用提醒
来源：http://qa.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://rh.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://dh.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tl.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fq.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://el.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yn.gzmigu.cn

—— 文件结束 ——
来源：http://xy.yuntaijiaju.cn

================================================================================
来源：http://py.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://aq.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://je.panjiajie.cn

================================================================================
来源：http://ro.panjiajie.cn

【收录内容】
来源：http://fq.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qk.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mp.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://uw.huixiangedu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gd.jianghongdianzi.cn

【使用说明】
来源：http://wf.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pc.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mw.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cb.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ui.colortex.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lc.521024.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wn.shxzukj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tw.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uk.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ap.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tm.huanxung.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ls.bookmarksfly.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://he.yuexingan06.cn

【文件统计】
来源：http://qh.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gv.nicolike.cn

--------------------------------------------------------------------------------
来源：http://rj.521024.cn

目  录
来源：http://ah.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qd.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zp.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ur.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ov.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bh.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bl.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gy.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sb.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gi.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jf.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://et.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qt.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cc.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xf.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://me.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://od.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rn.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lm.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hp.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lc.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uv.chemitech.net.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dv.521024.cn

================================================================================
来源：http://tl.nszjky.cn

A. 基础语法与类型
来源：http://mo.huixiangedu.cn

================================================================================
来源：http://tj.newstarts.cn

[A01] Hello World
来源：http://ie.huanxung.cn

Py:   print("Hello, World!")
来源：http://fu.9csxet.cn

PHP:  echo "Hello, World!";
来源：http://jk.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://rw.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wo.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://my.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://qu.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://sb.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://is.huanxung.cn

[A02] 变量声明与赋值
来源：http://wz.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pn.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ra.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ht.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sv.lnxyls.cn

Java: String name = "Alex"; int age = 20;
来源：http://gd.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://uc.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://jf.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ay.haigaiapp.cn

[A03] 常量定义
来源：http://fj.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://me.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://tf.asd995.cn

JS:   const PI = 3.14159;
来源：http://ww.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://tj.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://nl.shtwfgs.cn

Go:   const PI = 3.14159
来源：http://yz.hnjuh.cn

Ruby: PI = 3.14159
来源：http://fq.colortex.cn

C#:   const double PI = 3.14159;
来源：http://hh.chemitech.net.cn

[A04] 判断变量类型
来源：http://rk.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ts.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ou.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vm.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://nk.asd995.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://iq.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uc.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wf.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://jp.shxzskj.cn

[A05] 整数除法与取模
来源：http://bs.chemitech.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hr.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pe.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hz.shxzskj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zt.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://ne.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://ss.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://ab.jianghongdianzi.cn

C#:   7 / 2; 7 % 2
来源：http://ay.muxihuayi.cn

[A06] 字符串转数字
来源：http://py.lnxyls.cn

Py:   int("42"); float("3.14")
来源：http://xj.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ti.jianghongdianzi.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bt.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kb.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fw.nszjky.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bb.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zo.shtwfgs.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://be.huixiangedu.cn

[A07] 数字转字符串
来源：http://sl.jctech888.com.cn

Py:   str(42)
来源：http://sq.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://ro.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://rj.jianghongdianzi.cn

TS:   String(42)
来源：http://la.panjiajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://eh.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://wm.haigaiapp.cn

Ruby: 42.to_s
来源：http://vd.bookmarksfly.cn

C#:   42.ToString()
来源：http://ed.bjjhwx.cn

[A08] 取整与四舍五入
来源：http://as.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://uz.shxzukj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://sn.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lu.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://oq.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ha.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vc.shxzukj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ro.jianghongdianzi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nd.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://ro.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cj.haigaiapp.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gj.colortex.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tq.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://iz.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://sy.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://lp.nszjky.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gp.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bq.panjiajie.cn

[A10] 生成随机数
来源：http://iz.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://kr.shxzskj.cn

PHP:  random_int(1, 100);
来源：http://uk.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ws.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rl.shxzskj.cn

Java: new Random().nextInt(100) + 1
来源：http://cr.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qj.bjjhwx.cn

Ruby: rand(1..100)
来源：http://zy.colortex.cn

C#:   new Random().Next(1, 101)
来源：http://kf.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://fu.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://mp.newstarts.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bt.szxytkj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cv.huixinmuqiang.cn

TS:   x > 0 ? "yes" : "no"
来源：http://pn.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://oq.huixinmuqiang.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bj.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://nu.chemitech.net.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nm.521024.cn

[A12] 字符串插值 / 格式化
来源：http://sw.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://op.hnjuh.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cw.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://xx.jianghongdianzi.cn

TS:   `Hello, ${name}!`
来源：http://ca.hahajie.cn

Java: "Hello, %s!".formatted(name)
来源：http://hb.newstarts.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xi.shxzskj.cn

Ruby: "Hello, #{name}!"
来源：http://oi.newstarts.cn

C#:   $"Hello, {name}!"
来源：http://hi.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fe.jctech888.com.cn

Py:   "第一行\n第二行"
来源：http://hr.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://lk.hnjuh.cn

JS:   "第一行\n第二行"
来源：http://eu.yuexingan06.cn

TS:   "第一行\n第二行"
来源：http://ma.shtwfgs.cn

Java: "第一行\n第二行"
来源：http://xy.wgjwhj.cn

Go:   "第一行\n第二行"
来源：http://fj.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://qn.nicolike.cn

C#:   "第一行\n第二行"
来源：http://xk.bjjhwx.cn

[A14] 注释写法
来源：http://qh.szxytkj.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://up.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://dd.colortex.cn

JS:   // 单行；/* 多行 */
来源：http://pg.lnxyls.cn

TS:   // 单行；/* 多行 */
来源：http://rz.hnjuh.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://gw.jianghongdianzi.cn

Go:   // 单行；/* 多行 */
来源：http://to.521024.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ny.wgjwhj.cn

C#:   // 单行；/* 多行 */
来源：http://ay.nszjky.cn

[A15] 空值判断与默认值
来源：http://pa.shtwfgs.cn

Py:   value = data or "默认值"
来源：http://aw.nicolike.cn

PHP:  $value = $data ?? "默认值";
来源：http://zt.hnjuh.cn

JS:   const value = data ?? "默认值";
来源：http://jc.colortex.cn

TS:   const value = data ?? "默认值";
来源：http://dh.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://do.asd995.cn

Go:   if data == "" { data = "默认值" }
来源：http://ht.shtwfgs.cn

Ruby: value = data || "默认值"
来源：http://lq.nicolike.cn

C#:   var value = data ?? "默认值";
来源：http://vz.9csxet.cn

[A16] 真假值判断规则
来源：http://pl.shxzukj.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://oc.muxihuayi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dl.yuexingan06.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pt.szxytkj.cn

TS:   if (!x) {}
来源：http://mc.shxzskj.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mv.wgjwhj.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://of.huanxung.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xq.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xm.colortex.cn

[A17] 位运算
来源：http://iq.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://is.huixiangedu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://eq.bookmarksfly.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jy.chemitech.net.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hj.yuexingan06.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pz.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kh.nicolike.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://us.shxzskj.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ko.nicolike.cn

[A18] 字符与 ASCII 码互转
来源：http://hm.shxzskj.cn

Py:   ord("A"); chr(65)
来源：http://ov.asd995.cn

PHP:  ord("A"); chr(65)
来源：http://sh.huixiangedu.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qs.bookmarksfly.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rh.9csxet.cn

Java: (int) 'A'; (char) 65
来源：http://zp.yuexingan06.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rx.shtwfgs.cn

Ruby: "A".ord; 65.chr
来源：http://oy.newstarts.cn


<!-- 参考信息 -->