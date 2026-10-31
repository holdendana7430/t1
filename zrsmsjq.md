代发 wailian999

[U75] PHP：依赖注入
来源：http://ze.chemitech.net.cn

composer require psr/container
来源：http://qd.wgjwhj.cn

[U76] PHP：简单路由
来源：http://et.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://na.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://jf.haigaiapp.cn

composer require twig/twig
来源：http://dc.shxzskj.cn

[U78] PHP：单元测试
来源：http://xv.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://he.huanxung.cn

[U79] PHP：静态分析
来源：http://xy.nicolike.cn

composer require --dev phpstan/phpstan
来源：http://fn.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://iq.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cc.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://dv.szxytkj.cn

npm init -y;  npm i express
来源：http://nl.nicolike.cn

[U82] JS：package.json 脚本
来源：http://ol.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ad.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://cx.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zx.521024.cn

[U84] JS：CommonJS 写法
来源：http://jb.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ad.jianghongdianzi.cn

[U85] JS：可选链
来源：http://ou.nicolike.cn

a?.b?.c
来源：http://iu.szxytkj.cn

[U86] JS：空值合并
来源：http://ch.bjjhwx.cn

a ?? b
来源：http://jo.shxzukj.cn

[U87] JS：解构默认值
来源：http://we.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://zi.lnxyls.cn

[U88] JS：对象展开合并
来源：http://hn.bookmarksfly.cn

{ ...a, ...b }
来源：http://vt.shtwfgs.cn

[U89] JS：数组去重
来源：http://cv.szsharing.cn

[...new Set(arr)]
来源：http://bw.szsharing.cn

[U90] JS：数字数组排序
来源：http://ni.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://kh.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://zd.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hm.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://tq.nszjky.cn

structuredClone(obj)
来源：http://sq.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://dn.shxzskj.cn

`共 ${n} 条`
来源：http://ak.shxzskj.cn

[U94] JS：箭头函数
来源：http://qr.asd995.cn

const double = x => x * 2;
来源：http://nc.gzmigu.cn

[U95] JS：Promise 包装
来源：http://yc.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://cb.9csxet.cn

[U96] JS：async/await 与异常
来源：http://sw.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bx.lnxyls.cn

[U97] JS：并发请求
来源：http://kl.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bw.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://wu.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nu.yuexingan06.cn

[U99] JS：事件监听
来源：http://rw.nicolike.cn

el.addEventListener("click", e => {})
来源：http://la.haigaiapp.cn

[U100] JS：DOM 查询
来源：http://ag.szxytkj.cn

document.querySelector(".item")
来源：http://af.nicolike.cn

[U101] JS：classList 操作
来源：http://qt.gzmigu.cn

el.classList.toggle("active")
来源：http://vf.muxihuayi.cn

[U102] JS：本地存储
来源：http://lx.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ea.lnxyls.cn

[U103] JS：定时器
来源：http://uz.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mw.yuntaijiaju.cn

[U104] JS：防抖
来源：http://ub.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rr.shtwfgs.cn

[U105] JS：节流
来源：http://xu.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uu.panjiajie.cn

[U106] JS：日期格式化
来源：http://xy.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lp.huanxung.cn

[U107] JS：数字千分位
来源：http://vh.yuexingan06.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ib.szsharing.cn

[U108] JS：随机整数
来源：http://ob.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gu.szsharing.cn

[U109] JS：数组分组
来源：http://zv.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://eo.bjjhwx.cn

[U110] JS：数组分块
来源：http://mt.muxihuayi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xn.huanxung.cn

[U111] JS：对象转 Map
来源：http://mc.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://ol.wgjwhj.cn

[U112] JS：字符串补位
来源：http://wn.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://ba.nicolike.cn

[U113] JS：正则替换全部
来源：http://qj.shxzukj.cn

s.replaceAll("a", "b")
来源：http://vs.colortex.cn

[U114] JS：JSON 深比较
来源：http://if.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pa.szxytkj.cn

[U115] JS：生成 UUID
来源：http://eg.wgjwhj.cn

crypto.randomUUID()
来源：http://kz.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://hs.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://uw.yuexingan06.cn

[U117] JS：单元测试
来源：http://ir.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://bc.lnxyls.cn

[U118] JS：开发服务器
来源：http://he.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://ep.shxzskj.cn

[U119] JS：生产构建
来源：http://mi.nszjky.cn

npx vite build
来源：http://rj.521024.cn

[U120] JS：读取环境变量（Vite）
来源：http://nw.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://ny.asd995.cn

================================================================================
来源：http://qb.newstarts.cn

统计汇总
来源：http://ig.asd995.cn

================================================================================
来源：http://ju.szsharing.cn

按语言统计（条）：
来源：http://bz.gzmigu.cn

Python ......... 252
来源：http://zj.wgjwhj.cn

PHP ............ 252
来源：http://np.jianghongdianzi.cn

JavaScript ..... 252
来源：http://mi.9csxet.cn

TypeScript ..... 212
来源：http://vf.hnjuh.cn

Java ........... 212
来源：http://eq.wgjwhj.cn

Go ............. 212
来源：http://by.gzmigu.cn

Ruby ........... 212
来源：http://sc.huixiangedu.cn

C# ............. 212
来源：http://bm.nszjky.cn

C .............. 30
来源：http://bk.muxihuayi.cn

C++ ............ 30
来源：http://yl.huanxung.cn

SQL ............ 90
来源：http://rn.haigaiapp.cn

Bash ........... 80
来源：http://fj.lnxyls.cn

Kotlin ......... 15
来源：http://nl.huixiangedu.cn

Swift .......... 15
来源：http://ek.colortex.cn

Lua ............ 10
来源：http://ib.chemitech.net.cn

Perl ........... 10
来源：http://ym.shxzskj.cn

Scala .......... 10
来源：http://ps.bookmarksfly.cn

------------------------------------
来源：http://pj.bjjhwx.cn

合计 ........... 2106 条
来源：http://yd.szsharing.cn

按章节统计：
来源：http://fg.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qk.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zj.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xw.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://om.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ti.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nf.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tt.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qe.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tn.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yr.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zx.lnxyls.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uv.nszjky.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ip.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ff.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gy.asd995.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fr.shtwfgs.cn

Q SQL 专题                              90
来源：http://vz.bjjhwx.cn

R Bash 专题                             80
来源：http://wi.szsharing.cn

S C / C++ 专题                          60
来源：http://dn.haigaiapp.cn

T 其他语言补充                          60
来源：http://pa.shxzukj.cn

U 高频实用片段                         120
来源：http://lb.bjjhwx.cn

------------------------------------
来源：http://hd.shxzukj.cn

合计                                  2106 条
来源：http://wd.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://fv.chemitech.net.cn

使用提醒
来源：http://lt.newstarts.cn

--------------------------------------------------------------------------------
来源：http://gu.shxzskj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fg.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://il.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://jm.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xz.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oz.shxzskj.cn

—— 文件结束 ——
来源：http://ul.haigaiapp.cn

================================================================================
来源：http://ym.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://wc.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://ml.gzmigu.cn

================================================================================
来源：http://ok.jianghongdianzi.cn

【收录内容】
来源：http://ju.muxihuayi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fn.9csxet.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yo.shtwfgs.cn

SQL · Bash · C · C++
来源：http://de.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qe.huixinmuqiang.cn

【使用说明】
来源：http://zl.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sj.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://hh.jctech888.com.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xh.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hm.panjiajie.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zo.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kv.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mm.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zb.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cd.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xp.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vw.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wg.muxihuayi.cn

【文件统计】
来源：http://jy.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qo.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://za.jctech888.com.cn

目  录
来源：http://ts.szsharing.cn

--------------------------------------------------------------------------------
来源：http://hn.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fw.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://bt.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://br.yuntaijiaju.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://gh.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bd.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ww.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iq.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://to.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zr.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://la.9csxet.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://dj.colortex.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nk.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://rr.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fh.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kj.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kd.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wm.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://lt.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eg.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ay.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lr.szxytkj.cn

================================================================================
来源：http://pb.lnxyls.cn

A. 基础语法与类型
来源：http://cb.huixiangedu.cn

================================================================================
来源：http://ll.shxzskj.cn

[A01] Hello World
来源：http://md.gzmigu.cn

Py:   print("Hello, World!")
来源：http://td.asd995.cn

PHP:  echo "Hello, World!";
来源：http://ak.asd995.cn

JS:   console.log("Hello, World!");
来源：http://wa.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ik.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://ua.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://tl.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://il.hnjuh.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xj.shxzukj.cn

[A02] 变量声明与赋值
来源：http://sg.shxzskj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ks.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://np.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ll.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ka.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://tf.yuntaijiaju.cn

Go:   name := "Alex"; age := 20
来源：http://zs.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://dh.panjiajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://kl.huixiangedu.cn

[A03] 常量定义
来源：http://kg.chemitech.net.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fw.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://rl.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://hp.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://ak.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://lc.shxzskj.cn

Go:   const PI = 3.14159
来源：http://gm.gzmigu.cn

Ruby: PI = 3.14159
来源：http://ad.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://pw.hnjuh.cn

[A04] 判断变量类型
来源：http://aa.521024.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://do.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ga.bjjhwx.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zj.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://re.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://jx.nszjky.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vf.chemitech.net.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://km.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://mr.haigaiapp.cn

[A05] 整数除法与取模
来源：http://cv.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qo.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ug.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wj.nszjky.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lv.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://gq.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://bd.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://us.szsharing.cn

C#:   7 / 2; 7 % 2
来源：http://en.muxihuayi.cn

[A06] 字符串转数字
来源：http://oz.bookmarksfly.cn

Py:   int("42"); float("3.14")
来源：http://my.shxzskj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kb.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ph.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ix.yuexingan06.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://za.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://yi.shtwfgs.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://dj.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ky.jianghongdianzi.cn

[A07] 数字转字符串
来源：http://zu.szxytkj.cn

Py:   str(42)
来源：http://hr.521024.cn

PHP:  (string) 42; strval(42)
来源：http://qn.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://wu.shxzskj.cn

TS:   String(42)
来源：http://qu.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vs.huixinmuqiang.cn

Go:   strconv.Itoa(42)
来源：http://gt.lnxyls.cn

Ruby: 42.to_s
来源：http://ug.yuntaijiaju.cn

C#:   42.ToString()
来源：http://nk.panjiajie.cn

[A08] 取整与四舍五入
来源：http://he.jianghongdianzi.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://xb.chemitech.net.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wn.huixinmuqiang.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://as.yuntaijiaju.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gs.colortex.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://uo.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tf.521024.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ln.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wq.lnxyls.cn

[A09] 绝对值与最大最小值
来源：http://gf.huanxung.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://jv.bookmarksfly.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pl.asd995.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://we.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://yl.colortex.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://br.hahajie.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wq.yuexingan06.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ce.shtwfgs.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://kd.shtwfgs.cn

[A10] 生成随机数
来源：http://kf.haigaiapp.cn

Py:   import random; random.randint(1, 100)
来源：http://cm.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://mx.newstarts.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://ct.shxzukj.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://nx.nicolike.cn

Java: new Random().nextInt(100) + 1
来源：http://qb.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mk.yuexingan06.cn

Ruby: rand(1..100)
来源：http://ap.lnxyls.cn

C#:   new Random().Next(1, 101)
来源：http://xt.shtwfgs.cn

[A11] 条件表达式（三元）
来源：http://pm.yuexingan06.cn

Py:   "yes" if x > 0 else "no"
来源：http://xi.521024.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://wk.szsharing.cn

JS:   x > 0 ? "yes" : "no"
来源：http://da.newstarts.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fx.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://lx.huanxung.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://yg.yuntaijiaju.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://pp.yuexingan06.cn

C#:   x > 0 ? "yes" : "no"
来源：http://lo.521024.cn

[A12] 字符串插值 / 格式化
来源：http://zw.hahajie.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://sj.huixiangedu.cn


<!-- 参考信息 -->