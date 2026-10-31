代发 wailian999

[U65] PHP：会话
来源：http://dd.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sl.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://fb.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ji.huanxung.cn

[U67] PHP：处理文件上传
来源：http://dl.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rb.shxzukj.cn

[U68] PHP：PDO 连接
来源：http://oh.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ak.colortex.cn

[U69] PHP：PDO 预处理
来源：http://il.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yh.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://pj.shtwfgs.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ur.nszjky.cn

[U71] PHP：抛出异常
来源：http://bs.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://ca.nicolike.cn

[U72] PHP：写错误日志
来源：http://mi.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://oz.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://sp.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://mx.hahajie.cn

[U74] PHP：读取环境变量
来源：http://fb.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://hc.panjiajie.cn

[U75] PHP：依赖注入
来源：http://xv.9csxet.cn

composer require psr/container
来源：http://ln.hnjuh.cn

[U76] PHP：简单路由
来源：http://ll.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ke.bjjhwx.cn

[U77] PHP：模板渲染
来源：http://ff.yuntaijiaju.cn

composer require twig/twig
来源：http://kt.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://vd.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://kx.panjiajie.cn

[U79] PHP：静态分析
来源：http://bo.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://ox.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://aa.nicolike.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://al.hahajie.cn

[U81] JS：初始化项目
来源：http://vy.huixiangedu.cn

npm init -y;  npm i express
来源：http://qw.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://uv.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ia.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://rj.colortex.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ih.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://nq.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jh.nicolike.cn

[U85] JS：可选链
来源：http://lk.newstarts.cn

a?.b?.c
来源：http://gu.nszjky.cn

[U86] JS：空值合并
来源：http://qd.9csxet.cn

a ?? b
来源：http://ws.jianghongdianzi.cn

[U87] JS：解构默认值
来源：http://an.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://vk.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://fx.yuntaijiaju.cn

{ ...a, ...b }
来源：http://yt.colortex.cn

[U89] JS：数组去重
来源：http://ja.yuntaijiaju.cn

[...new Set(arr)]
来源：http://oo.shxzskj.cn

[U90] JS：数字数组排序
来源：http://rg.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://ev.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://wu.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vc.gzmigu.cn

[U92] JS：深拷贝
来源：http://be.bookmarksfly.cn

structuredClone(obj)
来源：http://tv.haigaiapp.cn

[U93] JS：模板字符串
来源：http://rt.asd995.cn

`共 ${n} 条`
来源：http://gd.shxzskj.cn

[U94] JS：箭头函数
来源：http://fm.nicolike.cn

const double = x => x * 2;
来源：http://qq.lnxyls.cn

[U95] JS：Promise 包装
来源：http://mw.huixiangedu.cn

new Promise((resolve, reject) => {})
来源：http://ck.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://vq.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gl.lnxyls.cn

[U97] JS：并发请求
来源：http://ve.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nr.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://fm.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gu.shxzskj.cn

[U99] JS：事件监听
来源：http://dj.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://bv.521024.cn

[U100] JS：DOM 查询
来源：http://tl.nszjky.cn

document.querySelector(".item")
来源：http://ky.colortex.cn

[U101] JS：classList 操作
来源：http://xk.nicolike.cn

el.classList.toggle("active")
来源：http://pc.shxzskj.cn

[U102] JS：本地存储
来源：http://ts.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hf.yuntaijiaju.cn

[U103] JS：定时器
来源：http://nh.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hg.muxihuayi.cn

[U104] JS：防抖
来源：http://ks.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://th.newstarts.cn

[U105] JS：节流
来源：http://fv.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://de.hahajie.cn

[U106] JS：日期格式化
来源：http://pt.lnxyls.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lt.nicolike.cn

[U107] JS：数字千分位
来源：http://yv.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qz.521024.cn

[U108] JS：随机整数
来源：http://pe.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zr.shxzukj.cn

[U109] JS：数组分组
来源：http://hm.jianghongdianzi.cn

Object.groupBy(arr, x => x.type)
来源：http://dt.yuexingan06.cn

[U110] JS：数组分块
来源：http://qp.yuexingan06.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tr.hahajie.cn

[U111] JS：对象转 Map
来源：http://bo.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://es.gzmigu.cn

[U112] JS：字符串补位
来源：http://pr.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://wu.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://xi.gzmigu.cn

s.replaceAll("a", "b")
来源：http://zo.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://mf.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bj.colortex.cn

[U115] JS：生成 UUID
来源：http://xj.chemitech.net.cn

crypto.randomUUID()
来源：http://dm.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://xz.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://dp.panjiajie.cn

[U117] JS：单元测试
来源：http://hq.asd995.cn

npm i -D vitest;  npx vitest
来源：http://xt.lnxyls.cn

[U118] JS：开发服务器
来源：http://of.bjjhwx.cn

npm i -D vite;  npx vite
来源：http://lf.wgjwhj.cn

[U119] JS：生产构建
来源：http://dk.nicolike.cn

npx vite build
来源：http://di.newstarts.cn

[U120] JS：读取环境变量（Vite）
来源：http://uz.shxzukj.cn

import.meta.env.VITE_API_URL
来源：http://lo.szsharing.cn

================================================================================
来源：http://yr.shxzskj.cn

统计汇总
来源：http://re.9csxet.cn

================================================================================
来源：http://rn.huixiangedu.cn

按语言统计（条）：
来源：http://dn.hnjuh.cn

Python ......... 252
来源：http://zx.muxihuayi.cn

PHP ............ 252
来源：http://fx.chemitech.net.cn

JavaScript ..... 252
来源：http://ge.colortex.cn

TypeScript ..... 212
来源：http://lc.gzmigu.cn

Java ........... 212
来源：http://wk.shxzskj.cn

Go ............. 212
来源：http://yp.shxzukj.cn

Ruby ........... 212
来源：http://no.muxihuayi.cn

C# ............. 212
来源：http://eh.bjjhwx.cn

C .............. 30
来源：http://ty.hnjuh.cn

C++ ............ 30
来源：http://fy.jianghongdianzi.cn

SQL ............ 90
来源：http://wh.yuexingan06.cn

Bash ........... 80
来源：http://vj.wgjwhj.cn

Kotlin ......... 15
来源：http://kd.nszjky.cn

Swift .......... 15
来源：http://dm.shxzskj.cn

Lua ............ 10
来源：http://xc.wgjwhj.cn

Perl ........... 10
来源：http://bw.shtwfgs.cn

Scala .......... 10
来源：http://jm.huanxung.cn

------------------------------------
来源：http://vz.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://kv.haigaiapp.cn

按章节统计：
来源：http://dw.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xy.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qd.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dw.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jb.chemitech.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ec.szxytkj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://or.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qq.szxytkj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qd.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://td.gzmigu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://hy.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wx.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dq.gzmigu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ip.shxzskj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bx.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eb.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xp.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://pl.hnjuh.cn

R Bash 专题                             80
来源：http://oi.shxzukj.cn

S C / C++ 专题                          60
来源：http://rt.yuexingan06.cn

T 其他语言补充                          60
来源：http://rw.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://bl.shtwfgs.cn

------------------------------------
来源：http://cr.hahajie.cn

合计                                  2106 条
来源：http://yn.nszjky.cn

--------------------------------------------------------------------------------
来源：http://bj.shxzskj.cn

使用提醒
来源：http://ul.9csxet.cn

--------------------------------------------------------------------------------
来源：http://jl.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jg.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jc.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qe.huixiangedu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mj.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fb.szxytkj.cn

—— 文件结束 ——
来源：http://xa.nicolike.cn

================================================================================
来源：http://cu.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://vj.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://jf.nicolike.cn

================================================================================
来源：http://sb.nszjky.cn

【收录内容】
来源：http://zs.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vo.bookmarksfly.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://sc.gzmigu.cn

SQL · Bash · C · C++
来源：http://vd.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hq.jianghongdianzi.cn

【使用说明】
来源：http://dc.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vg.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mq.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://cq.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tk.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://be.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://th.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://sn.huixinmuqiang.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yk.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ez.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wu.huixinmuqiang.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wv.muxihuayi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ll.shxzskj.cn

【文件统计】
来源：http://bq.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nf.asd995.cn

--------------------------------------------------------------------------------
来源：http://cf.szxytkj.cn

目  录
来源：http://wh.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://nz.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mv.colortex.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yf.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://pw.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://fi.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sg.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hw.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://pb.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ub.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fl.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jx.shxzskj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://js.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xa.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jh.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ge.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://es.bookmarksfly.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://jv.yuexingan06.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rq.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://so.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zo.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qj.huixiangedu.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://va.wgjwhj.cn

================================================================================
来源：http://ax.haigaiapp.cn

A. 基础语法与类型
来源：http://po.bookmarksfly.cn

================================================================================
来源：http://si.bjjhwx.cn

[A01] Hello World
来源：http://on.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://fr.shxzskj.cn

PHP:  echo "Hello, World!";
来源：http://lo.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://ob.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ey.huanxung.cn

Java: System.out.println("Hello, World!");
来源：http://vl.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://lq.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://hs.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ae.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://zr.wgjwhj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://le.newstarts.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sn.colortex.cn

JS:   let name = "Alex"; const age = 20;
来源：http://re.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qz.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://cq.haigaiapp.cn

Go:   name := "Alex"; age := 20
来源：http://gy.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://ol.shxzskj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ps.bjjhwx.cn

[A03] 常量定义
来源：http://fr.hahajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lw.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://ui.jianghongdianzi.cn

JS:   const PI = 3.14159;
来源：http://rg.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://ke.gzmigu.cn

Java: static final double PI = 3.14159;
来源：http://nw.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://wo.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://qv.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://uz.panjiajie.cn

[A04] 判断变量类型
来源：http://rv.haigaiapp.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://go.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pf.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mq.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://zq.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pf.szsharing.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ka.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hm.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://uj.shxzukj.cn

[A05] 整数除法与取模
来源：http://vb.asd995.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cv.haigaiapp.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://by.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bk.chemitech.net.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jw.asd995.cn

Java: 7 / 2; 7 % 2
来源：http://tp.521024.cn

Go:   7 / 2; 7 % 2
来源：http://kh.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://zg.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://gf.hahajie.cn

[A06] 字符串转数字
来源：http://cn.9csxet.cn

Py:   int("42"); float("3.14")
来源：http://tp.521024.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://iy.jctech888.com.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://zw.bookmarksfly.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ki.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wf.jctech888.com.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xh.wgjwhj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wp.bjjhwx.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://yn.521024.cn

[A07] 数字转字符串
来源：http://sy.wgjwhj.cn

Py:   str(42)
来源：http://lk.jianghongdianzi.cn

PHP:  (string) 42; strval(42)
来源：http://am.colortex.cn

JS:   String(42); (42).toString()
来源：http://yr.asd995.cn

TS:   String(42)
来源：http://tc.gzmigu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ql.jianghongdianzi.cn

Go:   strconv.Itoa(42)
来源：http://ez.hnjuh.cn

Ruby: 42.to_s
来源：http://aq.szsharing.cn

C#:   42.ToString()
来源：http://sb.huanxung.cn

[A08] 取整与四舍五入
来源：http://cx.nszjky.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://nb.haigaiapp.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ai.bookmarksfly.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://pz.newstarts.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://jn.yuexingan06.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lc.yuexingan06.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://bb.hahajie.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://ge.yuexingan06.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mn.yuntaijiaju.cn

[A09] 绝对值与最大最小值
来源：http://pd.yuntaijiaju.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tc.nszjky.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://dj.chemitech.net.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jg.yuexingan06.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nu.521024.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wa.nszjky.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wk.colortex.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://po.huixiangedu.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://zj.yuexingan06.cn


<!-- 参考信息 -->