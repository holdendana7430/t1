代发 wailian999

[U59] PHP：自定义排序
来源：http://ja.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ft.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://yd.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://om.szsharing.cn

[U61] PHP：正则
来源：http://fs.nszjky.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ts.newstarts.cn

[U62] PHP：日期对象
来源：http://ww.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mg.nicolike.cn

[U63] PHP：文件读写
来源：http://uo.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ui.521024.cn

[U64] PHP：目录遍历
来源：http://oc.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://ws.huanxung.cn

[U65] PHP：会话
来源：http://uh.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pm.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://ax.gzmigu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://bl.hahajie.cn

[U67] PHP：处理文件上传
来源：http://jn.jctech888.com.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sm.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://gb.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eg.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://lf.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oi.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ej.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mx.gzmigu.cn

[U71] PHP：抛出异常
来源：http://zn.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://fw.huanxung.cn

[U72] PHP：写错误日志
来源：http://sd.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://ue.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://ei.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://bj.shxzskj.cn

[U74] PHP：读取环境变量
来源：http://fb.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://oe.colortex.cn

[U75] PHP：依赖注入
来源：http://dy.hahajie.cn

composer require psr/container
来源：http://qh.huanxung.cn

[U76] PHP：简单路由
来源：http://ew.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ic.nicolike.cn

[U77] PHP：模板渲染
来源：http://yv.hahajie.cn

composer require twig/twig
来源：http://zl.huixiangedu.cn

[U78] PHP：单元测试
来源：http://gy.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://op.haigaiapp.cn

[U79] PHP：静态分析
来源：http://dn.521024.cn

composer require --dev phpstan/phpstan
来源：http://fu.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://in.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zv.bjjhwx.cn

[U81] JS：初始化项目
来源：http://eu.yuexingan06.cn

npm init -y;  npm i express
来源：http://dk.nszjky.cn

[U82] JS：package.json 脚本
来源：http://lr.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cu.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://ub.asd995.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jc.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://fr.szxytkj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qd.bookmarksfly.cn

[U85] JS：可选链
来源：http://cu.huixinmuqiang.cn

a?.b?.c
来源：http://al.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ju.wgjwhj.cn

a ?? b
来源：http://lq.chemitech.net.cn

[U87] JS：解构默认值
来源：http://bt.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://ge.shxzukj.cn

[U88] JS：对象展开合并
来源：http://wo.bookmarksfly.cn

{ ...a, ...b }
来源：http://bk.shxzukj.cn

[U89] JS：数组去重
来源：http://fh.521024.cn

[...new Set(arr)]
来源：http://fk.nicolike.cn

[U90] JS：数字数组排序
来源：http://rk.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://sx.lnxyls.cn

[U91] JS：对象键值遍历
来源：http://tk.hahajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hf.nicolike.cn

[U92] JS：深拷贝
来源：http://ge.bookmarksfly.cn

structuredClone(obj)
来源：http://kd.521024.cn

[U93] JS：模板字符串
来源：http://pw.bjjhwx.cn

`共 ${n} 条`
来源：http://ox.huixinmuqiang.cn

[U94] JS：箭头函数
来源：http://ko.huixinmuqiang.cn

const double = x => x * 2;
来源：http://xu.shxzukj.cn

[U95] JS：Promise 包装
来源：http://qp.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://jc.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://gp.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bb.colortex.cn

[U97] JS：并发请求
来源：http://mw.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rx.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://qn.lnxyls.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wo.szxytkj.cn

[U99] JS：事件监听
来源：http://ff.521024.cn

el.addEventListener("click", e => {})
来源：http://ni.shxzskj.cn

[U100] JS：DOM 查询
来源：http://oq.colortex.cn

document.querySelector(".item")
来源：http://gz.szsharing.cn

[U101] JS：classList 操作
来源：http://jz.bookmarksfly.cn

el.classList.toggle("active")
来源：http://ko.lnxyls.cn

[U102] JS：本地存储
来源：http://ez.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://km.hnjuh.cn

[U103] JS：定时器
来源：http://uw.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wi.bookmarksfly.cn

[U104] JS：防抖
来源：http://yf.huanxung.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xc.muxihuayi.cn

[U105] JS：节流
来源：http://qw.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://eq.hahajie.cn

[U106] JS：日期格式化
来源：http://gp.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://gb.521024.cn

[U107] JS：数字千分位
来源：http://ib.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ew.szsharing.cn

[U108] JS：随机整数
来源：http://ru.hahajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wj.9csxet.cn

[U109] JS：数组分组
来源：http://qv.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://sl.nszjky.cn

[U110] JS：数组分块
来源：http://vp.haigaiapp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bu.9csxet.cn

[U111] JS：对象转 Map
来源：http://mr.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://ie.asd995.cn

[U112] JS：字符串补位
来源：http://if.521024.cn

"7".padStart(3, "0")
来源：http://yf.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://wd.nicolike.cn

s.replaceAll("a", "b")
来源：http://hj.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://iw.szxytkj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ns.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://yp.yuexingan06.cn

crypto.randomUUID()
来源：http://kj.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://yu.huixinmuqiang.cn

/** @param {string} name */ function f(name) {}
来源：http://dr.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://fy.hahajie.cn

npm i -D vitest;  npx vitest
来源：http://mt.chemitech.net.cn

[U118] JS：开发服务器
来源：http://kw.gzmigu.cn

npm i -D vite;  npx vite
来源：http://jb.szsharing.cn

[U119] JS：生产构建
来源：http://yb.huanxung.cn

npx vite build
来源：http://cu.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://qs.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://oi.jianghongdianzi.cn

================================================================================
来源：http://pz.bjjhwx.cn

统计汇总
来源：http://lv.colortex.cn

================================================================================
来源：http://fx.haigaiapp.cn

按语言统计（条）：
来源：http://ww.asd995.cn

Python ......... 252
来源：http://ih.muxihuayi.cn

PHP ............ 252
来源：http://tw.yuexingan06.cn

JavaScript ..... 252
来源：http://rq.hahajie.cn

TypeScript ..... 212
来源：http://yn.panjiajie.cn

Java ........... 212
来源：http://mj.nszjky.cn

Go ............. 212
来源：http://pw.nszjky.cn

Ruby ........... 212
来源：http://mp.521024.cn

C# ............. 212
来源：http://vq.yuntaijiaju.cn

C .............. 30
来源：http://ng.bookmarksfly.cn

C++ ............ 30
来源：http://at.bookmarksfly.cn

SQL ............ 90
来源：http://ek.asd995.cn

Bash ........... 80
来源：http://nf.wgjwhj.cn

Kotlin ......... 15
来源：http://xa.yuntaijiaju.cn

Swift .......... 15
来源：http://ho.asd995.cn

Lua ............ 10
来源：http://xn.muxihuayi.cn

Perl ........... 10
来源：http://ee.wgjwhj.cn

Scala .......... 10
来源：http://mx.hnjuh.cn

------------------------------------
来源：http://tv.huanxung.cn

合计 ........... 2106 条
来源：http://oy.shxzukj.cn

按章节统计：
来源：http://wi.jctech888.com.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mm.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wm.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rw.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://of.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ua.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://uj.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nm.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://yi.hnjuh.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://se.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://az.huanxung.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jl.hnjuh.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rn.yuntaijiaju.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yd.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ic.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uj.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hd.wgjwhj.cn

Q SQL 专题                              90
来源：http://wh.newstarts.cn

R Bash 专题                             80
来源：http://eb.szsharing.cn

S C / C++ 专题                          60
来源：http://yy.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://gz.bookmarksfly.cn

U 高频实用片段                         120
来源：http://vy.bjjhwx.cn

------------------------------------
来源：http://ai.yuntaijiaju.cn

合计                                  2106 条
来源：http://uz.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://hb.haigaiapp.cn

使用提醒
来源：http://ui.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://dp.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qa.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jn.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ne.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yt.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ub.shtwfgs.cn

—— 文件结束 ——
来源：http://vk.panjiajie.cn

================================================================================
来源：http://sk.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ps.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://vs.bjjhwx.cn

================================================================================
来源：http://dl.gzmigu.cn

【收录内容】
来源：http://ya.colortex.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://er.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://qp.shxzukj.cn

SQL · Bash · C · C++
来源：http://if.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ku.nszjky.cn

【使用说明】
来源：http://ds.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nc.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xj.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://sb.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hf.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://zp.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://df.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ud.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jx.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wk.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cy.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cx.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wg.9csxet.cn

【文件统计】
来源：http://pp.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rn.asd995.cn

--------------------------------------------------------------------------------
来源：http://my.shxzskj.cn

目  录
来源：http://ft.huanxung.cn

--------------------------------------------------------------------------------
来源：http://xj.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ww.szxytkj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dh.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://at.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rx.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://aj.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gf.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://od.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qb.shxzskj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://oh.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ir.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://iw.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://py.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ry.newstarts.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gm.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cb.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sy.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gs.huanxung.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yr.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://eh.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ue.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zi.shxzukj.cn

================================================================================
来源：http://ag.newstarts.cn

A. 基础语法与类型
来源：http://xs.shtwfgs.cn

================================================================================
来源：http://yq.bjjhwx.cn

[A01] Hello World
来源：http://nh.9csxet.cn

Py:   print("Hello, World!")
来源：http://nv.newstarts.cn

PHP:  echo "Hello, World!";
来源：http://kg.asd995.cn

JS:   console.log("Hello, World!");
来源：http://xu.huanxung.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fh.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://vu.wgjwhj.cn

Go:   fmt.Println("Hello, World!")
来源：http://iq.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ct.wgjwhj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ku.nicolike.cn

[A02] 变量声明与赋值
来源：http://xk.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yb.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qa.newstarts.cn

JS:   let name = "Alex"; const age = 20;
来源：http://mn.gzmigu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://sj.panjiajie.cn

Java: String name = "Alex"; int age = 20;
来源：http://jt.chemitech.net.cn

Go:   name := "Alex"; age := 20
来源：http://dl.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://bw.bjjhwx.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gs.nszjky.cn

[A03] 常量定义
来源：http://cx.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://sz.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://nh.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://ji.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://ew.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://xk.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://bf.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://ai.colortex.cn

C#:   const double PI = 3.14159;
来源：http://sw.szsharing.cn

[A04] 判断变量类型
来源：http://ln.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://va.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rm.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://by.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://tu.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ss.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://if.colortex.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://er.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://ab.bjjhwx.cn

[A05] 整数除法与取模
来源：http://oy.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://zb.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ou.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://rz.huixinmuqiang.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kr.jianghongdianzi.cn

Java: 7 / 2; 7 % 2
来源：http://up.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://co.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://vs.szxytkj.cn

C#:   7 / 2; 7 % 2
来源：http://zs.panjiajie.cn

[A06] 字符串转数字
来源：http://rg.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://mu.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://er.gzmigu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://nz.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ch.shxzskj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ir.yuexingan06.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ws.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://il.nicolike.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://pa.521024.cn

[A07] 数字转字符串
来源：http://sg.nszjky.cn

Py:   str(42)
来源：http://bv.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://wy.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://od.shxzskj.cn

TS:   String(42)
来源：http://xk.hahajie.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://iv.nicolike.cn

Go:   strconv.Itoa(42)
来源：http://mi.bjjhwx.cn

Ruby: 42.to_s
来源：http://fa.gzmigu.cn

C#:   42.ToString()
来源：http://lc.wgjwhj.cn

[A08] 取整与四舍五入
来源：http://ce.9csxet.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://cm.hahajie.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ze.nicolike.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://bu.yuexingan06.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://cd.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://tn.9csxet.cn


<!-- 参考信息 -->