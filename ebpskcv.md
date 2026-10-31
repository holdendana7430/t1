代发 wailian999

[U81] JS：初始化项目
来源：http://uy.lnxyls.cn

npm init -y;  npm i express
来源：http://cp.nszjky.cn

[U82] JS：package.json 脚本
来源：http://qh.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ke.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://gm.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lz.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://vi.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wg.huixiangedu.cn

[U85] JS：可选链
来源：http://mj.hnjuh.cn

a?.b?.c
来源：http://jt.shtwfgs.cn

[U86] JS：空值合并
来源：http://jz.bjjhwx.cn

a ?? b
来源：http://ar.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://bt.asd995.cn

const { a = 1, b = 2 } = obj;
来源：http://sk.521024.cn

[U88] JS：对象展开合并
来源：http://yj.shxzukj.cn

{ ...a, ...b }
来源：http://ul.bjjhwx.cn

[U89] JS：数组去重
来源：http://pa.bookmarksfly.cn

[...new Set(arr)]
来源：http://mc.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://za.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://hm.newstarts.cn

[U91] JS：对象键值遍历
来源：http://zh.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rq.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://tv.hahajie.cn

structuredClone(obj)
来源：http://bw.bjjhwx.cn

[U93] JS：模板字符串
来源：http://sk.bjjhwx.cn

`共 ${n} 条`
来源：http://md.asd995.cn

[U94] JS：箭头函数
来源：http://fn.chemitech.net.cn

const double = x => x * 2;
来源：http://oa.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://ve.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://rz.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://do.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ya.huanxung.cn

[U97] JS：并发请求
来源：http://fi.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qd.panjiajie.cn

[U98] JS：fetch 带 JSON
来源：http://kr.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://kl.gzmigu.cn

[U99] JS：事件监听
来源：http://gz.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://qh.9csxet.cn

[U100] JS：DOM 查询
来源：http://fw.wgjwhj.cn

document.querySelector(".item")
来源：http://dj.9csxet.cn

[U101] JS：classList 操作
来源：http://by.521024.cn

el.classList.toggle("active")
来源：http://wa.hnjuh.cn

[U102] JS：本地存储
来源：http://mn.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://iu.huixinmuqiang.cn

[U103] JS：定时器
来源：http://dx.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wl.chemitech.net.cn

[U104] JS：防抖
来源：http://mb.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cl.jianghongdianzi.cn

[U105] JS：节流
来源：http://qv.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fm.nszjky.cn

[U106] JS：日期格式化
来源：http://ox.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vw.muxihuayi.cn

[U107] JS：数字千分位
来源：http://qg.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lc.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://vp.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ec.newstarts.cn

[U109] JS：数组分组
来源：http://dh.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://gb.hahajie.cn

[U110] JS：数组分块
来源：http://ag.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cz.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://rg.colortex.cn

new Map(Object.entries(obj))
来源：http://ms.shxzskj.cn

[U112] JS：字符串补位
来源：http://ef.colortex.cn

"7".padStart(3, "0")
来源：http://bt.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://xi.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://gc.521024.cn

[U114] JS：JSON 深比较
来源：http://tw.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wf.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://sc.nszjky.cn

crypto.randomUUID()
来源：http://kj.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://rl.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://zt.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://yj.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://of.haigaiapp.cn

[U118] JS：开发服务器
来源：http://nu.521024.cn

npm i -D vite;  npx vite
来源：http://qd.hnjuh.cn

[U119] JS：生产构建
来源：http://jf.colortex.cn

npx vite build
来源：http://np.shtwfgs.cn

[U120] JS：读取环境变量（Vite）
来源：http://hd.asd995.cn

import.meta.env.VITE_API_URL
来源：http://mz.shxzukj.cn

================================================================================
来源：http://jo.gzmigu.cn

统计汇总
来源：http://mr.huixinmuqiang.cn

================================================================================
来源：http://ah.nicolike.cn

按语言统计（条）：
来源：http://sz.muxihuayi.cn

Python ......... 252
来源：http://wm.gzmigu.cn

PHP ............ 252
来源：http://kr.hnjuh.cn

JavaScript ..... 252
来源：http://ei.shxzukj.cn

TypeScript ..... 212
来源：http://iv.colortex.cn

Java ........... 212
来源：http://sz.yuntaijiaju.cn

Go ............. 212
来源：http://ev.521024.cn

Ruby ........... 212
来源：http://jo.nszjky.cn

C# ............. 212
来源：http://qt.shtwfgs.cn

C .............. 30
来源：http://ve.huixiangedu.cn

C++ ............ 30
来源：http://mh.yuexingan06.cn

SQL ............ 90
来源：http://vy.hnjuh.cn

Bash ........... 80
来源：http://cy.shxzskj.cn

Kotlin ......... 15
来源：http://kb.shtwfgs.cn

Swift .......... 15
来源：http://iw.haigaiapp.cn

Lua ............ 10
来源：http://wa.asd995.cn

Perl ........... 10
来源：http://wq.huanxung.cn

Scala .......... 10
来源：http://ma.panjiajie.cn

------------------------------------
来源：http://qi.nicolike.cn

合计 ........... 2106 条
来源：http://vv.nszjky.cn

按章节统计：
来源：http://rt.asd995.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vq.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xc.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sz.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://li.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uz.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tq.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bg.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cz.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mj.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nc.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iv.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://eo.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://qn.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ka.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mn.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hp.haigaiapp.cn

Q SQL 专题                              90
来源：http://gx.asd995.cn

R Bash 专题                             80
来源：http://qn.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://xf.nszjky.cn

T 其他语言补充                          60
来源：http://fo.shtwfgs.cn

U 高频实用片段                         120
来源：http://hi.lnxyls.cn

------------------------------------
来源：http://bk.muxihuayi.cn

合计                                  2106 条
来源：http://aa.asd995.cn

--------------------------------------------------------------------------------
来源：http://rw.hnjuh.cn

使用提醒
来源：http://hr.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://jn.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ja.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gb.lnxyls.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ln.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://qq.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ez.huixinmuqiang.cn

—— 文件结束 ——
来源：http://fo.shxzukj.cn

================================================================================
来源：http://cm.bjjhwx.cn

程序语言常见例子速查手册（2024 版）
来源：http://ir.nszjky.cn

Common Programming Examples Cheat Book
来源：http://tl.shxzukj.cn

================================================================================
来源：http://ki.shxzskj.cn

【收录内容】
来源：http://uk.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://of.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pm.shtwfgs.cn

SQL · Bash · C · C++
来源：http://mo.huixinmuqiang.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kt.huixiangedu.cn

【使用说明】
来源：http://op.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gn.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uj.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sb.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://an.yuexingan06.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qh.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pb.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hn.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wt.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pw.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ik.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gz.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ce.szxytkj.cn

【文件统计】
来源：http://ru.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cy.nicolike.cn

--------------------------------------------------------------------------------
来源：http://iv.jianghongdianzi.cn

目  录
来源：http://tu.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://to.yuntaijiaju.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nd.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bz.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vd.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://le.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ja.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wq.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://yc.9csxet.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yj.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sv.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yr.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://hv.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lf.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://xe.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xp.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qd.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rw.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nl.newstarts.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ja.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vl.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://lc.gzmigu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kf.szxytkj.cn

================================================================================
来源：http://oy.szsharing.cn

A. 基础语法与类型
来源：http://td.yuexingan06.cn

================================================================================
来源：http://bg.lnxyls.cn

[A01] Hello World
来源：http://kc.asd995.cn

Py:   print("Hello, World!")
来源：http://mg.nszjky.cn

PHP:  echo "Hello, World!";
来源：http://ad.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://bz.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zs.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://gp.shxzukj.cn

Go:   fmt.Println("Hello, World!")
来源：http://kl.gzmigu.cn

Ruby: puts "Hello, World!"
来源：http://hf.nszjky.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xu.panjiajie.cn

[A02] 变量声明与赋值
来源：http://oj.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yc.wgjwhj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xh.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ey.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ch.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://jv.colortex.cn

Go:   name := "Alex"; age := 20
来源：http://qo.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://yd.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://wz.nicolike.cn

[A03] 常量定义
来源：http://np.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ym.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://li.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://pj.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://sv.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://mi.colortex.cn

Go:   const PI = 3.14159
来源：http://ap.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://du.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://ae.nicolike.cn

[A04] 判断变量类型
来源：http://ke.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yb.szsharing.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pw.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qg.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://wd.lnxyls.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qz.jctech888.com.cn

Go:   reflect.TypeOf(x).Name()
来源：http://tt.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hm.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://og.jianghongdianzi.cn

[A05] 整数除法与取模
来源：http://ps.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ke.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://il.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ar.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tv.panjiajie.cn

Java: 7 / 2; 7 % 2
来源：http://by.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://vy.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://yg.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://jm.muxihuayi.cn

[A06] 字符串转数字
来源：http://ja.huixinmuqiang.cn

Py:   int("42"); float("3.14")
来源：http://ym.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jn.shxzskj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bk.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uk.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ka.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cg.hahajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fx.wgjwhj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ni.asd995.cn

[A07] 数字转字符串
来源：http://rt.lnxyls.cn

Py:   str(42)
来源：http://or.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://fh.huanxung.cn

JS:   String(42); (42).toString()
来源：http://gg.shxzukj.cn

TS:   String(42)
来源：http://jw.muxihuayi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vb.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://la.newstarts.cn

Ruby: 42.to_s
来源：http://uq.hnjuh.cn

C#:   42.ToString()
来源：http://lw.asd995.cn

[A08] 取整与四舍五入
来源：http://tz.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://zt.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://am.muxihuayi.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://et.9csxet.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://xe.bjjhwx.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://yy.newstarts.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ve.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://tr.szxytkj.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tp.muxihuayi.cn

[A09] 绝对值与最大最小值
来源：http://kc.shxzskj.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://vb.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://bd.bjjhwx.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://of.nicolike.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wb.haigaiapp.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://tc.shtwfgs.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sr.shxzskj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://cm.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ig.huanxung.cn

[A10] 生成随机数
来源：http://jr.huanxung.cn

Py:   import random; random.randint(1, 100)
来源：http://zx.yuexingan06.cn

PHP:  random_int(1, 100);
来源：http://fo.gzmigu.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://oj.yuntaijiaju.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://eh.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://au.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kf.wgjwhj.cn

Ruby: rand(1..100)
来源：http://yc.haigaiapp.cn

C#:   new Random().Next(1, 101)
来源：http://ho.newstarts.cn

[A11] 条件表达式（三元）
来源：http://yc.gzmigu.cn

Py:   "yes" if x > 0 else "no"
来源：http://of.colortex.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://xv.bookmarksfly.cn

JS:   x > 0 ? "yes" : "no"
来源：http://zx.nszjky.cn

TS:   x > 0 ? "yes" : "no"
来源：http://lh.asd995.cn

Java: x > 0 ? "yes" : "no"
来源：http://eb.asd995.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://nl.9csxet.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://hq.nicolike.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lr.huixinmuqiang.cn

[A12] 字符串插值 / 格式化
来源：http://kn.huixiangedu.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://og.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lf.hnjuh.cn

JS:   `Hello, ${name}!`
来源：http://tp.nszjky.cn

TS:   `Hello, ${name}!`
来源：http://ro.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://sx.huanxung.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hm.huixinmuqiang.cn

Ruby: "Hello, #{name}!"
来源：http://uc.yuexingan06.cn

C#:   $"Hello, {name}!"
来源：http://yy.huanxung.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://bn.jianghongdianzi.cn

Py:   "第一行\n第二行"
来源：http://tc.szsharing.cn

PHP:  "第一行\n第二行"
来源：http://dj.haigaiapp.cn

JS:   "第一行\n第二行"
来源：http://tq.huanxung.cn

TS:   "第一行\n第二行"
来源：http://iw.asd995.cn


<!-- 参考信息 -->