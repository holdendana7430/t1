代发 wailian999

[U91] JS：对象键值遍历
来源：http://ma.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://yu.szsharing.cn

[U92] JS：深拷贝
来源：http://bi.panjiajie.cn

structuredClone(obj)
来源：http://pr.szxytkj.cn

[U93] JS：模板字符串
来源：http://qe.colortex.cn

`共 ${n} 条`
来源：http://cf.shxzskj.cn

[U94] JS：箭头函数
来源：http://av.yuntaijiaju.cn

const double = x => x * 2;
来源：http://iv.9csxet.cn

[U95] JS：Promise 包装
来源：http://fx.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://uv.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://la.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nc.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://vl.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ym.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://de.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ot.lnxyls.cn

[U99] JS：事件监听
来源：http://hb.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://yq.bjjhwx.cn

[U100] JS：DOM 查询
来源：http://xc.bookmarksfly.cn

document.querySelector(".item")
来源：http://rh.521024.cn

[U101] JS：classList 操作
来源：http://eg.shxzukj.cn

el.classList.toggle("active")
来源：http://lm.bookmarksfly.cn

[U102] JS：本地存储
来源：http://pn.jctech888.com.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lk.yuntaijiaju.cn

[U103] JS：定时器
来源：http://bs.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xo.wgjwhj.cn

[U104] JS：防抖
来源：http://zj.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fu.nszjky.cn

[U105] JS：节流
来源：http://yy.panjiajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bx.hahajie.cn

[U106] JS：日期格式化
来源：http://ut.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://el.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://ud.huanxung.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://as.huanxung.cn

[U108] JS：随机整数
来源：http://jc.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hr.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://kh.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://ty.newstarts.cn

[U110] JS：数组分块
来源：http://aq.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uc.nicolike.cn

[U111] JS：对象转 Map
来源：http://ab.shxzukj.cn

new Map(Object.entries(obj))
来源：http://dk.newstarts.cn

[U112] JS：字符串补位
来源：http://mg.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://kq.colortex.cn

[U113] JS：正则替换全部
来源：http://ux.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://en.jianghongdianzi.cn

[U114] JS：JSON 深比较
来源：http://dv.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sj.shxzskj.cn

[U115] JS：生成 UUID
来源：http://tr.jianghongdianzi.cn

crypto.randomUUID()
来源：http://sx.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://ds.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://op.shxzskj.cn

[U117] JS：单元测试
来源：http://cy.asd995.cn

npm i -D vitest;  npx vitest
来源：http://yf.9csxet.cn

[U118] JS：开发服务器
来源：http://nj.huanxung.cn

npm i -D vite;  npx vite
来源：http://cp.haigaiapp.cn

[U119] JS：生产构建
来源：http://nr.szsharing.cn

npx vite build
来源：http://bb.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://jh.szxytkj.cn

import.meta.env.VITE_API_URL
来源：http://dj.szsharing.cn

================================================================================
来源：http://mv.shtwfgs.cn

统计汇总
来源：http://vm.nszjky.cn

================================================================================
来源：http://uc.haigaiapp.cn

按语言统计（条）：
来源：http://ru.nicolike.cn

Python ......... 252
来源：http://me.shtwfgs.cn

PHP ............ 252
来源：http://sw.haigaiapp.cn

JavaScript ..... 252
来源：http://gj.bjjhwx.cn

TypeScript ..... 212
来源：http://uh.bookmarksfly.cn

Java ........... 212
来源：http://jo.nszjky.cn

Go ............. 212
来源：http://ok.huixinmuqiang.cn

Ruby ........... 212
来源：http://ja.yuexingan06.cn

C# ............. 212
来源：http://ua.colortex.cn

C .............. 30
来源：http://rv.shtwfgs.cn

C++ ............ 30
来源：http://zg.9csxet.cn

SQL ............ 90
来源：http://ci.shxzskj.cn

Bash ........... 80
来源：http://dj.hnjuh.cn

Kotlin ......... 15
来源：http://xk.lnxyls.cn

Swift .......... 15
来源：http://rt.bookmarksfly.cn

Lua ............ 10
来源：http://qe.yuexingan06.cn

Perl ........... 10
来源：http://tm.bjjhwx.cn

Scala .......... 10
来源：http://bg.huixinmuqiang.cn

------------------------------------
来源：http://ed.jctech888.com.cn

合计 ........... 2106 条
来源：http://pc.muxihuayi.cn

按章节统计：
来源：http://vi.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ef.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://jh.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ht.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sd.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tk.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ao.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ro.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fb.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wz.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rt.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yx.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hp.521024.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://jb.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://yu.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fd.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ml.hnjuh.cn

Q SQL 专题                              90
来源：http://yv.yuexingan06.cn

R Bash 专题                             80
来源：http://za.521024.cn

S C / C++ 专题                          60
来源：http://ba.yuexingan06.cn

T 其他语言补充                          60
来源：http://fd.wgjwhj.cn

U 高频实用片段                         120
来源：http://mc.nszjky.cn

------------------------------------
来源：http://ru.jctech888.com.cn

合计                                  2106 条
来源：http://fk.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ud.shxzskj.cn

使用提醒
来源：http://yo.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://tq.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zo.shxzskj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ha.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yp.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hp.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bi.yuntaijiaju.cn

—— 文件结束 ——
来源：http://gx.wgjwhj.cn

================================================================================
来源：http://my.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ee.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://of.bookmarksfly.cn

================================================================================
来源：http://wb.yuntaijiaju.cn

【收录内容】
来源：http://kk.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dm.shxzskj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ds.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://hu.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://is.newstarts.cn

【使用说明】
来源：http://em.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dx.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ny.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wi.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wi.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ac.bookmarksfly.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ks.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ec.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://es.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vv.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://iz.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fk.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vy.lnxyls.cn

【文件统计】
来源：http://ye.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ys.nicolike.cn

--------------------------------------------------------------------------------
来源：http://mu.shtwfgs.cn

目  录
来源：http://af.szsharing.cn

--------------------------------------------------------------------------------
来源：http://kl.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ol.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://an.colortex.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://es.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cf.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oz.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://na.shtwfgs.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iv.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zh.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://kf.colortex.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bj.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ro.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://id.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qu.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uz.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wk.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cp.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://lz.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lw.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fk.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ri.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mg.shxzukj.cn

================================================================================
来源：http://vc.jctech888.com.cn

A. 基础语法与类型
来源：http://om.521024.cn

================================================================================
来源：http://qy.huixiangedu.cn

[A01] Hello World
来源：http://qa.huanxung.cn

Py:   print("Hello, World!")
来源：http://tq.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://ep.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://pk.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jd.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://mc.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://el.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://du.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://pm.yuntaijiaju.cn

[A02] 变量声明与赋值
来源：http://nz.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rd.muxihuayi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dv.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hy.szxytkj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sv.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://ws.huanxung.cn

Go:   name := "Alex"; age := 20
来源：http://la.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://rx.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hq.shtwfgs.cn

[A03] 常量定义
来源：http://pr.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pr.jianghongdianzi.cn

PHP:  const PI = 3.14159;
来源：http://lb.521024.cn

JS:   const PI = 3.14159;
来源：http://ll.bookmarksfly.cn

TS:   const PI: number = 3.14159;
来源：http://em.colortex.cn

Java: static final double PI = 3.14159;
来源：http://pk.hahajie.cn

Go:   const PI = 3.14159
来源：http://fv.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://tt.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://qu.lnxyls.cn

[A04] 判断变量类型
来源：http://sm.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://id.yuexingan06.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://vr.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://of.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://vp.nszjky.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oi.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vg.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ei.521024.cn

C#:   x.GetType().Name; x is int
来源：http://nk.shxzukj.cn

[A05] 整数除法与取模
来源：http://gx.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cm.hahajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gh.newstarts.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://iu.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ef.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://rb.haigaiapp.cn

Go:   7 / 2; 7 % 2
来源：http://et.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://jc.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://nh.chemitech.net.cn

[A06] 字符串转数字
来源：http://xw.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://io.lnxyls.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hy.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yy.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://oj.nicolike.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ix.haigaiapp.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://gg.szxytkj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ds.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vq.muxihuayi.cn

[A07] 数字转字符串
来源：http://an.szsharing.cn

Py:   str(42)
来源：http://fv.shxzskj.cn

PHP:  (string) 42; strval(42)
来源：http://hq.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://le.muxihuayi.cn

TS:   String(42)
来源：http://zv.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://uk.panjiajie.cn

Go:   strconv.Itoa(42)
来源：http://ll.shxzskj.cn

Ruby: 42.to_s
来源：http://fv.shtwfgs.cn

C#:   42.ToString()
来源：http://bu.muxihuayi.cn

[A08] 取整与四舍五入
来源：http://ad.lnxyls.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://jz.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gh.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xq.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://am.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gp.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://el.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xx.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://eb.chemitech.net.cn

[A09] 绝对值与最大最小值
来源：http://nw.wgjwhj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://am.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://uy.huixinmuqiang.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vc.szsharing.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://cj.yuexingan06.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://dl.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.bookmarksfly.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mf.panjiajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://eh.jctech888.com.cn

[A10] 生成随机数
来源：http://oc.bookmarksfly.cn

Py:   import random; random.randint(1, 100)
来源：http://ya.szsharing.cn

PHP:  random_int(1, 100);
来源：http://ve.haigaiapp.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://we.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hm.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://tq.nicolike.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://um.huixiangedu.cn

Ruby: rand(1..100)
来源：http://bo.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://ed.asd995.cn

[A11] 条件表达式（三元）
来源：http://sw.bookmarksfly.cn

Py:   "yes" if x > 0 else "no"
来源：http://my.bjjhwx.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://az.huanxung.cn

JS:   x > 0 ? "yes" : "no"
来源：http://vv.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://gc.shxzskj.cn

Java: x > 0 ? "yes" : "no"
来源：http://wq.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://bi.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://tq.gzmigu.cn

C#:   x > 0 ? "yes" : "no"
来源：http://fs.hahajie.cn

[A12] 字符串插值 / 格式化
来源：http://tk.shxzskj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wa.9csxet.cn

JS:   `Hello, ${name}!`
来源：http://gi.521024.cn

TS:   `Hello, ${name}!`
来源：http://uu.huixinmuqiang.cn

Java: "Hello, %s!".formatted(name)
来源：http://du.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ua.asd995.cn

Ruby: "Hello, #{name}!"
来源：http://dc.huixinmuqiang.cn

C#:   $"Hello, {name}!"
来源：http://fh.shxzskj.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://fg.shtwfgs.cn

Py:   "第一行\n第二行"
来源：http://wy.yuntaijiaju.cn

PHP:  "第一行\n第二行"
来源：http://yj.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://cn.bjjhwx.cn

TS:   "第一行\n第二行"
来源：http://uo.lnxyls.cn

Java: "第一行\n第二行"
来源：http://vw.gzmigu.cn

Go:   "第一行\n第二行"
来源：http://ig.9csxet.cn

Ruby: "第一行\n第二行"
来源：http://gc.gzmigu.cn

C#:   "第一行\n第二行"
来源：http://ax.shtwfgs.cn

[A14] 注释写法
来源：http://xc.9csxet.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nj.nicolike.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yx.9csxet.cn

JS:   // 单行；/* 多行 */
来源：http://ue.jctech888.com.cn

TS:   // 单行；/* 多行 */
来源：http://qr.shxzskj.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dr.huanxung.cn

Go:   // 单行；/* 多行 */
来源：http://xp.shxzukj.cn

Ruby: # 单行；=begin 多行 =end
来源：http://az.chemitech.net.cn

C#:   // 单行；/* 多行 */
来源：http://pf.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://uu.panjiajie.cn

Py:   value = data or "默认值"
来源：http://ct.szsharing.cn

PHP:  $value = $data ?? "默认值";
来源：http://uh.521024.cn

JS:   const value = data ?? "默认值";
来源：http://gf.huanxung.cn

TS:   const value = data ?? "默认值";
来源：http://xy.nszjky.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yf.9csxet.cn

Go:   if data == "" { data = "默认值" }
来源：http://qq.asd995.cn


<!-- 参考信息 -->