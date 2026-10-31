代发 wailian999

[U61] PHP：正则
来源：http://cq.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aj.colortex.cn

[U62] PHP：日期对象
来源：http://ff.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xc.szsharing.cn

[U63] PHP：文件读写
来源：http://pt.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ah.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://cr.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://ai.lnxyls.cn

[U65] PHP：会话
来源：http://se.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bh.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://wk.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ta.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://vb.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zj.lnxyls.cn

[U68] PHP：PDO 连接
来源：http://xv.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lm.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://ch.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xa.hahajie.cn

[U70] PHP：PDO 事务
来源：http://ri.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qh.gzmigu.cn

[U71] PHP：抛出异常
来源：http://gn.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://el.nszjky.cn

[U72] PHP：写错误日志
来源：http://ho.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://xi.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://fd.asd995.cn

parse_ini_file("config.ini", true)
来源：http://jh.muxihuayi.cn

[U74] PHP：读取环境变量
来源：http://et.bookmarksfly.cn

getenv("APP_ENV") ?: "production"
来源：http://vh.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://kr.9csxet.cn

composer require psr/container
来源：http://sn.jctech888.com.cn

[U76] PHP：简单路由
来源：http://ev.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pl.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://pm.hnjuh.cn

composer require twig/twig
来源：http://eh.szxytkj.cn

[U78] PHP：单元测试
来源：http://vn.colortex.cn

composer require --dev phpunit/phpunit
来源：http://it.shxzskj.cn

[U79] PHP：静态分析
来源：http://lv.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://jp.newstarts.cn

[U80] PHP：代码规范修复
来源：http://sc.lnxyls.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://th.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://xk.shxzskj.cn

npm init -y;  npm i express
来源：http://sv.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://sj.panjiajie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://de.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://cr.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iq.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://ku.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://rt.jctech888.com.cn

[U85] JS：可选链
来源：http://bo.jianghongdianzi.cn

a?.b?.c
来源：http://tm.huixiangedu.cn

[U86] JS：空值合并
来源：http://hv.jctech888.com.cn

a ?? b
来源：http://jz.yuexingan06.cn

[U87] JS：解构默认值
来源：http://ce.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://qs.shxzskj.cn

[U88] JS：对象展开合并
来源：http://ac.panjiajie.cn

{ ...a, ...b }
来源：http://jx.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://jy.jianghongdianzi.cn

[...new Set(arr)]
来源：http://zm.panjiajie.cn

[U90] JS：数字数组排序
来源：http://zc.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://pt.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://gy.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kq.huanxung.cn

[U92] JS：深拷贝
来源：http://uz.bjjhwx.cn

structuredClone(obj)
来源：http://qa.521024.cn

[U93] JS：模板字符串
来源：http://df.asd995.cn

`共 ${n} 条`
来源：http://sy.szsharing.cn

[U94] JS：箭头函数
来源：http://ob.nszjky.cn

const double = x => x * 2;
来源：http://nu.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://dm.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://jl.szsharing.cn

[U96] JS：async/await 与异常
来源：http://cl.gzmigu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://se.colortex.cn

[U97] JS：并发请求
来源：http://mk.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hv.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://ar.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://op.newstarts.cn

[U99] JS：事件监听
来源：http://gz.hahajie.cn

el.addEventListener("click", e => {})
来源：http://vo.yuntaijiaju.cn

[U100] JS：DOM 查询
来源：http://fw.asd995.cn

document.querySelector(".item")
来源：http://jv.wgjwhj.cn

[U101] JS：classList 操作
来源：http://qf.yuexingan06.cn

el.classList.toggle("active")
来源：http://se.521024.cn

[U102] JS：本地存储
来源：http://dj.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dj.newstarts.cn

[U103] JS：定时器
来源：http://mp.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://bw.hnjuh.cn

[U104] JS：防抖
来源：http://bt.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yn.bjjhwx.cn

[U105] JS：节流
来源：http://pg.shxzskj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://sq.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://pb.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qq.shtwfgs.cn

[U107] JS：数字千分位
来源：http://lk.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gb.nszjky.cn

[U108] JS：随机整数
来源：http://rp.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mq.nicolike.cn

[U109] JS：数组分组
来源：http://op.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://fx.shxzskj.cn

[U110] JS：数组分块
来源：http://nv.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dt.gzmigu.cn

[U111] JS：对象转 Map
来源：http://os.hnjuh.cn

new Map(Object.entries(obj))
来源：http://xv.jctech888.com.cn

[U112] JS：字符串补位
来源：http://lj.9csxet.cn

"7".padStart(3, "0")
来源：http://xv.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://mq.szsharing.cn

s.replaceAll("a", "b")
来源：http://gf.shxzskj.cn

[U114] JS：JSON 深比较
来源：http://bi.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://eg.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://ym.newstarts.cn

crypto.randomUUID()
来源：http://xs.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://sb.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://jt.bookmarksfly.cn

[U117] JS：单元测试
来源：http://uk.colortex.cn

npm i -D vitest;  npx vitest
来源：http://jm.nicolike.cn

[U118] JS：开发服务器
来源：http://zi.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://wt.szsharing.cn

[U119] JS：生产构建
来源：http://rx.huixinmuqiang.cn

npx vite build
来源：http://on.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://vt.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://gs.hahajie.cn

================================================================================
来源：http://id.colortex.cn

统计汇总
来源：http://wn.panjiajie.cn

================================================================================
来源：http://ou.panjiajie.cn

按语言统计（条）：
来源：http://ra.jianghongdianzi.cn

Python ......... 252
来源：http://uk.lnxyls.cn

PHP ............ 252
来源：http://fw.jianghongdianzi.cn

JavaScript ..... 252
来源：http://tb.lnxyls.cn

TypeScript ..... 212
来源：http://os.hahajie.cn

Java ........... 212
来源：http://cu.hnjuh.cn

Go ............. 212
来源：http://hl.shxzukj.cn

Ruby ........... 212
来源：http://bw.yuntaijiaju.cn

C# ............. 212
来源：http://es.521024.cn

C .............. 30
来源：http://fx.huixiangedu.cn

C++ ............ 30
来源：http://lg.nicolike.cn

SQL ............ 90
来源：http://wi.asd995.cn

Bash ........... 80
来源：http://vh.jianghongdianzi.cn

Kotlin ......... 15
来源：http://dr.chemitech.net.cn

Swift .......... 15
来源：http://bp.hahajie.cn

Lua ............ 10
来源：http://iy.bookmarksfly.cn

Perl ........... 10
来源：http://kw.lnxyls.cn

Scala .......... 10
来源：http://se.muxihuayi.cn

------------------------------------
来源：http://ka.nicolike.cn

合计 ........... 2106 条
来源：http://qj.bjjhwx.cn

按章节统计：
来源：http://vz.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ed.shxzskj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tm.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zg.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fa.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ee.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xo.huixinmuqiang.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://za.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xi.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xi.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ff.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://gx.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cl.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://di.huixiangedu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ud.hnjuh.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sb.jctech888.com.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yb.hahajie.cn

Q SQL 专题                              90
来源：http://rw.szxytkj.cn

R Bash 专题                             80
来源：http://zy.wgjwhj.cn

S C / C++ 专题                          60
来源：http://aa.521024.cn

T 其他语言补充                          60
来源：http://eb.wgjwhj.cn

U 高频实用片段                         120
来源：http://bl.szxytkj.cn

------------------------------------
来源：http://hc.jctech888.com.cn

合计                                  2106 条
来源：http://wq.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ko.jianghongdianzi.cn

使用提醒
来源：http://gv.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://zu.9csxet.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ia.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://lz.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hc.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wy.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oj.asd995.cn

—— 文件结束 ——
来源：http://tq.shxzskj.cn

================================================================================
来源：http://yj.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://js.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://ug.yuexingan06.cn

================================================================================
来源：http://xd.wgjwhj.cn

【收录内容】
来源：http://zd.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ky.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ie.yuexingan06.cn

SQL · Bash · C · C++
来源：http://yl.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://rh.gzmigu.cn

【使用说明】
来源：http://fa.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bd.haigaiapp.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cp.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hf.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hi.chemitech.net.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ac.shtwfgs.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ir.lnxyls.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qs.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xp.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bc.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://gh.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rj.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ln.wgjwhj.cn

【文件统计】
来源：http://yr.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fg.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ha.newstarts.cn

目  录
来源：http://dk.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://co.521024.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://cp.asd995.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yd.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://lp.521024.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hb.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bn.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vu.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ye.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://il.szxytkj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sm.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pt.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lo.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://fs.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qd.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xm.panjiajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jg.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sk.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yl.chemitech.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ty.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sy.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qi.shxzskj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://pc.jctech888.com.cn

================================================================================
来源：http://ro.shtwfgs.cn

A. 基础语法与类型
来源：http://vr.jctech888.com.cn

================================================================================
来源：http://xk.gzmigu.cn

[A01] Hello World
来源：http://qw.bjjhwx.cn

Py:   print("Hello, World!")
来源：http://hg.521024.cn

PHP:  echo "Hello, World!";
来源：http://ei.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://le.szxytkj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vs.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://sc.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://qx.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://wg.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ru.newstarts.cn

[A02] 变量声明与赋值
来源：http://je.newstarts.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://au.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dt.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://kc.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rt.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://wa.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://so.hahajie.cn

Ruby: name = "Alex"; age = 20
来源：http://hg.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://tl.lnxyls.cn

[A03] 常量定义
来源：http://ke.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ls.nicolike.cn

PHP:  const PI = 3.14159;
来源：http://pb.nszjky.cn

JS:   const PI = 3.14159;
来源：http://rh.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://tm.chemitech.net.cn

Java: static final double PI = 3.14159;
来源：http://xb.hnjuh.cn

Go:   const PI = 3.14159
来源：http://fe.szxytkj.cn

Ruby: PI = 3.14159
来源：http://rw.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://jb.hahajie.cn

[A04] 判断变量类型
来源：http://hk.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ii.asd995.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://hr.nicolike.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tt.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://qd.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zi.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yu.shxzskj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://uv.521024.cn

C#:   x.GetType().Name; x is int
来源：http://wa.szsharing.cn

[A05] 整数除法与取模
来源：http://bb.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ng.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ng.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pd.szsharing.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qu.bjjhwx.cn

Java: 7 / 2; 7 % 2
来源：http://ix.yuexingan06.cn

Go:   7 / 2; 7 % 2
来源：http://bx.huixinmuqiang.cn

Ruby: 7 / 2; 7 % 2
来源：http://ov.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://lv.szsharing.cn

[A06] 字符串转数字
来源：http://yb.huanxung.cn

Py:   int("42"); float("3.14")
来源：http://az.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xv.haigaiapp.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ln.szxytkj.cn

TS:   parseInt("42", 10); Number("42")
来源：http://qr.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ne.huixinmuqiang.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://rf.nicolike.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lp.shxzskj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://ys.lnxyls.cn

[A07] 数字转字符串
来源：http://fj.bjjhwx.cn

Py:   str(42)
来源：http://wo.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://pk.nszjky.cn

JS:   String(42); (42).toString()
来源：http://wh.jianghongdianzi.cn

TS:   String(42)
来源：http://ew.wgjwhj.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://dh.muxihuayi.cn

Go:   strconv.Itoa(42)
来源：http://bc.colortex.cn

Ruby: 42.to_s
来源：http://lk.9csxet.cn

C#:   42.ToString()
来源：http://qs.hnjuh.cn

[A08] 取整与四舍五入
来源：http://kh.bookmarksfly.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sw.colortex.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ay.huixiangedu.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://rt.szsharing.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yg.bookmarksfly.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://jl.bjjhwx.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://au.colortex.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://vk.hahajie.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://yv.shtwfgs.cn

[A09] 绝对值与最大最小值
来源：http://vw.muxihuayi.cn


<!-- 参考信息 -->