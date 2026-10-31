代发 wailian999

[U105] JS：节流
来源：http://jp.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://op.wgjwhj.cn

[U106] JS：日期格式化
来源：http://iq.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bb.chemitech.net.cn

[U107] JS：数字千分位
来源：http://px.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kf.bjjhwx.cn

[U108] JS：随机整数
来源：http://co.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ia.shtwfgs.cn

[U109] JS：数组分组
来源：http://ap.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://ip.muxihuayi.cn

[U110] JS：数组分块
来源：http://jd.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://um.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://re.lnxyls.cn

new Map(Object.entries(obj))
来源：http://jd.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://az.wgjwhj.cn

"7".padStart(3, "0")
来源：http://zr.hahajie.cn

[U113] JS：正则替换全部
来源：http://cn.panjiajie.cn

s.replaceAll("a", "b")
来源：http://hc.9csxet.cn

[U114] JS：JSON 深比较
来源：http://ym.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://he.huanxung.cn

[U115] JS：生成 UUID
来源：http://qh.huixinmuqiang.cn

crypto.randomUUID()
来源：http://is.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://zb.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://qt.panjiajie.cn

[U117] JS：单元测试
来源：http://rk.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://lu.huanxung.cn

[U118] JS：开发服务器
来源：http://iu.yuexingan06.cn

npm i -D vite;  npx vite
来源：http://si.nszjky.cn

[U119] JS：生产构建
来源：http://rq.yuntaijiaju.cn

npx vite build
来源：http://bi.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://sm.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://vw.jianghongdianzi.cn

================================================================================
来源：http://sl.hahajie.cn

统计汇总
来源：http://rh.haigaiapp.cn

================================================================================
来源：http://fg.shxzukj.cn

按语言统计（条）：
来源：http://fc.nicolike.cn

Python ......... 252
来源：http://do.colortex.cn

PHP ............ 252
来源：http://no.haigaiapp.cn

JavaScript ..... 252
来源：http://fy.521024.cn

TypeScript ..... 212
来源：http://lb.shxzskj.cn

Java ........... 212
来源：http://vr.panjiajie.cn

Go ............. 212
来源：http://ay.9csxet.cn

Ruby ........... 212
来源：http://ki.huixinmuqiang.cn

C# ............. 212
来源：http://lv.lnxyls.cn

C .............. 30
来源：http://lw.szsharing.cn

C++ ............ 30
来源：http://cr.panjiajie.cn

SQL ............ 90
来源：http://te.lnxyls.cn

Bash ........... 80
来源：http://em.nszjky.cn

Kotlin ......... 15
来源：http://ec.yuntaijiaju.cn

Swift .......... 15
来源：http://xg.bookmarksfly.cn

Lua ............ 10
来源：http://yh.huixiangedu.cn

Perl ........... 10
来源：http://oc.shxzskj.cn

Scala .......... 10
来源：http://ho.521024.cn

------------------------------------
来源：http://pf.lnxyls.cn

合计 ........... 2106 条
来源：http://rl.wgjwhj.cn

按章节统计：
来源：http://sx.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hy.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://pz.muxihuayi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://su.lnxyls.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://un.521024.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ep.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ig.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zk.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ol.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dm.yuexingan06.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sr.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://so.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dr.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hq.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://df.nicolike.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ey.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ep.wgjwhj.cn

Q SQL 专题                              90
来源：http://ee.shxzskj.cn

R Bash 专题                             80
来源：http://un.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://ic.hnjuh.cn

T 其他语言补充                          60
来源：http://uh.szxytkj.cn

U 高频实用片段                         120
来源：http://qq.shxzukj.cn

------------------------------------
来源：http://nt.hnjuh.cn

合计                                  2106 条
来源：http://oi.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://kw.gzmigu.cn

使用提醒
来源：http://ff.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://wo.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://bo.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fb.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ho.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wb.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://px.shxzukj.cn

—— 文件结束 ——
来源：http://zl.lnxyls.cn

================================================================================
来源：http://tf.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://pl.huanxung.cn

Common Programming Examples Cheat Book
来源：http://am.nicolike.cn

================================================================================
来源：http://be.9csxet.cn

【收录内容】
来源：http://oq.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://us.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gh.asd995.cn

SQL · Bash · C · C++
来源：http://si.hahajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uo.hnjuh.cn

【使用说明】
来源：http://rz.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://br.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nz.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sr.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wh.asd995.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rt.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zf.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://at.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nt.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vy.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qp.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fv.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tt.shxzskj.cn

【文件统计】
来源：http://op.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gp.nicolike.cn

--------------------------------------------------------------------------------
来源：http://rs.huixinmuqiang.cn

目  录
来源：http://at.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://kw.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ra.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jl.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ch.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://to.colortex.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://zx.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kd.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jg.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yx.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sj.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ld.huanxung.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yn.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ss.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cl.colortex.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rc.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fi.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ta.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nh.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://gt.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ur.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ae.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bh.huanxung.cn

================================================================================
来源：http://li.yuntaijiaju.cn

A. 基础语法与类型
来源：http://bn.lnxyls.cn

================================================================================
来源：http://lq.wgjwhj.cn

[A01] Hello World
来源：http://kh.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://wh.szsharing.cn

PHP:  echo "Hello, World!";
来源：http://rh.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://gl.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zh.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://nv.bookmarksfly.cn

Go:   fmt.Println("Hello, World!")
来源：http://zn.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://lo.szxytkj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://tu.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://jz.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gq.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aw.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sm.colortex.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://vq.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://cl.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://lr.jianghongdianzi.cn

Ruby: name = "Alex"; age = 20
来源：http://fe.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qm.colortex.cn

[A03] 常量定义
来源：http://af.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sd.szxytkj.cn

PHP:  const PI = 3.14159;
来源：http://yq.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://zf.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://hi.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://rl.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://ui.shtwfgs.cn

Ruby: PI = 3.14159
来源：http://za.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://jk.gzmigu.cn

[A04] 判断变量类型
来源：http://bp.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://uf.hnjuh.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uw.huixinmuqiang.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hd.lnxyls.cn

TS:   typeof x; x instanceof Date
来源：http://bh.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yq.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://de.szxytkj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nf.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://cc.gzmigu.cn

[A05] 整数除法与取模
来源：http://no.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vn.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ri.gzmigu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rt.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ch.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://fm.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://rf.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ek.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://ol.shtwfgs.cn

[A06] 字符串转数字
来源：http://um.521024.cn

Py:   int("42"); float("3.14")
来源：http://eh.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hg.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xk.jctech888.com.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qp.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xf.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://np.bjjhwx.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ft.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xw.newstarts.cn

[A07] 数字转字符串
来源：http://il.lnxyls.cn

Py:   str(42)
来源：http://sl.bookmarksfly.cn

PHP:  (string) 42; strval(42)
来源：http://cp.lnxyls.cn

JS:   String(42); (42).toString()
来源：http://oh.bookmarksfly.cn

TS:   String(42)
来源：http://wu.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cb.hahajie.cn

Go:   strconv.Itoa(42)
来源：http://xa.szsharing.cn

Ruby: 42.to_s
来源：http://sj.521024.cn

C#:   42.ToString()
来源：http://jq.asd995.cn

[A08] 取整与四舍五入
来源：http://to.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rr.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yn.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://no.nszjky.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cm.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ka.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://lz.haigaiapp.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://td.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wz.521024.cn

[A09] 绝对值与最大最小值
来源：http://ti.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ew.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://fk.521024.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://qz.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://de.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qs.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dz.jianghongdianzi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://nt.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xf.521024.cn

[A10] 生成随机数
来源：http://og.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://st.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://ql.bookmarksfly.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kr.lnxyls.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fb.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://hq.szxytkj.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://fh.9csxet.cn

Ruby: rand(1..100)
来源：http://ks.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://uw.haigaiapp.cn

[A11] 条件表达式（三元）
来源：http://jg.szxytkj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qf.shtwfgs.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qc.bjjhwx.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ku.wgjwhj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gs.haigaiapp.cn

Java: x > 0 ? "yes" : "no"
来源：http://as.9csxet.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oo.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hw.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lt.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://zf.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://un.huanxung.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lp.wgjwhj.cn

JS:   `Hello, ${name}!`
来源：http://kw.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://fu.szxytkj.cn

Java: "Hello, %s!".formatted(name)
来源：http://pe.jctech888.com.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://pk.nszjky.cn

Ruby: "Hello, #{name}!"
来源：http://om.nszjky.cn

C#:   $"Hello, {name}!"
来源：http://wx.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fk.muxihuayi.cn

Py:   "第一行\n第二行"
来源：http://ut.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://ur.bjjhwx.cn

JS:   "第一行\n第二行"
来源：http://uu.asd995.cn

TS:   "第一行\n第二行"
来源：http://im.9csxet.cn

Java: "第一行\n第二行"
来源：http://ei.nicolike.cn

Go:   "第一行\n第二行"
来源：http://it.panjiajie.cn

Ruby: "第一行\n第二行"
来源：http://xc.bookmarksfly.cn

C#:   "第一行\n第二行"
来源：http://if.huixiangedu.cn

[A14] 注释写法
来源：http://ru.shtwfgs.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://lm.yuexingan06.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://bh.bookmarksfly.cn

JS:   // 单行；/* 多行 */
来源：http://hx.asd995.cn

TS:   // 单行；/* 多行 */
来源：http://vy.521024.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ih.gzmigu.cn

Go:   // 单行；/* 多行 */
来源：http://oh.wgjwhj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pp.huanxung.cn

C#:   // 单行；/* 多行 */
来源：http://xr.lnxyls.cn

[A15] 空值判断与默认值
来源：http://au.nicolike.cn

Py:   value = data or "默认值"
来源：http://mh.huixinmuqiang.cn

PHP:  $value = $data ?? "默认值";
来源：http://nq.huixiangedu.cn

JS:   const value = data ?? "默认值";
来源：http://kl.asd995.cn

TS:   const value = data ?? "默认值";
来源：http://ey.bjjhwx.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ck.szsharing.cn

Go:   if data == "" { data = "默认值" }
来源：http://jj.nszjky.cn

Ruby: value = data || "默认值"
来源：http://rm.jianghongdianzi.cn

C#:   var value = data ?? "默认值";
来源：http://gl.chemitech.net.cn

[A16] 真假值判断规则
来源：http://vd.nszjky.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://if.hahajie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hl.hnjuh.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yc.shxzukj.cn

TS:   if (!x) {}
来源：http://it.shtwfgs.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qd.huixinmuqiang.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wm.bookmarksfly.cn

Ruby: unless x            # nil 与 false 为假
来源：http://wu.szxytkj.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vn.nszjky.cn

[A17] 位运算
来源：http://zj.haigaiapp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kd.yuntaijiaju.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ju.haigaiapp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gn.nicolike.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dy.bjjhwx.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ec.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://au.haigaiapp.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xh.panjiajie.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xb.521024.cn

[A18] 字符与 ASCII 码互转
来源：http://ok.shxzukj.cn

Py:   ord("A"); chr(65)
来源：http://lg.jianghongdianzi.cn

PHP:  ord("A"); chr(65)
来源：http://pd.shxzukj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ag.huixinmuqiang.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kv.huixiangedu.cn

Java: (int) 'A'; (char) 65
来源：http://qc.jianghongdianzi.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wm.chemitech.net.cn

Ruby: "A".ord; 65.chr
来源：http://vc.yuexingan06.cn


<!-- 参考信息 -->