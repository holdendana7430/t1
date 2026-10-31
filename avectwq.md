代发 wailian999

[U103] JS：定时器
来源：http://um.huixinmuqiang.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gb.9csxet.cn

[U104] JS：防抖
来源：http://ox.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ov.szsharing.cn

[U105] JS：节流
来源：http://ph.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ks.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://dp.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bo.szxytkj.cn

[U107] JS：数字千分位
来源：http://ga.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gf.shtwfgs.cn

[U108] JS：随机整数
来源：http://ib.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gz.newstarts.cn

[U109] JS：数组分组
来源：http://bi.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://xh.bjjhwx.cn

[U110] JS：数组分块
来源：http://pd.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fr.hnjuh.cn

[U111] JS：对象转 Map
来源：http://zm.newstarts.cn

new Map(Object.entries(obj))
来源：http://tl.asd995.cn

[U112] JS：字符串补位
来源：http://mq.asd995.cn

"7".padStart(3, "0")
来源：http://bn.colortex.cn

[U113] JS：正则替换全部
来源：http://ys.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://jb.9csxet.cn

[U114] JS：JSON 深比较
来源：http://kr.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://jo.hnjuh.cn

[U115] JS：生成 UUID
来源：http://te.wgjwhj.cn

crypto.randomUUID()
来源：http://gn.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://ri.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://ze.chemitech.net.cn

[U117] JS：单元测试
来源：http://dk.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://zt.shxzukj.cn

[U118] JS：开发服务器
来源：http://zy.lnxyls.cn

npm i -D vite;  npx vite
来源：http://ds.shxzskj.cn

[U119] JS：生产构建
来源：http://bx.panjiajie.cn

npx vite build
来源：http://gd.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://rn.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://cd.shxzukj.cn

================================================================================
来源：http://wk.huanxung.cn

统计汇总
来源：http://cu.wgjwhj.cn

================================================================================
来源：http://zi.newstarts.cn

按语言统计（条）：
来源：http://qa.bjjhwx.cn

Python ......... 252
来源：http://jf.9csxet.cn

PHP ............ 252
来源：http://so.hnjuh.cn

JavaScript ..... 252
来源：http://em.jianghongdianzi.cn

TypeScript ..... 212
来源：http://ie.shxzskj.cn

Java ........... 212
来源：http://fw.shxzskj.cn

Go ............. 212
来源：http://ry.shxzukj.cn

Ruby ........... 212
来源：http://ee.yuntaijiaju.cn

C# ............. 212
来源：http://pc.9csxet.cn

C .............. 30
来源：http://qy.huanxung.cn

C++ ............ 30
来源：http://xu.szxytkj.cn

SQL ............ 90
来源：http://ka.nszjky.cn

Bash ........... 80
来源：http://sb.panjiajie.cn

Kotlin ......... 15
来源：http://cp.haigaiapp.cn

Swift .......... 15
来源：http://hc.nicolike.cn

Lua ............ 10
来源：http://ix.newstarts.cn

Perl ........... 10
来源：http://fo.jctech888.com.cn

Scala .......... 10
来源：http://pt.shxzskj.cn

------------------------------------
来源：http://di.9csxet.cn

合计 ........... 2106 条
来源：http://uc.bookmarksfly.cn

按章节统计：
来源：http://ow.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ek.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vl.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ow.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fc.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vx.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rg.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ps.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fb.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ix.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://io.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oo.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tf.huixiangedu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vm.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qe.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://so.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://vr.chemitech.net.cn

Q SQL 专题                              90
来源：http://nu.huixiangedu.cn

R Bash 专题                             80
来源：http://bt.panjiajie.cn

S C / C++ 专题                          60
来源：http://dz.panjiajie.cn

T 其他语言补充                          60
来源：http://uj.wgjwhj.cn

U 高频实用片段                         120
来源：http://ab.szsharing.cn

------------------------------------
来源：http://ym.huixiangedu.cn

合计                                  2106 条
来源：http://pv.nicolike.cn

--------------------------------------------------------------------------------
来源：http://zx.nicolike.cn

使用提醒
来源：http://wa.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://fv.yuntaijiaju.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vq.colortex.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ut.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rd.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vw.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xa.colortex.cn

—— 文件结束 ——
来源：http://ni.shtwfgs.cn

================================================================================
来源：http://xw.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://xq.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://yl.shtwfgs.cn

================================================================================
来源：http://el.hahajie.cn

【收录内容】
来源：http://cn.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jt.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tk.bjjhwx.cn

SQL · Bash · C · C++
来源：http://bt.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wb.jctech888.com.cn

【使用说明】
来源：http://fr.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mc.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uf.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://co.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yi.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ff.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tg.asd995.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zd.panjiajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pk.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tp.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ua.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yj.chemitech.net.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://br.9csxet.cn

【文件统计】
来源：http://hr.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jj.nicolike.cn

--------------------------------------------------------------------------------
来源：http://cw.shxzskj.cn

目  录
来源：http://nz.szsharing.cn

--------------------------------------------------------------------------------
来源：http://la.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://hn.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jq.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tw.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ei.wgjwhj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qz.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nq.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qe.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wm.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cl.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wt.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ma.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rz.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xk.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tc.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rc.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://py.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ov.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://uk.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cc.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bt.hnjuh.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lf.9csxet.cn

================================================================================
来源：http://yf.jctech888.com.cn

A. 基础语法与类型
来源：http://yd.jctech888.com.cn

================================================================================
来源：http://wa.jianghongdianzi.cn

[A01] Hello World
来源：http://wb.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://qs.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://bt.yuexingan06.cn

JS:   console.log("Hello, World!");
来源：http://dq.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://km.yuntaijiaju.cn

Java: System.out.println("Hello, World!");
来源：http://of.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://im.asd995.cn

Ruby: puts "Hello, World!"
来源：http://ap.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://yf.nszjky.cn

[A02] 变量声明与赋值
来源：http://cj.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://py.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lo.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iu.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://si.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://lh.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://gc.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://kh.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rz.asd995.cn

[A03] 常量定义
来源：http://pm.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://yz.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://df.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://gv.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://kl.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://kf.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://gb.lnxyls.cn

Ruby: PI = 3.14159
来源：http://fy.shxzskj.cn

C#:   const double PI = 3.14159;
来源：http://vg.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://ia.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dc.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ck.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://gd.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://gw.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oq.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pt.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oa.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://ua.wgjwhj.cn

[A05] 整数除法与取模
来源：http://tr.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bw.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sz.panjiajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rb.9csxet.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sy.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://qt.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://yf.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://wz.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://qp.szsharing.cn

[A06] 字符串转数字
来源：http://cf.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://fa.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://eg.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oh.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ct.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ie.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ms.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bi.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ry.shxzukj.cn

[A07] 数字转字符串
来源：http://de.hahajie.cn

Py:   str(42)
来源：http://od.newstarts.cn

PHP:  (string) 42; strval(42)
来源：http://pb.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://cc.shxzskj.cn

TS:   String(42)
来源：http://il.huixinmuqiang.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uf.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://ec.hahajie.cn

Ruby: 42.to_s
来源：http://fb.shxzskj.cn

C#:   42.ToString()
来源：http://kq.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://sc.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gd.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ed.huanxung.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pw.nicolike.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eb.lnxyls.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tj.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://jk.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://se.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qu.colortex.cn

[A09] 绝对值与最大最小值
来源：http://dv.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rx.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xg.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tb.chemitech.net.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://gb.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://qd.panjiajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://gq.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ac.nszjky.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://qv.jianghongdianzi.cn

[A10] 生成随机数
来源：http://my.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ed.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://xd.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://lo.9csxet.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fg.szxytkj.cn

Java: new Random().nextInt(100) + 1
来源：http://bh.bookmarksfly.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://er.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://yi.hnjuh.cn

C#:   new Random().Next(1, 101)
来源：http://kc.asd995.cn

[A11] 条件表达式（三元）
来源：http://bh.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://pu.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cn.hnjuh.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ns.yuntaijiaju.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yt.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://yk.hahajie.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://lj.lnxyls.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://mq.newstarts.cn

C#:   x > 0 ? "yes" : "no"
来源：http://qz.bookmarksfly.cn

[A12] 字符串插值 / 格式化
来源：http://qk.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bi.jianghongdianzi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ks.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://mz.lnxyls.cn

TS:   `Hello, ${name}!`
来源：http://kp.lnxyls.cn

Java: "Hello, %s!".formatted(name)
来源：http://nv.muxihuayi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ob.colortex.cn

Ruby: "Hello, #{name}!"
来源：http://gm.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://sa.haigaiapp.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ej.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://vz.jianghongdianzi.cn

PHP:  "第一行\n第二行"
来源：http://rh.hahajie.cn

JS:   "第一行\n第二行"
来源：http://oy.huanxung.cn

TS:   "第一行\n第二行"
来源：http://pr.9csxet.cn

Java: "第一行\n第二行"
来源：http://vy.huixiangedu.cn

Go:   "第一行\n第二行"
来源：http://qr.chemitech.net.cn

Ruby: "第一行\n第二行"
来源：http://pk.chemitech.net.cn

C#:   "第一行\n第二行"
来源：http://ef.shxzskj.cn

[A14] 注释写法
来源：http://jp.hahajie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://fj.szxytkj.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://hl.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ob.shxzukj.cn

TS:   // 单行；/* 多行 */
来源：http://ju.panjiajie.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tw.hnjuh.cn

Go:   // 单行；/* 多行 */
来源：http://up.colortex.cn

Ruby: # 单行；=begin 多行 =end
来源：http://pw.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://yz.hnjuh.cn

[A15] 空值判断与默认值
来源：http://gi.panjiajie.cn

Py:   value = data or "默认值"
来源：http://fi.jianghongdianzi.cn

PHP:  $value = $data ?? "默认值";
来源：http://iy.huixinmuqiang.cn

JS:   const value = data ?? "默认值";
来源：http://ec.yuexingan06.cn

TS:   const value = data ?? "默认值";
来源：http://zk.lnxyls.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zz.shtwfgs.cn

Go:   if data == "" { data = "默认值" }
来源：http://lg.nszjky.cn

Ruby: value = data || "默认值"
来源：http://qu.haigaiapp.cn

C#:   var value = data ?? "默认值";
来源：http://zh.asd995.cn

[A16] 真假值判断规则
来源：http://qa.panjiajie.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wb.lnxyls.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mh.shxzskj.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gh.szsharing.cn

TS:   if (!x) {}
来源：http://sk.jctech888.com.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tu.colortex.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://bh.nicolike.cn

Ruby: unless x            # nil 与 false 为假
来源：http://qa.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gh.huanxung.cn

[A17] 位运算
来源：http://wh.gzmigu.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sw.521024.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pr.shtwfgs.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://et.yuexingan06.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qy.szsharing.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rh.shtwfgs.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jf.yuexingan06.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cw.bjjhwx.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pj.9csxet.cn

[A18] 字符与 ASCII 码互转
来源：http://xk.szsharing.cn

Py:   ord("A"); chr(65)
来源：http://io.muxihuayi.cn

PHP:  ord("A"); chr(65)
来源：http://nt.wgjwhj.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jw.jctech888.com.cn


<!-- 参考信息 -->