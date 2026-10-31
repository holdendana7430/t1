代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://xx.asd995.cn

parse_ini_file("config.ini", true)
来源：http://dz.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://gl.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ea.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://dd.jctech888.com.cn

composer require psr/container
来源：http://ig.shxzskj.cn

[U76] PHP：简单路由
来源：http://mi.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://up.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://iq.asd995.cn

composer require twig/twig
来源：http://ag.muxihuayi.cn

[U78] PHP：单元测试
来源：http://ut.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://aq.521024.cn

[U79] PHP：静态分析
来源：http://fw.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://bf.hahajie.cn

[U80] PHP：代码规范修复
来源：http://me.hnjuh.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ag.szsharing.cn

[U81] JS：初始化项目
来源：http://kt.jianghongdianzi.cn

npm init -y;  npm i express
来源：http://rr.huanxung.cn

[U82] JS：package.json 脚本
来源：http://kv.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vd.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://sf.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ht.shxzukj.cn

[U84] JS：CommonJS 写法
来源：http://tp.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://je.colortex.cn

[U85] JS：可选链
来源：http://rf.panjiajie.cn

a?.b?.c
来源：http://np.gzmigu.cn

[U86] JS：空值合并
来源：http://ky.bookmarksfly.cn

a ?? b
来源：http://fr.gzmigu.cn

[U87] JS：解构默认值
来源：http://mt.chemitech.net.cn

const { a = 1, b = 2 } = obj;
来源：http://gx.chemitech.net.cn

[U88] JS：对象展开合并
来源：http://vi.9csxet.cn

{ ...a, ...b }
来源：http://xb.huanxung.cn

[U89] JS：数组去重
来源：http://sd.szxytkj.cn

[...new Set(arr)]
来源：http://ba.shtwfgs.cn

[U90] JS：数字数组排序
来源：http://gu.shxzukj.cn

[...arr].sort((a, b) => a - b)
来源：http://yh.nicolike.cn

[U91] JS：对象键值遍历
来源：http://ie.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bw.szxytkj.cn

[U92] JS：深拷贝
来源：http://xj.huixinmuqiang.cn

structuredClone(obj)
来源：http://pm.shtwfgs.cn

[U93] JS：模板字符串
来源：http://mt.hahajie.cn

`共 ${n} 条`
来源：http://lw.hahajie.cn

[U94] JS：箭头函数
来源：http://gs.panjiajie.cn

const double = x => x * 2;
来源：http://xh.9csxet.cn

[U95] JS：Promise 包装
来源：http://fl.colortex.cn

new Promise((resolve, reject) => {})
来源：http://xq.nszjky.cn

[U96] JS：async/await 与异常
来源：http://oh.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qv.huixinmuqiang.cn

[U97] JS：并发请求
来源：http://rr.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ns.shtwfgs.cn

[U98] JS：fetch 带 JSON
来源：http://pw.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yb.szxytkj.cn

[U99] JS：事件监听
来源：http://pv.bookmarksfly.cn

el.addEventListener("click", e => {})
来源：http://cl.hahajie.cn

[U100] JS：DOM 查询
来源：http://ao.hahajie.cn

document.querySelector(".item")
来源：http://ac.9csxet.cn

[U101] JS：classList 操作
来源：http://gp.chemitech.net.cn

el.classList.toggle("active")
来源：http://xv.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://gy.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://za.gzmigu.cn

[U103] JS：定时器
来源：http://kh.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zv.szxytkj.cn

[U104] JS：防抖
来源：http://qz.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vz.shtwfgs.cn

[U105] JS：节流
来源：http://yf.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://az.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://ds.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oc.haigaiapp.cn

[U107] JS：数字千分位
来源：http://ht.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ci.wgjwhj.cn

[U108] JS：随机整数
来源：http://dg.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uq.newstarts.cn

[U109] JS：数组分组
来源：http://kc.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://jb.panjiajie.cn

[U110] JS：数组分块
来源：http://ts.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://nm.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://go.panjiajie.cn

new Map(Object.entries(obj))
来源：http://xu.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://ek.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://cz.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://mu.asd995.cn

s.replaceAll("a", "b")
来源：http://lq.bjjhwx.cn

[U114] JS：JSON 深比较
来源：http://yl.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wl.gzmigu.cn

[U115] JS：生成 UUID
来源：http://jo.colortex.cn

crypto.randomUUID()
来源：http://xu.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://qi.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://vw.muxihuayi.cn

[U117] JS：单元测试
来源：http://fc.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://am.yuexingan06.cn

[U118] JS：开发服务器
来源：http://if.gzmigu.cn

npm i -D vite;  npx vite
来源：http://wn.lnxyls.cn

[U119] JS：生产构建
来源：http://qj.chemitech.net.cn

npx vite build
来源：http://lk.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ur.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://qo.hnjuh.cn

================================================================================
来源：http://uc.lnxyls.cn

统计汇总
来源：http://tx.muxihuayi.cn

================================================================================
来源：http://im.yuexingan06.cn

按语言统计（条）：
来源：http://or.hahajie.cn

Python ......... 252
来源：http://sm.panjiajie.cn

PHP ............ 252
来源：http://if.huixinmuqiang.cn

JavaScript ..... 252
来源：http://le.huanxung.cn

TypeScript ..... 212
来源：http://ta.hahajie.cn

Java ........... 212
来源：http://wa.shtwfgs.cn

Go ............. 212
来源：http://wj.shxzukj.cn

Ruby ........... 212
来源：http://wl.colortex.cn

C# ............. 212
来源：http://xu.panjiajie.cn

C .............. 30
来源：http://ya.9csxet.cn

C++ ............ 30
来源：http://pv.muxihuayi.cn

SQL ............ 90
来源：http://du.yuntaijiaju.cn

Bash ........... 80
来源：http://xy.huixinmuqiang.cn

Kotlin ......... 15
来源：http://ss.wgjwhj.cn

Swift .......... 15
来源：http://lc.colortex.cn

Lua ............ 10
来源：http://ip.nicolike.cn

Perl ........... 10
来源：http://iw.nszjky.cn

Scala .......... 10
来源：http://fc.asd995.cn

------------------------------------
来源：http://sf.yuexingan06.cn

合计 ........... 2106 条
来源：http://qe.chemitech.net.cn

按章节统计：
来源：http://sp.lnxyls.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zn.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ff.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bp.hnjuh.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ae.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wb.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fk.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://eq.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ya.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zp.hnjuh.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wm.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://zi.chemitech.net.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ns.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yl.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ps.huanxung.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ve.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pw.asd995.cn

Q SQL 专题                              90
来源：http://vq.panjiajie.cn

R Bash 专题                             80
来源：http://vr.yuexingan06.cn

S C / C++ 专题                          60
来源：http://fz.bookmarksfly.cn

T 其他语言补充                          60
来源：http://cu.shtwfgs.cn

U 高频实用片段                         120
来源：http://rq.panjiajie.cn

------------------------------------
来源：http://kv.huixiangedu.cn

合计                                  2106 条
来源：http://au.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://le.newstarts.cn

使用提醒
来源：http://nn.newstarts.cn

--------------------------------------------------------------------------------
来源：http://gi.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xj.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lm.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zk.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ji.haigaiapp.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kq.chemitech.net.cn

—— 文件结束 ——
来源：http://jl.muxihuayi.cn

================================================================================
来源：http://qo.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://zj.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://la.nicolike.cn

================================================================================
来源：http://xt.jianghongdianzi.cn

【收录内容】
来源：http://og.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ao.nicolike.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://py.521024.cn

SQL · Bash · C · C++
来源：http://aw.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fn.huixiangedu.cn

【使用说明】
来源：http://wb.yuntaijiaju.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://np.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xw.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://tj.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zd.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wo.bjjhwx.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tk.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yw.lnxyls.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gi.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ql.gzmigu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vr.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bd.nszjky.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yg.yuntaijiaju.cn

【文件统计】
来源：http://gm.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lq.szsharing.cn

--------------------------------------------------------------------------------
来源：http://tb.wgjwhj.cn

目  录
来源：http://rn.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://kd.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bn.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://sc.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://uq.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://kn.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ii.521024.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://po.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ce.shxzukj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xs.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jv.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ga.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://az.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://zn.jianghongdianzi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://iy.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cy.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://sd.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cp.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bz.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pp.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://va.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vl.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://oh.nicolike.cn

================================================================================
来源：http://lo.wgjwhj.cn

A. 基础语法与类型
来源：http://ty.lnxyls.cn

================================================================================
来源：http://fj.haigaiapp.cn

[A01] Hello World
来源：http://bk.szsharing.cn

Py:   print("Hello, World!")
来源：http://tb.bookmarksfly.cn

PHP:  echo "Hello, World!";
来源：http://cd.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://ei.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uc.nicolike.cn

Java: System.out.println("Hello, World!");
来源：http://sw.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://sf.shxzukj.cn

Ruby: puts "Hello, World!"
来源：http://sp.521024.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vm.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://lj.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://po.lnxyls.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://vy.szxytkj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://um.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fq.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://tl.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://kn.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://mr.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://pl.huixinmuqiang.cn

[A03] 常量定义
来源：http://uy.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://rp.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://xi.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://ge.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://pw.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://mh.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://nt.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://mw.colortex.cn

C#:   const double PI = 3.14159;
来源：http://jz.9csxet.cn

[A04] 判断变量类型
来源：http://tn.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://rs.szxytkj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ce.jianghongdianzi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wn.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://vz.9csxet.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yz.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ph.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://it.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://ik.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://sp.nszjky.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hx.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nu.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pi.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pp.szxytkj.cn

Java: 7 / 2; 7 % 2
来源：http://qo.szsharing.cn

Go:   7 / 2; 7 % 2
来源：http://mk.haigaiapp.cn

Ruby: 7 / 2; 7 % 2
来源：http://ku.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://yl.9csxet.cn

[A06] 字符串转数字
来源：http://dl.chemitech.net.cn

Py:   int("42"); float("3.14")
来源：http://sv.colortex.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ip.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vd.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lf.asd995.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ih.szxytkj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ma.bookmarksfly.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://os.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://do.yuntaijiaju.cn

[A07] 数字转字符串
来源：http://zn.shxzukj.cn

Py:   str(42)
来源：http://sk.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://cj.shxzukj.cn

JS:   String(42); (42).toString()
来源：http://cr.huanxung.cn

TS:   String(42)
来源：http://pt.yuntaijiaju.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://zj.huixiangedu.cn

Go:   strconv.Itoa(42)
来源：http://ln.chemitech.net.cn

Ruby: 42.to_s
来源：http://tw.huixinmuqiang.cn

C#:   42.ToString()
来源：http://nj.newstarts.cn

[A08] 取整与四舍五入
来源：http://ml.wgjwhj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ng.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wm.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vj.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ka.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iq.hnjuh.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qq.asd995.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ee.haigaiapp.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://si.jctech888.com.cn

[A09] 绝对值与最大最小值
来源：http://rg.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://bt.lnxyls.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ng.szxytkj.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tq.bjjhwx.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://bi.bjjhwx.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://cr.muxihuayi.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://xd.yuntaijiaju.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://kx.lnxyls.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://jx.haigaiapp.cn

[A10] 生成随机数
来源：http://mp.yuntaijiaju.cn

Py:   import random; random.randint(1, 100)
来源：http://np.asd995.cn

PHP:  random_int(1, 100);
来源：http://xi.jianghongdianzi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wj.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://jy.lnxyls.cn

Java: new Random().nextInt(100) + 1
来源：http://id.shtwfgs.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wx.bjjhwx.cn

Ruby: rand(1..100)
来源：http://xd.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://ec.nszjky.cn

[A11] 条件表达式（三元）
来源：http://vf.wgjwhj.cn

Py:   "yes" if x > 0 else "no"
来源：http://cm.shxzskj.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://yd.yuntaijiaju.cn

JS:   x > 0 ? "yes" : "no"
来源：http://rj.szxytkj.cn

TS:   x > 0 ? "yes" : "no"
来源：http://yo.nicolike.cn

Java: x > 0 ? "yes" : "no"
来源：http://ue.muxihuayi.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://ys.shtwfgs.cn


<!-- 参考信息 -->