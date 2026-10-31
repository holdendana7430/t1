代发 wailian999

[U79] PHP：静态分析
来源：http://tc.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://ou.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://zu.wgjwhj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jx.521024.cn

[U81] JS：初始化项目
来源：http://je.szsharing.cn

npm init -y;  npm i express
来源：http://pk.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://re.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zx.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://al.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gh.szxytkj.cn

[U84] JS：CommonJS 写法
来源：http://tp.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uz.nszjky.cn

[U85] JS：可选链
来源：http://cw.muxihuayi.cn

a?.b?.c
来源：http://xu.shxzskj.cn

[U86] JS：空值合并
来源：http://pd.newstarts.cn

a ?? b
来源：http://hq.haigaiapp.cn

[U87] JS：解构默认值
来源：http://ex.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://lu.colortex.cn

[U88] JS：对象展开合并
来源：http://ik.huixinmuqiang.cn

{ ...a, ...b }
来源：http://js.yuexingan06.cn

[U89] JS：数组去重
来源：http://cw.huixiangedu.cn

[...new Set(arr)]
来源：http://de.hahajie.cn

[U90] JS：数字数组排序
来源：http://aj.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://cs.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://jl.szsharing.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vi.jctech888.com.cn

[U92] JS：深拷贝
来源：http://ts.hnjuh.cn

structuredClone(obj)
来源：http://fc.wgjwhj.cn

[U93] JS：模板字符串
来源：http://wt.bookmarksfly.cn

`共 ${n} 条`
来源：http://qn.wgjwhj.cn

[U94] JS：箭头函数
来源：http://is.colortex.cn

const double = x => x * 2;
来源：http://lp.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://oj.asd995.cn

new Promise((resolve, reject) => {})
来源：http://rn.huanxung.cn

[U96] JS：async/await 与异常
来源：http://ok.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wx.gzmigu.cn

[U97] JS：并发请求
来源：http://xb.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yc.jianghongdianzi.cn

[U98] JS：fetch 带 JSON
来源：http://or.szsharing.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zi.jctech888.com.cn

[U99] JS：事件监听
来源：http://mr.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://fe.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://we.yuntaijiaju.cn

document.querySelector(".item")
来源：http://ob.wgjwhj.cn

[U101] JS：classList 操作
来源：http://yu.wgjwhj.cn

el.classList.toggle("active")
来源：http://ae.chemitech.net.cn

[U102] JS：本地存储
来源：http://ve.newstarts.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ho.shtwfgs.cn

[U103] JS：定时器
来源：http://vc.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zp.muxihuayi.cn

[U104] JS：防抖
来源：http://mo.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iq.shxzukj.cn

[U105] JS：节流
来源：http://ou.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://my.yuexingan06.cn

[U106] JS：日期格式化
来源：http://zu.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sp.newstarts.cn

[U107] JS：数字千分位
来源：http://ob.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://he.hahajie.cn

[U108] JS：随机整数
来源：http://cd.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mu.yuexingan06.cn

[U109] JS：数组分组
来源：http://kb.shxzukj.cn

Object.groupBy(arr, x => x.type)
来源：http://an.panjiajie.cn

[U110] JS：数组分块
来源：http://or.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ep.hnjuh.cn

[U111] JS：对象转 Map
来源：http://an.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://ds.jctech888.com.cn

[U112] JS：字符串补位
来源：http://bk.huanxung.cn

"7".padStart(3, "0")
来源：http://pp.nszjky.cn

[U113] JS：正则替换全部
来源：http://zl.nszjky.cn

s.replaceAll("a", "b")
来源：http://lz.szsharing.cn

[U114] JS：JSON 深比较
来源：http://go.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oy.shxzukj.cn

[U115] JS：生成 UUID
来源：http://xw.huanxung.cn

crypto.randomUUID()
来源：http://cm.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://ng.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://oh.wgjwhj.cn

[U117] JS：单元测试
来源：http://jo.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://rm.nszjky.cn

[U118] JS：开发服务器
来源：http://dt.huanxung.cn

npm i -D vite;  npx vite
来源：http://lk.hnjuh.cn

[U119] JS：生产构建
来源：http://rh.shxzukj.cn

npx vite build
来源：http://sf.szsharing.cn

[U120] JS：读取环境变量（Vite）
来源：http://zf.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://rx.521024.cn

================================================================================
来源：http://ez.shxzukj.cn

统计汇总
来源：http://kl.szsharing.cn

================================================================================
来源：http://wz.colortex.cn

按语言统计（条）：
来源：http://ze.chemitech.net.cn

Python ......... 252
来源：http://rl.bjjhwx.cn

PHP ............ 252
来源：http://at.shxzskj.cn

JavaScript ..... 252
来源：http://ze.szxytkj.cn

TypeScript ..... 212
来源：http://ej.szxytkj.cn

Java ........... 212
来源：http://ar.gzmigu.cn

Go ............. 212
来源：http://bs.haigaiapp.cn

Ruby ........... 212
来源：http://mw.panjiajie.cn

C# ............. 212
来源：http://oa.bjjhwx.cn

C .............. 30
来源：http://mt.huixiangedu.cn

C++ ............ 30
来源：http://nz.jianghongdianzi.cn

SQL ............ 90
来源：http://bb.wgjwhj.cn

Bash ........... 80
来源：http://yw.colortex.cn

Kotlin ......... 15
来源：http://df.521024.cn

Swift .......... 15
来源：http://sj.haigaiapp.cn

Lua ............ 10
来源：http://vt.huixiangedu.cn

Perl ........... 10
来源：http://ix.gzmigu.cn

Scala .......... 10
来源：http://cr.shxzukj.cn

------------------------------------
来源：http://dz.jctech888.com.cn

合计 ........... 2106 条
来源：http://ma.shxzskj.cn

按章节统计：
来源：http://qb.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wa.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ur.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oc.9csxet.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pz.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xz.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jf.yuntaijiaju.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://gs.lnxyls.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hc.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dk.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://to.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iu.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lq.chemitech.net.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ds.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vr.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://db.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lr.szsharing.cn

Q SQL 专题                              90
来源：http://bj.9csxet.cn

R Bash 专题                             80
来源：http://fk.szxytkj.cn

S C / C++ 专题                          60
来源：http://xo.huanxung.cn

T 其他语言补充                          60
来源：http://lw.bjjhwx.cn

U 高频实用片段                         120
来源：http://cf.nszjky.cn

------------------------------------
来源：http://js.szxytkj.cn

合计                                  2106 条
来源：http://vp.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ou.panjiajie.cn

使用提醒
来源：http://ge.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://zd.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uz.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fd.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fr.hnjuh.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://si.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bg.panjiajie.cn

—— 文件结束 ——
来源：http://dx.szsharing.cn

================================================================================
来源：http://nn.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://ni.9csxet.cn

Common Programming Examples Cheat Book
来源：http://yc.nicolike.cn

================================================================================
来源：http://mf.huixinmuqiang.cn

【收录内容】
来源：http://hd.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xg.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oj.hnjuh.cn

SQL · Bash · C · C++
来源：http://zq.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ip.huixiangedu.cn

【使用说明】
来源：http://vo.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://df.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yq.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ql.hnjuh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xn.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wy.szxytkj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ke.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wc.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gc.huixiangedu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dw.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xv.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lt.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zp.shtwfgs.cn

【文件统计】
来源：http://wb.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bx.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://zw.asd995.cn

目  录
来源：http://cd.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://fk.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ll.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gb.muxihuayi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hb.nicolike.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ua.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wa.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sc.hahajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iu.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zl.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ia.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://rx.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sz.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pf.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://it.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bs.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mi.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lv.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ju.yuntaijiaju.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wc.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nj.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yk.asd995.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wc.yuntaijiaju.cn

================================================================================
来源：http://dl.hahajie.cn

A. 基础语法与类型
来源：http://wd.chemitech.net.cn

================================================================================
来源：http://nb.shxzskj.cn

[A01] Hello World
来源：http://ky.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://xg.521024.cn

PHP:  echo "Hello, World!";
来源：http://nx.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://fq.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ab.wgjwhj.cn

Java: System.out.println("Hello, World!");
来源：http://kt.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://rk.nszjky.cn

Ruby: puts "Hello, World!"
来源：http://wy.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://qa.panjiajie.cn

[A02] 变量声明与赋值
来源：http://gy.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zp.jctech888.com.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zu.chemitech.net.cn

JS:   let name = "Alex"; const age = 20;
来源：http://al.shtwfgs.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dw.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://ju.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://ri.shxzukj.cn

Ruby: name = "Alex"; age = 20
来源：http://ih.9csxet.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ws.521024.cn

[A03] 常量定义
来源：http://wq.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dc.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://kv.521024.cn

JS:   const PI = 3.14159;
来源：http://dt.szsharing.cn

TS:   const PI: number = 3.14159;
来源：http://pd.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://ls.shxzskj.cn

Go:   const PI = 3.14159
来源：http://is.nszjky.cn

Ruby: PI = 3.14159
来源：http://nb.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://hr.521024.cn

[A04] 判断变量类型
来源：http://xg.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wx.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dq.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vk.yuexingan06.cn

TS:   typeof x; x instanceof Date
来源：http://oy.hnjuh.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lr.hahajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://lu.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hs.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://qd.huanxung.cn

[A05] 整数除法与取模
来源：http://qo.hahajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bk.chemitech.net.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://if.yuexingan06.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ol.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://el.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://fd.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://vg.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://zk.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://fg.muxihuayi.cn

[A06] 字符串转数字
来源：http://dn.jctech888.com.cn

Py:   int("42"); float("3.14")
来源：http://jx.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://to.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://an.hahajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://if.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wd.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://kp.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sc.colortex.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qd.jctech888.com.cn

[A07] 数字转字符串
来源：http://vu.521024.cn

Py:   str(42)
来源：http://rg.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://lg.hahajie.cn

JS:   String(42); (42).toString()
来源：http://om.newstarts.cn

TS:   String(42)
来源：http://ry.szxytkj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zc.nszjky.cn

Go:   strconv.Itoa(42)
来源：http://fd.shtwfgs.cn

Ruby: 42.to_s
来源：http://mu.jctech888.com.cn

C#:   42.ToString()
来源：http://wz.gzmigu.cn

[A08] 取整与四舍五入
来源：http://lt.huixinmuqiang.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kl.shtwfgs.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://nn.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hu.jianghongdianzi.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ji.shxzskj.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://na.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://zq.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://qh.yuntaijiaju.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ni.szsharing.cn

[A09] 绝对值与最大最小值
来源：http://ei.bookmarksfly.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://se.szxytkj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ae.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ba.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hk.shxzukj.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cn.newstarts.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ly.huixinmuqiang.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ck.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://is.hnjuh.cn

[A10] 生成随机数
来源：http://zg.asd995.cn

Py:   import random; random.randint(1, 100)
来源：http://zb.hnjuh.cn

PHP:  random_int(1, 100);
来源：http://nj.yuntaijiaju.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://jt.haigaiapp.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://rq.bookmarksfly.cn

Java: new Random().nextInt(100) + 1
来源：http://vu.gzmigu.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qv.asd995.cn

Ruby: rand(1..100)
来源：http://dp.hahajie.cn

C#:   new Random().Next(1, 101)
来源：http://db.wgjwhj.cn

[A11] 条件表达式（三元）
来源：http://kj.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://dj.hahajie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://og.muxihuayi.cn

JS:   x > 0 ? "yes" : "no"
来源：http://sn.hnjuh.cn

TS:   x > 0 ? "yes" : "no"
来源：http://ez.szxytkj.cn

Java: x > 0 ? "yes" : "no"
来源：http://kr.jianghongdianzi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://oo.muxihuayi.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://xq.colortex.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ow.nszjky.cn

[A12] 字符串插值 / 格式化
来源：http://rt.wgjwhj.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://iv.szsharing.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://iq.huixinmuqiang.cn

JS:   `Hello, ${name}!`
来源：http://to.newstarts.cn

TS:   `Hello, ${name}!`
来源：http://xu.muxihuayi.cn

Java: "Hello, %s!".formatted(name)
来源：http://kw.szxytkj.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://rp.szsharing.cn

Ruby: "Hello, #{name}!"
来源：http://ga.yuntaijiaju.cn

C#:   $"Hello, {name}!"
来源：http://kf.nszjky.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://df.nszjky.cn


<!-- 参考信息 -->