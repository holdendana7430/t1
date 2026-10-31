代发 wailian999

[U79] PHP：静态分析
来源：http://kx.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://wf.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://lz.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ta.huixiangedu.cn

[U81] JS：初始化项目
来源：http://ky.nicolike.cn

npm init -y;  npm i express
来源：http://mo.wgjwhj.cn

[U82] JS：package.json 脚本
来源：http://pi.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yn.chemitech.net.cn

[U83] JS：ES Module 导入导出
来源：http://mw.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ka.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://qp.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://aw.shxzskj.cn

[U85] JS：可选链
来源：http://qw.shtwfgs.cn

a?.b?.c
来源：http://qk.newstarts.cn

[U86] JS：空值合并
来源：http://bp.szxytkj.cn

a ?? b
来源：http://fw.muxihuayi.cn

[U87] JS：解构默认值
来源：http://ov.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://gy.shxzskj.cn

[U88] JS：对象展开合并
来源：http://pw.shtwfgs.cn

{ ...a, ...b }
来源：http://yx.huixiangedu.cn

[U89] JS：数组去重
来源：http://ez.panjiajie.cn

[...new Set(arr)]
来源：http://cm.szxytkj.cn

[U90] JS：数字数组排序
来源：http://cw.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://md.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://vv.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ky.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://kz.yuexingan06.cn

structuredClone(obj)
来源：http://fx.bookmarksfly.cn

[U93] JS：模板字符串
来源：http://sx.nicolike.cn

`共 ${n} 条`
来源：http://qc.nicolike.cn

[U94] JS：箭头函数
来源：http://uk.shxzskj.cn

const double = x => x * 2;
来源：http://dv.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://lp.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://bs.yuexingan06.cn

[U96] JS：async/await 与异常
来源：http://ql.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mf.shtwfgs.cn

[U97] JS：并发请求
来源：http://lf.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://vo.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://ub.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ba.huanxung.cn

[U99] JS：事件监听
来源：http://fp.colortex.cn

el.addEventListener("click", e => {})
来源：http://zv.521024.cn

[U100] JS：DOM 查询
来源：http://je.521024.cn

document.querySelector(".item")
来源：http://hx.asd995.cn

[U101] JS：classList 操作
来源：http://ey.wgjwhj.cn

el.classList.toggle("active")
来源：http://vl.muxihuayi.cn

[U102] JS：本地存储
来源：http://it.bjjhwx.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://aq.hahajie.cn

[U103] JS：定时器
来源：http://qg.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qa.nicolike.cn

[U104] JS：防抖
来源：http://qp.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fp.asd995.cn

[U105] JS：节流
来源：http://ji.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://op.huixiangedu.cn

[U106] JS：日期格式化
来源：http://pz.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rf.colortex.cn

[U107] JS：数字千分位
来源：http://nu.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://iy.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://cr.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://go.panjiajie.cn

[U109] JS：数组分组
来源：http://wp.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://ga.jctech888.com.cn

[U110] JS：数组分块
来源：http://jc.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bq.9csxet.cn

[U111] JS：对象转 Map
来源：http://rq.521024.cn

new Map(Object.entries(obj))
来源：http://pi.asd995.cn

[U112] JS：字符串补位
来源：http://km.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://gs.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://zo.lnxyls.cn

s.replaceAll("a", "b")
来源：http://cc.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://sf.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uh.newstarts.cn

[U115] JS：生成 UUID
来源：http://jc.bjjhwx.cn

crypto.randomUUID()
来源：http://fo.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://df.nszjky.cn

/** @param {string} name */ function f(name) {}
来源：http://rs.521024.cn

[U117] JS：单元测试
来源：http://cv.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://so.lnxyls.cn

[U118] JS：开发服务器
来源：http://hq.9csxet.cn

npm i -D vite;  npx vite
来源：http://uo.szxytkj.cn

[U119] JS：生产构建
来源：http://gk.521024.cn

npx vite build
来源：http://vb.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://xc.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://to.shxzukj.cn

================================================================================
来源：http://nn.shtwfgs.cn

统计汇总
来源：http://rc.szxytkj.cn

================================================================================
来源：http://zi.hnjuh.cn

按语言统计（条）：
来源：http://hi.gzmigu.cn

Python ......... 252
来源：http://rc.hnjuh.cn

PHP ............ 252
来源：http://zq.hnjuh.cn

JavaScript ..... 252
来源：http://yh.bjjhwx.cn

TypeScript ..... 212
来源：http://ya.panjiajie.cn

Java ........... 212
来源：http://yn.colortex.cn

Go ............. 212
来源：http://yx.nszjky.cn

Ruby ........... 212
来源：http://pd.gzmigu.cn

C# ............. 212
来源：http://nc.wgjwhj.cn

C .............. 30
来源：http://wx.huixinmuqiang.cn

C++ ............ 30
来源：http://kx.newstarts.cn

SQL ............ 90
来源：http://cx.jctech888.com.cn

Bash ........... 80
来源：http://kh.jianghongdianzi.cn

Kotlin ......... 15
来源：http://iu.hahajie.cn

Swift .......... 15
来源：http://cl.jianghongdianzi.cn

Lua ............ 10
来源：http://jg.jianghongdianzi.cn

Perl ........... 10
来源：http://xp.9csxet.cn

Scala .......... 10
来源：http://lf.jctech888.com.cn

------------------------------------
来源：http://uy.9csxet.cn

合计 ........... 2106 条
来源：http://ni.nicolike.cn

按章节统计：
来源：http://vu.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ck.hnjuh.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mh.newstarts.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://le.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sc.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://me.521024.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hc.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xi.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qt.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wc.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ah.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oa.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cw.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ov.shtwfgs.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vw.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jb.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qt.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://nm.hnjuh.cn

R Bash 专题                             80
来源：http://om.shtwfgs.cn

S C / C++ 专题                          60
来源：http://wb.huixiangedu.cn

T 其他语言补充                          60
来源：http://br.bookmarksfly.cn

U 高频实用片段                         120
来源：http://ml.szsharing.cn

------------------------------------
来源：http://xm.haigaiapp.cn

合计                                  2106 条
来源：http://en.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ex.hahajie.cn

使用提醒
来源：http://et.521024.cn

--------------------------------------------------------------------------------
来源：http://cm.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aj.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tf.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uv.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zd.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://er.yuexingan06.cn

—— 文件结束 ——
来源：http://qh.szxytkj.cn

================================================================================
来源：http://bg.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://wi.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://pd.yuexingan06.cn

================================================================================
来源：http://oe.wgjwhj.cn

【收录内容】
来源：http://pp.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ta.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iu.chemitech.net.cn

SQL · Bash · C · C++
来源：http://la.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uz.gzmigu.cn

【使用说明】
来源：http://oi.hnjuh.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ou.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uk.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jz.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ye.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pj.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tf.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tz.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ag.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fs.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yw.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ls.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mm.hahajie.cn

【文件统计】
来源：http://xb.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ph.hahajie.cn

--------------------------------------------------------------------------------
来源：http://uc.yuntaijiaju.cn

目  录
来源：http://qc.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://yo.chemitech.net.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fc.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dd.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cw.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vf.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xx.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qc.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://kn.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nv.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bo.huixiangedu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fg.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://js.huixinmuqiang.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://yb.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://az.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cr.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lm.shxzukj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cz.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ej.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://fs.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qn.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qz.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zo.asd995.cn

================================================================================
来源：http://fu.wgjwhj.cn

A. 基础语法与类型
来源：http://zd.yuntaijiaju.cn

================================================================================
来源：http://rz.szsharing.cn

[A01] Hello World
来源：http://sx.newstarts.cn

Py:   print("Hello, World!")
来源：http://rp.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://rl.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://bu.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://aq.panjiajie.cn

Java: System.out.println("Hello, World!");
来源：http://tl.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://me.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://ed.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vt.9csxet.cn

[A02] 变量声明与赋值
来源：http://qk.hnjuh.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hp.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vt.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://cu.muxihuayi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://by.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://mv.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://ki.bjjhwx.cn

Ruby: name = "Alex"; age = 20
来源：http://fr.colortex.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ko.haigaiapp.cn

[A03] 常量定义
来源：http://of.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qp.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://ve.yuntaijiaju.cn

JS:   const PI = 3.14159;
来源：http://jq.haigaiapp.cn

TS:   const PI: number = 3.14159;
来源：http://kj.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://ov.szxytkj.cn

Go:   const PI = 3.14159
来源：http://jt.hahajie.cn

Ruby: PI = 3.14159
来源：http://lj.lnxyls.cn

C#:   const double PI = 3.14159;
来源：http://jv.shtwfgs.cn

[A04] 判断变量类型
来源：http://fs.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dt.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://md.szxytkj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fm.newstarts.cn

TS:   typeof x; x instanceof Date
来源：http://yf.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lo.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mu.shxzukj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qy.shtwfgs.cn

C#:   x.GetType().Name; x is int
来源：http://eq.lnxyls.cn

[A05] 整数除法与取模
来源：http://pe.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://vr.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://iy.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sj.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ut.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://fq.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://lk.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://bx.nicolike.cn

C#:   7 / 2; 7 % 2
来源：http://ws.lnxyls.cn

[A06] 字符串转数字
来源：http://nm.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://oa.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dz.nicolike.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://br.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ss.jctech888.com.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jn.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://oj.shxzukj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pc.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uh.szxytkj.cn

[A07] 数字转字符串
来源：http://bo.wgjwhj.cn

Py:   str(42)
来源：http://kf.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://or.wgjwhj.cn

JS:   String(42); (42).toString()
来源：http://ut.asd995.cn

TS:   String(42)
来源：http://fd.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://va.bjjhwx.cn

Go:   strconv.Itoa(42)
来源：http://bo.bjjhwx.cn

Ruby: 42.to_s
来源：http://od.yuexingan06.cn

C#:   42.ToString()
来源：http://qt.jianghongdianzi.cn

[A08] 取整与四舍五入
来源：http://ui.huanxung.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qk.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://gd.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://il.huixinmuqiang.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yv.9csxet.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zw.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dt.panjiajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yx.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://jg.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://mk.hnjuh.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://rx.jctech888.com.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tk.huixiangedu.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://pf.newstarts.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bj.jctech888.com.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://du.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ie.huixiangedu.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hu.nicolike.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://bg.szxytkj.cn

[A10] 生成随机数
来源：http://ek.nszjky.cn

Py:   import random; random.randint(1, 100)
来源：http://pg.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://lj.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://de.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://zg.yuntaijiaju.cn

Java: new Random().nextInt(100) + 1
来源：http://uz.panjiajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mq.shxzukj.cn

Ruby: rand(1..100)
来源：http://dg.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://he.jctech888.com.cn

[A11] 条件表达式（三元）
来源：http://ix.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://wf.9csxet.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ah.jianghongdianzi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://tj.bjjhwx.cn

TS:   x > 0 ? "yes" : "no"
来源：http://dz.huixinmuqiang.cn

Java: x > 0 ? "yes" : "no"
来源：http://jj.szsharing.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://dd.shxzskj.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://iz.lnxyls.cn

C#:   x > 0 ? "yes" : "no"
来源：http://zt.gzmigu.cn

[A12] 字符串插值 / 格式化
来源：http://cu.shtwfgs.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bs.bookmarksfly.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://uq.shxzskj.cn

JS:   `Hello, ${name}!`
来源：http://gc.bookmarksfly.cn

TS:   `Hello, ${name}!`
来源：http://oa.huixiangedu.cn

Java: "Hello, %s!".formatted(name)
来源：http://yx.hahajie.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vi.shxzukj.cn

Ruby: "Hello, #{name}!"
来源：http://zn.haigaiapp.cn

C#:   $"Hello, {name}!"
来源：http://fo.lnxyls.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://ty.chemitech.net.cn


<!-- 参考信息 -->