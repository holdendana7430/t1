代发 wailian999

[U71] PHP：抛出异常
来源：http://ie.nicolike.cn

throw new RuntimeException("失败", 500);
来源：http://ni.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://hc.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://hb.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://sh.huanxung.cn

parse_ini_file("config.ini", true)
来源：http://ta.colortex.cn

[U74] PHP：读取环境变量
来源：http://fi.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://yy.9csxet.cn

[U75] PHP：依赖注入
来源：http://wi.chemitech.net.cn

composer require psr/container
来源：http://oh.huanxung.cn

[U76] PHP：简单路由
来源：http://lx.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ic.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://lu.nszjky.cn

composer require twig/twig
来源：http://dz.haigaiapp.cn

[U78] PHP：单元测试
来源：http://dl.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://ly.szsharing.cn

[U79] PHP：静态分析
来源：http://oc.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://fh.huixinmuqiang.cn

[U80] PHP：代码规范修复
来源：http://hy.bookmarksfly.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zm.yuexingan06.cn

[U81] JS：初始化项目
来源：http://zp.colortex.cn

npm init -y;  npm i express
来源：http://sa.hahajie.cn

[U82] JS：package.json 脚本
来源：http://vu.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ai.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://wn.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zt.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://ho.shxzukj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ip.newstarts.cn

[U85] JS：可选链
来源：http://wf.lnxyls.cn

a?.b?.c
来源：http://tz.szxytkj.cn

[U86] JS：空值合并
来源：http://pb.jianghongdianzi.cn

a ?? b
来源：http://oc.gzmigu.cn

[U87] JS：解构默认值
来源：http://xx.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://rt.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://ke.jianghongdianzi.cn

{ ...a, ...b }
来源：http://en.huanxung.cn

[U89] JS：数组去重
来源：http://jf.shxzukj.cn

[...new Set(arr)]
来源：http://sl.huanxung.cn

[U90] JS：数字数组排序
来源：http://lj.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://fz.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://xy.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lg.shxzskj.cn

[U92] JS：深拷贝
来源：http://yi.9csxet.cn

structuredClone(obj)
来源：http://oo.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://va.yuexingan06.cn

`共 ${n} 条`
来源：http://wg.panjiajie.cn

[U94] JS：箭头函数
来源：http://jc.haigaiapp.cn

const double = x => x * 2;
来源：http://he.wgjwhj.cn

[U95] JS：Promise 包装
来源：http://fx.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://se.newstarts.cn

[U96] JS：async/await 与异常
来源：http://hq.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cb.wgjwhj.cn

[U97] JS：并发请求
来源：http://se.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hf.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://hv.colortex.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zp.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://fp.yuexingan06.cn

el.addEventListener("click", e => {})
来源：http://wh.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://cp.nszjky.cn

document.querySelector(".item")
来源：http://hn.huixiangedu.cn

[U101] JS：classList 操作
来源：http://go.yuexingan06.cn

el.classList.toggle("active")
来源：http://fl.chemitech.net.cn

[U102] JS：本地存储
来源：http://ip.muxihuayi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ce.chemitech.net.cn

[U103] JS：定时器
来源：http://wv.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ag.wgjwhj.cn

[U104] JS：防抖
来源：http://ep.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qo.yuntaijiaju.cn

[U105] JS：节流
来源：http://hb.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fj.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://do.bjjhwx.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yc.haigaiapp.cn

[U107] JS：数字千分位
来源：http://qy.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gd.yuntaijiaju.cn

[U108] JS：随机整数
来源：http://gh.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cy.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://wd.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://mr.colortex.cn

[U110] JS：数组分块
来源：http://bu.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xs.panjiajie.cn

[U111] JS：对象转 Map
来源：http://cx.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://xt.muxihuayi.cn

[U112] JS：字符串补位
来源：http://oi.lnxyls.cn

"7".padStart(3, "0")
来源：http://bi.gzmigu.cn

[U113] JS：正则替换全部
来源：http://bt.muxihuayi.cn

s.replaceAll("a", "b")
来源：http://co.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://wt.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wa.lnxyls.cn

[U115] JS：生成 UUID
来源：http://fh.shxzskj.cn

crypto.randomUUID()
来源：http://sg.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://fv.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://vv.huixiangedu.cn

[U117] JS：单元测试
来源：http://qn.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://xc.shtwfgs.cn

[U118] JS：开发服务器
来源：http://ma.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://ua.nicolike.cn

[U119] JS：生产构建
来源：http://qf.shxzskj.cn

npx vite build
来源：http://gc.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://cg.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://jh.bookmarksfly.cn

================================================================================
来源：http://ji.chemitech.net.cn

统计汇总
来源：http://pq.shxzskj.cn

================================================================================
来源：http://ol.newstarts.cn

按语言统计（条）：
来源：http://zd.shtwfgs.cn

Python ......... 252
来源：http://fd.chemitech.net.cn

PHP ............ 252
来源：http://op.wgjwhj.cn

JavaScript ..... 252
来源：http://mb.shxzukj.cn

TypeScript ..... 212
来源：http://ur.lnxyls.cn

Java ........... 212
来源：http://on.chemitech.net.cn

Go ............. 212
来源：http://ky.521024.cn

Ruby ........... 212
来源：http://me.hnjuh.cn

C# ............. 212
来源：http://cv.lnxyls.cn

C .............. 30
来源：http://kt.huanxung.cn

C++ ............ 30
来源：http://rv.colortex.cn

SQL ............ 90
来源：http://sa.huixinmuqiang.cn

Bash ........... 80
来源：http://yj.huanxung.cn

Kotlin ......... 15
来源：http://pp.jianghongdianzi.cn

Swift .......... 15
来源：http://ur.huanxung.cn

Lua ............ 10
来源：http://ii.huixinmuqiang.cn

Perl ........... 10
来源：http://ns.hnjuh.cn

Scala .......... 10
来源：http://ue.bookmarksfly.cn

------------------------------------
来源：http://kd.hahajie.cn

合计 ........... 2106 条
来源：http://ii.jianghongdianzi.cn

按章节统计：
来源：http://ty.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sg.colortex.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ij.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kb.panjiajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zw.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zq.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yz.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jm.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qz.bookmarksfly.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cx.bookmarksfly.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://np.yuntaijiaju.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://km.gzmigu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://up.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mj.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ib.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wu.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ap.muxihuayi.cn

Q SQL 专题                              90
来源：http://bj.shxzskj.cn

R Bash 专题                             80
来源：http://ip.muxihuayi.cn

S C / C++ 专题                          60
来源：http://vj.nszjky.cn

T 其他语言补充                          60
来源：http://pr.colortex.cn

U 高频实用片段                         120
来源：http://uj.huixiangedu.cn

------------------------------------
来源：http://up.shxzukj.cn

合计                                  2106 条
来源：http://it.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ks.bjjhwx.cn

使用提醒
来源：http://xw.nicolike.cn

--------------------------------------------------------------------------------
来源：http://vg.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hw.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ms.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cy.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zn.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://np.bookmarksfly.cn

—— 文件结束 ——
来源：http://vi.muxihuayi.cn

================================================================================
来源：http://ho.9csxet.cn

程序语言常见例子速查手册（2024 版）
来源：http://bs.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://xq.521024.cn

================================================================================
来源：http://wy.newstarts.cn

【收录内容】
来源：http://sf.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rk.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lm.wgjwhj.cn

SQL · Bash · C · C++
来源：http://fh.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fn.szxytkj.cn

【使用说明】
来源：http://nr.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cw.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://na.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sy.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://eq.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://sj.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dx.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zq.yuntaijiaju.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vu.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ok.jctech888.com.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wk.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ya.nicolike.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vg.huanxung.cn

【文件统计】
来源：http://zt.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jy.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://ff.bjjhwx.cn

目  录
来源：http://jk.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ct.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tm.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ol.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://td.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nh.szxytkj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bm.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tl.muxihuayi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gv.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lj.panjiajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://df.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ia.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tk.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ld.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kq.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vf.muxihuayi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cw.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vn.newstarts.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wx.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yl.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://cn.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://xj.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://iz.jianghongdianzi.cn

================================================================================
来源：http://pt.szxytkj.cn

A. 基础语法与类型
来源：http://ir.hnjuh.cn

================================================================================
来源：http://zg.bookmarksfly.cn

[A01] Hello World
来源：http://oh.huanxung.cn

Py:   print("Hello, World!")
来源：http://me.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://mr.bjjhwx.cn

JS:   console.log("Hello, World!");
来源：http://ni.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qz.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://gg.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://pv.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://zf.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://iy.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://di.colortex.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://dt.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qa.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tl.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ge.yuexingan06.cn

Java: String name = "Alex"; int age = 20;
来源：http://jp.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://sb.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://jc.yuexingan06.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jy.huixiangedu.cn

[A03] 常量定义
来源：http://wo.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vu.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://kl.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://cg.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://hp.huixiangedu.cn

Java: static final double PI = 3.14159;
来源：http://xy.9csxet.cn

Go:   const PI = 3.14159
来源：http://gb.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://hf.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://nm.bjjhwx.cn

[A04] 判断变量类型
来源：http://wu.huixiangedu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://de.muxihuayi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fh.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ei.shxzskj.cn

TS:   typeof x; x instanceof Date
来源：http://bj.szxytkj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://em.yuntaijiaju.cn

Go:   reflect.TypeOf(x).Name()
来源：http://su.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vq.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://gk.shtwfgs.cn

[A05] 整数除法与取模
来源：http://pe.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cb.bookmarksfly.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://js.szsharing.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ma.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oy.colortex.cn

Java: 7 / 2; 7 % 2
来源：http://fe.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://tc.shxzukj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qk.hnjuh.cn

C#:   7 / 2; 7 % 2
来源：http://ph.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://xk.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://up.yuntaijiaju.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gk.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://cu.asd995.cn

TS:   parseInt("42", 10); Number("42")
来源：http://tp.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wd.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://in.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://vt.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cz.shxzukj.cn

[A07] 数字转字符串
来源：http://er.wgjwhj.cn

Py:   str(42)
来源：http://wh.szsharing.cn

PHP:  (string) 42; strval(42)
来源：http://vz.bjjhwx.cn

JS:   String(42); (42).toString()
来源：http://gz.colortex.cn

TS:   String(42)
来源：http://zf.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ts.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://ru.jctech888.com.cn

Ruby: 42.to_s
来源：http://wp.9csxet.cn

C#:   42.ToString()
来源：http://ps.gzmigu.cn

[A08] 取整与四舍五入
来源：http://ki.panjiajie.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://oj.lnxyls.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://pz.nszjky.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ms.huanxung.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hb.szsharing.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ot.hahajie.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://eh.9csxet.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://pk.hnjuh.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ok.bjjhwx.cn

[A09] 绝对值与最大最小值
来源：http://sl.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://yw.shxzukj.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ap.newstarts.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://kq.jianghongdianzi.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sl.lnxyls.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jg.haigaiapp.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://py.hnjuh.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://id.hahajie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://dj.shxzskj.cn

[A10] 生成随机数
来源：http://nn.szxytkj.cn

Py:   import random; random.randint(1, 100)
来源：http://zx.lnxyls.cn

PHP:  random_int(1, 100);
来源：http://zo.jctech888.com.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://cc.bookmarksfly.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://dd.huixinmuqiang.cn

Java: new Random().nextInt(100) + 1
来源：http://gf.hnjuh.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://yo.9csxet.cn

Ruby: rand(1..100)
来源：http://wy.jianghongdianzi.cn

C#:   new Random().Next(1, 101)
来源：http://fj.jianghongdianzi.cn

[A11] 条件表达式（三元）
来源：http://pz.huanxung.cn

Py:   "yes" if x > 0 else "no"
来源：http://mq.asd995.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://cs.haigaiapp.cn


<!-- 参考信息 -->