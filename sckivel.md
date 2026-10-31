代发 wailian999

[U103] JS：定时器
来源：http://ll.nszjky.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bi.hahajie.cn

[U104] JS：防抖
来源：http://nx.panjiajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gb.jianghongdianzi.cn

[U105] JS：节流
来源：http://df.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ts.muxihuayi.cn

[U106] JS：日期格式化
来源：http://vp.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://uj.shxzskj.cn

[U107] JS：数字千分位
来源：http://qx.9csxet.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ue.huanxung.cn

[U108] JS：随机整数
来源：http://ru.bookmarksfly.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://be.hahajie.cn

[U109] JS：数组分组
来源：http://fu.yuntaijiaju.cn

Object.groupBy(arr, x => x.type)
来源：http://bo.shxzskj.cn

[U110] JS：数组分块
来源：http://cn.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yr.szsharing.cn

[U111] JS：对象转 Map
来源：http://ei.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://ns.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://pl.521024.cn

"7".padStart(3, "0")
来源：http://li.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://py.colortex.cn

s.replaceAll("a", "b")
来源：http://pz.colortex.cn

[U114] JS：JSON 深比较
来源：http://zg.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xr.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://du.huixiangedu.cn

crypto.randomUUID()
来源：http://do.asd995.cn

[U116] JS：类型检查（JSDoc）
来源：http://qz.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://bg.bookmarksfly.cn

[U117] JS：单元测试
来源：http://mv.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://sl.shtwfgs.cn

[U118] JS：开发服务器
来源：http://ti.szxytkj.cn

npm i -D vite;  npx vite
来源：http://zi.shtwfgs.cn

[U119] JS：生产构建
来源：http://yd.newstarts.cn

npx vite build
来源：http://ba.shxzskj.cn

[U120] JS：读取环境变量（Vite）
来源：http://pv.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://xi.newstarts.cn

================================================================================
来源：http://zw.colortex.cn

统计汇总
来源：http://ww.huanxung.cn

================================================================================
来源：http://ez.szsharing.cn

按语言统计（条）：
来源：http://tu.szxytkj.cn

Python ......... 252
来源：http://cs.asd995.cn

PHP ............ 252
来源：http://xr.bookmarksfly.cn

JavaScript ..... 252
来源：http://yx.yuntaijiaju.cn

TypeScript ..... 212
来源：http://wx.panjiajie.cn

Java ........... 212
来源：http://uc.yuntaijiaju.cn

Go ............. 212
来源：http://hx.yuntaijiaju.cn

Ruby ........... 212
来源：http://xr.jctech888.com.cn

C# ............. 212
来源：http://ao.shtwfgs.cn

C .............. 30
来源：http://ym.asd995.cn

C++ ............ 30
来源：http://rz.jctech888.com.cn

SQL ............ 90
来源：http://ck.9csxet.cn

Bash ........... 80
来源：http://gn.shxzskj.cn

Kotlin ......... 15
来源：http://uo.9csxet.cn

Swift .......... 15
来源：http://jv.yuexingan06.cn

Lua ............ 10
来源：http://gx.nicolike.cn

Perl ........... 10
来源：http://vq.huixiangedu.cn

Scala .......... 10
来源：http://yd.huixinmuqiang.cn

------------------------------------
来源：http://fm.haigaiapp.cn

合计 ........... 2106 条
来源：http://km.huixiangedu.cn

按章节统计：
来源：http://xi.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jl.huanxung.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ds.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ld.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zm.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zc.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gu.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kx.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://bh.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vr.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ff.hnjuh.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bu.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pu.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://uc.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qf.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gv.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://io.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://jf.szsharing.cn

R Bash 专题                             80
来源：http://sh.gzmigu.cn

S C / C++ 专题                          60
来源：http://pa.yuexingan06.cn

T 其他语言补充                          60
来源：http://mw.szxytkj.cn

U 高频实用片段                         120
来源：http://ug.yuntaijiaju.cn

------------------------------------
来源：http://rc.nicolike.cn

合计                                  2106 条
来源：http://sp.nszjky.cn

--------------------------------------------------------------------------------
来源：http://zi.shtwfgs.cn

使用提醒
来源：http://hk.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://fh.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wa.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gg.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://da.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ux.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zc.shxzukj.cn

—— 文件结束 ——
来源：http://wd.bjjhwx.cn

================================================================================
来源：http://bx.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://oq.szsharing.cn

Common Programming Examples Cheat Book
来源：http://iy.shtwfgs.cn

================================================================================
来源：http://sx.jctech888.com.cn

【收录内容】
来源：http://lp.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ha.colortex.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nm.shxzukj.cn

SQL · Bash · C · C++
来源：http://qx.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ii.shtwfgs.cn

【使用说明】
来源：http://er.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://kx.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://er.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ku.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gp.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kt.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jt.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cs.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gw.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tv.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gl.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yt.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://il.lnxyls.cn

【文件统计】
来源：http://ee.hahajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rr.asd995.cn

--------------------------------------------------------------------------------
来源：http://cw.asd995.cn

目  录
来源：http://dk.nszjky.cn

--------------------------------------------------------------------------------
来源：http://js.asd995.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yz.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vr.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ff.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://je.szsharing.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hc.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xq.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://co.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sw.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://nn.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://py.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vi.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nz.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jn.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jj.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ro.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ia.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://up.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wv.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iv.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wo.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ds.9csxet.cn

================================================================================
来源：http://dm.szxytkj.cn

A. 基础语法与类型
来源：http://vq.huanxung.cn

================================================================================
来源：http://qb.nicolike.cn

[A01] Hello World
来源：http://si.shxzukj.cn

Py:   print("Hello, World!")
来源：http://eb.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://hf.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://ej.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://it.shxzukj.cn

Java: System.out.println("Hello, World!");
来源：http://uq.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://pu.asd995.cn

Ruby: puts "Hello, World!"
来源：http://oy.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hs.9csxet.cn

[A02] 变量声明与赋值
来源：http://ta.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://nf.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nm.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wb.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cm.szsharing.cn

Java: String name = "Alex"; int age = 20;
来源：http://oz.shtwfgs.cn

Go:   name := "Alex"; age := 20
来源：http://qm.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://tp.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://td.bookmarksfly.cn

[A03] 常量定义
来源：http://ls.muxihuayi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sn.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://pp.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://uu.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://pb.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ff.nszjky.cn

Go:   const PI = 3.14159
来源：http://gp.lnxyls.cn

Ruby: PI = 3.14159
来源：http://av.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://td.jianghongdianzi.cn

[A04] 判断变量类型
来源：http://ic.lnxyls.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://mn.haigaiapp.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qg.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rb.jctech888.com.cn

TS:   typeof x; x instanceof Date
来源：http://dp.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hi.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://md.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pm.muxihuayi.cn

C#:   x.GetType().Name; x is int
来源：http://jk.jctech888.com.cn

[A05] 整数除法与取模
来源：http://zu.shtwfgs.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ml.szxytkj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jq.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://my.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qe.yuntaijiaju.cn

Java: 7 / 2; 7 % 2
来源：http://hi.nicolike.cn

Go:   7 / 2; 7 % 2
来源：http://xb.shtwfgs.cn

Ruby: 7 / 2; 7 % 2
来源：http://bv.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://ez.shxzukj.cn

[A06] 字符串转数字
来源：http://kx.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://pb.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vu.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ky.shtwfgs.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uq.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yd.yuntaijiaju.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fe.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://we.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rz.521024.cn

[A07] 数字转字符串
来源：http://fq.szxytkj.cn

Py:   str(42)
来源：http://uu.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://jr.hahajie.cn

JS:   String(42); (42).toString()
来源：http://bm.shxzskj.cn

TS:   String(42)
来源：http://du.521024.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sx.wgjwhj.cn

Go:   strconv.Itoa(42)
来源：http://ah.yuntaijiaju.cn

Ruby: 42.to_s
来源：http://mw.521024.cn

C#:   42.ToString()
来源：http://ra.hnjuh.cn

[A08] 取整与四舍五入
来源：http://lw.asd995.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ju.wgjwhj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qc.gzmigu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hr.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sl.panjiajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://if.jctech888.com.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bh.wgjwhj.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ow.chemitech.net.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wy.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://zw.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bm.hahajie.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xo.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://sg.hahajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tj.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ii.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ct.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tg.huanxung.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://sc.bookmarksfly.cn

[A10] 生成随机数
来源：http://yq.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://sh.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://hx.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://sc.jianghongdianzi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fd.panjiajie.cn

Java: new Random().nextInt(100) + 1
来源：http://sn.9csxet.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hv.yuexingan06.cn

Ruby: rand(1..100)
来源：http://ie.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://pq.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://dk.asd995.cn

Py:   "yes" if x > 0 else "no"
来源：http://ff.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qd.panjiajie.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ok.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lg.colortex.cn

Java: x > 0 ? "yes" : "no"
来源：http://nv.haigaiapp.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ro.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://zk.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xs.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://qq.jianghongdianzi.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ur.bjjhwx.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zb.jctech888.com.cn

JS:   `Hello, ${name}!`
来源：http://fv.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://ma.colortex.cn

Java: "Hello, %s!".formatted(name)
来源：http://cz.yuntaijiaju.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qb.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://wv.panjiajie.cn

C#:   $"Hello, {name}!"
来源：http://vr.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://jz.newstarts.cn

Py:   "第一行\n第二行"
来源：http://hz.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://ow.wgjwhj.cn

JS:   "第一行\n第二行"
来源：http://qy.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://ly.panjiajie.cn

Java: "第一行\n第二行"
来源：http://bu.panjiajie.cn

Go:   "第一行\n第二行"
来源：http://gq.haigaiapp.cn

Ruby: "第一行\n第二行"
来源：http://rp.hahajie.cn

C#:   "第一行\n第二行"
来源：http://gb.yuntaijiaju.cn

[A14] 注释写法
来源：http://mf.muxihuayi.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://ak.yuntaijiaju.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://wn.panjiajie.cn

JS:   // 单行；/* 多行 */
来源：http://bg.muxihuayi.cn

TS:   // 单行；/* 多行 */
来源：http://mk.yuntaijiaju.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iq.shxzukj.cn

Go:   // 单行；/* 多行 */
来源：http://an.huixinmuqiang.cn

Ruby: # 单行；=begin 多行 =end
来源：http://qz.szsharing.cn

C#:   // 单行；/* 多行 */
来源：http://az.asd995.cn

[A15] 空值判断与默认值
来源：http://zf.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://bn.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://is.9csxet.cn

JS:   const value = data ?? "默认值";
来源：http://lb.huixinmuqiang.cn

TS:   const value = data ?? "默认值";
来源：http://vy.wgjwhj.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://zf.gzmigu.cn

Go:   if data == "" { data = "默认值" }
来源：http://un.huanxung.cn

Ruby: value = data || "默认值"
来源：http://bf.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://te.colortex.cn

[A16] 真假值判断规则
来源：http://bl.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ia.huixiangedu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tt.yuntaijiaju.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ur.nicolike.cn

TS:   if (!x) {}
来源：http://bg.huixinmuqiang.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wo.jctech888.com.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kf.newstarts.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gl.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ae.wgjwhj.cn

[A17] 位运算
来源：http://hr.chemitech.net.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ji.wgjwhj.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://to.newstarts.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fx.shxzukj.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ji.nszjky.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cu.gzmigu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ov.yuntaijiaju.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ql.bookmarksfly.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sz.szxytkj.cn

[A18] 字符与 ASCII 码互转
来源：http://lk.newstarts.cn

Py:   ord("A"); chr(65)
来源：http://tz.huixiangedu.cn

PHP:  ord("A"); chr(65)
来源：http://mz.bjjhwx.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sn.panjiajie.cn


<!-- 参考信息 -->