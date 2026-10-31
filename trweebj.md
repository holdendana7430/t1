代发 wailian999

[U81] JS：初始化项目
来源：http://bp.jctech888.com.cn

npm init -y;  npm i express
来源：http://ws.colortex.cn

[U82] JS：package.json 脚本
来源：http://vt.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dj.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://oc.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kk.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://xl.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://an.shxzukj.cn

[U85] JS：可选链
来源：http://jh.huanxung.cn

a?.b?.c
来源：http://zf.hnjuh.cn

[U86] JS：空值合并
来源：http://nk.huixinmuqiang.cn

a ?? b
来源：http://ne.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://gu.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://hj.szsharing.cn

[U88] JS：对象展开合并
来源：http://ot.521024.cn

{ ...a, ...b }
来源：http://lv.bookmarksfly.cn

[U89] JS：数组去重
来源：http://ak.shtwfgs.cn

[...new Set(arr)]
来源：http://qz.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://vt.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://cf.nicolike.cn

[U91] JS：对象键值遍历
来源：http://gi.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://as.szsharing.cn

[U92] JS：深拷贝
来源：http://te.yuexingan06.cn

structuredClone(obj)
来源：http://ct.huixiangedu.cn

[U93] JS：模板字符串
来源：http://dj.colortex.cn

`共 ${n} 条`
来源：http://gm.gzmigu.cn

[U94] JS：箭头函数
来源：http://br.yuexingan06.cn

const double = x => x * 2;
来源：http://cq.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ll.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://lx.szxytkj.cn

[U96] JS：async/await 与异常
来源：http://xg.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://re.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://km.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rq.wgjwhj.cn

[U98] JS：fetch 带 JSON
来源：http://lu.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zw.asd995.cn

[U99] JS：事件监听
来源：http://pw.gzmigu.cn

el.addEventListener("click", e => {})
来源：http://dz.newstarts.cn

[U100] JS：DOM 查询
来源：http://ef.jianghongdianzi.cn

document.querySelector(".item")
来源：http://xl.wgjwhj.cn

[U101] JS：classList 操作
来源：http://rz.hnjuh.cn

el.classList.toggle("active")
来源：http://pv.chemitech.net.cn

[U102] JS：本地存储
来源：http://ez.lnxyls.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hl.shtwfgs.cn

[U103] JS：定时器
来源：http://ni.szxytkj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xz.shtwfgs.cn

[U104] JS：防抖
来源：http://po.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gf.huanxung.cn

[U105] JS：节流
来源：http://vi.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wc.yuexingan06.cn

[U106] JS：日期格式化
来源：http://gi.szsharing.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xg.yuexingan06.cn

[U107] JS：数字千分位
来源：http://go.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kt.bookmarksfly.cn

[U108] JS：随机整数
来源：http://xx.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gm.huanxung.cn

[U109] JS：数组分组
来源：http://ev.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://jn.nszjky.cn

[U110] JS：数组分块
来源：http://ok.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://aj.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://ug.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://iu.panjiajie.cn

[U112] JS：字符串补位
来源：http://aj.gzmigu.cn

"7".padStart(3, "0")
来源：http://tm.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://rs.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://wb.521024.cn

[U114] JS：JSON 深比较
来源：http://uz.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lt.szsharing.cn

[U115] JS：生成 UUID
来源：http://ax.shxzukj.cn

crypto.randomUUID()
来源：http://hd.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://yn.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://lr.panjiajie.cn

[U117] JS：单元测试
来源：http://eq.colortex.cn

npm i -D vitest;  npx vitest
来源：http://gh.hahajie.cn

[U118] JS：开发服务器
来源：http://bu.shxzskj.cn

npm i -D vite;  npx vite
来源：http://vz.panjiajie.cn

[U119] JS：生产构建
来源：http://wv.huanxung.cn

npx vite build
来源：http://lf.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ei.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://cp.gzmigu.cn

================================================================================
来源：http://sa.521024.cn

统计汇总
来源：http://ad.huixiangedu.cn

================================================================================
来源：http://fw.wgjwhj.cn

按语言统计（条）：
来源：http://lv.bookmarksfly.cn

Python ......... 252
来源：http://ko.colortex.cn

PHP ............ 252
来源：http://ew.jianghongdianzi.cn

JavaScript ..... 252
来源：http://wp.panjiajie.cn

TypeScript ..... 212
来源：http://bt.shtwfgs.cn

Java ........... 212
来源：http://ic.wgjwhj.cn

Go ............. 212
来源：http://fh.jianghongdianzi.cn

Ruby ........... 212
来源：http://sd.panjiajie.cn

C# ............. 212
来源：http://sq.shxzskj.cn

C .............. 30
来源：http://ou.huixiangedu.cn

C++ ............ 30
来源：http://fq.yuexingan06.cn

SQL ............ 90
来源：http://ri.yuexingan06.cn

Bash ........... 80
来源：http://mk.nicolike.cn

Kotlin ......... 15
来源：http://mu.nicolike.cn

Swift .......... 15
来源：http://du.huanxung.cn

Lua ............ 10
来源：http://xb.gzmigu.cn

Perl ........... 10
来源：http://wo.shxzskj.cn

Scala .......... 10
来源：http://au.asd995.cn

------------------------------------
来源：http://yr.hnjuh.cn

合计 ........... 2106 条
来源：http://xg.szsharing.cn

按章节统计：
来源：http://wf.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cv.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nz.bjjhwx.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oo.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pj.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gu.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yj.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cg.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wt.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uj.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://cy.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dj.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qp.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://iy.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://za.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pf.bjjhwx.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rc.bookmarksfly.cn

Q SQL 专题                              90
来源：http://qo.jctech888.com.cn

R Bash 专题                             80
来源：http://kp.bjjhwx.cn

S C / C++ 专题                          60
来源：http://dy.shxzskj.cn

T 其他语言补充                          60
来源：http://uz.szxytkj.cn

U 高频实用片段                         120
来源：http://yc.bjjhwx.cn

------------------------------------
来源：http://wt.nicolike.cn

合计                                  2106 条
来源：http://gm.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://bo.huixiangedu.cn

使用提醒
来源：http://wv.nszjky.cn

--------------------------------------------------------------------------------
来源：http://kz.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lb.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dh.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jj.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lb.521024.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ub.jianghongdianzi.cn

—— 文件结束 ——
来源：http://kx.gzmigu.cn

================================================================================
来源：http://xa.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://ga.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://ji.521024.cn

================================================================================
来源：http://ht.yuntaijiaju.cn

【收录内容】
来源：http://se.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hv.szsharing.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ag.huixiangedu.cn

SQL · Bash · C · C++
来源：http://xj.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://sl.9csxet.cn

【使用说明】
来源：http://qy.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fj.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ol.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hl.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ip.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ks.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wa.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ei.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ri.shxzskj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dx.muxihuayi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://or.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yg.gzmigu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hn.asd995.cn

【文件统计】
来源：http://lh.muxihuayi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hj.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://os.yuntaijiaju.cn

目  录
来源：http://cp.newstarts.cn

--------------------------------------------------------------------------------
来源：http://le.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zh.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pz.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cq.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pq.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mg.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wm.shxzskj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nm.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rx.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qr.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jz.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nc.yuntaijiaju.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cv.huixiangedu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fx.chemitech.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vn.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fb.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://yv.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fo.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vn.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gl.gzmigu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rk.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yb.hahajie.cn

================================================================================
来源：http://jx.panjiajie.cn

A. 基础语法与类型
来源：http://xk.colortex.cn

================================================================================
来源：http://vz.521024.cn

[A01] Hello World
来源：http://td.szsharing.cn

Py:   print("Hello, World!")
来源：http://dw.jctech888.com.cn

PHP:  echo "Hello, World!";
来源：http://ge.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://ol.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zb.521024.cn

Java: System.out.println("Hello, World!");
来源：http://ir.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://rr.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://iu.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://hl.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://iz.muxihuayi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yj.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bo.szsharing.cn

JS:   let name = "Alex"; const age = 20;
来源：http://xj.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://in.shxzukj.cn

Java: String name = "Alex"; int age = 20;
来源：http://he.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://ok.colortex.cn

Ruby: name = "Alex"; age = 20
来源：http://zf.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gl.chemitech.net.cn

[A03] 常量定义
来源：http://qt.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://cs.huixiangedu.cn

PHP:  const PI = 3.14159;
来源：http://hw.9csxet.cn

JS:   const PI = 3.14159;
来源：http://ve.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://ok.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://cl.asd995.cn

Go:   const PI = 3.14159
来源：http://eu.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://ww.521024.cn

C#:   const double PI = 3.14159;
来源：http://vy.newstarts.cn

[A04] 判断变量类型
来源：http://oq.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bu.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yh.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hu.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://xv.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ny.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pw.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uq.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://ek.521024.cn

[A05] 整数除法与取模
来源：http://mi.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lh.bjjhwx.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gh.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jm.yuexingan06.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wo.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://jh.521024.cn

Go:   7 / 2; 7 % 2
来源：http://ar.chemitech.net.cn

Ruby: 7 / 2; 7 % 2
来源：http://ar.lnxyls.cn

C#:   7 / 2; 7 % 2
来源：http://yb.shxzskj.cn

[A06] 字符串转数字
来源：http://vr.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://oy.nszjky.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sz.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jq.huixinmuqiang.cn

TS:   parseInt("42", 10); Number("42")
来源：http://nf.521024.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mx.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rn.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://aw.gzmigu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rx.gzmigu.cn

[A07] 数字转字符串
来源：http://fo.wgjwhj.cn

Py:   str(42)
来源：http://fr.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://us.shtwfgs.cn

JS:   String(42); (42).toString()
来源：http://gu.colortex.cn

TS:   String(42)
来源：http://je.huanxung.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://yb.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://lz.521024.cn

Ruby: 42.to_s
来源：http://zz.shxzskj.cn

C#:   42.ToString()
来源：http://tt.hnjuh.cn

[A08] 取整与四舍五入
来源：http://uq.szsharing.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ux.hnjuh.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://zx.hahajie.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://oj.hahajie.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://pd.nszjky.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hj.9csxet.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vt.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wd.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cu.szxytkj.cn

[A09] 绝对值与最大最小值
来源：http://ri.szsharing.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wm.yuexingan06.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xc.jctech888.com.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://rb.wgjwhj.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://pl.yuntaijiaju.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ct.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wo.haigaiapp.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xw.gzmigu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jk.newstarts.cn

[A10] 生成随机数
来源：http://tz.jianghongdianzi.cn

Py:   import random; random.randint(1, 100)
来源：http://bc.shtwfgs.cn

PHP:  random_int(1, 100);
来源：http://uf.hahajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wa.muxihuayi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://qw.nszjky.cn

Java: new Random().nextInt(100) + 1
来源：http://uq.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ip.bjjhwx.cn

Ruby: rand(1..100)
来源：http://ot.shxzskj.cn

C#:   new Random().Next(1, 101)
来源：http://rt.yuntaijiaju.cn

[A11] 条件表达式（三元）
来源：http://jz.jianghongdianzi.cn

Py:   "yes" if x > 0 else "no"
来源：http://lp.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://bv.asd995.cn

JS:   x > 0 ? "yes" : "no"
来源：http://dj.bookmarksfly.cn

TS:   x > 0 ? "yes" : "no"
来源：http://am.huixiangedu.cn

Java: x > 0 ? "yes" : "no"
来源：http://lc.nszjky.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ba.haigaiapp.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://uk.shxzskj.cn

C#:   x > 0 ? "yes" : "no"
来源：http://bb.hnjuh.cn

[A12] 字符串插值 / 格式化
来源：http://fw.szsharing.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ya.szxytkj.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ic.yuexingan06.cn

JS:   `Hello, ${name}!`
来源：http://tf.yuexingan06.cn

TS:   `Hello, ${name}!`
来源：http://mp.yuntaijiaju.cn

Java: "Hello, %s!".formatted(name)
来源：http://dd.colortex.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://uf.newstarts.cn

Ruby: "Hello, #{name}!"
来源：http://jk.hnjuh.cn

C#:   $"Hello, {name}!"
来源：http://ks.jctech888.com.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ka.gzmigu.cn

Py:   "第一行\n第二行"
来源：http://aq.huixinmuqiang.cn

PHP:  "第一行\n第二行"
来源：http://ed.huixinmuqiang.cn

JS:   "第一行\n第二行"
来源：http://ow.chemitech.net.cn

TS:   "第一行\n第二行"
来源：http://la.yuexingan06.cn


<!-- 参考信息 -->