代发 wailian999

[U55] PHP：match 表达式
来源：http://ra.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ve.wgjwhj.cn

[U56] PHP：命名参数
来源：http://cq.newstarts.cn

f(a: 1, b: 2)
来源：http://zs.nicolike.cn

[U57] PHP：字符串插值
来源：http://nn.muxihuayi.cn

"值: {$a}"
来源：http://ap.muxihuayi.cn

[U58] PHP：数组三件套
来源：http://jy.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://eg.hahajie.cn

[U59] PHP：自定义排序
来源：http://to.hnjuh.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://or.asd995.cn

[U60] PHP：JSON 编解码
来源：http://tw.szxytkj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://pn.asd995.cn

[U61] PHP：正则
来源：http://ai.shxzukj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lo.hnjuh.cn

[U62] PHP：日期对象
来源：http://mf.9csxet.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lp.szxytkj.cn

[U63] PHP：文件读写
来源：http://wk.gzmigu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://et.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://yr.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://xj.nicolike.cn

[U65] PHP：会话
来源：http://cv.yuexingan06.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xh.chemitech.net.cn

[U66] PHP：设置 Cookie
来源：http://ec.nszjky.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qt.newstarts.cn

[U67] PHP：处理文件上传
来源：http://ul.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sn.newstarts.cn

[U68] PHP：PDO 连接
来源：http://dc.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vc.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://vy.panjiajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ys.gzmigu.cn

[U70] PHP：PDO 事务
来源：http://mz.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://il.nszjky.cn

[U71] PHP：抛出异常
来源：http://mz.muxihuayi.cn

throw new RuntimeException("失败", 500);
来源：http://rm.521024.cn

[U72] PHP：写错误日志
来源：http://hw.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://ti.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://ci.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://bw.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://dy.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://ji.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://me.asd995.cn

composer require psr/container
来源：http://iz.shtwfgs.cn

[U76] PHP：简单路由
来源：http://hr.hahajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fx.huanxung.cn

[U77] PHP：模板渲染
来源：http://jx.yuntaijiaju.cn

composer require twig/twig
来源：http://mj.shxzskj.cn

[U78] PHP：单元测试
来源：http://li.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://cq.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://ii.muxihuayi.cn

composer require --dev phpstan/phpstan
来源：http://cl.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://wo.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ie.chemitech.net.cn

[U81] JS：初始化项目
来源：http://ad.jctech888.com.cn

npm init -y;  npm i express
来源：http://eq.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://vw.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xv.szxytkj.cn

[U83] JS：ES Module 导入导出
来源：http://sn.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vm.huixinmuqiang.cn

[U84] JS：CommonJS 写法
来源：http://fi.jctech888.com.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yr.shtwfgs.cn

[U85] JS：可选链
来源：http://uu.szxytkj.cn

a?.b?.c
来源：http://lf.newstarts.cn

[U86] JS：空值合并
来源：http://jc.huixiangedu.cn

a ?? b
来源：http://iq.yuntaijiaju.cn

[U87] JS：解构默认值
来源：http://qw.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://zd.asd995.cn

[U88] JS：对象展开合并
来源：http://od.colortex.cn

{ ...a, ...b }
来源：http://qd.hahajie.cn

[U89] JS：数组去重
来源：http://wj.nicolike.cn

[...new Set(arr)]
来源：http://xv.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://db.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://lp.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://rq.wgjwhj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ue.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://es.hnjuh.cn

structuredClone(obj)
来源：http://lj.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ov.shxzskj.cn

`共 ${n} 条`
来源：http://eb.wgjwhj.cn

[U94] JS：箭头函数
来源：http://ol.huixinmuqiang.cn

const double = x => x * 2;
来源：http://ku.hahajie.cn

[U95] JS：Promise 包装
来源：http://wv.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://sb.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://yb.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pk.hnjuh.cn

[U97] JS：并发请求
来源：http://qz.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kt.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://vc.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sw.huixiangedu.cn

[U99] JS：事件监听
来源：http://ga.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://ag.huanxung.cn

[U100] JS：DOM 查询
来源：http://ul.hnjuh.cn

document.querySelector(".item")
来源：http://wv.haigaiapp.cn

[U101] JS：classList 操作
来源：http://gf.gzmigu.cn

el.classList.toggle("active")
来源：http://nz.newstarts.cn

[U102] JS：本地存储
来源：http://jk.panjiajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ti.chemitech.net.cn

[U103] JS：定时器
来源：http://ff.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hj.bookmarksfly.cn

[U104] JS：防抖
来源：http://zx.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kf.jianghongdianzi.cn

[U105] JS：节流
来源：http://fh.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ro.haigaiapp.cn

[U106] JS：日期格式化
来源：http://dx.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ql.nszjky.cn

[U107] JS：数字千分位
来源：http://pm.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gw.jctech888.com.cn

[U108] JS：随机整数
来源：http://ka.nszjky.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tw.hahajie.cn

[U109] JS：数组分组
来源：http://oh.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://tp.jianghongdianzi.cn

[U110] JS：数组分块
来源：http://yi.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wz.szsharing.cn

[U111] JS：对象转 Map
来源：http://qv.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://oc.colortex.cn

[U112] JS：字符串补位
来源：http://bo.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://zg.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://gg.shxzskj.cn

s.replaceAll("a", "b")
来源：http://ao.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://ti.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xw.jctech888.com.cn

[U115] JS：生成 UUID
来源：http://lt.szxytkj.cn

crypto.randomUUID()
来源：http://br.9csxet.cn

[U116] JS：类型检查（JSDoc）
来源：http://dp.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://ds.gzmigu.cn

[U117] JS：单元测试
来源：http://gv.521024.cn

npm i -D vitest;  npx vitest
来源：http://dm.panjiajie.cn

[U118] JS：开发服务器
来源：http://of.panjiajie.cn

npm i -D vite;  npx vite
来源：http://ss.jianghongdianzi.cn

[U119] JS：生产构建
来源：http://bb.jctech888.com.cn

npx vite build
来源：http://op.haigaiapp.cn

[U120] JS：读取环境变量（Vite）
来源：http://md.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://vz.szxytkj.cn

================================================================================
来源：http://rn.wgjwhj.cn

统计汇总
来源：http://tf.521024.cn

================================================================================
来源：http://tz.huixiangedu.cn

按语言统计（条）：
来源：http://tj.jctech888.com.cn

Python ......... 252
来源：http://ho.521024.cn

PHP ............ 252
来源：http://qm.wgjwhj.cn

JavaScript ..... 252
来源：http://am.haigaiapp.cn

TypeScript ..... 212
来源：http://um.huixiangedu.cn

Java ........... 212
来源：http://cz.nicolike.cn

Go ............. 212
来源：http://xy.bookmarksfly.cn

Ruby ........... 212
来源：http://dz.shtwfgs.cn

C# ............. 212
来源：http://bu.hahajie.cn

C .............. 30
来源：http://xh.muxihuayi.cn

C++ ............ 30
来源：http://mo.panjiajie.cn

SQL ............ 90
来源：http://bh.521024.cn

Bash ........... 80
来源：http://hy.huixiangedu.cn

Kotlin ......... 15
来源：http://xn.bjjhwx.cn

Swift .......... 15
来源：http://gk.yuntaijiaju.cn

Lua ............ 10
来源：http://dk.shxzukj.cn

Perl ........... 10
来源：http://zg.nicolike.cn

Scala .......... 10
来源：http://ge.nicolike.cn

------------------------------------
来源：http://og.huixinmuqiang.cn

合计 ........... 2106 条
来源：http://fy.huixiangedu.cn

按章节统计：
来源：http://ia.9csxet.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dg.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://oe.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rj.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://qm.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wp.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://as.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ei.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oq.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rn.huixinmuqiang.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wh.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cz.muxihuayi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nt.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rx.szxytkj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://oe.bookmarksfly.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://kz.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qc.9csxet.cn

Q SQL 专题                              90
来源：http://aq.yuexingan06.cn

R Bash 专题                             80
来源：http://jj.chemitech.net.cn

S C / C++ 专题                          60
来源：http://lt.nicolike.cn

T 其他语言补充                          60
来源：http://bg.gzmigu.cn

U 高频实用片段                         120
来源：http://vk.huixiangedu.cn

------------------------------------
来源：http://nb.shxzukj.cn

合计                                  2106 条
来源：http://jw.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://wq.nszjky.cn

使用提醒
来源：http://bg.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://mx.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lu.szxytkj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://yp.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hm.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cd.nicolike.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bz.huixinmuqiang.cn

—— 文件结束 ——
来源：http://hb.huanxung.cn

================================================================================
来源：http://rj.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://kt.asd995.cn

Common Programming Examples Cheat Book
来源：http://cd.asd995.cn

================================================================================
来源：http://zs.521024.cn

【收录内容】
来源：http://dd.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vq.nszjky.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xs.szsharing.cn

SQL · Bash · C · C++
来源：http://le.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ht.yuexingan06.cn

【使用说明】
来源：http://qu.newstarts.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rf.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ux.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iu.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://bo.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://tr.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://au.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yu.9csxet.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ak.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fy.panjiajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nl.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jj.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://yd.asd995.cn

【文件统计】
来源：http://ym.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ni.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://la.bjjhwx.cn

目  录
来源：http://mu.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ea.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jy.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ht.yuntaijiaju.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kt.9csxet.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wv.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://iq.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://iy.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://iu.szsharing.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wv.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mv.nszjky.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ey.colortex.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ew.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mb.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eh.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xl.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ds.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://so.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://hz.panjiajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ah.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ra.asd995.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cg.muxihuayi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wo.jctech888.com.cn

================================================================================
来源：http://bu.hahajie.cn

A. 基础语法与类型
来源：http://qp.nicolike.cn

================================================================================
来源：http://oc.colortex.cn

[A01] Hello World
来源：http://wk.lnxyls.cn

Py:   print("Hello, World!")
来源：http://lb.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://uq.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://az.hahajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mt.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://in.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://kx.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://wt.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sv.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://av.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ll.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fa.521024.cn

JS:   let name = "Alex"; const age = 20;
来源：http://km.yuexingan06.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fv.colortex.cn

Java: String name = "Alex"; int age = 20;
来源：http://tn.huixiangedu.cn

Go:   name := "Alex"; age := 20
来源：http://jm.yuntaijiaju.cn

Ruby: name = "Alex"; age = 20
来源：http://fq.nicolike.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ac.huanxung.cn

[A03] 常量定义
来源：http://sl.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://px.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://ca.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://et.huanxung.cn

TS:   const PI: number = 3.14159;
来源：http://ev.newstarts.cn

Java: static final double PI = 3.14159;
来源：http://xn.lnxyls.cn

Go:   const PI = 3.14159
来源：http://do.newstarts.cn

Ruby: PI = 3.14159
来源：http://xj.wgjwhj.cn

C#:   const double PI = 3.14159;
来源：http://xi.bookmarksfly.cn

[A04] 判断变量类型
来源：http://kf.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ef.nszjky.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://nw.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qj.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://ye.shtwfgs.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://lk.shtwfgs.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bm.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ms.shxzukj.cn

C#:   x.GetType().Name; x is int
来源：http://ih.szxytkj.cn

[A05] 整数除法与取模
来源：http://kf.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hn.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gm.shtwfgs.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://xj.huanxung.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aa.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://xp.yuntaijiaju.cn

Go:   7 / 2; 7 % 2
来源：http://vp.bookmarksfly.cn

Ruby: 7 / 2; 7 % 2
来源：http://dx.colortex.cn

C#:   7 / 2; 7 % 2
来源：http://ra.nszjky.cn

[A06] 字符串转数字
来源：http://uj.shtwfgs.cn

Py:   int("42"); float("3.14")
来源：http://rj.shtwfgs.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://td.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gv.yuexingan06.cn

TS:   parseInt("42", 10); Number("42")
来源：http://kf.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://uy.gzmigu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zy.panjiajie.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bq.lnxyls.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wh.gzmigu.cn

[A07] 数字转字符串
来源：http://im.chemitech.net.cn

Py:   str(42)
来源：http://ia.yuexingan06.cn

PHP:  (string) 42; strval(42)
来源：http://lz.huanxung.cn

JS:   String(42); (42).toString()
来源：http://yh.bookmarksfly.cn

TS:   String(42)
来源：http://hk.chemitech.net.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://cd.chemitech.net.cn

Go:   strconv.Itoa(42)
来源：http://rt.hahajie.cn


<!-- 参考信息 -->