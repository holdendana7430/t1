代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://jn.colortex.cn

parse_ini_file("config.ini", true)
来源：http://ip.asd995.cn

[U74] PHP：读取环境变量
来源：http://ud.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://dj.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://kq.nicolike.cn

composer require psr/container
来源：http://no.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://nk.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://dg.gzmigu.cn

[U77] PHP：模板渲染
来源：http://du.shxzukj.cn

composer require twig/twig
来源：http://bc.panjiajie.cn

[U78] PHP：单元测试
来源：http://if.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://rn.hnjuh.cn

[U79] PHP：静态分析
来源：http://ew.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://sd.shxzukj.cn

[U80] PHP：代码规范修复
来源：http://zs.gzmigu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qh.asd995.cn

[U81] JS：初始化项目
来源：http://tl.chemitech.net.cn

npm init -y;  npm i express
来源：http://tz.colortex.cn

[U82] JS：package.json 脚本
来源：http://ic.yuexingan06.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://td.shxzukj.cn

[U83] JS：ES Module 导入导出
来源：http://jh.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ww.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://qv.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lw.nszjky.cn

[U85] JS：可选链
来源：http://he.szxytkj.cn

a?.b?.c
来源：http://ev.newstarts.cn

[U86] JS：空值合并
来源：http://ho.yuexingan06.cn

a ?? b
来源：http://nn.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://bs.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://yb.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://jl.huixinmuqiang.cn

{ ...a, ...b }
来源：http://aw.bookmarksfly.cn

[U89] JS：数组去重
来源：http://dc.nszjky.cn

[...new Set(arr)]
来源：http://jb.lnxyls.cn

[U90] JS：数字数组排序
来源：http://co.asd995.cn

[...arr].sort((a, b) => a - b)
来源：http://lu.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://hz.nicolike.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gi.9csxet.cn

[U92] JS：深拷贝
来源：http://er.gzmigu.cn

structuredClone(obj)
来源：http://vr.jctech888.com.cn

[U93] JS：模板字符串
来源：http://rr.gzmigu.cn

`共 ${n} 条`
来源：http://sv.colortex.cn

[U94] JS：箭头函数
来源：http://hj.hnjuh.cn

const double = x => x * 2;
来源：http://co.panjiajie.cn

[U95] JS：Promise 包装
来源：http://cp.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://vx.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://el.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ti.shxzukj.cn

[U97] JS：并发请求
来源：http://hc.lnxyls.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pc.hnjuh.cn

[U98] JS：fetch 带 JSON
来源：http://lg.jianghongdianzi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ga.szxytkj.cn

[U99] JS：事件监听
来源：http://tl.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://zl.asd995.cn

[U100] JS：DOM 查询
来源：http://yu.lnxyls.cn

document.querySelector(".item")
来源：http://ng.jianghongdianzi.cn

[U101] JS：classList 操作
来源：http://ie.521024.cn

el.classList.toggle("active")
来源：http://sx.shxzukj.cn

[U102] JS：本地存储
来源：http://mj.huixinmuqiang.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://df.bjjhwx.cn

[U103] JS：定时器
来源：http://it.panjiajie.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tx.hahajie.cn

[U104] JS：防抖
来源：http://mp.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lu.huixinmuqiang.cn

[U105] JS：节流
来源：http://pv.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uk.newstarts.cn

[U106] JS：日期格式化
来源：http://zg.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jw.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://bh.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://en.szxytkj.cn

[U108] JS：随机整数
来源：http://wg.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://or.szxytkj.cn

[U109] JS：数组分组
来源：http://eo.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://bu.shtwfgs.cn

[U110] JS：数组分块
来源：http://jr.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rq.colortex.cn

[U111] JS：对象转 Map
来源：http://iq.asd995.cn

new Map(Object.entries(obj))
来源：http://wt.bjjhwx.cn

[U112] JS：字符串补位
来源：http://bv.nicolike.cn

"7".padStart(3, "0")
来源：http://ia.lnxyls.cn

[U113] JS：正则替换全部
来源：http://bl.nicolike.cn

s.replaceAll("a", "b")
来源：http://fw.521024.cn

[U114] JS：JSON 深比较
来源：http://if.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oo.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://pa.lnxyls.cn

crypto.randomUUID()
来源：http://gz.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://ht.bjjhwx.cn

/** @param {string} name */ function f(name) {}
来源：http://rb.yuexingan06.cn

[U117] JS：单元测试
来源：http://is.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://jr.panjiajie.cn

[U118] JS：开发服务器
来源：http://bs.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://rp.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://kr.panjiajie.cn

npx vite build
来源：http://sz.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://dx.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://bn.asd995.cn

================================================================================
来源：http://ch.huixiangedu.cn

统计汇总
来源：http://ia.asd995.cn

================================================================================
来源：http://gx.szxytkj.cn

按语言统计（条）：
来源：http://sb.jianghongdianzi.cn

Python ......... 252
来源：http://qz.521024.cn

PHP ............ 252
来源：http://ii.szxytkj.cn

JavaScript ..... 252
来源：http://sv.yuexingan06.cn

TypeScript ..... 212
来源：http://mn.hahajie.cn

Java ........... 212
来源：http://es.lnxyls.cn

Go ............. 212
来源：http://bd.shtwfgs.cn

Ruby ........... 212
来源：http://ac.jianghongdianzi.cn

C# ............. 212
来源：http://bq.muxihuayi.cn

C .............. 30
来源：http://ju.nszjky.cn

C++ ............ 30
来源：http://md.muxihuayi.cn

SQL ............ 90
来源：http://lv.lnxyls.cn

Bash ........... 80
来源：http://nn.nicolike.cn

Kotlin ......... 15
来源：http://mv.huixiangedu.cn

Swift .......... 15
来源：http://ur.muxihuayi.cn

Lua ............ 10
来源：http://dk.newstarts.cn

Perl ........... 10
来源：http://js.shtwfgs.cn

Scala .......... 10
来源：http://qr.haigaiapp.cn

------------------------------------
来源：http://pb.wgjwhj.cn

合计 ........... 2106 条
来源：http://ko.huanxung.cn

按章节统计：
来源：http://tv.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bu.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sm.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jc.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rb.bjjhwx.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bi.yuntaijiaju.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gl.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ej.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wn.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tg.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://am.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pi.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fs.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nf.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bm.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://me.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ef.chemitech.net.cn

Q SQL 专题                              90
来源：http://ue.huixinmuqiang.cn

R Bash 专题                             80
来源：http://bt.panjiajie.cn

S C / C++ 专题                          60
来源：http://wv.jctech888.com.cn

T 其他语言补充                          60
来源：http://sj.gzmigu.cn

U 高频实用片段                         120
来源：http://fn.shxzskj.cn

------------------------------------
来源：http://sa.szxytkj.cn

合计                                  2106 条
来源：http://ev.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://se.yuntaijiaju.cn

使用提醒
来源：http://nl.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://pc.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mx.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wr.jianghongdianzi.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ct.muxihuayi.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zk.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bn.shtwfgs.cn

—— 文件结束 ——
来源：http://ah.shxzskj.cn

================================================================================
来源：http://gz.shtwfgs.cn

程序语言常见例子速查手册（2024 版）
来源：http://ft.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://vs.yuntaijiaju.cn

================================================================================
来源：http://ld.szxytkj.cn

【收录内容】
来源：http://ae.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jq.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bx.hahajie.cn

SQL · Bash · C · C++
来源：http://xv.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vi.huixiangedu.cn

【使用说明】
来源：http://ud.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bz.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://me.hahajie.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ay.shxzukj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fc.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xc.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://or.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wn.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mp.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tp.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dm.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kz.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ez.bookmarksfly.cn

【文件统计】
来源：http://pj.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://hn.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://vr.shtwfgs.cn

目  录
来源：http://tw.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://wq.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uz.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sr.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hf.wgjwhj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ym.huanxung.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://or.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ik.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://oj.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://oo.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ot.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ka.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mv.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://md.jctech888.com.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ij.gzmigu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gf.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://kk.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tq.jctech888.com.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dn.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xy.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fo.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://dt.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ua.9csxet.cn

================================================================================
来源：http://po.newstarts.cn

A. 基础语法与类型
来源：http://ek.huixiangedu.cn

================================================================================
来源：http://br.lnxyls.cn

[A01] Hello World
来源：http://ke.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ux.asd995.cn

PHP:  echo "Hello, World!";
来源：http://lk.asd995.cn

JS:   console.log("Hello, World!");
来源：http://bm.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rm.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://xt.huanxung.cn

Go:   fmt.Println("Hello, World!")
来源：http://du.chemitech.net.cn

Ruby: puts "Hello, World!"
来源：http://hh.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ey.bjjhwx.cn

[A02] 变量声明与赋值
来源：http://ye.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qm.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://mq.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ce.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://pg.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://ro.gzmigu.cn

Go:   name := "Alex"; age := 20
来源：http://mj.asd995.cn

Ruby: name = "Alex"; age = 20
来源：http://yt.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pt.haigaiapp.cn

[A03] 常量定义
来源：http://ck.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xt.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://om.bjjhwx.cn

JS:   const PI = 3.14159;
来源：http://us.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://bo.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://nj.panjiajie.cn

Go:   const PI = 3.14159
来源：http://yv.asd995.cn

Ruby: PI = 3.14159
来源：http://bz.asd995.cn

C#:   const double PI = 3.14159;
来源：http://db.huixiangedu.cn

[A04] 判断变量类型
来源：http://sa.panjiajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://tu.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cx.colortex.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tv.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://ik.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dd.newstarts.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ea.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xt.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://sg.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://li.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://gx.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yo.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ss.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pr.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://rw.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://nx.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://no.haigaiapp.cn

C#:   7 / 2; 7 % 2
来源：http://wz.huixinmuqiang.cn

[A06] 字符串转数字
来源：http://ro.asd995.cn

Py:   int("42"); float("3.14")
来源：http://ra.szxytkj.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zn.huixinmuqiang.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://qt.shxzskj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ml.shtwfgs.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ri.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qa.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://ld.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://kd.panjiajie.cn

[A07] 数字转字符串
来源：http://tm.yuexingan06.cn

Py:   str(42)
来源：http://yb.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://ej.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://ms.szsharing.cn

TS:   String(42)
来源：http://zu.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qq.huanxung.cn

Go:   strconv.Itoa(42)
来源：http://hz.521024.cn

Ruby: 42.to_s
来源：http://ms.huanxung.cn

C#:   42.ToString()
来源：http://yk.chemitech.net.cn

[A08] 取整与四舍五入
来源：http://ly.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://fs.bookmarksfly.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mc.lnxyls.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gb.bjjhwx.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zw.hahajie.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://od.muxihuayi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wv.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://cz.bookmarksfly.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bb.jianghongdianzi.cn

[A09] 绝对值与最大最小值
来源：http://qk.jianghongdianzi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://kh.huanxung.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mn.yuexingan06.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://nv.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://dk.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://il.jianghongdianzi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://dw.nicolike.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wg.wgjwhj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://lc.hahajie.cn

[A10] 生成随机数
来源：http://ce.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ls.wgjwhj.cn

PHP:  random_int(1, 100);
来源：http://nh.szsharing.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://py.jctech888.com.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hq.colortex.cn

Java: new Random().nextInt(100) + 1
来源：http://jt.newstarts.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://ro.chemitech.net.cn

Ruby: rand(1..100)
来源：http://am.shxzukj.cn

C#:   new Random().Next(1, 101)
来源：http://hv.521024.cn

[A11] 条件表达式（三元）
来源：http://gf.lnxyls.cn

Py:   "yes" if x > 0 else "no"
来源：http://wj.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://uj.huixiangedu.cn

JS:   x > 0 ? "yes" : "no"
来源：http://ff.asd995.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qz.panjiajie.cn

Java: x > 0 ? "yes" : "no"
来源：http://vn.hnjuh.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://eg.muxihuayi.cn


<!-- 参考信息 -->