代发 wailian999

[U77] PHP：模板渲染
来源：http://kv.bookmarksfly.cn

composer require twig/twig
来源：http://nn.asd995.cn

[U78] PHP：单元测试
来源：http://pa.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://ty.jctech888.com.cn

[U79] PHP：静态分析
来源：http://mb.asd995.cn

composer require --dev phpstan/phpstan
来源：http://dk.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://qy.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://nb.yuexingan06.cn

[U81] JS：初始化项目
来源：http://bl.panjiajie.cn

npm init -y;  npm i express
来源：http://cx.shxzskj.cn

[U82] JS：package.json 脚本
来源：http://fo.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pj.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ue.huixiangedu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kd.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://qj.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zx.newstarts.cn

[U85] JS：可选链
来源：http://vd.newstarts.cn

a?.b?.c
来源：http://ag.nicolike.cn

[U86] JS：空值合并
来源：http://hj.newstarts.cn

a ?? b
来源：http://xp.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://aq.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://tk.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://ex.521024.cn

{ ...a, ...b }
来源：http://jf.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://qv.bookmarksfly.cn

[...new Set(arr)]
来源：http://cy.hahajie.cn

[U90] JS：数字数组排序
来源：http://ep.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://af.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://fx.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://or.shtwfgs.cn

[U92] JS：深拷贝
来源：http://sz.szsharing.cn

structuredClone(obj)
来源：http://af.wgjwhj.cn

[U93] JS：模板字符串
来源：http://rn.huixinmuqiang.cn

`共 ${n} 条`
来源：http://cb.haigaiapp.cn

[U94] JS：箭头函数
来源：http://hg.asd995.cn

const double = x => x * 2;
来源：http://gl.bjjhwx.cn

[U95] JS：Promise 包装
来源：http://lc.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://nv.nicolike.cn

[U96] JS：async/await 与异常
来源：http://ht.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ru.panjiajie.cn

[U97] JS：并发请求
来源：http://ov.huixinmuqiang.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rs.nszjky.cn

[U98] JS：fetch 带 JSON
来源：http://ln.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rn.wgjwhj.cn

[U99] JS：事件监听
来源：http://cy.9csxet.cn

el.addEventListener("click", e => {})
来源：http://pa.szsharing.cn

[U100] JS：DOM 查询
来源：http://uu.shxzukj.cn

document.querySelector(".item")
来源：http://gi.huanxung.cn

[U101] JS：classList 操作
来源：http://si.szxytkj.cn

el.classList.toggle("active")
来源：http://ap.shxzskj.cn

[U102] JS：本地存储
来源：http://et.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bj.newstarts.cn

[U103] JS：定时器
来源：http://bk.bookmarksfly.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://um.gzmigu.cn

[U104] JS：防抖
来源：http://bs.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rr.szxytkj.cn

[U105] JS：节流
来源：http://nt.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rd.shtwfgs.cn

[U106] JS：日期格式化
来源：http://oo.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vb.9csxet.cn

[U107] JS：数字千分位
来源：http://rf.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ix.nicolike.cn

[U108] JS：随机整数
来源：http://bu.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://or.521024.cn

[U109] JS：数组分组
来源：http://uu.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://bn.szsharing.cn

[U110] JS：数组分块
来源：http://ag.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zn.lnxyls.cn

[U111] JS：对象转 Map
来源：http://bu.panjiajie.cn

new Map(Object.entries(obj))
来源：http://xf.panjiajie.cn

[U112] JS：字符串补位
来源：http://ul.muxihuayi.cn

"7".padStart(3, "0")
来源：http://kt.huanxung.cn

[U113] JS：正则替换全部
来源：http://la.nicolike.cn

s.replaceAll("a", "b")
来源：http://xg.hahajie.cn

[U114] JS：JSON 深比较
来源：http://dp.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ot.shxzskj.cn

[U115] JS：生成 UUID
来源：http://ln.wgjwhj.cn

crypto.randomUUID()
来源：http://ai.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://kl.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://ad.szxytkj.cn

[U117] JS：单元测试
来源：http://ma.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://mq.wgjwhj.cn

[U118] JS：开发服务器
来源：http://ca.szsharing.cn

npm i -D vite;  npx vite
来源：http://yq.bookmarksfly.cn

[U119] JS：生产构建
来源：http://xy.haigaiapp.cn

npx vite build
来源：http://pk.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://gw.yuntaijiaju.cn

import.meta.env.VITE_API_URL
来源：http://pk.huixiangedu.cn

================================================================================
来源：http://gx.asd995.cn

统计汇总
来源：http://jx.chemitech.net.cn

================================================================================
来源：http://ct.nicolike.cn

按语言统计（条）：
来源：http://cu.gzmigu.cn

Python ......... 252
来源：http://yg.huixinmuqiang.cn

PHP ............ 252
来源：http://ny.shxzukj.cn

JavaScript ..... 252
来源：http://mj.shxzskj.cn

TypeScript ..... 212
来源：http://hd.jctech888.com.cn

Java ........... 212
来源：http://ic.wgjwhj.cn

Go ............. 212
来源：http://yw.panjiajie.cn

Ruby ........... 212
来源：http://fg.newstarts.cn

C# ............. 212
来源：http://hf.panjiajie.cn

C .............. 30
来源：http://xm.521024.cn

C++ ............ 30
来源：http://ew.szxytkj.cn

SQL ............ 90
来源：http://vj.newstarts.cn

Bash ........... 80
来源：http://xy.bookmarksfly.cn

Kotlin ......... 15
来源：http://jx.colortex.cn

Swift .......... 15
来源：http://ua.asd995.cn

Lua ............ 10
来源：http://ln.panjiajie.cn

Perl ........... 10
来源：http://py.521024.cn

Scala .......... 10
来源：http://kx.wgjwhj.cn

------------------------------------
来源：http://rk.lnxyls.cn

合计 ........... 2106 条
来源：http://qt.nicolike.cn

按章节统计：
来源：http://vz.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oc.nicolike.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ub.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cq.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mw.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lp.hnjuh.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nm.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kr.wgjwhj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://km.wgjwhj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ec.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fi.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zs.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zp.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fg.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xp.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nm.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jm.lnxyls.cn

Q SQL 专题                              90
来源：http://sp.nszjky.cn

R Bash 专题                             80
来源：http://wa.shtwfgs.cn

S C / C++ 专题                          60
来源：http://wu.haigaiapp.cn

T 其他语言补充                          60
来源：http://hq.shxzukj.cn

U 高频实用片段                         120
来源：http://vu.yuexingan06.cn

------------------------------------
来源：http://ha.huixiangedu.cn

合计                                  2106 条
来源：http://sz.521024.cn

--------------------------------------------------------------------------------
来源：http://tp.9csxet.cn

使用提醒
来源：http://mu.9csxet.cn

--------------------------------------------------------------------------------
来源：http://hk.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lp.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hw.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://oy.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ho.hahajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://av.gzmigu.cn

—— 文件结束 ——
来源：http://im.nszjky.cn

================================================================================
来源：http://qv.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://vk.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://uk.bjjhwx.cn

================================================================================
来源：http://tx.lnxyls.cn

【收录内容】
来源：http://uq.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rz.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uz.gzmigu.cn

SQL · Bash · C · C++
来源：http://ci.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qf.muxihuayi.cn

【使用说明】
来源：http://cq.shxzukj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ct.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ji.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kw.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eb.wgjwhj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://du.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://em.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lz.muxihuayi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yu.szxytkj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hi.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lb.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cq.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://of.9csxet.cn

【文件统计】
来源：http://yp.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hk.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://dq.nicolike.cn

目  录
来源：http://kj.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://qi.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pt.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fw.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gt.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wr.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ws.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xb.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wp.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ju.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bb.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wu.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wk.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qn.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dq.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xo.colortex.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xo.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bz.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ci.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zz.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ic.yuexingan06.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vz.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xe.asd995.cn

================================================================================
来源：http://ji.colortex.cn

A. 基础语法与类型
来源：http://av.bookmarksfly.cn

================================================================================
来源：http://wh.shtwfgs.cn

[A01] Hello World
来源：http://ec.gzmigu.cn

Py:   print("Hello, World!")
来源：http://ul.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://qw.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://em.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qa.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://lr.yuexingan06.cn

Go:   fmt.Println("Hello, World!")
来源：http://nv.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://ws.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sb.shxzskj.cn

[A02] 变量声明与赋值
来源：http://ma.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sz.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dj.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ge.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jl.shxzskj.cn

Java: String name = "Alex"; int age = 20;
来源：http://li.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://hd.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://jh.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sc.colortex.cn

[A03] 常量定义
来源：http://km.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vq.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://sm.huanxung.cn

JS:   const PI = 3.14159;
来源：http://xz.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://ak.asd995.cn

Java: static final double PI = 3.14159;
来源：http://hc.bookmarksfly.cn

Go:   const PI = 3.14159
来源：http://wz.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://cr.szxytkj.cn

C#:   const double PI = 3.14159;
来源：http://fg.gzmigu.cn

[A04] 判断变量类型
来源：http://od.jianghongdianzi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://go.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wv.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qq.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://cz.haigaiapp.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://bp.nicolike.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hy.shtwfgs.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vi.gzmigu.cn

C#:   x.GetType().Name; x is int
来源：http://aa.hnjuh.cn

[A05] 整数除法与取模
来源：http://cl.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ss.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jz.colortex.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cl.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mn.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://te.jianghongdianzi.cn

Go:   7 / 2; 7 % 2
来源：http://bd.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://zn.shtwfgs.cn

C#:   7 / 2; 7 % 2
来源：http://tj.hnjuh.cn

[A06] 字符串转数字
来源：http://xm.huixiangedu.cn

Py:   int("42"); float("3.14")
来源：http://hi.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vg.bjjhwx.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://lt.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://fg.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ar.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://re.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://km.huixiangedu.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jx.gzmigu.cn

[A07] 数字转字符串
来源：http://ag.521024.cn

Py:   str(42)
来源：http://hw.szxytkj.cn

PHP:  (string) 42; strval(42)
来源：http://pp.shxzskj.cn

JS:   String(42); (42).toString()
来源：http://ot.shxzukj.cn

TS:   String(42)
来源：http://yl.jctech888.com.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zy.521024.cn

Go:   strconv.Itoa(42)
来源：http://at.huanxung.cn

Ruby: 42.to_s
来源：http://xs.9csxet.cn

C#:   42.ToString()
来源：http://np.bookmarksfly.cn

[A08] 取整与四舍五入
来源：http://eg.jctech888.com.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://yw.szxytkj.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ar.colortex.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://uq.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://lt.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lp.shxzskj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ao.bookmarksfly.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://xl.521024.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vv.shxzukj.cn

[A09] 绝对值与最大最小值
来源：http://jq.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://lf.huixinmuqiang.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dn.haigaiapp.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://yp.jctech888.com.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://ba.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uz.yuntaijiaju.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ei.bookmarksfly.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://nt.chemitech.net.cn

[A10] 生成随机数
来源：http://nx.521024.cn

Py:   import random; random.randint(1, 100)
来源：http://ng.asd995.cn

PHP:  random_int(1, 100);
来源：http://ct.huixinmuqiang.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://og.panjiajie.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ck.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://vq.jianghongdianzi.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://sn.shtwfgs.cn

Ruby: rand(1..100)
来源：http://mk.bookmarksfly.cn

C#:   new Random().Next(1, 101)
来源：http://gj.shxzukj.cn

[A11] 条件表达式（三元）
来源：http://gn.521024.cn

Py:   "yes" if x > 0 else "no"
来源：http://cn.szxytkj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://nl.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://gv.shtwfgs.cn

TS:   x > 0 ? "yes" : "no"
来源：http://zj.wgjwhj.cn

Java: x > 0 ? "yes" : "no"
来源：http://jx.szxytkj.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://sf.huanxung.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://fm.bookmarksfly.cn

C#:   x > 0 ? "yes" : "no"
来源：http://nc.9csxet.cn

[A12] 字符串插值 / 格式化
来源：http://dx.panjiajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wy.muxihuayi.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://lm.gzmigu.cn

JS:   `Hello, ${name}!`
来源：http://fl.shxzskj.cn

TS:   `Hello, ${name}!`
来源：http://qb.shtwfgs.cn

Java: "Hello, %s!".formatted(name)
来源：http://au.jctech888.com.cn


<!-- 参考信息 -->