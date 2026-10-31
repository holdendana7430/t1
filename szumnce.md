代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://cv.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sm.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://di.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rg.haigaiapp.cn

[U85] JS：可选链
来源：http://to.gzmigu.cn

a?.b?.c
来源：http://dv.jianghongdianzi.cn

[U86] JS：空值合并
来源：http://rj.colortex.cn

a ?? b
来源：http://yl.nszjky.cn

[U87] JS：解构默认值
来源：http://nx.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://al.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://zv.huixiangedu.cn

{ ...a, ...b }
来源：http://ry.chemitech.net.cn

[U89] JS：数组去重
来源：http://bp.lnxyls.cn

[...new Set(arr)]
来源：http://fc.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://ha.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://xc.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://ep.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wl.shtwfgs.cn

[U92] JS：深拷贝
来源：http://tu.colortex.cn

structuredClone(obj)
来源：http://wv.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://zm.jianghongdianzi.cn

`共 ${n} 条`
来源：http://kt.asd995.cn

[U94] JS：箭头函数
来源：http://tn.shtwfgs.cn

const double = x => x * 2;
来源：http://qy.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://xe.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://un.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://mx.9csxet.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ly.newstarts.cn

[U97] JS：并发请求
来源：http://en.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://xq.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://dl.nszjky.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://be.521024.cn

[U99] JS：事件监听
来源：http://br.nicolike.cn

el.addEventListener("click", e => {})
来源：http://dc.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://zo.panjiajie.cn

document.querySelector(".item")
来源：http://wq.colortex.cn

[U101] JS：classList 操作
来源：http://gx.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://gy.9csxet.cn

[U102] JS：本地存储
来源：http://hg.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://kb.shxzskj.cn

[U103] JS：定时器
来源：http://yc.jianghongdianzi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mb.521024.cn

[U104] JS：防抖
来源：http://zv.huixinmuqiang.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tb.9csxet.cn

[U105] JS：节流
来源：http://hy.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ew.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://cz.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qo.shtwfgs.cn

[U107] JS：数字千分位
来源：http://vb.newstarts.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mr.gzmigu.cn

[U108] JS：随机整数
来源：http://ec.haigaiapp.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://if.jctech888.com.cn

[U109] JS：数组分组
来源：http://jn.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://ey.521024.cn

[U110] JS：数组分块
来源：http://nk.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iq.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://xw.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://xe.hahajie.cn

[U112] JS：字符串补位
来源：http://ky.shtwfgs.cn

"7".padStart(3, "0")
来源：http://sc.shxzukj.cn

[U113] JS：正则替换全部
来源：http://ad.szxytkj.cn

s.replaceAll("a", "b")
来源：http://nq.colortex.cn

[U114] JS：JSON 深比较
来源：http://sc.muxihuayi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sb.asd995.cn

[U115] JS：生成 UUID
来源：http://qz.newstarts.cn

crypto.randomUUID()
来源：http://mx.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://yp.muxihuayi.cn

/** @param {string} name */ function f(name) {}
来源：http://uc.jctech888.com.cn

[U117] JS：单元测试
来源：http://kg.jianghongdianzi.cn

npm i -D vitest;  npx vitest
来源：http://uz.jctech888.com.cn

[U118] JS：开发服务器
来源：http://bm.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://gx.bookmarksfly.cn

[U119] JS：生产构建
来源：http://il.jianghongdianzi.cn

npx vite build
来源：http://ny.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://zb.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://jl.shxzskj.cn

================================================================================
来源：http://yy.yuexingan06.cn

统计汇总
来源：http://fk.yuexingan06.cn

================================================================================
来源：http://vz.521024.cn

按语言统计（条）：
来源：http://xh.hahajie.cn

Python ......... 252
来源：http://ca.szxytkj.cn

PHP ............ 252
来源：http://vu.9csxet.cn

JavaScript ..... 252
来源：http://bg.newstarts.cn

TypeScript ..... 212
来源：http://xl.nicolike.cn

Java ........... 212
来源：http://iq.shxzskj.cn

Go ............. 212
来源：http://xz.lnxyls.cn

Ruby ........... 212
来源：http://yf.gzmigu.cn

C# ............. 212
来源：http://pz.hnjuh.cn

C .............. 30
来源：http://yk.shtwfgs.cn

C++ ............ 30
来源：http://qw.nszjky.cn

SQL ............ 90
来源：http://sl.asd995.cn

Bash ........... 80
来源：http://xe.newstarts.cn

Kotlin ......... 15
来源：http://mb.jianghongdianzi.cn

Swift .......... 15
来源：http://oi.yuntaijiaju.cn

Lua ............ 10
来源：http://qi.huixiangedu.cn

Perl ........... 10
来源：http://tf.jianghongdianzi.cn

Scala .......... 10
来源：http://uu.huixiangedu.cn

------------------------------------
来源：http://wa.shtwfgs.cn

合计 ........... 2106 条
来源：http://yt.bjjhwx.cn

按章节统计：
来源：http://tf.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rk.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nc.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zc.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://az.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://in.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lq.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://un.hnjuh.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ev.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ju.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lf.colortex.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sw.bjjhwx.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ha.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://di.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://tz.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yj.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wg.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://gw.huixiangedu.cn

R Bash 专题                             80
来源：http://mv.hahajie.cn

S C / C++ 专题                          60
来源：http://wa.shxzskj.cn

T 其他语言补充                          60
来源：http://gn.huanxung.cn

U 高频实用片段                         120
来源：http://yr.haigaiapp.cn

------------------------------------
来源：http://vs.shtwfgs.cn

合计                                  2106 条
来源：http://ls.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://xi.yuexingan06.cn

使用提醒
来源：http://de.asd995.cn

--------------------------------------------------------------------------------
来源：http://rw.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nw.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tu.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dm.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ze.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tr.yuntaijiaju.cn

—— 文件结束 ——
来源：http://sq.szsharing.cn

================================================================================
来源：http://tt.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://tl.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://qj.nicolike.cn

================================================================================
来源：http://cz.szxytkj.cn

【收录内容】
来源：http://ur.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vi.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bo.yuexingan06.cn

SQL · Bash · C · C++
来源：http://se.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dj.yuexingan06.cn

【使用说明】
来源：http://rs.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vb.shtwfgs.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gl.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bq.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eb.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ag.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iy.wgjwhj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tp.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cn.colortex.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bj.chemitech.net.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bv.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uv.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qp.szsharing.cn

【文件统计】
来源：http://it.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://oy.newstarts.cn

--------------------------------------------------------------------------------
来源：http://sz.colortex.cn

目  录
来源：http://zd.nszjky.cn

--------------------------------------------------------------------------------
来源：http://tc.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://qj.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vp.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ko.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zq.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ak.asd995.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://cw.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uw.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ot.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://az.9csxet.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mj.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xn.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tn.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xi.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xt.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pc.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jw.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://li.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ll.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sg.lnxyls.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tw.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rl.9csxet.cn

================================================================================
来源：http://yz.521024.cn

A. 基础语法与类型
来源：http://qf.521024.cn

================================================================================
来源：http://av.jctech888.com.cn

[A01] Hello World
来源：http://ph.hahajie.cn

Py:   print("Hello, World!")
来源：http://od.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://bu.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://mu.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ml.521024.cn

Java: System.out.println("Hello, World!");
来源：http://eq.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://uv.huixinmuqiang.cn

Ruby: puts "Hello, World!"
来源：http://ql.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lc.nszjky.cn

[A02] 变量声明与赋值
来源：http://dk.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jd.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ir.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://bw.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://iw.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://xw.lnxyls.cn

Go:   name := "Alex"; age := 20
来源：http://mj.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://kz.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ew.nicolike.cn

[A03] 常量定义
来源：http://lq.yuexingan06.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jf.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://xn.newstarts.cn

JS:   const PI = 3.14159;
来源：http://ue.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://bp.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://gm.gzmigu.cn

Go:   const PI = 3.14159
来源：http://sv.nszjky.cn

Ruby: PI = 3.14159
来源：http://pn.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://ud.yuexingan06.cn

[A04] 判断变量类型
来源：http://yx.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oq.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oj.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://eg.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://lq.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wl.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jv.jctech888.com.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gt.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://fz.hnjuh.cn

[A05] 整数除法与取模
来源：http://dh.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sz.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rg.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lj.gzmigu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://iz.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://ag.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://mi.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://to.521024.cn

C#:   7 / 2; 7 % 2
来源：http://uc.muxihuayi.cn

[A06] 字符串转数字
来源：http://hu.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://dm.panjiajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://be.szxytkj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xp.colortex.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yd.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ly.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qu.muxihuayi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hw.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dr.colortex.cn

[A07] 数字转字符串
来源：http://rm.muxihuayi.cn

Py:   str(42)
来源：http://ke.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://cu.yuntaijiaju.cn

JS:   String(42); (42).toString()
来源：http://mx.szxytkj.cn

TS:   String(42)
来源：http://lo.hnjuh.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://sl.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://nq.shxzukj.cn

Ruby: 42.to_s
来源：http://rt.nicolike.cn

C#:   42.ToString()
来源：http://kc.shxzukj.cn

[A08] 取整与四舍五入
来源：http://eo.newstarts.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hi.panjiajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xi.wgjwhj.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xg.szxytkj.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pc.jianghongdianzi.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mb.nicolike.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://cc.newstarts.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yl.asd995.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zm.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://kf.9csxet.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://at.gzmigu.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qp.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ds.panjiajie.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ra.shtwfgs.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://bl.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://vh.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://uf.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wv.szxytkj.cn

[A10] 生成随机数
来源：http://km.huixiangedu.cn

Py:   import random; random.randint(1, 100)
来源：http://yf.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://du.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xe.yuexingan06.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qi.asd995.cn

Java: new Random().nextInt(100) + 1
来源：http://wj.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://pd.gzmigu.cn

Ruby: rand(1..100)
来源：http://zr.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://tm.bookmarksfly.cn

[A11] 条件表达式（三元）
来源：http://go.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://zj.huixinmuqiang.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yn.yuexingan06.cn

JS:   x > 0 ? "yes" : "no"
来源：http://av.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ik.lnxyls.cn

Java: x > 0 ? "yes" : "no"
来源：http://cw.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://wq.asd995.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://qt.nszjky.cn

C#:   x > 0 ? "yes" : "no"
来源：http://uk.newstarts.cn

[A12] 字符串插值 / 格式化
来源：http://ha.huanxung.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sy.newstarts.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://tp.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://uu.szsharing.cn

TS:   `Hello, ${name}!`
来源：http://yo.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://bf.shtwfgs.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://ix.haigaiapp.cn

Ruby: "Hello, #{name}!"
来源：http://yi.9csxet.cn

C#:   $"Hello, {name}!"
来源：http://xc.9csxet.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://gu.haigaiapp.cn

Py:   "第一行\n第二行"
来源：http://iw.colortex.cn

PHP:  "第一行\n第二行"
来源：http://wr.gzmigu.cn

JS:   "第一行\n第二行"
来源：http://ew.shtwfgs.cn

TS:   "第一行\n第二行"
来源：http://qi.wgjwhj.cn

Java: "第一行\n第二行"
来源：http://vz.asd995.cn

Go:   "第一行\n第二行"
来源：http://sy.lnxyls.cn

Ruby: "第一行\n第二行"
来源：http://wm.haigaiapp.cn

C#:   "第一行\n第二行"
来源：http://ga.nszjky.cn


<!-- 参考信息 -->