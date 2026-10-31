代发 wailian999

[U53] PHP：空合并运算符
来源：http://gp.hnjuh.cn

$v = $a ?? $b ?? "default";
来源：http://sf.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://lu.hnjuh.cn

$obj?->method()
来源：http://nv.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://nt.lnxyls.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pl.asd995.cn

[U56] PHP：命名参数
来源：http://cd.521024.cn

f(a: 1, b: 2)
来源：http://pt.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://fk.szxytkj.cn

"值: {$a}"
来源：http://ox.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://cj.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qq.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://hv.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rb.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://ir.szsharing.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ju.chemitech.net.cn

[U61] PHP：正则
来源：http://qg.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gp.shxzskj.cn

[U62] PHP：日期对象
来源：http://js.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nt.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://wz.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://br.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://qr.chemitech.net.cn

glob("dir/*.php");  scandir("dir");
来源：http://eb.hnjuh.cn

[U65] PHP：会话
来源：http://ow.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://sk.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://me.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sn.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://np.haigaiapp.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bo.huixiangedu.cn

[U68] PHP：PDO 连接
来源：http://ea.yuntaijiaju.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rh.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://zb.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hm.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://ua.bjjhwx.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xi.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://av.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://fk.szxytkj.cn

[U72] PHP：写错误日志
来源：http://xs.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://sx.haigaiapp.cn

[U73] PHP：读取 ini 配置
来源：http://zq.chemitech.net.cn

parse_ini_file("config.ini", true)
来源：http://xx.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://mq.bjjhwx.cn

getenv("APP_ENV") ?: "production"
来源：http://yb.yuexingan06.cn

[U75] PHP：依赖注入
来源：http://cf.nszjky.cn

composer require psr/container
来源：http://ql.colortex.cn

[U76] PHP：简单路由
来源：http://fi.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://di.colortex.cn

[U77] PHP：模板渲染
来源：http://vt.newstarts.cn

composer require twig/twig
来源：http://sm.jianghongdianzi.cn

[U78] PHP：单元测试
来源：http://of.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://wu.hnjuh.cn

[U79] PHP：静态分析
来源：http://qq.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://hu.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://sd.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xp.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://mw.shxzskj.cn

npm init -y;  npm i express
来源：http://ir.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://xy.jianghongdianzi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wv.bjjhwx.cn

[U83] JS：ES Module 导入导出
来源：http://bj.newstarts.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ms.chemitech.net.cn

[U84] JS：CommonJS 写法
来源：http://ym.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ue.jctech888.com.cn

[U85] JS：可选链
来源：http://mc.yuexingan06.cn

a?.b?.c
来源：http://tq.nicolike.cn

[U86] JS：空值合并
来源：http://gg.jctech888.com.cn

a ?? b
来源：http://mf.szsharing.cn

[U87] JS：解构默认值
来源：http://rs.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://ap.yuntaijiaju.cn

[U88] JS：对象展开合并
来源：http://yt.yuexingan06.cn

{ ...a, ...b }
来源：http://fy.muxihuayi.cn

[U89] JS：数组去重
来源：http://bp.hahajie.cn

[...new Set(arr)]
来源：http://fu.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://ok.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://kr.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://qk.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kb.huixinmuqiang.cn

[U92] JS：深拷贝
来源：http://ug.9csxet.cn

structuredClone(obj)
来源：http://tr.muxihuayi.cn

[U93] JS：模板字符串
来源：http://ej.panjiajie.cn

`共 ${n} 条`
来源：http://ac.yuexingan06.cn

[U94] JS：箭头函数
来源：http://sr.colortex.cn

const double = x => x * 2;
来源：http://mw.newstarts.cn

[U95] JS：Promise 包装
来源：http://su.jianghongdianzi.cn

new Promise((resolve, reject) => {})
来源：http://xa.chemitech.net.cn

[U96] JS：async/await 与异常
来源：http://xl.hahajie.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://jw.bjjhwx.cn

[U97] JS：并发请求
来源：http://ra.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kx.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://zl.9csxet.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lv.9csxet.cn

[U99] JS：事件监听
来源：http://kn.colortex.cn

el.addEventListener("click", e => {})
来源：http://gu.chemitech.net.cn

[U100] JS：DOM 查询
来源：http://up.521024.cn

document.querySelector(".item")
来源：http://fs.asd995.cn

[U101] JS：classList 操作
来源：http://ts.jctech888.com.cn

el.classList.toggle("active")
来源：http://nn.huixiangedu.cn

[U102] JS：本地存储
来源：http://gr.shtwfgs.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fg.huanxung.cn

[U103] JS：定时器
来源：http://th.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://sy.szxytkj.cn

[U104] JS：防抖
来源：http://te.hahajie.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://up.gzmigu.cn

[U105] JS：节流
来源：http://cb.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://yb.huixinmuqiang.cn

[U106] JS：日期格式化
来源：http://yz.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lx.9csxet.cn

[U107] JS：数字千分位
来源：http://rf.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qo.hahajie.cn

[U108] JS：随机整数
来源：http://ll.newstarts.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tq.jctech888.com.cn

[U109] JS：数组分组
来源：http://ig.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://sh.nicolike.cn

[U110] JS：数组分块
来源：http://oa.huanxung.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qb.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://gk.521024.cn

new Map(Object.entries(obj))
来源：http://ro.bjjhwx.cn

[U112] JS：字符串补位
来源：http://pb.lnxyls.cn

"7".padStart(3, "0")
来源：http://ie.lnxyls.cn

[U113] JS：正则替换全部
来源：http://vq.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://jf.muxihuayi.cn

[U114] JS：JSON 深比较
来源：http://lg.wgjwhj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://iq.newstarts.cn

[U115] JS：生成 UUID
来源：http://dh.huixinmuqiang.cn

crypto.randomUUID()
来源：http://sb.haigaiapp.cn

[U116] JS：类型检查（JSDoc）
来源：http://zj.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://mr.jianghongdianzi.cn

[U117] JS：单元测试
来源：http://uv.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://ne.9csxet.cn

[U118] JS：开发服务器
来源：http://mf.szsharing.cn

npm i -D vite;  npx vite
来源：http://dw.9csxet.cn

[U119] JS：生产构建
来源：http://gg.haigaiapp.cn

npx vite build
来源：http://mr.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://zh.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://xy.yuntaijiaju.cn

================================================================================
来源：http://ql.szxytkj.cn

统计汇总
来源：http://yj.chemitech.net.cn

================================================================================
来源：http://lb.szsharing.cn

按语言统计（条）：
来源：http://ir.wgjwhj.cn

Python ......... 252
来源：http://po.bookmarksfly.cn

PHP ............ 252
来源：http://mn.nszjky.cn

JavaScript ..... 252
来源：http://fc.huixinmuqiang.cn

TypeScript ..... 212
来源：http://ir.haigaiapp.cn

Java ........... 212
来源：http://yu.jianghongdianzi.cn

Go ............. 212
来源：http://nw.wgjwhj.cn

Ruby ........... 212
来源：http://ic.szxytkj.cn

C# ............. 212
来源：http://kb.bookmarksfly.cn

C .............. 30
来源：http://rk.gzmigu.cn

C++ ............ 30
来源：http://lw.yuntaijiaju.cn

SQL ............ 90
来源：http://sn.nicolike.cn

Bash ........... 80
来源：http://ju.yuntaijiaju.cn

Kotlin ......... 15
来源：http://mu.newstarts.cn

Swift .......... 15
来源：http://aa.haigaiapp.cn

Lua ............ 10
来源：http://zm.colortex.cn

Perl ........... 10
来源：http://go.9csxet.cn

Scala .......... 10
来源：http://yy.jianghongdianzi.cn

------------------------------------
来源：http://od.hahajie.cn

合计 ........... 2106 条
来源：http://wp.yuexingan06.cn

按章节统计：
来源：http://ki.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gp.jianghongdianzi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rv.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oc.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rf.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zi.9csxet.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mv.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ho.shtwfgs.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://au.nszjky.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bu.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ie.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://uw.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ad.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mn.521024.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bk.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tw.szsharing.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://om.gzmigu.cn

Q SQL 专题                              90
来源：http://ok.colortex.cn

R Bash 专题                             80
来源：http://vy.gzmigu.cn

S C / C++ 专题                          60
来源：http://wg.hnjuh.cn

T 其他语言补充                          60
来源：http://bg.chemitech.net.cn

U 高频实用片段                         120
来源：http://tp.panjiajie.cn

------------------------------------
来源：http://jv.huixinmuqiang.cn

合计                                  2106 条
来源：http://tv.nszjky.cn

--------------------------------------------------------------------------------
来源：http://el.yuexingan06.cn

使用提醒
来源：http://an.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://vl.asd995.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://aq.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ba.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zg.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xu.shtwfgs.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mw.huixinmuqiang.cn

—— 文件结束 ——
来源：http://tv.shtwfgs.cn

================================================================================
来源：http://ex.521024.cn

程序语言常见例子速查手册（2024 版）
来源：http://xd.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://au.asd995.cn

================================================================================
来源：http://no.521024.cn

【收录内容】
来源：http://at.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://sm.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://eq.szsharing.cn

SQL · Bash · C · C++
来源：http://uv.nszjky.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xx.gzmigu.cn

【使用说明】
来源：http://zq.huanxung.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://db.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yt.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://zo.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ac.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lz.nicolike.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://kf.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ox.bookmarksfly.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ev.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://kv.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://zg.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ks.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://gr.shtwfgs.cn

【文件统计】
来源：http://av.colortex.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zj.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://ql.panjiajie.cn

目  录
来源：http://ge.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://ws.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sw.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ef.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zf.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ng.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://sn.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dk.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://tw.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ef.haigaiapp.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vb.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://qj.hahajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zh.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pl.wgjwhj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lb.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://dy.gzmigu.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ar.szsharing.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ro.jianghongdianzi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wq.haigaiapp.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ek.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://kf.chemitech.net.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tp.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://on.shxzskj.cn

================================================================================
来源：http://ra.nszjky.cn

A. 基础语法与类型
来源：http://jt.hahajie.cn

================================================================================
来源：http://rl.shxzukj.cn

[A01] Hello World
来源：http://xf.nicolike.cn

Py:   print("Hello, World!")
来源：http://tw.huixiangedu.cn

PHP:  echo "Hello, World!";
来源：http://gu.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://jx.shtwfgs.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rg.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://jx.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://bf.bjjhwx.cn

Ruby: puts "Hello, World!"
来源：http://ko.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://en.szsharing.cn

[A02] 变量声明与赋值
来源：http://yb.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ck.haigaiapp.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rr.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qm.shxzskj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bp.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://vh.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://dl.szxytkj.cn

Ruby: name = "Alex"; age = 20
来源：http://df.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://me.9csxet.cn

[A03] 常量定义
来源：http://so.nszjky.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ok.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://zt.wgjwhj.cn

JS:   const PI = 3.14159;
来源：http://ui.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://nx.wgjwhj.cn

Java: static final double PI = 3.14159;
来源：http://mu.bjjhwx.cn

Go:   const PI = 3.14159
来源：http://hy.hnjuh.cn

Ruby: PI = 3.14159
来源：http://ln.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://aq.jctech888.com.cn

[A04] 判断变量类型
来源：http://mc.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xw.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://di.muxihuayi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://to.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://ng.muxihuayi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gr.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://fo.hahajie.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dz.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://uh.huanxung.cn

[A05] 整数除法与取模
来源：http://rj.szxytkj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ig.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://am.hahajie.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://np.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://aq.haigaiapp.cn

Java: 7 / 2; 7 % 2
来源：http://gc.asd995.cn

Go:   7 / 2; 7 % 2
来源：http://yw.yuexingan06.cn

Ruby: 7 / 2; 7 % 2
来源：http://ru.asd995.cn

C#:   7 / 2; 7 % 2
来源：http://kc.lnxyls.cn

[A06] 字符串转数字
来源：http://om.jianghongdianzi.cn

Py:   int("42"); float("3.14")
来源：http://vh.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ml.colortex.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bc.haigaiapp.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ob.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://es.newstarts.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ka.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://pj.newstarts.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zo.colortex.cn

[A07] 数字转字符串
来源：http://nt.muxihuayi.cn

Py:   str(42)
来源：http://iq.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://zc.jctech888.com.cn


<!-- 参考信息 -->