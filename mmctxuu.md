代发 wailian999

[U81] JS：初始化项目
来源：http://rp.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://ib.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://ty.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lo.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ue.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ce.nicolike.cn

[U84] JS：CommonJS 写法
来源：http://at.bjjhwx.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wa.521024.cn

[U85] JS：可选链
来源：http://hf.bookmarksfly.cn

a?.b?.c
来源：http://ul.gzmigu.cn

[U86] JS：空值合并
来源：http://po.bjjhwx.cn

a ?? b
来源：http://yc.shtwfgs.cn

[U87] JS：解构默认值
来源：http://hg.yuexingan06.cn

const { a = 1, b = 2 } = obj;
来源：http://wy.shxzskj.cn

[U88] JS：对象展开合并
来源：http://es.hahajie.cn

{ ...a, ...b }
来源：http://km.szxytkj.cn

[U89] JS：数组去重
来源：http://kw.shtwfgs.cn

[...new Set(arr)]
来源：http://pv.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ih.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://gg.9csxet.cn

[U91] JS：对象键值遍历
来源：http://nn.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ez.asd995.cn

[U92] JS：深拷贝
来源：http://ab.nszjky.cn

structuredClone(obj)
来源：http://kt.szxytkj.cn

[U93] JS：模板字符串
来源：http://nq.jctech888.com.cn

`共 ${n} 条`
来源：http://yj.jctech888.com.cn

[U94] JS：箭头函数
来源：http://bf.lnxyls.cn

const double = x => x * 2;
来源：http://ru.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://gi.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://zb.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://lk.shxzskj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://aa.huixiangedu.cn

[U97] JS：并发请求
来源：http://qn.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nq.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://pb.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://hv.bookmarksfly.cn

[U99] JS：事件监听
来源：http://pz.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://tu.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://ir.panjiajie.cn

document.querySelector(".item")
来源：http://qc.szsharing.cn

[U101] JS：classList 操作
来源：http://lp.bookmarksfly.cn

el.classList.toggle("active")
来源：http://zu.panjiajie.cn

[U102] JS：本地存储
来源：http://rt.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://th.gzmigu.cn

[U103] JS：定时器
来源：http://nk.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qj.chemitech.net.cn

[U104] JS：防抖
来源：http://se.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rv.bjjhwx.cn

[U105] JS：节流
来源：http://ds.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mp.yuexingan06.cn

[U106] JS：日期格式化
来源：http://iw.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ux.szxytkj.cn

[U107] JS：数字千分位
来源：http://rz.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ge.huanxung.cn

[U108] JS：随机整数
来源：http://fr.jctech888.com.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ln.hahajie.cn

[U109] JS：数组分组
来源：http://cl.panjiajie.cn

Object.groupBy(arr, x => x.type)
来源：http://fy.shxzskj.cn

[U110] JS：数组分块
来源：http://xy.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://av.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://eq.hnjuh.cn

new Map(Object.entries(obj))
来源：http://qv.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://wo.9csxet.cn

"7".padStart(3, "0")
来源：http://rs.shxzukj.cn

[U113] JS：正则替换全部
来源：http://zc.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://hb.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://wb.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vt.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://nc.lnxyls.cn

crypto.randomUUID()
来源：http://wl.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://eu.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://fh.bookmarksfly.cn

[U117] JS：单元测试
来源：http://iy.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://ge.gzmigu.cn

[U118] JS：开发服务器
来源：http://px.asd995.cn

npm i -D vite;  npx vite
来源：http://dh.hahajie.cn

[U119] JS：生产构建
来源：http://zj.asd995.cn

npx vite build
来源：http://tr.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://uu.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://kd.panjiajie.cn

================================================================================
来源：http://dj.hnjuh.cn

统计汇总
来源：http://mm.huixinmuqiang.cn

================================================================================
来源：http://rd.panjiajie.cn

按语言统计（条）：
来源：http://do.shxzukj.cn

Python ......... 252
来源：http://cn.colortex.cn

PHP ............ 252
来源：http://uv.9csxet.cn

JavaScript ..... 252
来源：http://dx.huixinmuqiang.cn

TypeScript ..... 212
来源：http://no.hahajie.cn

Java ........... 212
来源：http://lo.newstarts.cn

Go ............. 212
来源：http://up.nszjky.cn

Ruby ........... 212
来源：http://xo.wgjwhj.cn

C# ............. 212
来源：http://yb.hnjuh.cn

C .............. 30
来源：http://eo.newstarts.cn

C++ ............ 30
来源：http://gj.lnxyls.cn

SQL ............ 90
来源：http://ur.9csxet.cn

Bash ........... 80
来源：http://oj.huixiangedu.cn

Kotlin ......... 15
来源：http://mk.bookmarksfly.cn

Swift .......... 15
来源：http://fb.shxzskj.cn

Lua ............ 10
来源：http://ft.hahajie.cn

Perl ........... 10
来源：http://iw.huixiangedu.cn

Scala .......... 10
来源：http://bl.newstarts.cn

------------------------------------
来源：http://np.muxihuayi.cn

合计 ........... 2106 条
来源：http://xi.asd995.cn

按章节统计：
来源：http://so.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://tx.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qb.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://hj.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gd.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gz.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vw.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://oi.jctech888.com.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cj.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hg.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tr.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fo.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pz.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fw.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vl.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uz.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eo.szxytkj.cn

Q SQL 专题                              90
来源：http://du.521024.cn

R Bash 专题                             80
来源：http://hl.huixiangedu.cn

S C / C++ 专题                          60
来源：http://dc.haigaiapp.cn

T 其他语言补充                          60
来源：http://wo.bjjhwx.cn

U 高频实用片段                         120
来源：http://tk.szxytkj.cn

------------------------------------
来源：http://ia.shxzskj.cn

合计                                  2106 条
来源：http://zy.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://oi.gzmigu.cn

使用提醒
来源：http://je.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://mb.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uk.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pr.muxihuayi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ao.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rp.yuntaijiaju.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fv.huixiangedu.cn

—— 文件结束 ——
来源：http://ls.newstarts.cn

================================================================================
来源：http://ow.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://yv.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://lh.bookmarksfly.cn

================================================================================
来源：http://io.bjjhwx.cn

【收录内容】
来源：http://rm.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lv.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yj.wgjwhj.cn

SQL · Bash · C · C++
来源：http://cy.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cq.lnxyls.cn

【使用说明】
来源：http://rd.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hc.huixinmuqiang.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xw.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vg.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bn.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cc.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hh.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fq.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://bh.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bh.shtwfgs.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ud.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dz.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zz.szsharing.cn

【文件统计】
来源：http://tk.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kp.nicolike.cn

--------------------------------------------------------------------------------
来源：http://wt.bjjhwx.cn

目  录
来源：http://dp.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ul.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gk.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ax.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wa.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://be.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mb.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hj.yuntaijiaju.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tr.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://fh.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zk.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ab.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://jx.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fo.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nr.nszjky.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ig.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fy.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wk.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qd.jianghongdianzi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://st.hahajie.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://yw.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ez.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dz.muxihuayi.cn

================================================================================
来源：http://fi.lnxyls.cn

A. 基础语法与类型
来源：http://jk.shtwfgs.cn

================================================================================
来源：http://rl.huixinmuqiang.cn

[A01] Hello World
来源：http://xy.colortex.cn

Py:   print("Hello, World!")
来源：http://kh.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://mn.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://lh.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://jo.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://hx.shtwfgs.cn

Go:   fmt.Println("Hello, World!")
来源：http://io.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://qk.shxzskj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vv.gzmigu.cn

[A02] 变量声明与赋值
来源：http://um.jctech888.com.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://du.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ql.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fq.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rk.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://ma.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://yf.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://dc.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yx.yuntaijiaju.cn

[A03] 常量定义
来源：http://ls.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tk.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://bk.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://bx.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://qa.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://il.9csxet.cn

Go:   const PI = 3.14159
来源：http://up.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://vh.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://iq.shtwfgs.cn

[A04] 判断变量类型
来源：http://sm.gzmigu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://oy.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sq.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ou.haigaiapp.cn

TS:   typeof x; x instanceof Date
来源：http://sc.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fz.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://le.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://fh.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://hr.wgjwhj.cn

[A05] 整数除法与取模
来源：http://yw.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wq.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pf.szxytkj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mw.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://hw.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://gx.szxytkj.cn

Go:   7 / 2; 7 % 2
来源：http://ge.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://fb.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://dx.chemitech.net.cn

[A06] 字符串转数字
来源：http://kx.521024.cn

Py:   int("42"); float("3.14")
来源：http://vk.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://uk.9csxet.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ai.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://po.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rl.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bg.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://om.panjiajie.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xv.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://sz.bjjhwx.cn

Py:   str(42)
来源：http://bv.shtwfgs.cn

PHP:  (string) 42; strval(42)
来源：http://dh.szsharing.cn

JS:   String(42); (42).toString()
来源：http://wb.newstarts.cn

TS:   String(42)
来源：http://po.shtwfgs.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yc.521024.cn

Go:   strconv.Itoa(42)
来源：http://ta.newstarts.cn

Ruby: 42.to_s
来源：http://ve.521024.cn

C#:   42.ToString()
来源：http://rm.huixiangedu.cn

[A08] 取整与四舍五入
来源：http://vi.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bc.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gi.jianghongdianzi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ps.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qn.yuntaijiaju.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zw.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xx.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ng.muxihuayi.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://nq.521024.cn

[A09] 绝对值与最大最小值
来源：http://yp.colortex.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ym.szsharing.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://nm.shxzukj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xa.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://tt.jianghongdianzi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://xa.9csxet.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hl.panjiajie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://eq.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://tx.chemitech.net.cn

[A10] 生成随机数
来源：http://hr.shtwfgs.cn

Py:   import random; random.randint(1, 100)
来源：http://eu.szsharing.cn

PHP:  random_int(1, 100);
来源：http://wa.chemitech.net.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://au.shxzskj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ct.gzmigu.cn

Java: new Random().nextInt(100) + 1
来源：http://ms.huixiangedu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mo.gzmigu.cn

Ruby: rand(1..100)
来源：http://dl.szxytkj.cn

C#:   new Random().Next(1, 101)
来源：http://qq.hnjuh.cn

[A11] 条件表达式（三元）
来源：http://dl.shtwfgs.cn

Py:   "yes" if x > 0 else "no"
来源：http://we.hnjuh.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qj.colortex.cn

JS:   x > 0 ? "yes" : "no"
来源：http://yr.colortex.cn

TS:   x > 0 ? "yes" : "no"
来源：http://eg.gzmigu.cn

Java: x > 0 ? "yes" : "no"
来源：http://mi.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://os.shtwfgs.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fr.shtwfgs.cn

C#:   x > 0 ? "yes" : "no"
来源：http://mg.nicolike.cn

[A12] 字符串插值 / 格式化
来源：http://bv.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ko.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ov.asd995.cn

JS:   `Hello, ${name}!`
来源：http://hn.panjiajie.cn

TS:   `Hello, ${name}!`
来源：http://fw.hnjuh.cn

Java: "Hello, %s!".formatted(name)
来源：http://kk.chemitech.net.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fh.nicolike.cn

Ruby: "Hello, #{name}!"
来源：http://ml.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://lf.jianghongdianzi.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://wm.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://mj.huixiangedu.cn

PHP:  "第一行\n第二行"
来源：http://an.yuexingan06.cn

JS:   "第一行\n第二行"
来源：http://kb.jctech888.com.cn

TS:   "第一行\n第二行"
来源：http://wd.shxzskj.cn


<!-- 参考信息 -->