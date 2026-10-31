代发 wailian999

[U101] JS：classList 操作
来源：http://nc.hahajie.cn

el.classList.toggle("active")
来源：http://vd.nicolike.cn

[U102] JS：本地存储
来源：http://te.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://au.nicolike.cn

[U103] JS：定时器
来源：http://eh.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ln.lnxyls.cn

[U104] JS：防抖
来源：http://hi.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ca.panjiajie.cn

[U105] JS：节流
来源：http://jp.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ee.shxzskj.cn

[U106] JS：日期格式化
来源：http://vb.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uu.huanxung.cn

[U107] JS：数字千分位
来源：http://fu.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vl.9csxet.cn

[U108] JS：随机整数
来源：http://gu.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pf.newstarts.cn

[U109] JS：数组分组
来源：http://pc.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://in.wgjwhj.cn

[U110] JS：数组分块
来源：http://qi.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jb.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://rp.hahajie.cn

new Map(Object.entries(obj))
来源：http://kn.newstarts.cn

[U112] JS：字符串补位
来源：http://vp.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://mz.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://wo.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://tw.nicolike.cn

[U114] JS：JSON 深比较
来源：http://wz.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fk.huanxung.cn

[U115] JS：生成 UUID
来源：http://cz.shtwfgs.cn

crypto.randomUUID()
来源：http://ab.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://em.wgjwhj.cn

/** @param {string} name */ function f(name) {}
来源：http://dt.chemitech.net.cn

[U117] JS：单元测试
来源：http://cr.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://jh.huixinmuqiang.cn

[U118] JS：开发服务器
来源：http://zt.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://io.jctech888.com.cn

[U119] JS：生产构建
来源：http://pr.colortex.cn

npx vite build
来源：http://fd.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://el.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://ju.jctech888.com.cn

================================================================================
来源：http://lq.szsharing.cn

统计汇总
来源：http://zq.chemitech.net.cn

================================================================================
来源：http://sm.szxytkj.cn

按语言统计（条）：
来源：http://rn.nicolike.cn

Python ......... 252
来源：http://et.9csxet.cn

PHP ............ 252
来源：http://wc.panjiajie.cn

JavaScript ..... 252
来源：http://bi.shxzskj.cn

TypeScript ..... 212
来源：http://ob.haigaiapp.cn

Java ........... 212
来源：http://nb.lnxyls.cn

Go ............. 212
来源：http://xs.shxzukj.cn

Ruby ........... 212
来源：http://hn.shtwfgs.cn

C# ............. 212
来源：http://yx.lnxyls.cn

C .............. 30
来源：http://ph.521024.cn

C++ ............ 30
来源：http://ye.huanxung.cn

SQL ............ 90
来源：http://mw.szsharing.cn

Bash ........... 80
来源：http://pq.gzmigu.cn

Kotlin ......... 15
来源：http://zc.9csxet.cn

Swift .......... 15
来源：http://oz.nszjky.cn

Lua ............ 10
来源：http://nr.shxzukj.cn

Perl ........... 10
来源：http://zr.panjiajie.cn

Scala .......... 10
来源：http://xw.szsharing.cn

------------------------------------
来源：http://xd.jctech888.com.cn

合计 ........... 2106 条
来源：http://ga.muxihuayi.cn

按章节统计：
来源：http://nd.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nb.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ha.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dw.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qf.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zl.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nd.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mq.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qj.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mf.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gl.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eg.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jj.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uq.hahajie.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uv.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mm.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ld.9csxet.cn

Q SQL 专题                              90
来源：http://lp.shtwfgs.cn

R Bash 专题                             80
来源：http://ck.hnjuh.cn

S C / C++ 专题                          60
来源：http://kk.asd995.cn

T 其他语言补充                          60
来源：http://bs.jctech888.com.cn

U 高频实用片段                         120
来源：http://ea.yuexingan06.cn

------------------------------------
来源：http://dn.jctech888.com.cn

合计                                  2106 条
来源：http://ns.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ir.muxihuayi.cn

使用提醒
来源：http://qu.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://qi.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ts.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ip.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qo.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gs.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kp.lnxyls.cn

—— 文件结束 ——
来源：http://ol.lnxyls.cn

================================================================================
来源：http://up.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://aw.hahajie.cn

Common Programming Examples Cheat Book
来源：http://mj.muxihuayi.cn

================================================================================
来源：http://lx.colortex.cn

【收录内容】
来源：http://uq.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zo.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tc.shxzskj.cn

SQL · Bash · C · C++
来源：http://jp.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://np.newstarts.cn

【使用说明】
来源：http://vg.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ew.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cw.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fj.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zt.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ai.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xy.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gf.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yh.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lm.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hr.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gy.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qn.nszjky.cn

【文件统计】
来源：http://av.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ta.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://jy.nicolike.cn

目  录
来源：http://sc.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://io.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://df.shxzskj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ql.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pc.chemitech.net.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zs.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://rr.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zo.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vh.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gx.nicolike.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ef.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nh.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dp.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qp.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://yw.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ss.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cu.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ve.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cx.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oo.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eu.bjjhwx.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ye.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yv.shxzukj.cn

================================================================================
来源：http://gb.yuntaijiaju.cn

A. 基础语法与类型
来源：http://dv.huixiangedu.cn

================================================================================
来源：http://mp.lnxyls.cn

[A01] Hello World
来源：http://nz.szsharing.cn

Py:   print("Hello, World!")
来源：http://ab.jianghongdianzi.cn

PHP:  echo "Hello, World!";
来源：http://iu.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://io.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rf.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://qh.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://rb.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://nn.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://it.shxzskj.cn

[A02] 变量声明与赋值
来源：http://fr.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fn.yuexingan06.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ms.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ou.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xz.jctech888.com.cn

Java: String name = "Alex"; int age = 20;
来源：http://cu.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ve.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://zz.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gr.hnjuh.cn

[A03] 常量定义
来源：http://qi.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mk.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://rp.colortex.cn

JS:   const PI = 3.14159;
来源：http://vq.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://sr.521024.cn

Java: static final double PI = 3.14159;
来源：http://ak.nszjky.cn

Go:   const PI = 3.14159
来源：http://he.szxytkj.cn

Ruby: PI = 3.14159
来源：http://aa.yuntaijiaju.cn

C#:   const double PI = 3.14159;
来源：http://zx.bjjhwx.cn

[A04] 判断变量类型
来源：http://uu.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fn.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tq.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wa.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://qj.huixiangedu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wu.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://at.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qf.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://fr.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://cr.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uh.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tm.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sw.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cn.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://yw.shtwfgs.cn

Go:   7 / 2; 7 % 2
来源：http://vf.bjjhwx.cn

Ruby: 7 / 2; 7 % 2
来源：http://sa.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://ip.9csxet.cn

[A06] 字符串转数字
来源：http://sa.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://gy.hnjuh.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pd.hahajie.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eu.shxzukj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://az.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ev.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oi.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xy.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://km.lnxyls.cn

[A07] 数字转字符串
来源：http://ej.yuntaijiaju.cn

Py:   str(42)
来源：http://qi.colortex.cn

PHP:  (string) 42; strval(42)
来源：http://dl.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://li.huanxung.cn

TS:   String(42)
来源：http://io.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wq.haigaiapp.cn

Go:   strconv.Itoa(42)
来源：http://su.521024.cn

Ruby: 42.to_s
来源：http://yf.hahajie.cn

C#:   42.ToString()
来源：http://uc.9csxet.cn

[A08] 取整与四舍五入
来源：http://uh.colortex.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kz.shxzskj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kx.newstarts.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oc.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://rg.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kg.nszjky.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://so.yuexingan06.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://zd.huixinmuqiang.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yp.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://ei.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://cd.panjiajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rc.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rz.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ub.hahajie.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cr.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dc.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ym.yuntaijiaju.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dw.jianghongdianzi.cn

[A10] 生成随机数
来源：http://nt.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://sg.hahajie.cn

PHP:  random_int(1, 100);
来源：http://bo.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zx.nszjky.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mg.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://ne.yuexingan06.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://af.huixinmuqiang.cn

Ruby: rand(1..100)
来源：http://ci.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://kn.chemitech.net.cn

[A11] 条件表达式（三元）
来源：http://au.hahajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://tf.yuntaijiaju.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yq.newstarts.cn

JS:   x > 0 ? "yes" : "no"
来源：http://cl.jctech888.com.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fp.shxzukj.cn

Java: x > 0 ? "yes" : "no"
来源：http://jh.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ov.gzmigu.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://cp.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://om.colortex.cn

[A12] 字符串插值 / 格式化
来源：http://cs.521024.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://xh.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wk.muxihuayi.cn

JS:   `Hello, ${name}!`
来源：http://rg.hahajie.cn

TS:   `Hello, ${name}!`
来源：http://yk.szsharing.cn

Java: "Hello, %s!".formatted(name)
来源：http://ex.9csxet.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ac.szxytkj.cn

Ruby: "Hello, #{name}!"
来源：http://dc.chemitech.net.cn

C#:   $"Hello, {name}!"
来源：http://wa.panjiajie.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://hy.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://nr.hahajie.cn

PHP:  "第一行\n第二行"
来源：http://gc.9csxet.cn

JS:   "第一行\n第二行"
来源：http://vb.521024.cn

TS:   "第一行\n第二行"
来源：http://na.szxytkj.cn

Java: "第一行\n第二行"
来源：http://dq.chemitech.net.cn

Go:   "第一行\n第二行"
来源：http://cf.wgjwhj.cn

Ruby: "第一行\n第二行"
来源：http://rj.nicolike.cn

C#:   "第一行\n第二行"
来源：http://hy.jctech888.com.cn

[A14] 注释写法
来源：http://oe.chemitech.net.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://eh.521024.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rz.lnxyls.cn

JS:   // 单行；/* 多行 */
来源：http://mu.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://ic.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wd.newstarts.cn

Go:   // 单行；/* 多行 */
来源：http://nj.jianghongdianzi.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ww.nicolike.cn

C#:   // 单行；/* 多行 */
来源：http://yw.9csxet.cn

[A15] 空值判断与默认值
来源：http://sk.wgjwhj.cn

Py:   value = data or "默认值"
来源：http://rq.huanxung.cn

PHP:  $value = $data ?? "默认值";
来源：http://tb.jianghongdianzi.cn

JS:   const value = data ?? "默认值";
来源：http://xb.haigaiapp.cn

TS:   const value = data ?? "默认值";
来源：http://fu.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zo.jctech888.com.cn

Go:   if data == "" { data = "默认值" }
来源：http://zq.huixinmuqiang.cn

Ruby: value = data || "默认值"
来源：http://go.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://yu.yuntaijiaju.cn

[A16] 真假值判断规则
来源：http://ro.yuexingan06.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tb.shxzskj.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hc.newstarts.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rz.nszjky.cn

TS:   if (!x) {}
来源：http://yy.panjiajie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pp.nszjky.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cn.shxzskj.cn

Ruby: unless x            # nil 与 false 为假
来源：http://zu.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sv.bookmarksfly.cn

[A17] 位运算
来源：http://sj.yuntaijiaju.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yx.yuexingan06.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hn.wgjwhj.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sm.haigaiapp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gd.lnxyls.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kz.bookmarksfly.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fl.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cr.huixinmuqiang.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vx.bookmarksfly.cn


<!-- 参考信息 -->