代发 wailian999

[U69] PHP：PDO 预处理
来源：http://ek.asd995.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ki.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://mm.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wp.gzmigu.cn

[U71] PHP：抛出异常
来源：http://li.szsharing.cn

throw new RuntimeException("失败", 500);
来源：http://cl.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://yf.9csxet.cn

error_log("失败: " . $e->getMessage());
来源：http://ig.shxzukj.cn

[U73] PHP：读取 ini 配置
来源：http://dg.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://th.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://ov.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://bl.shxzukj.cn

[U75] PHP：依赖注入
来源：http://ba.nicolike.cn

composer require psr/container
来源：http://uc.gzmigu.cn

[U76] PHP：简单路由
来源：http://zt.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jm.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://bx.9csxet.cn

composer require twig/twig
来源：http://mo.bjjhwx.cn

[U78] PHP：单元测试
来源：http://fn.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://ir.nicolike.cn

[U79] PHP：静态分析
来源：http://vw.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://kc.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://no.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hb.shxzskj.cn

[U81] JS：初始化项目
来源：http://bg.hnjuh.cn

npm init -y;  npm i express
来源：http://nr.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://ew.huanxung.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ak.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://kf.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://dm.yuexingan06.cn

[U84] JS：CommonJS 写法
来源：http://cd.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://uo.muxihuayi.cn

[U85] JS：可选链
来源：http://vw.newstarts.cn

a?.b?.c
来源：http://ch.lnxyls.cn

[U86] JS：空值合并
来源：http://xu.szsharing.cn

a ?? b
来源：http://ra.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://ly.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://po.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://cl.521024.cn

{ ...a, ...b }
来源：http://rz.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://sf.asd995.cn

[...new Set(arr)]
来源：http://tk.gzmigu.cn

[U90] JS：数字数组排序
来源：http://ie.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://un.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://re.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nh.shtwfgs.cn

[U92] JS：深拷贝
来源：http://ko.newstarts.cn

structuredClone(obj)
来源：http://wa.hahajie.cn

[U93] JS：模板字符串
来源：http://ey.521024.cn

`共 ${n} 条`
来源：http://gm.hahajie.cn

[U94] JS：箭头函数
来源：http://yl.nszjky.cn

const double = x => x * 2;
来源：http://aj.yuntaijiaju.cn

[U95] JS：Promise 包装
来源：http://av.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://rt.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://ql.jianghongdianzi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qs.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://fw.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://lq.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://hd.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://rx.gzmigu.cn

[U99] JS：事件监听
来源：http://bq.jctech888.com.cn

el.addEventListener("click", e => {})
来源：http://qb.panjiajie.cn

[U100] JS：DOM 查询
来源：http://fw.shxzskj.cn

document.querySelector(".item")
来源：http://at.shxzskj.cn

[U101] JS：classList 操作
来源：http://vi.yuexingan06.cn

el.classList.toggle("active")
来源：http://mm.hnjuh.cn

[U102] JS：本地存储
来源：http://mo.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xi.nszjky.cn

[U103] JS：定时器
来源：http://cd.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kk.gzmigu.cn

[U104] JS：防抖
来源：http://bu.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vy.9csxet.cn

[U105] JS：节流
来源：http://cf.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cp.wgjwhj.cn

[U106] JS：日期格式化
来源：http://fa.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://su.chemitech.net.cn

[U107] JS：数字千分位
来源：http://qm.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://md.shtwfgs.cn

[U108] JS：随机整数
来源：http://pw.chemitech.net.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wk.lnxyls.cn

[U109] JS：数组分组
来源：http://yd.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://vn.haigaiapp.cn

[U110] JS：数组分块
来源：http://si.asd995.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://na.colortex.cn

[U111] JS：对象转 Map
来源：http://jl.colortex.cn

new Map(Object.entries(obj))
来源：http://wh.huixiangedu.cn

[U112] JS：字符串补位
来源：http://ne.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://zh.szsharing.cn

[U113] JS：正则替换全部
来源：http://nx.nszjky.cn

s.replaceAll("a", "b")
来源：http://fo.colortex.cn

[U114] JS：JSON 深比较
来源：http://tr.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xn.colortex.cn

[U115] JS：生成 UUID
来源：http://hz.muxihuayi.cn

crypto.randomUUID()
来源：http://hv.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://oj.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://al.asd995.cn

[U117] JS：单元测试
来源：http://ys.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://yo.hnjuh.cn

[U118] JS：开发服务器
来源：http://so.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://uf.bjjhwx.cn

[U119] JS：生产构建
来源：http://cc.wgjwhj.cn

npx vite build
来源：http://rc.jianghongdianzi.cn

[U120] JS：读取环境变量（Vite）
来源：http://yx.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://og.lnxyls.cn

================================================================================
来源：http://tk.521024.cn

统计汇总
来源：http://of.panjiajie.cn

================================================================================
来源：http://fv.jctech888.com.cn

按语言统计（条）：
来源：http://vc.yuexingan06.cn

Python ......... 252
来源：http://mu.hnjuh.cn

PHP ............ 252
来源：http://hs.chemitech.net.cn

JavaScript ..... 252
来源：http://df.hahajie.cn

TypeScript ..... 212
来源：http://vb.shxzskj.cn

Java ........... 212
来源：http://od.szsharing.cn

Go ............. 212
来源：http://nq.shxzukj.cn

Ruby ........... 212
来源：http://oo.jianghongdianzi.cn

C# ............. 212
来源：http://vk.yuexingan06.cn

C .............. 30
来源：http://zt.huanxung.cn

C++ ............ 30
来源：http://ni.szsharing.cn

SQL ............ 90
来源：http://xo.yuntaijiaju.cn

Bash ........... 80
来源：http://vr.hnjuh.cn

Kotlin ......... 15
来源：http://ky.jctech888.com.cn

Swift .......... 15
来源：http://uz.newstarts.cn

Lua ............ 10
来源：http://lh.hnjuh.cn

Perl ........... 10
来源：http://nl.jianghongdianzi.cn

Scala .......... 10
来源：http://oa.jianghongdianzi.cn

------------------------------------
来源：http://zm.shxzukj.cn

合计 ........... 2106 条
来源：http://lv.szxytkj.cn

按章节统计：
来源：http://em.huixiangedu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sx.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rb.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nz.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sw.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mq.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yu.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hj.hahajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dg.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fx.nicolike.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wq.lnxyls.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ek.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sc.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://he.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pu.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pj.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fu.nszjky.cn

Q SQL 专题                              90
来源：http://lr.shxzskj.cn

R Bash 专题                             80
来源：http://qt.shtwfgs.cn

S C / C++ 专题                          60
来源：http://mc.szxytkj.cn

T 其他语言补充                          60
来源：http://ix.nszjky.cn

U 高频实用片段                         120
来源：http://io.asd995.cn

------------------------------------
来源：http://uw.bookmarksfly.cn

合计                                  2106 条
来源：http://lv.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://vz.bjjhwx.cn

使用提醒
来源：http://jj.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://eh.521024.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://at.521024.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fy.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tm.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://jd.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pb.shtwfgs.cn

—— 文件结束 ——
来源：http://mu.shtwfgs.cn

================================================================================
来源：http://nk.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://nx.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://sq.muxihuayi.cn

================================================================================
来源：http://wk.huixinmuqiang.cn

【收录内容】
来源：http://rn.huanxung.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rh.jctech888.com.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bi.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://ek.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://qf.haigaiapp.cn

【使用说明】
来源：http://yb.huixinmuqiang.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ay.wgjwhj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nw.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://au.nszjky.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oa.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fg.9csxet.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iz.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ot.newstarts.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jx.szsharing.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://df.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://on.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://kk.huanxung.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mq.jctech888.com.cn

【文件统计】
来源：http://it.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vv.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://ma.yuntaijiaju.cn

目  录
来源：http://es.521024.cn

--------------------------------------------------------------------------------
来源：http://fg.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ku.huixiangedu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://de.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fp.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oe.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vt.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dn.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gy.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ep.lnxyls.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qq.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ky.nicolike.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tp.shxzukj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pb.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tj.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tr.jctech888.com.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ki.hnjuh.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://to.muxihuayi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qh.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://kc.hnjuh.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ul.jctech888.com.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ch.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ra.yuexingan06.cn

================================================================================
来源：http://zd.haigaiapp.cn

A. 基础语法与类型
来源：http://pw.gzmigu.cn

================================================================================
来源：http://es.shxzskj.cn

[A01] Hello World
来源：http://gd.nicolike.cn

Py:   print("Hello, World!")
来源：http://fe.asd995.cn

PHP:  echo "Hello, World!";
来源：http://hq.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://dz.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://gb.newstarts.cn

Java: System.out.println("Hello, World!");
来源：http://tu.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://jz.newstarts.cn

Ruby: puts "Hello, World!"
来源：http://hx.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://fg.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://pm.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bj.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ux.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://pq.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ae.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://xe.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://wl.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://ug.jianghongdianzi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://mt.muxihuayi.cn

[A03] 常量定义
来源：http://gz.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ef.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://bl.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://pe.shtwfgs.cn

TS:   const PI: number = 3.14159;
来源：http://ns.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://ah.shxzskj.cn

Go:   const PI = 3.14159
来源：http://mm.nicolike.cn

Ruby: PI = 3.14159
来源：http://db.panjiajie.cn

C#:   const double PI = 3.14159;
来源：http://bt.szxytkj.cn

[A04] 判断变量类型
来源：http://jt.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qe.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xk.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nz.9csxet.cn

TS:   typeof x; x instanceof Date
来源：http://jy.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ty.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://zh.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hz.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://yw.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://tz.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hv.huanxung.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gt.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nm.panjiajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oi.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://ce.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://hj.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://sd.521024.cn

C#:   7 / 2; 7 % 2
来源：http://fa.jianghongdianzi.cn

[A06] 字符串转数字
来源：http://ir.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://ak.hahajie.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nt.521024.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xr.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://hw.huanxung.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gm.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://pp.yuntaijiaju.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fu.huanxung.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jf.jctech888.com.cn

[A07] 数字转字符串
来源：http://xx.huixiangedu.cn

Py:   str(42)
来源：http://de.huixiangedu.cn

PHP:  (string) 42; strval(42)
来源：http://xj.muxihuayi.cn

JS:   String(42); (42).toString()
来源：http://do.newstarts.cn

TS:   String(42)
来源：http://lc.asd995.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rf.hnjuh.cn

Go:   strconv.Itoa(42)
来源：http://fn.huixiangedu.cn

Ruby: 42.to_s
来源：http://no.521024.cn

C#:   42.ToString()
来源：http://wx.szxytkj.cn

[A08] 取整与四舍五入
来源：http://eq.gzmigu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bf.nszjky.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tq.yuntaijiaju.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rw.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://ki.521024.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://gh.shxzukj.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ur.huixiangedu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://yb.huixiangedu.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ou.huixinmuqiang.cn

[A09] 绝对值与最大最小值
来源：http://lv.newstarts.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://qx.chemitech.net.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://qk.szsharing.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://iz.lnxyls.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mi.huixiangedu.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://jo.jctech888.com.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mr.wgjwhj.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://tr.9csxet.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zm.shxzukj.cn

[A10] 生成随机数
来源：http://ce.nicolike.cn

Py:   import random; random.randint(1, 100)
来源：http://ds.9csxet.cn

PHP:  random_int(1, 100);
来源：http://mn.9csxet.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wx.szsharing.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://ti.9csxet.cn

Java: new Random().nextInt(100) + 1
来源：http://aj.jctech888.com.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://cv.jianghongdianzi.cn

Ruby: rand(1..100)
来源：http://pc.hahajie.cn


<!-- 参考信息 -->