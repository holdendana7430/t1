代发 wailian999

[U91] JS：对象键值遍历
来源：http://uz.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qe.chemitech.net.cn

[U92] JS：深拷贝
来源：http://dw.haigaiapp.cn

structuredClone(obj)
来源：http://fm.asd995.cn

[U93] JS：模板字符串
来源：http://as.bookmarksfly.cn

`共 ${n} 条`
来源：http://zs.shxzukj.cn

[U94] JS：箭头函数
来源：http://zl.jianghongdianzi.cn

const double = x => x * 2;
来源：http://xa.huixiangedu.cn

[U95] JS：Promise 包装
来源：http://mj.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://fc.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://oc.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://eo.haigaiapp.cn

[U97] JS：并发请求
来源：http://zf.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://mt.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://yt.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://or.hnjuh.cn

[U99] JS：事件监听
来源：http://oa.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://eu.huanxung.cn

[U100] JS：DOM 查询
来源：http://fs.nicolike.cn

document.querySelector(".item")
来源：http://jt.panjiajie.cn

[U101] JS：classList 操作
来源：http://kc.shtwfgs.cn

el.classList.toggle("active")
来源：http://gj.521024.cn

[U102] JS：本地存储
来源：http://fe.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ob.szsharing.cn

[U103] JS：定时器
来源：http://qa.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yq.wgjwhj.cn

[U104] JS：防抖
来源：http://oz.muxihuayi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kh.jianghongdianzi.cn

[U105] JS：节流
来源：http://jx.huixiangedu.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rv.hahajie.cn

[U106] JS：日期格式化
来源：http://mm.jianghongdianzi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://tw.asd995.cn

[U107] JS：数字千分位
来源：http://vk.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xx.gzmigu.cn

[U108] JS：随机整数
来源：http://fd.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bf.shtwfgs.cn

[U109] JS：数组分组
来源：http://cs.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://xp.huanxung.cn

[U110] JS：数组分块
来源：http://mo.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vs.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://xa.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://oe.szsharing.cn

[U112] JS：字符串补位
来源：http://qa.nszjky.cn

"7".padStart(3, "0")
来源：http://xa.shxzskj.cn

[U113] JS：正则替换全部
来源：http://vo.lnxyls.cn

s.replaceAll("a", "b")
来源：http://dx.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://gg.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nv.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://so.shxzskj.cn

crypto.randomUUID()
来源：http://wi.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://ys.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://nv.shtwfgs.cn

[U117] JS：单元测试
来源：http://ye.szsharing.cn

npm i -D vitest;  npx vitest
来源：http://ag.szsharing.cn

[U118] JS：开发服务器
来源：http://ad.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://fn.bjjhwx.cn

[U119] JS：生产构建
来源：http://pw.huixinmuqiang.cn

npx vite build
来源：http://kh.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://nj.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://gn.lnxyls.cn

================================================================================
来源：http://mb.huanxung.cn

统计汇总
来源：http://as.shtwfgs.cn

================================================================================
来源：http://lj.gzmigu.cn

按语言统计（条）：
来源：http://mf.asd995.cn

Python ......... 252
来源：http://hf.szxytkj.cn

PHP ............ 252
来源：http://sz.haigaiapp.cn

JavaScript ..... 252
来源：http://ch.haigaiapp.cn

TypeScript ..... 212
来源：http://zf.shxzskj.cn

Java ........... 212
来源：http://ci.bjjhwx.cn

Go ............. 212
来源：http://sm.shxzskj.cn

Ruby ........... 212
来源：http://yq.yuntaijiaju.cn

C# ............. 212
来源：http://ey.wgjwhj.cn

C .............. 30
来源：http://to.yuexingan06.cn

C++ ............ 30
来源：http://cn.huixinmuqiang.cn

SQL ............ 90
来源：http://uk.bjjhwx.cn

Bash ........... 80
来源：http://lq.yuexingan06.cn

Kotlin ......... 15
来源：http://vz.colortex.cn

Swift .......... 15
来源：http://ez.shtwfgs.cn

Lua ............ 10
来源：http://wz.newstarts.cn

Perl ........... 10
来源：http://qd.szxytkj.cn

Scala .......... 10
来源：http://uw.colortex.cn

------------------------------------
来源：http://jn.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://yt.shtwfgs.cn

按章节统计：
来源：http://wy.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nd.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fw.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cs.huixiangedu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://lu.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vy.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ob.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jr.asd995.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kx.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pd.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://te.shtwfgs.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pa.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://gx.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hl.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zy.shtwfgs.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://cu.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rg.newstarts.cn

Q SQL 专题                              90
来源：http://dy.shxzukj.cn

R Bash 专题                             80
来源：http://bc.bjjhwx.cn

S C / C++ 专题                          60
来源：http://rr.shxzukj.cn

T 其他语言补充                          60
来源：http://nc.nszjky.cn

U 高频实用片段                         120
来源：http://mq.huixiangedu.cn

------------------------------------
来源：http://yz.szsharing.cn

合计                                  2106 条
来源：http://ff.colortex.cn

--------------------------------------------------------------------------------
来源：http://yz.gzmigu.cn

使用提醒
来源：http://in.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://wc.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xl.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tl.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qb.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ze.jctech888.com.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qr.521024.cn

—— 文件结束 ——
来源：http://ku.hnjuh.cn

================================================================================
来源：http://ca.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://xl.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://ln.asd995.cn

================================================================================
来源：http://ae.jianghongdianzi.cn

【收录内容】
来源：http://fy.szsharing.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ry.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ti.9csxet.cn

SQL · Bash · C · C++
来源：http://va.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pi.shxzskj.cn

【使用说明】
来源：http://ql.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vm.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ye.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mj.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vc.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xz.nszjky.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://sp.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lc.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yc.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lw.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lp.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oz.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yj.szxytkj.cn

【文件统计】
来源：http://yc.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wl.colortex.cn

--------------------------------------------------------------------------------
来源：http://cv.jctech888.com.cn

目  录
来源：http://xa.nicolike.cn

--------------------------------------------------------------------------------
来源：http://gd.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wi.shxzukj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nb.newstarts.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ws.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cs.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qw.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fy.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gn.hnjuh.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uj.yuntaijiaju.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lw.yuntaijiaju.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qa.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nr.gzmigu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qj.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mb.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://nz.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://bi.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ue.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://of.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bg.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sy.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bl.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bh.newstarts.cn

================================================================================
来源：http://gt.shxzukj.cn

A. 基础语法与类型
来源：http://ly.wgjwhj.cn

================================================================================
来源：http://cq.wgjwhj.cn

[A01] Hello World
来源：http://ft.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://tu.lnxyls.cn

PHP:  echo "Hello, World!";
来源：http://zv.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://kc.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ri.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://bj.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://jq.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://sy.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vq.9csxet.cn

[A02] 变量声明与赋值
来源：http://et.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qe.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ju.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sk.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://on.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://vk.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://gx.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://mc.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mv.shtwfgs.cn

[A03] 常量定义
来源：http://br.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://go.colortex.cn

PHP:  const PI = 3.14159;
来源：http://dk.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://lh.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://xv.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://ya.hahajie.cn

Go:   const PI = 3.14159
来源：http://jl.hahajie.cn

Ruby: PI = 3.14159
来源：http://js.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://qe.jctech888.com.cn

[A04] 判断变量类型
来源：http://pi.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://vm.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://kp.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xa.bjjhwx.cn

TS:   typeof x; x instanceof Date
来源：http://gz.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fv.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ja.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fe.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://qx.shxzskj.cn

[A05] 整数除法与取模
来源：http://gf.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://si.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://xa.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hw.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bn.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://tn.panjiajie.cn

Go:   7 / 2; 7 % 2
来源：http://zn.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://yc.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://tb.yuexingan06.cn

[A06] 字符串转数字
来源：http://co.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://sj.asd995.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ps.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://op.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://iq.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xc.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://si.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ta.521024.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uz.newstarts.cn

[A07] 数字转字符串
来源：http://he.yuntaijiaju.cn

Py:   str(42)
来源：http://hq.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://kz.szsharing.cn

JS:   String(42); (42).toString()
来源：http://ad.hahajie.cn

TS:   String(42)
来源：http://ai.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://lc.shxzukj.cn

Go:   strconv.Itoa(42)
来源：http://bw.colortex.cn

Ruby: 42.to_s
来源：http://hq.huixinmuqiang.cn

C#:   42.ToString()
来源：http://pf.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://kl.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://um.muxihuayi.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://fz.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ra.521024.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jw.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tv.jianghongdianzi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://fc.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rt.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yy.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://mx.asd995.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xq.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nm.gzmigu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://my.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lw.huanxung.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tc.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://aj.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://aj.muxihuayi.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pv.szxytkj.cn

[A10] 生成随机数
来源：http://bo.hahajie.cn

Py:   import random; random.randint(1, 100)
来源：http://dq.chemitech.net.cn

PHP:  random_int(1, 100);
来源：http://au.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://qq.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://lm.hnjuh.cn

Java: new Random().nextInt(100) + 1
来源：http://se.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gd.huanxung.cn

Ruby: rand(1..100)
来源：http://um.bjjhwx.cn

C#:   new Random().Next(1, 101)
来源：http://ff.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://ca.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://qb.haigaiapp.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://vo.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://qy.jianghongdianzi.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qj.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://ol.wgjwhj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dn.hahajie.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xv.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://eb.lnxyls.cn

[A12] 字符串插值 / 格式化
来源：http://bd.yuntaijiaju.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hk.huixinmuqiang.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://au.chemitech.net.cn

JS:   `Hello, ${name}!`
来源：http://yn.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://vl.bookmarksfly.cn

Java: "Hello, %s!".formatted(name)
来源：http://nk.haigaiapp.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kg.jctech888.com.cn

Ruby: "Hello, #{name}!"
来源：http://xd.colortex.cn

C#:   $"Hello, {name}!"
来源：http://ww.gzmigu.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://me.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://jl.szxytkj.cn

PHP:  "第一行\n第二行"
来源：http://nl.jctech888.com.cn

JS:   "第一行\n第二行"
来源：http://gh.9csxet.cn

TS:   "第一行\n第二行"
来源：http://yv.chemitech.net.cn

Java: "第一行\n第二行"
来源：http://wl.bjjhwx.cn

Go:   "第一行\n第二行"
来源：http://qr.huanxung.cn

Ruby: "第一行\n第二行"
来源：http://qm.wgjwhj.cn

C#:   "第一行\n第二行"
来源：http://yw.9csxet.cn

[A14] 注释写法
来源：http://se.yuexingan06.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://vs.jctech888.com.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ry.nszjky.cn

JS:   // 单行；/* 多行 */
来源：http://kr.jianghongdianzi.cn

TS:   // 单行；/* 多行 */
来源：http://ul.jianghongdianzi.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vh.shxzskj.cn

Go:   // 单行；/* 多行 */
来源：http://lr.huixiangedu.cn

Ruby: # 单行；=begin 多行 =end
来源：http://od.colortex.cn

C#:   // 单行；/* 多行 */
来源：http://da.muxihuayi.cn

[A15] 空值判断与默认值
来源：http://zo.asd995.cn

Py:   value = data or "默认值"
来源：http://ck.yuexingan06.cn

PHP:  $value = $data ?? "默认值";
来源：http://sd.hahajie.cn

JS:   const value = data ?? "默认值";
来源：http://sq.lnxyls.cn

TS:   const value = data ?? "默认值";
来源：http://ve.newstarts.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tp.nicolike.cn

Go:   if data == "" { data = "默认值" }
来源：http://je.nicolike.cn


<!-- 参考信息 -->