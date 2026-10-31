代发 wailian999

[U47] PHP：联合类型
来源：http://co.9csxet.cn

int|string $id
来源：http://jn.shxzskj.cn

[U48] PHP：纯枚举
来源：http://yo.shxzskj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://td.shtwfgs.cn

[U49] PHP：只读属性
来源：http://mq.colortex.cn

public readonly string $name
来源：http://ce.asd995.cn

[U50] PHP：构造器属性提升
来源：http://qe.shtwfgs.cn

public function __construct(private int $id) {}
来源：http://jv.chemitech.net.cn

[U51] PHP：数组解构
来源：http://py.shtwfgs.cn

[$a, $b] = $arr;
来源：http://tw.521024.cn

[U52] PHP：箭头函数
来源：http://oi.chemitech.net.cn

$double = fn($x) => $x * 2;
来源：http://fy.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://yb.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://nl.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://mg.hahajie.cn

$obj?->method()
来源：http://vz.lnxyls.cn

[U55] PHP：match 表达式
来源：http://ju.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vz.wgjwhj.cn

[U56] PHP：命名参数
来源：http://ru.szxytkj.cn

f(a: 1, b: 2)
来源：http://yk.huanxung.cn

[U57] PHP：字符串插值
来源：http://ef.shxzukj.cn

"值: {$a}"
来源：http://pq.panjiajie.cn

[U58] PHP：数组三件套
来源：http://mn.huanxung.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mt.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://yv.521024.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ge.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://zm.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rs.haigaiapp.cn

[U61] PHP：正则
来源：http://kn.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ph.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://sm.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fz.colortex.cn

[U63] PHP：文件读写
来源：http://qx.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mm.asd995.cn

[U64] PHP：目录遍历
来源：http://yb.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://eo.muxihuayi.cn

[U65] PHP：会话
来源：http://hx.wgjwhj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://le.newstarts.cn

[U66] PHP：设置 Cookie
来源：http://ej.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xq.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://jt.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://he.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://wu.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fv.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://zv.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rt.panjiajie.cn

[U70] PHP：PDO 事务
来源：http://il.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eu.shxzukj.cn

[U71] PHP：抛出异常
来源：http://ay.lnxyls.cn

throw new RuntimeException("失败", 500);
来源：http://fr.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://mw.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://wu.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://et.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://fu.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://qf.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://iq.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://yy.bookmarksfly.cn

composer require psr/container
来源：http://ac.asd995.cn

[U76] PHP：简单路由
来源：http://mb.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mi.asd995.cn

[U77] PHP：模板渲染
来源：http://oz.huixinmuqiang.cn

composer require twig/twig
来源：http://io.shtwfgs.cn

[U78] PHP：单元测试
来源：http://wk.shtwfgs.cn

composer require --dev phpunit/phpunit
来源：http://jl.newstarts.cn

[U79] PHP：静态分析
来源：http://xo.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://dt.hnjuh.cn

[U80] PHP：代码规范修复
来源：http://lp.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hf.jianghongdianzi.cn

[U81] JS：初始化项目
来源：http://qq.wgjwhj.cn

npm init -y;  npm i express
来源：http://cs.haigaiapp.cn

[U82] JS：package.json 脚本
来源：http://sx.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ck.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://xv.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://mx.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://kn.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oy.shtwfgs.cn

[U85] JS：可选链
来源：http://wo.nicolike.cn

a?.b?.c
来源：http://aj.jctech888.com.cn

[U86] JS：空值合并
来源：http://we.nszjky.cn

a ?? b
来源：http://sq.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://zq.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://bi.yuexingan06.cn

[U88] JS：对象展开合并
来源：http://do.lnxyls.cn

{ ...a, ...b }
来源：http://ad.wgjwhj.cn

[U89] JS：数组去重
来源：http://ys.bookmarksfly.cn

[...new Set(arr)]
来源：http://fi.colortex.cn

[U90] JS：数字数组排序
来源：http://rg.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://ok.newstarts.cn

[U91] JS：对象键值遍历
来源：http://ub.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xt.lnxyls.cn

[U92] JS：深拷贝
来源：http://gu.nicolike.cn

structuredClone(obj)
来源：http://ro.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://fh.yuntaijiaju.cn

`共 ${n} 条`
来源：http://nf.panjiajie.cn

[U94] JS：箭头函数
来源：http://zt.lnxyls.cn

const double = x => x * 2;
来源：http://fr.9csxet.cn

[U95] JS：Promise 包装
来源：http://yt.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://nw.asd995.cn

[U96] JS：async/await 与异常
来源：http://bs.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://vv.chemitech.net.cn

[U97] JS：并发请求
来源：http://sx.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iz.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://cx.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vq.hahajie.cn

[U99] JS：事件监听
来源：http://sk.hahajie.cn

el.addEventListener("click", e => {})
来源：http://vw.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://ye.huanxung.cn

document.querySelector(".item")
来源：http://qr.jctech888.com.cn

[U101] JS：classList 操作
来源：http://bq.hahajie.cn

el.classList.toggle("active")
来源：http://wm.nszjky.cn

[U102] JS：本地存储
来源：http://xu.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://by.szxytkj.cn

[U103] JS：定时器
来源：http://ie.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dj.jctech888.com.cn

[U104] JS：防抖
来源：http://bq.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gm.newstarts.cn

[U105] JS：节流
来源：http://aq.szxytkj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bv.shtwfgs.cn

[U106] JS：日期格式化
来源：http://hx.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wj.hahajie.cn

[U107] JS：数字千分位
来源：http://on.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ly.nicolike.cn

[U108] JS：随机整数
来源：http://zf.lnxyls.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ez.jctech888.com.cn

[U109] JS：数组分组
来源：http://la.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://ug.panjiajie.cn

[U110] JS：数组分块
来源：http://pq.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ol.lnxyls.cn

[U111] JS：对象转 Map
来源：http://oj.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://ju.shxzskj.cn

[U112] JS：字符串补位
来源：http://ar.szsharing.cn

"7".padStart(3, "0")
来源：http://ro.chemitech.net.cn

[U113] JS：正则替换全部
来源：http://wf.nicolike.cn

s.replaceAll("a", "b")
来源：http://mk.newstarts.cn

[U114] JS：JSON 深比较
来源：http://iq.yuexingan06.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rr.521024.cn

[U115] JS：生成 UUID
来源：http://if.nicolike.cn

crypto.randomUUID()
来源：http://lq.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://ao.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://pc.szsharing.cn

[U117] JS：单元测试
来源：http://xk.yuntaijiaju.cn

npm i -D vitest;  npx vitest
来源：http://cf.hnjuh.cn

[U118] JS：开发服务器
来源：http://ph.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://zj.bookmarksfly.cn

[U119] JS：生产构建
来源：http://oz.hahajie.cn

npx vite build
来源：http://am.panjiajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://av.shxzskj.cn

import.meta.env.VITE_API_URL
来源：http://kb.lnxyls.cn

================================================================================
来源：http://gb.bjjhwx.cn

统计汇总
来源：http://kr.haigaiapp.cn

================================================================================
来源：http://bl.colortex.cn

按语言统计（条）：
来源：http://ha.yuntaijiaju.cn

Python ......... 252
来源：http://iv.shtwfgs.cn

PHP ............ 252
来源：http://lf.jctech888.com.cn

JavaScript ..... 252
来源：http://ny.nszjky.cn

TypeScript ..... 212
来源：http://wt.shxzskj.cn

Java ........... 212
来源：http://lx.wgjwhj.cn

Go ............. 212
来源：http://ql.lnxyls.cn

Ruby ........... 212
来源：http://xj.haigaiapp.cn

C# ............. 212
来源：http://ag.huanxung.cn

C .............. 30
来源：http://yg.bookmarksfly.cn

C++ ............ 30
来源：http://dp.yuexingan06.cn

SQL ............ 90
来源：http://ln.asd995.cn

Bash ........... 80
来源：http://bl.nszjky.cn

Kotlin ......... 15
来源：http://fm.huixinmuqiang.cn

Swift .......... 15
来源：http://fw.bjjhwx.cn

Lua ............ 10
来源：http://ad.hahajie.cn

Perl ........... 10
来源：http://jn.lnxyls.cn

Scala .......... 10
来源：http://ls.jctech888.com.cn

------------------------------------
来源：http://aq.chemitech.net.cn

合计 ........... 2106 条
来源：http://uk.jctech888.com.cn

按章节统计：
来源：http://yb.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dh.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ox.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xb.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nc.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ap.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ur.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://up.muxihuayi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://zr.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://op.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gk.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oc.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ny.nicolike.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yh.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zo.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gg.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bg.wgjwhj.cn

Q SQL 专题                              90
来源：http://wy.jctech888.com.cn

R Bash 专题                             80
来源：http://et.colortex.cn

S C / C++ 专题                          60
来源：http://pl.colortex.cn

T 其他语言补充                          60
来源：http://gj.chemitech.net.cn

U 高频实用片段                         120
来源：http://if.yuexingan06.cn

------------------------------------
来源：http://pn.hnjuh.cn

合计                                  2106 条
来源：http://ld.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://cu.huanxung.cn

使用提醒
来源：http://rq.nszjky.cn

--------------------------------------------------------------------------------
来源：http://zk.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nf.yuexingan06.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://uz.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kf.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fc.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pl.lnxyls.cn

—— 文件结束 ——
来源：http://sx.gzmigu.cn

================================================================================
来源：http://pi.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://ko.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://sj.huixiangedu.cn

================================================================================
来源：http://vn.colortex.cn

【收录内容】
来源：http://im.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://dq.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xj.521024.cn

SQL · Bash · C · C++
来源：http://zh.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://na.wgjwhj.cn

【使用说明】
来源：http://cm.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bj.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bu.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://av.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wh.muxihuayi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://mn.yuexingan06.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://nq.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://gs.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pb.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vw.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qd.jianghongdianzi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gg.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dx.bookmarksfly.cn

【文件统计】
来源：http://tz.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gr.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ka.bjjhwx.cn

目  录
来源：http://ho.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://at.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mf.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dw.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ls.shtwfgs.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ea.jctech888.com.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wa.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gu.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mr.jianghongdianzi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lr.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ok.chemitech.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fu.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bg.bjjhwx.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qx.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tv.wgjwhj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rf.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mb.521024.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://uc.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xp.szxytkj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://or.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aj.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qt.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cs.bookmarksfly.cn

================================================================================
来源：http://or.jianghongdianzi.cn

A. 基础语法与类型
来源：http://zy.wgjwhj.cn

================================================================================
来源：http://yn.newstarts.cn

[A01] Hello World
来源：http://lu.newstarts.cn

Py:   print("Hello, World!")
来源：http://zv.muxihuayi.cn

PHP:  echo "Hello, World!";
来源：http://lh.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://da.newstarts.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ho.haigaiapp.cn

Java: System.out.println("Hello, World!");
来源：http://il.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://xn.szsharing.cn

Ruby: puts "Hello, World!"
来源：http://lr.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ws.szxytkj.cn

[A02] 变量声明与赋值
来源：http://qo.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vz.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fi.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tl.huixinmuqiang.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jx.nszjky.cn

Java: String name = "Alex"; int age = 20;
来源：http://le.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://jk.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://qm.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://id.gzmigu.cn

[A03] 常量定义
来源：http://uo.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://xa.panjiajie.cn

PHP:  const PI = 3.14159;
来源：http://eh.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://qo.lnxyls.cn

TS:   const PI: number = 3.14159;
来源：http://jo.hahajie.cn

Java: static final double PI = 3.14159;
来源：http://ac.colortex.cn

Go:   const PI = 3.14159
来源：http://lt.nicolike.cn

Ruby: PI = 3.14159
来源：http://io.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://ca.9csxet.cn

[A04] 判断变量类型
来源：http://ea.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ai.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://zu.yuexingan06.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zh.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://ye.panjiajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://av.bookmarksfly.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cq.wgjwhj.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://au.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://ba.nszjky.cn

[A05] 整数除法与取模
来源：http://fm.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fj.muxihuayi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ri.chemitech.net.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lq.szxytkj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kf.shtwfgs.cn

Java: 7 / 2; 7 % 2
来源：http://of.hnjuh.cn

Go:   7 / 2; 7 % 2
来源：http://el.huixiangedu.cn

Ruby: 7 / 2; 7 % 2
来源：http://ac.panjiajie.cn

C#:   7 / 2; 7 % 2
来源：http://pe.yuntaijiaju.cn


<!-- 参考信息 -->