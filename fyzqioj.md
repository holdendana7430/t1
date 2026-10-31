代发 wailian999

[U71] PHP：抛出异常
来源：http://sl.521024.cn

throw new RuntimeException("失败", 500);
来源：http://nx.jianghongdianzi.cn

[U72] PHP：写错误日志
来源：http://nj.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://bh.nicolike.cn

[U73] PHP：读取 ini 配置
来源：http://rm.colortex.cn

parse_ini_file("config.ini", true)
来源：http://ms.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://is.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://th.lnxyls.cn

[U75] PHP：依赖注入
来源：http://ob.9csxet.cn

composer require psr/container
来源：http://qd.wgjwhj.cn

[U76] PHP：简单路由
来源：http://jt.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qc.shxzskj.cn

[U77] PHP：模板渲染
来源：http://fg.haigaiapp.cn

composer require twig/twig
来源：http://xu.hahajie.cn

[U78] PHP：单元测试
来源：http://al.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://hk.shtwfgs.cn

[U79] PHP：静态分析
来源：http://fk.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://ug.jctech888.com.cn

[U80] PHP：代码规范修复
来源：http://pn.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ad.shxzukj.cn

[U81] JS：初始化项目
来源：http://uq.asd995.cn

npm init -y;  npm i express
来源：http://yb.szsharing.cn

[U82] JS：package.json 脚本
来源：http://xr.nicolike.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cp.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://hp.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://go.asd995.cn

[U84] JS：CommonJS 写法
来源：http://fi.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ds.jctech888.com.cn

[U85] JS：可选链
来源：http://gi.newstarts.cn

a?.b?.c
来源：http://jv.wgjwhj.cn

[U86] JS：空值合并
来源：http://ss.huixiangedu.cn

a ?? b
来源：http://xu.haigaiapp.cn

[U87] JS：解构默认值
来源：http://pg.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://jb.shxzskj.cn

[U88] JS：对象展开合并
来源：http://gs.bjjhwx.cn

{ ...a, ...b }
来源：http://oa.bjjhwx.cn

[U89] JS：数组去重
来源：http://ke.haigaiapp.cn

[...new Set(arr)]
来源：http://wc.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://zl.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://vn.shxzskj.cn

[U91] JS：对象键值遍历
来源：http://gw.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pn.muxihuayi.cn

[U92] JS：深拷贝
来源：http://pj.szsharing.cn

structuredClone(obj)
来源：http://mk.yuexingan06.cn

[U93] JS：模板字符串
来源：http://wx.szxytkj.cn

`共 ${n} 条`
来源：http://ez.521024.cn

[U94] JS：箭头函数
来源：http://ak.nszjky.cn

const double = x => x * 2;
来源：http://xz.9csxet.cn

[U95] JS：Promise 包装
来源：http://qa.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://xm.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://bu.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://em.haigaiapp.cn

[U97] JS：并发请求
来源：http://qr.yuexingan06.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://bk.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://tp.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tp.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://uo.9csxet.cn

el.addEventListener("click", e => {})
来源：http://qe.colortex.cn

[U100] JS：DOM 查询
来源：http://fo.yuexingan06.cn

document.querySelector(".item")
来源：http://ce.muxihuayi.cn

[U101] JS：classList 操作
来源：http://da.gzmigu.cn

el.classList.toggle("active")
来源：http://sl.asd995.cn

[U102] JS：本地存储
来源：http://pe.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://of.jctech888.com.cn

[U103] JS：定时器
来源：http://vm.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hr.szsharing.cn

[U104] JS：防抖
来源：http://hx.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ms.chemitech.net.cn

[U105] JS：节流
来源：http://ys.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://oc.521024.cn

[U106] JS：日期格式化
来源：http://zf.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://be.huanxung.cn

[U107] JS：数字千分位
来源：http://um.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cj.shxzukj.cn

[U108] JS：随机整数
来源：http://kr.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qj.szsharing.cn

[U109] JS：数组分组
来源：http://ga.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://pv.asd995.cn

[U110] JS：数组分块
来源：http://qi.shxzskj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uh.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://bc.colortex.cn

new Map(Object.entries(obj))
来源：http://px.lnxyls.cn

[U112] JS：字符串补位
来源：http://tz.hnjuh.cn

"7".padStart(3, "0")
来源：http://pj.huixiangedu.cn

[U113] JS：正则替换全部
来源：http://zs.shxzukj.cn

s.replaceAll("a", "b")
来源：http://ws.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://wc.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ue.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://rw.jianghongdianzi.cn

crypto.randomUUID()
来源：http://ef.bookmarksfly.cn

[U116] JS：类型检查（JSDoc）
来源：http://uf.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://tg.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://fd.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://ac.shxzskj.cn

[U118] JS：开发服务器
来源：http://cj.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://xn.521024.cn

[U119] JS：生产构建
来源：http://eg.wgjwhj.cn

npx vite build
来源：http://cz.9csxet.cn

[U120] JS：读取环境变量（Vite）
来源：http://il.muxihuayi.cn

import.meta.env.VITE_API_URL
来源：http://cl.yuexingan06.cn

================================================================================
来源：http://da.hnjuh.cn

统计汇总
来源：http://ju.9csxet.cn

================================================================================
来源：http://td.panjiajie.cn

按语言统计（条）：
来源：http://tu.muxihuayi.cn

Python ......... 252
来源：http://vc.yuntaijiaju.cn

PHP ............ 252
来源：http://ph.colortex.cn

JavaScript ..... 252
来源：http://oh.panjiajie.cn

TypeScript ..... 212
来源：http://ra.shxzukj.cn

Java ........... 212
来源：http://fo.bjjhwx.cn

Go ............. 212
来源：http://nc.shxzskj.cn

Ruby ........... 212
来源：http://un.szsharing.cn

C# ............. 212
来源：http://nl.muxihuayi.cn

C .............. 30
来源：http://ts.shxzukj.cn

C++ ............ 30
来源：http://jj.haigaiapp.cn

SQL ............ 90
来源：http://uo.yuexingan06.cn

Bash ........... 80
来源：http://xh.asd995.cn

Kotlin ......... 15
来源：http://mp.yuntaijiaju.cn

Swift .......... 15
来源：http://dg.nicolike.cn

Lua ............ 10
来源：http://ae.huixinmuqiang.cn

Perl ........... 10
来源：http://zb.nicolike.cn

Scala .......... 10
来源：http://rn.wgjwhj.cn

------------------------------------
来源：http://hd.panjiajie.cn

合计 ........... 2106 条
来源：http://st.hnjuh.cn

按章节统计：
来源：http://vr.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vb.huixiangedu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cf.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ew.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sq.9csxet.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jk.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nm.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://sc.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ue.jctech888.com.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://co.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://go.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gb.szsharing.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://us.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xi.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mm.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ei.nicolike.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://el.nszjky.cn

Q SQL 专题                              90
来源：http://td.nicolike.cn

R Bash 专题                             80
来源：http://pb.huanxung.cn

S C / C++ 专题                          60
来源：http://au.hahajie.cn

T 其他语言补充                          60
来源：http://cg.bookmarksfly.cn

U 高频实用片段                         120
来源：http://lb.bjjhwx.cn

------------------------------------
来源：http://lz.huanxung.cn

合计                                  2106 条
来源：http://pt.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://av.521024.cn

使用提醒
来源：http://gj.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://dw.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cf.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vq.wgjwhj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hu.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://et.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ov.bookmarksfly.cn

—— 文件结束 ——
来源：http://ns.haigaiapp.cn

================================================================================
来源：http://wu.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://xw.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://yf.huixinmuqiang.cn

================================================================================
来源：http://ol.muxihuayi.cn

【收录内容】
来源：http://gw.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://bw.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ze.colortex.cn

SQL · Bash · C · C++
来源：http://qy.jctech888.com.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wx.colortex.cn

【使用说明】
来源：http://hb.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lz.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://pk.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ex.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://er.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cv.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://rw.shtwfgs.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nq.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ki.521024.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oy.colortex.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ta.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dp.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bm.jctech888.com.cn

【文件统计】
来源：http://yc.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bx.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://do.gzmigu.cn

目  录
来源：http://dg.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://yb.shxzukj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wm.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xg.lnxyls.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://go.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eb.panjiajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nc.nicolike.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xe.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://um.szxytkj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ev.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mq.szxytkj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nv.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ns.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bb.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dm.huixiangedu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vf.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://fn.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fi.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dk.nicolike.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pe.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://iw.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vk.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://sh.nszjky.cn

================================================================================
来源：http://mi.9csxet.cn

A. 基础语法与类型
来源：http://yi.yuntaijiaju.cn

================================================================================
来源：http://ha.wgjwhj.cn

[A01] Hello World
来源：http://ry.huixiangedu.cn

Py:   print("Hello, World!")
来源：http://zz.panjiajie.cn

PHP:  echo "Hello, World!";
来源：http://aw.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://io.haigaiapp.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ou.9csxet.cn

Java: System.out.println("Hello, World!");
来源：http://by.haigaiapp.cn

Go:   fmt.Println("Hello, World!")
来源：http://bg.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://xg.asd995.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bh.panjiajie.cn

[A02] 变量声明与赋值
来源：http://tu.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iv.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ac.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mj.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://js.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://ce.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://ys.jctech888.com.cn

Ruby: name = "Alex"; age = 20
来源：http://ck.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ar.wgjwhj.cn

[A03] 常量定义
来源：http://zh.521024.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bv.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://my.nszjky.cn

JS:   const PI = 3.14159;
来源：http://xk.yuexingan06.cn

TS:   const PI: number = 3.14159;
来源：http://vc.jianghongdianzi.cn

Java: static final double PI = 3.14159;
来源：http://dl.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://fj.colortex.cn

Ruby: PI = 3.14159
来源：http://ea.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://pj.jctech888.com.cn

[A04] 判断变量类型
来源：http://tx.bookmarksfly.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://pv.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ir.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xn.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://ti.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rc.yuexingan06.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pp.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://wn.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://jq.szsharing.cn

[A05] 整数除法与取模
来源：http://ua.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://of.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tx.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mh.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ur.hnjuh.cn

Java: 7 / 2; 7 % 2
来源：http://yy.jctech888.com.cn

Go:   7 / 2; 7 % 2
来源：http://bx.jianghongdianzi.cn

Ruby: 7 / 2; 7 % 2
来源：http://sx.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://fu.gzmigu.cn

[A06] 字符串转数字
来源：http://gy.colortex.cn

Py:   int("42"); float("3.14")
来源：http://tk.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gl.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://eq.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jo.nszjky.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nh.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cb.jctech888.com.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tx.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ft.haigaiapp.cn

[A07] 数字转字符串
来源：http://uf.yuntaijiaju.cn

Py:   str(42)
来源：http://nk.huanxung.cn

PHP:  (string) 42; strval(42)
来源：http://fs.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://qp.colortex.cn

TS:   String(42)
来源：http://uc.newstarts.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ph.asd995.cn

Go:   strconv.Itoa(42)
来源：http://qu.szxytkj.cn

Ruby: 42.to_s
来源：http://fk.nszjky.cn

C#:   42.ToString()
来源：http://sk.shtwfgs.cn

[A08] 取整与四舍五入
来源：http://lg.shxzskj.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wn.huixiangedu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://qb.szsharing.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://lu.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://qi.gzmigu.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lf.huanxung.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wr.muxihuayi.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://wd.bjjhwx.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ah.panjiajie.cn

[A09] 绝对值与最大最小值
来源：http://yb.muxihuayi.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://oq.wgjwhj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://pj.jianghongdianzi.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://gr.bookmarksfly.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wy.nicolike.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ts.yuexingan06.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://me.shxzukj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hk.szxytkj.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fo.bookmarksfly.cn

[A10] 生成随机数
来源：http://nn.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ey.szxytkj.cn

PHP:  random_int(1, 100);
来源：http://bh.panjiajie.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://kh.huixiangedu.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://xs.hahajie.cn

Java: new Random().nextInt(100) + 1
来源：http://ih.hahajie.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://jm.shxzukj.cn

Ruby: rand(1..100)
来源：http://pa.szsharing.cn

C#:   new Random().Next(1, 101)
来源：http://rk.huanxung.cn

[A11] 条件表达式（三元）
来源：http://tx.shxzukj.cn

Py:   "yes" if x > 0 else "no"
来源：http://pu.yuexingan06.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://dn.9csxet.cn


<!-- 参考信息 -->