代发 wailian999

[U61] PHP：正则
来源：http://mj.yuexingan06.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ks.shxzskj.cn

[U62] PHP：日期对象
来源：http://yf.newstarts.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wj.asd995.cn

[U63] PHP：文件读写
来源：http://lj.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://kq.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://yg.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://in.shxzukj.cn

[U65] PHP：会话
来源：http://is.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mq.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://tt.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jl.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://yz.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lc.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://dk.jctech888.com.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ej.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ir.521024.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jf.haigaiapp.cn

[U70] PHP：PDO 事务
来源：http://th.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ix.9csxet.cn

[U71] PHP：抛出异常
来源：http://zk.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://jh.muxihuayi.cn

[U72] PHP：写错误日志
来源：http://tz.wgjwhj.cn

error_log("失败: " . $e->getMessage());
来源：http://my.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://rp.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://lp.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://ub.shtwfgs.cn

getenv("APP_ENV") ?: "production"
来源：http://wh.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ja.chemitech.net.cn

composer require psr/container
来源：http://qc.hahajie.cn

[U76] PHP：简单路由
来源：http://xf.shxzukj.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ke.nszjky.cn

[U77] PHP：模板渲染
来源：http://aw.521024.cn

composer require twig/twig
来源：http://er.newstarts.cn

[U78] PHP：单元测试
来源：http://bv.521024.cn

composer require --dev phpunit/phpunit
来源：http://tm.asd995.cn

[U79] PHP：静态分析
来源：http://pr.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://gg.asd995.cn

[U80] PHP：代码规范修复
来源：http://sy.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://my.bjjhwx.cn

[U81] JS：初始化项目
来源：http://cv.szsharing.cn

npm init -y;  npm i express
来源：http://hq.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://ds.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vm.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://th.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vl.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://vs.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://zl.muxihuayi.cn

[U85] JS：可选链
来源：http://np.nszjky.cn

a?.b?.c
来源：http://zj.jctech888.com.cn

[U86] JS：空值合并
来源：http://lh.bookmarksfly.cn

a ?? b
来源：http://nw.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://es.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://ky.szxytkj.cn

[U88] JS：对象展开合并
来源：http://lf.muxihuayi.cn

{ ...a, ...b }
来源：http://vc.jctech888.com.cn

[U89] JS：数组去重
来源：http://us.jctech888.com.cn

[...new Set(arr)]
来源：http://rc.colortex.cn

[U90] JS：数字数组排序
来源：http://sw.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://wz.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://qo.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hn.bjjhwx.cn

[U92] JS：深拷贝
来源：http://fi.newstarts.cn

structuredClone(obj)
来源：http://lt.szsharing.cn

[U93] JS：模板字符串
来源：http://za.yuexingan06.cn

`共 ${n} 条`
来源：http://mt.szsharing.cn

[U94] JS：箭头函数
来源：http://zc.huixiangedu.cn

const double = x => x * 2;
来源：http://sk.hahajie.cn

[U95] JS：Promise 包装
来源：http://pp.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://bc.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://uf.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wi.szsharing.cn

[U97] JS：并发请求
来源：http://xz.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kp.szsharing.cn

[U98] JS：fetch 带 JSON
来源：http://uz.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qu.muxihuayi.cn

[U99] JS：事件监听
来源：http://ie.asd995.cn

el.addEventListener("click", e => {})
来源：http://nt.shxzskj.cn

[U100] JS：DOM 查询
来源：http://xk.muxihuayi.cn

document.querySelector(".item")
来源：http://mm.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://ex.colortex.cn

el.classList.toggle("active")
来源：http://kt.bjjhwx.cn

[U102] JS：本地存储
来源：http://da.szxytkj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://xe.hnjuh.cn

[U103] JS：定时器
来源：http://oi.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xq.asd995.cn

[U104] JS：防抖
来源：http://jn.jianghongdianzi.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mv.shxzukj.cn

[U105] JS：节流
来源：http://ew.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ws.yuexingan06.cn

[U106] JS：日期格式化
来源：http://pt.panjiajie.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vn.colortex.cn

[U107] JS：数字千分位
来源：http://sb.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mq.yuexingan06.cn

[U108] JS：随机整数
来源：http://gv.hnjuh.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://km.huanxung.cn

[U109] JS：数组分组
来源：http://mj.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://um.huanxung.cn

[U110] JS：数组分块
来源：http://wy.lnxyls.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vi.panjiajie.cn

[U111] JS：对象转 Map
来源：http://at.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://wb.jianghongdianzi.cn

[U112] JS：字符串补位
来源：http://hy.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://qt.huanxung.cn

[U113] JS：正则替换全部
来源：http://ud.lnxyls.cn

s.replaceAll("a", "b")
来源：http://sf.huanxung.cn

[U114] JS：JSON 深比较
来源：http://xr.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rj.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://ix.bookmarksfly.cn

crypto.randomUUID()
来源：http://jn.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://lo.hahajie.cn

/** @param {string} name */ function f(name) {}
来源：http://kz.panjiajie.cn

[U117] JS：单元测试
来源：http://yt.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://nv.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://gv.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://ar.nicolike.cn

[U119] JS：生产构建
来源：http://eg.asd995.cn

npx vite build
来源：http://wg.muxihuayi.cn

[U120] JS：读取环境变量（Vite）
来源：http://tv.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://ob.muxihuayi.cn

================================================================================
来源：http://wd.yuntaijiaju.cn

统计汇总
来源：http://ge.bjjhwx.cn

================================================================================
来源：http://np.nicolike.cn

按语言统计（条）：
来源：http://us.shxzukj.cn

Python ......... 252
来源：http://ka.chemitech.net.cn

PHP ............ 252
来源：http://bx.huixiangedu.cn

JavaScript ..... 252
来源：http://ph.huixinmuqiang.cn

TypeScript ..... 212
来源：http://tw.szxytkj.cn

Java ........... 212
来源：http://cr.huanxung.cn

Go ............. 212
来源：http://sv.colortex.cn

Ruby ........... 212
来源：http://jy.szsharing.cn

C# ............. 212
来源：http://zn.panjiajie.cn

C .............. 30
来源：http://pl.huixinmuqiang.cn

C++ ............ 30
来源：http://wb.bjjhwx.cn

SQL ............ 90
来源：http://gp.chemitech.net.cn

Bash ........... 80
来源：http://bf.haigaiapp.cn

Kotlin ......... 15
来源：http://hg.haigaiapp.cn

Swift .......... 15
来源：http://vg.huixiangedu.cn

Lua ............ 10
来源：http://hj.yuexingan06.cn

Perl ........... 10
来源：http://ka.yuexingan06.cn

Scala .......... 10
来源：http://nj.huanxung.cn

------------------------------------
来源：http://qk.newstarts.cn

合计 ........... 2106 条
来源：http://zr.jianghongdianzi.cn

按章节统计：
来源：http://cn.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gu.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://li.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fl.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://so.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ye.hahajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://dw.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mj.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ho.haigaiapp.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jx.haigaiapp.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ev.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xs.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://de.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hh.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mb.chemitech.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jp.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ly.shxzskj.cn

Q SQL 专题                              90
来源：http://ad.jctech888.com.cn

R Bash 专题                             80
来源：http://yy.shxzskj.cn

S C / C++ 专题                          60
来源：http://rc.bookmarksfly.cn

T 其他语言补充                          60
来源：http://pj.hnjuh.cn

U 高频实用片段                         120
来源：http://xi.shtwfgs.cn

------------------------------------
来源：http://qo.huanxung.cn

合计                                  2106 条
来源：http://so.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://vx.panjiajie.cn

使用提醒
来源：http://wt.colortex.cn

--------------------------------------------------------------------------------
来源：http://kc.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nl.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kl.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fq.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zw.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://dk.nszjky.cn

—— 文件结束 ——
来源：http://fp.hnjuh.cn

================================================================================
来源：http://yh.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://di.yuexingan06.cn

Common Programming Examples Cheat Book
来源：http://ch.bookmarksfly.cn

================================================================================
来源：http://sj.hahajie.cn

【收录内容】
来源：http://uc.szsharing.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yt.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hv.gzmigu.cn

SQL · Bash · C · C++
来源：http://kd.colortex.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jb.bookmarksfly.cn

【使用说明】
来源：http://po.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vp.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://df.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wd.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://da.newstarts.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wr.chemitech.net.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kc.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zd.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ia.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bo.bookmarksfly.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kl.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://se.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kj.muxihuayi.cn

【文件统计】
来源：http://ch.wgjwhj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ad.szsharing.cn

--------------------------------------------------------------------------------
来源：http://wn.shtwfgs.cn

目  录
来源：http://tz.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://nt.szxytkj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rz.lnxyls.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ab.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dr.yuexingan06.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ar.chemitech.net.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jc.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uw.hnjuh.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bc.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://aq.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ul.bookmarksfly.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hw.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wm.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://db.bookmarksfly.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://at.huanxung.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ku.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jf.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cx.nicolike.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yx.wgjwhj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ao.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xo.szsharing.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tw.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ig.yuexingan06.cn

================================================================================
来源：http://if.chemitech.net.cn

A. 基础语法与类型
来源：http://qm.chemitech.net.cn

================================================================================
来源：http://ry.panjiajie.cn

[A01] Hello World
来源：http://vn.gzmigu.cn

Py:   print("Hello, World!")
来源：http://wz.asd995.cn

PHP:  echo "Hello, World!";
来源：http://le.asd995.cn

JS:   console.log("Hello, World!");
来源：http://ui.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://td.jctech888.com.cn

Java: System.out.println("Hello, World!");
来源：http://vg.szsharing.cn

Go:   fmt.Println("Hello, World!")
来源：http://bh.asd995.cn

Ruby: puts "Hello, World!"
来源：http://fi.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://zc.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://kj.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gs.panjiajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://nd.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://iv.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gc.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://pw.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://if.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://ww.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nx.yuexingan06.cn

[A03] 常量定义
来源：http://gr.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://op.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://au.panjiajie.cn

JS:   const PI = 3.14159;
来源：http://dc.szxytkj.cn

TS:   const PI: number = 3.14159;
来源：http://cz.huixinmuqiang.cn

Java: static final double PI = 3.14159;
来源：http://qc.hnjuh.cn

Go:   const PI = 3.14159
来源：http://uj.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://pc.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://ye.huixiangedu.cn

[A04] 判断变量类型
来源：http://gv.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fx.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://dq.shxzskj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zf.nszjky.cn

TS:   typeof x; x instanceof Date
来源：http://xf.huanxung.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://se.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://el.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://tk.asd995.cn

C#:   x.GetType().Name; x is int
来源：http://my.colortex.cn

[A05] 整数除法与取模
来源：http://cx.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wb.shxzukj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kh.hnjuh.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yk.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fq.muxihuayi.cn

Java: 7 / 2; 7 % 2
来源：http://fm.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://zh.newstarts.cn

Ruby: 7 / 2; 7 % 2
来源：http://so.9csxet.cn

C#:   7 / 2; 7 % 2
来源：http://hb.shxzukj.cn

[A06] 字符串转数字
来源：http://ld.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://hy.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xq.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gr.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://az.gzmigu.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gs.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://po.9csxet.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://hf.nszjky.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ph.muxihuayi.cn

[A07] 数字转字符串
来源：http://tn.yuexingan06.cn

Py:   str(42)
来源：http://jh.panjiajie.cn

PHP:  (string) 42; strval(42)
来源：http://eq.jctech888.com.cn

JS:   String(42); (42).toString()
来源：http://hg.nszjky.cn

TS:   String(42)
来源：http://dt.nszjky.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://rn.lnxyls.cn

Go:   strconv.Itoa(42)
来源：http://ou.panjiajie.cn

Ruby: 42.to_s
来源：http://cz.panjiajie.cn

C#:   42.ToString()
来源：http://az.hahajie.cn

[A08] 取整与四舍五入
来源：http://dg.huixiangedu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://su.jctech888.com.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kq.jctech888.com.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jv.colortex.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gf.chemitech.net.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fa.haigaiapp.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://qr.szsharing.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://bx.colortex.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yt.gzmigu.cn

[A09] 绝对值与最大最小值
来源：http://od.chemitech.net.cn


<!-- 参考信息 -->