代发 wailian999

[U55] PHP：match 表达式
来源：http://nr.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wt.colortex.cn

[U56] PHP：命名参数
来源：http://te.huixinmuqiang.cn

f(a: 1, b: 2)
来源：http://sl.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://mw.shxzskj.cn

"值: {$a}"
来源：http://nv.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://au.bjjhwx.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yz.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://rt.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sl.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://fs.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lb.shtwfgs.cn

[U61] PHP：正则
来源：http://tz.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ck.yuexingan06.cn

[U62] PHP：日期对象
来源：http://ya.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jc.nicolike.cn

[U63] PHP：文件读写
来源：http://mg.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://on.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://lm.haigaiapp.cn

glob("dir/*.php");  scandir("dir");
来源：http://rl.521024.cn

[U65] PHP：会话
来源：http://eg.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rb.colortex.cn

[U66] PHP：设置 Cookie
来源：http://go.shxzukj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ku.yuntaijiaju.cn

[U67] PHP：处理文件上传
来源：http://fr.asd995.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ep.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://uo.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qj.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://dq.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sj.szsharing.cn

[U70] PHP：PDO 事务
来源：http://lx.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ge.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://wb.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://ub.lnxyls.cn

[U72] PHP：写错误日志
来源：http://ur.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://py.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://bn.colortex.cn

parse_ini_file("config.ini", true)
来源：http://rw.nszjky.cn

[U74] PHP：读取环境变量
来源：http://sr.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://yw.nszjky.cn

[U75] PHP：依赖注入
来源：http://xi.huixiangedu.cn

composer require psr/container
来源：http://bq.huanxung.cn

[U76] PHP：简单路由
来源：http://iq.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://su.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://xp.chemitech.net.cn

composer require twig/twig
来源：http://re.asd995.cn

[U78] PHP：单元测试
来源：http://og.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://oz.huanxung.cn

[U79] PHP：静态分析
来源：http://wh.asd995.cn

composer require --dev phpstan/phpstan
来源：http://sc.wgjwhj.cn

[U80] PHP：代码规范修复
来源：http://fc.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qa.asd995.cn

[U81] JS：初始化项目
来源：http://id.shtwfgs.cn

npm init -y;  npm i express
来源：http://sz.9csxet.cn

[U82] JS：package.json 脚本
来源：http://oo.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uo.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://jm.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://nt.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://db.huixiangedu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ho.nicolike.cn

[U85] JS：可选链
来源：http://tc.newstarts.cn

a?.b?.c
来源：http://bf.panjiajie.cn

[U86] JS：空值合并
来源：http://sy.yuntaijiaju.cn

a ?? b
来源：http://st.9csxet.cn

[U87] JS：解构默认值
来源：http://mz.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://ol.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://do.9csxet.cn

{ ...a, ...b }
来源：http://qr.muxihuayi.cn

[U89] JS：数组去重
来源：http://fc.hnjuh.cn

[...new Set(arr)]
来源：http://xl.hnjuh.cn

[U90] JS：数字数组排序
来源：http://ng.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://ih.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://cp.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wp.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://bp.gzmigu.cn

structuredClone(obj)
来源：http://ke.shxzskj.cn

[U93] JS：模板字符串
来源：http://vy.jianghongdianzi.cn

`共 ${n} 条`
来源：http://ld.shxzskj.cn

[U94] JS：箭头函数
来源：http://rh.nicolike.cn

const double = x => x * 2;
来源：http://ia.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ys.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://dg.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://tz.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gu.panjiajie.cn

[U97] JS：并发请求
来源：http://hd.colortex.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tm.newstarts.cn

[U98] JS：fetch 带 JSON
来源：http://sw.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ep.jctech888.com.cn

[U99] JS：事件监听
来源：http://oh.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://lh.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://ba.szxytkj.cn

document.querySelector(".item")
来源：http://ya.newstarts.cn

[U101] JS：classList 操作
来源：http://lo.asd995.cn

el.classList.toggle("active")
来源：http://sh.newstarts.cn

[U102] JS：本地存储
来源：http://oo.bookmarksfly.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wn.nszjky.cn

[U103] JS：定时器
来源：http://qx.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ee.huixiangedu.cn

[U104] JS：防抖
来源：http://pj.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hl.huixinmuqiang.cn

[U105] JS：节流
来源：http://tw.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rc.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://sd.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oi.nicolike.cn

[U107] JS：数字千分位
来源：http://jv.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xh.huanxung.cn

[U108] JS：随机整数
来源：http://ig.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lt.shxzskj.cn

[U109] JS：数组分组
来源：http://cz.nszjky.cn

Object.groupBy(arr, x => x.type)
来源：http://jv.szxytkj.cn

[U110] JS：数组分块
来源：http://ic.jctech888.com.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://pr.hahajie.cn

[U111] JS：对象转 Map
来源：http://rm.newstarts.cn

new Map(Object.entries(obj))
来源：http://dx.521024.cn

[U112] JS：字符串补位
来源：http://xe.shtwfgs.cn

"7".padStart(3, "0")
来源：http://sq.shxzukj.cn

[U113] JS：正则替换全部
来源：http://za.newstarts.cn

s.replaceAll("a", "b")
来源：http://nj.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://ek.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lg.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://ne.huanxung.cn

crypto.randomUUID()
来源：http://un.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://og.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://gu.nicolike.cn

[U117] JS：单元测试
来源：http://rx.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://wa.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://bl.newstarts.cn

npm i -D vite;  npx vite
来源：http://ld.huixinmuqiang.cn

[U119] JS：生产构建
来源：http://rh.huixinmuqiang.cn

npx vite build
来源：http://yb.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://hd.huixiangedu.cn

import.meta.env.VITE_API_URL
来源：http://jo.huanxung.cn

================================================================================
来源：http://bi.shtwfgs.cn

统计汇总
来源：http://gh.huixiangedu.cn

================================================================================
来源：http://mp.shtwfgs.cn

按语言统计（条）：
来源：http://sx.yuexingan06.cn

Python ......... 252
来源：http://bo.newstarts.cn

PHP ............ 252
来源：http://dq.haigaiapp.cn

JavaScript ..... 252
来源：http://xs.bjjhwx.cn

TypeScript ..... 212
来源：http://iw.nszjky.cn

Java ........... 212
来源：http://it.wgjwhj.cn

Go ............. 212
来源：http://lb.huixinmuqiang.cn

Ruby ........... 212
来源：http://wy.colortex.cn

C# ............. 212
来源：http://iz.szsharing.cn

C .............. 30
来源：http://kc.bjjhwx.cn

C++ ............ 30
来源：http://qm.hnjuh.cn

SQL ............ 90
来源：http://lr.haigaiapp.cn

Bash ........... 80
来源：http://xd.bookmarksfly.cn

Kotlin ......... 15
来源：http://xk.huixiangedu.cn

Swift .......... 15
来源：http://nw.lnxyls.cn

Lua ............ 10
来源：http://xg.colortex.cn

Perl ........... 10
来源：http://ff.shtwfgs.cn

Scala .......... 10
来源：http://qp.haigaiapp.cn

------------------------------------
来源：http://wt.yuexingan06.cn

合计 ........... 2106 条
来源：http://kp.nszjky.cn

按章节统计：
来源：http://tw.jianghongdianzi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://nw.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gm.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mu.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ec.colortex.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ad.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pw.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tl.huanxung.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ep.bjjhwx.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lq.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bs.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bn.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wv.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ov.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hj.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bh.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jn.yuntaijiaju.cn

Q SQL 专题                              90
来源：http://rz.shtwfgs.cn

R Bash 专题                             80
来源：http://bi.shxzukj.cn

S C / C++ 专题                          60
来源：http://zc.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://wo.yuexingan06.cn

U 高频实用片段                         120
来源：http://ms.huixiangedu.cn

------------------------------------
来源：http://uh.szsharing.cn

合计                                  2106 条
来源：http://sw.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://cx.lnxyls.cn

使用提醒
来源：http://mh.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://jb.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://py.asd995.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://en.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sq.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://to.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://eo.hahajie.cn

—— 文件结束 ——
来源：http://vk.shxzskj.cn

================================================================================
来源：http://mg.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://pb.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://dm.nicolike.cn

================================================================================
来源：http://fr.szsharing.cn

【收录内容】
来源：http://ak.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rs.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ni.huanxung.cn

SQL · Bash · C · C++
来源：http://uu.shxzukj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bf.panjiajie.cn

【使用说明】
来源：http://jh.haigaiapp.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qi.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://sf.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wd.hahajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yw.lnxyls.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cb.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://st.chemitech.net.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fx.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jx.lnxyls.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mq.yuexingan06.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://so.yuexingan06.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cc.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://pt.bjjhwx.cn

【文件统计】
来源：http://sl.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gz.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://kf.colortex.cn

目  录
来源：http://uk.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://gu.szsharing.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tu.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://gv.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vr.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://je.gzmigu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sn.jianghongdianzi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qw.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fd.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://su.colortex.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tf.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ji.gzmigu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tc.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sj.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wu.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://by.bookmarksfly.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lk.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ud.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ah.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://nb.shxzskj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://gg.hahajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yp.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bi.hahajie.cn

================================================================================
来源：http://cs.hahajie.cn

A. 基础语法与类型
来源：http://nv.szsharing.cn

================================================================================
来源：http://ee.chemitech.net.cn

[A01] Hello World
来源：http://ty.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://la.shxzukj.cn

PHP:  echo "Hello, World!";
来源：http://eh.haigaiapp.cn

JS:   console.log("Hello, World!");
来源：http://bl.szsharing.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rc.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://lw.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://gs.szxytkj.cn

Ruby: puts "Hello, World!"
来源：http://uw.szsharing.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://gm.hnjuh.cn

[A02] 变量声明与赋值
来源：http://dk.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bt.szxytkj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ls.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ui.yuntaijiaju.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bl.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://fi.muxihuayi.cn

Go:   name := "Alex"; age := 20
来源：http://hp.bookmarksfly.cn

Ruby: name = "Alex"; age = 20
来源：http://kh.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jc.huixiangedu.cn

[A03] 常量定义
来源：http://ej.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fa.colortex.cn

PHP:  const PI = 3.14159;
来源：http://ak.szxytkj.cn

JS:   const PI = 3.14159;
来源：http://qo.chemitech.net.cn

TS:   const PI: number = 3.14159;
来源：http://iq.hnjuh.cn

Java: static final double PI = 3.14159;
来源：http://yf.panjiajie.cn

Go:   const PI = 3.14159
来源：http://gr.huixiangedu.cn

Ruby: PI = 3.14159
来源：http://fa.jianghongdianzi.cn

C#:   const double PI = 3.14159;
来源：http://xl.bjjhwx.cn

[A04] 判断变量类型
来源：http://mr.bjjhwx.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dm.bookmarksfly.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://sg.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tg.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://ch.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://yt.huanxung.cn

Go:   reflect.TypeOf(x).Name()
来源：http://yl.9csxet.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://pm.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://cu.shxzukj.cn

[A05] 整数除法与取模
来源：http://zn.yuexingan06.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xu.panjiajie.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mw.wgjwhj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uz.yuntaijiaju.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ay.yuexingan06.cn

Java: 7 / 2; 7 % 2
来源：http://ld.wgjwhj.cn

Go:   7 / 2; 7 % 2
来源：http://it.panjiajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://zv.muxihuayi.cn

C#:   7 / 2; 7 % 2
来源：http://qh.9csxet.cn

[A06] 字符串转数字
来源：http://ca.colortex.cn

Py:   int("42"); float("3.14")
来源：http://ii.szsharing.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xu.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ln.lnxyls.cn

TS:   parseInt("42", 10); Number("42")
来源：http://pi.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hr.shxzskj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wh.jianghongdianzi.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wk.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oe.521024.cn

[A07] 数字转字符串
来源：http://kt.jctech888.com.cn

Py:   str(42)
来源：http://lm.9csxet.cn

PHP:  (string) 42; strval(42)
来源：http://al.gzmigu.cn

JS:   String(42); (42).toString()
来源：http://qs.huanxung.cn

TS:   String(42)
来源：http://qw.huixiangedu.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://ke.szsharing.cn

Go:   strconv.Itoa(42)
来源：http://rt.huixinmuqiang.cn


<!-- 参考信息 -->