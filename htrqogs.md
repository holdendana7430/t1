代发 wailian999

[U79] PHP：静态分析
来源：http://nb.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://we.huanxung.cn

[U80] PHP：代码规范修复
来源：http://fl.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nn.yuexingan06.cn

[U81] JS：初始化项目
来源：http://bv.panjiajie.cn

npm init -y;  npm i express
来源：http://dv.szxytkj.cn

[U82] JS：package.json 脚本
来源：http://gp.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ob.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://wq.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://pd.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://dt.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vm.chemitech.net.cn

[U85] JS：可选链
来源：http://ob.bookmarksfly.cn

a?.b?.c
来源：http://bt.hahajie.cn

[U86] JS：空值合并
来源：http://as.hnjuh.cn

a ?? b
来源：http://fy.521024.cn

[U87] JS：解构默认值
来源：http://lj.9csxet.cn

const { a = 1, b = 2 } = obj;
来源：http://jv.shxzskj.cn

[U88] JS：对象展开合并
来源：http://uq.huanxung.cn

{ ...a, ...b }
来源：http://zp.muxihuayi.cn

[U89] JS：数组去重
来源：http://gg.hnjuh.cn

[...new Set(arr)]
来源：http://sz.shxzskj.cn

[U90] JS：数字数组排序
来源：http://pw.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://qf.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://dg.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kp.huanxung.cn

[U92] JS：深拷贝
来源：http://ht.panjiajie.cn

structuredClone(obj)
来源：http://xr.huixiangedu.cn

[U93] JS：模板字符串
来源：http://kc.huixiangedu.cn

`共 ${n} 条`
来源：http://yi.bjjhwx.cn

[U94] JS：箭头函数
来源：http://ce.szxytkj.cn

const double = x => x * 2;
来源：http://cn.huanxung.cn

[U95] JS：Promise 包装
来源：http://fa.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://nz.nszjky.cn

[U96] JS：async/await 与异常
来源：http://zu.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mq.szxytkj.cn

[U97] JS：并发请求
来源：http://zf.521024.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://th.nicolike.cn

[U98] JS：fetch 带 JSON
来源：http://vf.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oz.521024.cn

[U99] JS：事件监听
来源：http://kj.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://by.shxzukj.cn

[U100] JS：DOM 查询
来源：http://mz.szsharing.cn

document.querySelector(".item")
来源：http://hr.huixiangedu.cn

[U101] JS：classList 操作
来源：http://qy.bookmarksfly.cn

el.classList.toggle("active")
来源：http://rj.panjiajie.cn

[U102] JS：本地存储
来源：http://tl.asd995.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ox.huanxung.cn

[U103] JS：定时器
来源：http://dl.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mi.yuntaijiaju.cn

[U104] JS：防抖
来源：http://cn.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eg.wgjwhj.cn

[U105] JS：节流
来源：http://vj.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hv.jctech888.com.cn

[U106] JS：日期格式化
来源：http://xg.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dk.shtwfgs.cn

[U107] JS：数字千分位
来源：http://xj.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ly.muxihuayi.cn

[U108] JS：随机整数
来源：http://cz.shxzukj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://um.wgjwhj.cn

[U109] JS：数组分组
来源：http://ub.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://od.hnjuh.cn

[U110] JS：数组分块
来源：http://vv.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ww.wgjwhj.cn

[U111] JS：对象转 Map
来源：http://nx.lnxyls.cn

new Map(Object.entries(obj))
来源：http://sj.hnjuh.cn

[U112] JS：字符串补位
来源：http://zw.shxzukj.cn

"7".padStart(3, "0")
来源：http://bi.nszjky.cn

[U113] JS：正则替换全部
来源：http://nl.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://ef.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://ot.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://tv.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://ti.szsharing.cn

crypto.randomUUID()
来源：http://cw.yuexingan06.cn

[U116] JS：类型检查（JSDoc）
来源：http://qm.shxzskj.cn

/** @param {string} name */ function f(name) {}
来源：http://ew.newstarts.cn

[U117] JS：单元测试
来源：http://zj.colortex.cn

npm i -D vitest;  npx vitest
来源：http://pb.521024.cn

[U118] JS：开发服务器
来源：http://tp.nicolike.cn

npm i -D vite;  npx vite
来源：http://an.shtwfgs.cn

[U119] JS：生产构建
来源：http://en.jianghongdianzi.cn

npx vite build
来源：http://xb.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://gs.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://tq.jianghongdianzi.cn

================================================================================
来源：http://ie.huixinmuqiang.cn

统计汇总
来源：http://xg.jctech888.com.cn

================================================================================
来源：http://yg.shtwfgs.cn

按语言统计（条）：
来源：http://zt.huixinmuqiang.cn

Python ......... 252
来源：http://cz.bookmarksfly.cn

PHP ............ 252
来源：http://tu.shxzukj.cn

JavaScript ..... 252
来源：http://ai.shxzukj.cn

TypeScript ..... 212
来源：http://hh.chemitech.net.cn

Java ........... 212
来源：http://fv.shxzskj.cn

Go ............. 212
来源：http://ps.haigaiapp.cn

Ruby ........... 212
来源：http://ct.hnjuh.cn

C# ............. 212
来源：http://tb.shxzskj.cn

C .............. 30
来源：http://ib.9csxet.cn

C++ ............ 30
来源：http://ks.jctech888.com.cn

SQL ............ 90
来源：http://zg.szxytkj.cn

Bash ........... 80
来源：http://nc.9csxet.cn

Kotlin ......... 15
来源：http://by.wgjwhj.cn

Swift .......... 15
来源：http://so.muxihuayi.cn

Lua ............ 10
来源：http://fp.bjjhwx.cn

Perl ........... 10
来源：http://nt.521024.cn

Scala .......... 10
来源：http://ex.521024.cn

------------------------------------
来源：http://ba.szxytkj.cn

合计 ........... 2106 条
来源：http://cz.jianghongdianzi.cn

按章节统计：
来源：http://qj.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ws.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vp.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://eb.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oq.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://tv.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rq.gzmigu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://fv.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://vz.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hi.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yo.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wg.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cz.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ge.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ht.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ni.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pa.9csxet.cn

Q SQL 专题                              90
来源：http://km.panjiajie.cn

R Bash 专题                             80
来源：http://mb.nszjky.cn

S C / C++ 专题                          60
来源：http://wu.szsharing.cn

T 其他语言补充                          60
来源：http://aw.nicolike.cn

U 高频实用片段                         120
来源：http://lw.9csxet.cn

------------------------------------
来源：http://uu.yuexingan06.cn

合计                                  2106 条
来源：http://wm.9csxet.cn

--------------------------------------------------------------------------------
来源：http://zr.521024.cn

使用提醒
来源：http://ph.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://qw.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gn.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mw.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ik.huixinmuqiang.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ek.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://yr.nszjky.cn

—— 文件结束 ——
来源：http://yo.muxihuayi.cn

================================================================================
来源：http://kc.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://he.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://qj.521024.cn

================================================================================
来源：http://hb.huixiangedu.cn

【收录内容】
来源：http://nq.yuntaijiaju.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sf.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gg.huanxung.cn

SQL · Bash · C · C++
来源：http://ac.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ul.hahajie.cn

【使用说明】
来源：http://ha.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rh.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xo.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mv.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kh.hahajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hg.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xv.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wb.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pg.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://uk.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gc.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ic.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cc.gzmigu.cn

【文件统计】
来源：http://qa.hnjuh.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zy.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://bd.bjjhwx.cn

目  录
来源：http://xz.9csxet.cn

--------------------------------------------------------------------------------
来源：http://xz.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ee.521024.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nn.hnjuh.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oz.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://uj.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oj.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kt.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uv.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fu.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zo.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fu.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jl.nicolike.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://uq.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://aq.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fz.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hh.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ln.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lb.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bg.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vy.newstarts.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sa.nszjky.cn

================================================================================
来源：http://zf.asd995.cn

A. 基础语法与类型
来源：http://uw.wgjwhj.cn

================================================================================
来源：http://qv.jianghongdianzi.cn

[A01] Hello World
来源：http://sh.shtwfgs.cn

Py:   print("Hello, World!")
来源：http://xe.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://ja.9csxet.cn

JS:   console.log("Hello, World!");
来源：http://wz.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hx.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://ey.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://eg.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://gq.bookmarksfly.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zg.gzmigu.cn

[A02] 变量声明与赋值
来源：http://pt.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hp.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qp.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://oh.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ce.jianghongdianzi.cn

Java: String name = "Alex"; int age = 20;
来源：http://zi.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://xo.haigaiapp.cn

Ruby: name = "Alex"; age = 20
来源：http://xn.szxytkj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pe.hahajie.cn

[A03] 常量定义
来源：http://im.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ei.colortex.cn

PHP:  const PI = 3.14159;
来源：http://hm.lnxyls.cn

JS:   const PI = 3.14159;
来源：http://zw.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://zc.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://qr.szxytkj.cn

Go:   const PI = 3.14159
来源：http://ua.nicolike.cn

Ruby: PI = 3.14159
来源：http://fd.colortex.cn

C#:   const double PI = 3.14159;
来源：http://il.shxzukj.cn

[A04] 判断变量类型
来源：http://gq.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jw.9csxet.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://om.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://st.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://ug.shxzukj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://af.wgjwhj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ed.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qi.hnjuh.cn

C#:   x.GetType().Name; x is int
来源：http://ek.hahajie.cn

[A05] 整数除法与取模
来源：http://in.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rm.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ed.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://vg.wgjwhj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kb.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://oy.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://rk.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://wp.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://ft.bookmarksfly.cn

[A06] 字符串转数字
来源：http://sj.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://yx.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cj.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://hk.bjjhwx.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uf.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xj.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hd.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://xw.haigaiapp.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vj.colortex.cn

[A07] 数字转字符串
来源：http://cu.nszjky.cn

Py:   str(42)
来源：http://hn.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://vq.9csxet.cn

JS:   String(42); (42).toString()
来源：http://if.shtwfgs.cn

TS:   String(42)
来源：http://kb.yuexingan06.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://wk.9csxet.cn

Go:   strconv.Itoa(42)
来源：http://th.colortex.cn

Ruby: 42.to_s
来源：http://ep.wgjwhj.cn

C#:   42.ToString()
来源：http://iz.nszjky.cn

[A08] 取整与四舍五入
来源：http://qp.shtwfgs.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ij.huanxung.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://uq.asd995.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ec.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jo.newstarts.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://pl.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://yo.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pg.nicolike.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://zh.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://dl.nszjky.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ku.yuntaijiaju.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mz.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fu.muxihuayi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eq.huixinmuqiang.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://us.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://uk.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://lm.hnjuh.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://em.shxzukj.cn

[A10] 生成随机数
来源：http://cn.huixinmuqiang.cn

Py:   import random; random.randint(1, 100)
来源：http://qb.huixiangedu.cn

PHP:  random_int(1, 100);
来源：http://bh.muxihuayi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://zr.newstarts.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://yz.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://bc.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mz.9csxet.cn

Ruby: rand(1..100)
来源：http://la.521024.cn

C#:   new Random().Next(1, 101)
来源：http://xm.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://dt.panjiajie.cn

Py:   "yes" if x > 0 else "no"
来源：http://ou.lnxyls.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://qq.shxzukj.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zy.gzmigu.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ma.chemitech.net.cn

Java: x > 0 ? "yes" : "no"
来源：http://ho.bookmarksfly.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://gq.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xs.muxihuayi.cn

C#:   x > 0 ? "yes" : "no"
来源：http://vj.yuntaijiaju.cn

[A12] 字符串插值 / 格式化
来源：http://su.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ep.nszjky.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://of.shxzukj.cn

JS:   `Hello, ${name}!`
来源：http://tr.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://fu.bjjhwx.cn

Java: "Hello, %s!".formatted(name)
来源：http://gv.bjjhwx.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://un.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://cb.jctech888.com.cn

C#:   $"Hello, {name}!"
来源：http://gi.yuntaijiaju.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://xe.shxzukj.cn


<!-- 参考信息 -->