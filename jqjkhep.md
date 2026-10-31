代发 wailian999

[U93] JS：模板字符串
来源：http://ev.shxzukj.cn

`共 ${n} 条`
来源：http://zh.colortex.cn

[U94] JS：箭头函数
来源：http://er.huanxung.cn

const double = x => x * 2;
来源：http://ds.lnxyls.cn

[U95] JS：Promise 包装
来源：http://by.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://kj.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://kp.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hb.huanxung.cn

[U97] JS：并发请求
来源：http://zj.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ed.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://kv.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vp.wgjwhj.cn

[U99] JS：事件监听
来源：http://gg.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://nr.lnxyls.cn

[U100] JS：DOM 查询
来源：http://yh.muxihuayi.cn

document.querySelector(".item")
来源：http://us.nszjky.cn

[U101] JS：classList 操作
来源：http://xc.bookmarksfly.cn

el.classList.toggle("active")
来源：http://bq.huanxung.cn

[U102] JS：本地存储
来源：http://gd.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lf.hnjuh.cn

[U103] JS：定时器
来源：http://fw.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jy.shxzskj.cn

[U104] JS：防抖
来源：http://ue.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ca.bjjhwx.cn

[U105] JS：节流
来源：http://zy.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://jo.yuntaijiaju.cn

[U106] JS：日期格式化
来源：http://as.hahajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sx.panjiajie.cn

[U107] JS：数字千分位
来源：http://nm.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://op.colortex.cn

[U108] JS：随机整数
来源：http://bj.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ed.jctech888.com.cn

[U109] JS：数组分组
来源：http://ny.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://ch.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://sj.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qb.shtwfgs.cn

[U111] JS：对象转 Map
来源：http://mb.hahajie.cn

new Map(Object.entries(obj))
来源：http://zd.panjiajie.cn

[U112] JS：字符串补位
来源：http://mc.521024.cn

"7".padStart(3, "0")
来源：http://xl.panjiajie.cn

[U113] JS：正则替换全部
来源：http://ab.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://wo.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://si.gzmigu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lb.nszjky.cn

[U115] JS：生成 UUID
来源：http://hj.shxzukj.cn

crypto.randomUUID()
来源：http://tw.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://ju.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://qo.asd995.cn

[U117] JS：单元测试
来源：http://zz.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://po.wgjwhj.cn

[U118] JS：开发服务器
来源：http://bb.newstarts.cn

npm i -D vite;  npx vite
来源：http://ms.haigaiapp.cn

[U119] JS：生产构建
来源：http://mn.hahajie.cn

npx vite build
来源：http://ye.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://fh.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://dw.panjiajie.cn

================================================================================
来源：http://hp.jctech888.com.cn

统计汇总
来源：http://he.521024.cn

================================================================================
来源：http://py.hahajie.cn

按语言统计（条）：
来源：http://ru.jianghongdianzi.cn

Python ......... 252
来源：http://vk.nicolike.cn

PHP ............ 252
来源：http://th.gzmigu.cn

JavaScript ..... 252
来源：http://sd.hnjuh.cn

TypeScript ..... 212
来源：http://kz.bjjhwx.cn

Java ........... 212
来源：http://pk.lnxyls.cn

Go ............. 212
来源：http://ne.hnjuh.cn

Ruby ........... 212
来源：http://um.yuntaijiaju.cn

C# ............. 212
来源：http://bq.szsharing.cn

C .............. 30
来源：http://az.shxzskj.cn

C++ ............ 30
来源：http://ht.bjjhwx.cn

SQL ............ 90
来源：http://vo.huixiangedu.cn

Bash ........... 80
来源：http://oz.jianghongdianzi.cn

Kotlin ......... 15
来源：http://nj.521024.cn

Swift .......... 15
来源：http://re.yuexingan06.cn

Lua ............ 10
来源：http://qs.yuntaijiaju.cn

Perl ........... 10
来源：http://sx.yuntaijiaju.cn

Scala .......... 10
来源：http://sf.shxzukj.cn

------------------------------------
来源：http://tt.szsharing.cn

合计 ........... 2106 条
来源：http://wa.yuntaijiaju.cn

按章节统计：
来源：http://bo.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xq.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vt.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pf.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bo.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sv.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qi.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fo.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wh.huanxung.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ka.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rp.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lc.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wl.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mc.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ma.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wh.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yr.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://ie.nicolike.cn

R Bash 专题                             80
来源：http://wp.nszjky.cn

S C / C++ 专题                          60
来源：http://cn.huixiangedu.cn

T 其他语言补充                          60
来源：http://bb.huixiangedu.cn

U 高频实用片段                         120
来源：http://qb.newstarts.cn

------------------------------------
来源：http://rr.szxytkj.cn

合计                                  2106 条
来源：http://to.9csxet.cn

--------------------------------------------------------------------------------
来源：http://qc.jianghongdianzi.cn

使用提醒
来源：http://xy.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ti.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ko.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://te.huixinmuqiang.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dm.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xh.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tf.bjjhwx.cn

—— 文件结束 ——
来源：http://dc.huanxung.cn

================================================================================
来源：http://cr.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://py.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://zp.wgjwhj.cn

================================================================================
来源：http://ia.nicolike.cn

【收录内容】
来源：http://qu.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xr.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kx.hahajie.cn

SQL · Bash · C · C++
来源：http://wp.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xm.bookmarksfly.cn

【使用说明】
来源：http://ws.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xw.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pv.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://rl.wgjwhj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gj.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://oz.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hh.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nd.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ay.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zx.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kz.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://tp.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dk.colortex.cn

【文件统计】
来源：http://ep.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jb.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ze.lnxyls.cn

目  录
来源：http://cr.521024.cn

--------------------------------------------------------------------------------
来源：http://se.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://xi.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tz.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vc.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://at.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://cy.jctech888.com.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lc.yuexingan06.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ys.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ai.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://og.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://oi.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://uo.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://po.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dt.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zx.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nc.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ye.gzmigu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wy.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pf.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mh.jianghongdianzi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mw.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wc.9csxet.cn

================================================================================
来源：http://kq.huanxung.cn

A. 基础语法与类型
来源：http://mc.521024.cn

================================================================================
来源：http://mg.muxihuayi.cn

[A01] Hello World
来源：http://hr.gzmigu.cn

Py:   print("Hello, World!")
来源：http://oi.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://uw.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://up.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pt.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://ss.asd995.cn

Go:   fmt.Println("Hello, World!")
来源：http://lt.shxzskj.cn

Ruby: puts "Hello, World!"
来源：http://eh.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jc.wgjwhj.cn

[A02] 变量声明与赋值
来源：http://bg.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fe.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gh.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://du.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pt.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://jq.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://db.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://qh.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://io.jctech888.com.cn

[A03] 常量定义
来源：http://de.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://do.hnjuh.cn

PHP:  const PI = 3.14159;
来源：http://oc.colortex.cn

JS:   const PI = 3.14159;
来源：http://qe.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://uh.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://wl.shxzskj.cn

Go:   const PI = 3.14159
来源：http://ha.panjiajie.cn

Ruby: PI = 3.14159
来源：http://mu.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://ax.newstarts.cn

[A04] 判断变量类型
来源：http://cg.jctech888.com.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://nh.yuntaijiaju.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qz.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fc.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://wr.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jk.gzmigu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bx.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://da.colortex.cn

C#:   x.GetType().Name; x is int
来源：http://yc.jctech888.com.cn

[A05] 整数除法与取模
来源：http://em.haigaiapp.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://dc.9csxet.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iu.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nw.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://om.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://zf.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://oa.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://tf.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://rt.wgjwhj.cn

[A06] 字符串转数字
来源：http://mf.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://pn.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hc.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qx.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ce.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uv.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lr.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://be.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ch.nszjky.cn

[A07] 数字转字符串
来源：http://fy.huanxung.cn

Py:   str(42)
来源：http://jk.bjjhwx.cn

PHP:  (string) 42; strval(42)
来源：http://vy.yuexingan06.cn

JS:   String(42); (42).toString()
来源：http://mq.szxytkj.cn

TS:   String(42)
来源：http://qe.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://xp.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://vw.shtwfgs.cn

Ruby: 42.to_s
来源：http://ia.yuexingan06.cn

C#:   42.ToString()
来源：http://ds.szsharing.cn

[A08] 取整与四舍五入
来源：http://lz.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://gy.bjjhwx.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ad.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rt.shtwfgs.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sf.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://kr.asd995.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fu.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qq.lnxyls.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jj.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://oj.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://nf.hnjuh.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yo.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://cs.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xg.shxzskj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://us.bookmarksfly.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ju.shtwfgs.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wo.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tp.521024.cn

[A10] 生成随机数
来源：http://fk.chemitech.net.cn

Py:   import random; random.randint(1, 100)
来源：http://zn.521024.cn

PHP:  random_int(1, 100);
来源：http://yi.huanxung.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qh.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://va.bjjhwx.cn

Java: new Random().nextInt(100) + 1
来源：http://vz.asd995.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ze.shxzskj.cn

Ruby: rand(1..100)
来源：http://ht.huanxung.cn

C#:   new Random().Next(1, 101)
来源：http://ua.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://qt.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://lx.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bj.chemitech.net.cn

JS:   x > 0 ? "yes" : "no"
来源：http://jv.yuexingan06.cn

TS:   x > 0 ? "yes" : "no"
来源：http://bd.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://ze.521024.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yi.shxzukj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://ru.jianghongdianzi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://gu.chemitech.net.cn

[A12] 字符串插值 / 格式化
来源：http://vp.chemitech.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://fk.521024.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://fa.bjjhwx.cn

JS:   `Hello, ${name}!`
来源：http://ka.521024.cn

TS:   `Hello, ${name}!`
来源：http://kq.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://jp.nszjky.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wh.9csxet.cn

Ruby: "Hello, #{name}!"
来源：http://zs.colortex.cn

C#:   $"Hello, {name}!"
来源：http://xs.wgjwhj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://sg.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://qd.panjiajie.cn

PHP:  "第一行\n第二行"
来源：http://od.jianghongdianzi.cn

JS:   "第一行\n第二行"
来源：http://rl.huixiangedu.cn

TS:   "第一行\n第二行"
来源：http://pp.muxihuayi.cn

Java: "第一行\n第二行"
来源：http://iu.yuexingan06.cn

Go:   "第一行\n第二行"
来源：http://it.hnjuh.cn

Ruby: "第一行\n第二行"
来源：http://xt.bjjhwx.cn

C#:   "第一行\n第二行"
来源：http://rk.muxihuayi.cn

[A14] 注释写法
来源：http://kl.jctech888.com.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://es.colortex.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://mf.shxzskj.cn

JS:   // 单行；/* 多行 */
来源：http://ig.hahajie.cn

TS:   // 单行；/* 多行 */
来源：http://st.jctech888.com.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://yq.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://xw.jctech888.com.cn

Ruby: # 单行；=begin 多行 =end
来源：http://na.asd995.cn

C#:   // 单行；/* 多行 */
来源：http://mv.huanxung.cn

[A15] 空值判断与默认值
来源：http://js.bjjhwx.cn

Py:   value = data or "默认值"
来源：http://of.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://bi.lnxyls.cn

JS:   const value = data ?? "默认值";
来源：http://bs.bookmarksfly.cn

TS:   const value = data ?? "默认值";
来源：http://ft.jctech888.com.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lu.huanxung.cn

Go:   if data == "" { data = "默认值" }
来源：http://kg.muxihuayi.cn

Ruby: value = data || "默认值"
来源：http://pp.shxzskj.cn

C#:   var value = data ?? "默认值";
来源：http://wp.huixiangedu.cn

[A16] 真假值判断规则
来源：http://xj.chemitech.net.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://yj.gzmigu.cn


<!-- 参考信息 -->