代发 wailian999

[U53] PHP：空合并运算符
来源：http://ye.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://dq.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://ad.521024.cn

$obj?->method()
来源：http://pb.shxzukj.cn

[U55] PHP：match 表达式
来源：http://ao.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pq.bjjhwx.cn

[U56] PHP：命名参数
来源：http://mr.panjiajie.cn

f(a: 1, b: 2)
来源：http://yf.shxzukj.cn

[U57] PHP：字符串插值
来源：http://cb.yuexingan06.cn

"值: {$a}"
来源：http://uz.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://jf.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hx.hahajie.cn

[U59] PHP：自定义排序
来源：http://xm.yuntaijiaju.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lv.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://bx.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ia.bookmarksfly.cn

[U61] PHP：正则
来源：http://ea.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fk.szxytkj.cn

[U62] PHP：日期对象
来源：http://xq.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uh.9csxet.cn

[U63] PHP：文件读写
来源：http://lw.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aw.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://ur.panjiajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://fg.newstarts.cn

[U65] PHP：会话
来源：http://ki.nicolike.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pu.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://cn.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ka.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://rb.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vw.jctech888.com.cn

[U68] PHP：PDO 连接
来源：http://sg.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dh.yuexingan06.cn

[U69] PHP：PDO 预处理
来源：http://xw.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ax.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://ni.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ie.szsharing.cn

[U71] PHP：抛出异常
来源：http://js.shxzukj.cn

throw new RuntimeException("失败", 500);
来源：http://wo.newstarts.cn

[U72] PHP：写错误日志
来源：http://lv.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://cz.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://ch.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://wz.huixiangedu.cn

[U74] PHP：读取环境变量
来源：http://jz.jianghongdianzi.cn

getenv("APP_ENV") ?: "production"
来源：http://sm.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://fz.newstarts.cn

composer require psr/container
来源：http://yx.colortex.cn

[U76] PHP：简单路由
来源：http://rd.9csxet.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gi.shxzskj.cn

[U77] PHP：模板渲染
来源：http://ec.wgjwhj.cn

composer require twig/twig
来源：http://bo.newstarts.cn

[U78] PHP：单元测试
来源：http://oq.bjjhwx.cn

composer require --dev phpunit/phpunit
来源：http://xm.shxzskj.cn

[U79] PHP：静态分析
来源：http://bv.521024.cn

composer require --dev phpstan/phpstan
来源：http://ud.bookmarksfly.cn

[U80] PHP：代码规范修复
来源：http://il.huixiangedu.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mp.shtwfgs.cn

[U81] JS：初始化项目
来源：http://ow.chemitech.net.cn

npm init -y;  npm i express
来源：http://zb.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://bz.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bp.colortex.cn

[U83] JS：ES Module 导入导出
来源：http://re.szxytkj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://de.newstarts.cn

[U84] JS：CommonJS 写法
来源：http://th.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ph.panjiajie.cn

[U85] JS：可选链
来源：http://id.9csxet.cn

a?.b?.c
来源：http://pq.nszjky.cn

[U86] JS：空值合并
来源：http://qr.shxzskj.cn

a ?? b
来源：http://bu.colortex.cn

[U87] JS：解构默认值
来源：http://ji.shtwfgs.cn

const { a = 1, b = 2 } = obj;
来源：http://eu.colortex.cn

[U88] JS：对象展开合并
来源：http://tr.jctech888.com.cn

{ ...a, ...b }
来源：http://sw.hnjuh.cn

[U89] JS：数组去重
来源：http://ve.bjjhwx.cn

[...new Set(arr)]
来源：http://gl.shxzukj.cn

[U90] JS：数字数组排序
来源：http://bo.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://sn.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://ie.shxzukj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ih.haigaiapp.cn

[U92] JS：深拷贝
来源：http://my.shxzukj.cn

structuredClone(obj)
来源：http://eu.huixiangedu.cn

[U93] JS：模板字符串
来源：http://dy.huanxung.cn

`共 ${n} 条`
来源：http://ez.jctech888.com.cn

[U94] JS：箭头函数
来源：http://pq.szxytkj.cn

const double = x => x * 2;
来源：http://zx.newstarts.cn

[U95] JS：Promise 包装
来源：http://xp.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://db.nszjky.cn

[U96] JS：async/await 与异常
来源：http://dk.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://au.haigaiapp.cn

[U97] JS：并发请求
来源：http://gs.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rb.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://ww.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://br.bjjhwx.cn

[U99] JS：事件监听
来源：http://un.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://nd.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://xx.newstarts.cn

document.querySelector(".item")
来源：http://rq.hahajie.cn

[U101] JS：classList 操作
来源：http://ct.wgjwhj.cn

el.classList.toggle("active")
来源：http://fd.gzmigu.cn

[U102] JS：本地存储
来源：http://ke.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sp.wgjwhj.cn

[U103] JS：定时器
来源：http://cd.jctech888.com.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://er.gzmigu.cn

[U104] JS：防抖
来源：http://fu.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ev.szxytkj.cn

[U105] JS：节流
来源：http://br.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://av.hahajie.cn

[U106] JS：日期格式化
来源：http://il.gzmigu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ta.shtwfgs.cn

[U107] JS：数字千分位
来源：http://af.panjiajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uj.521024.cn

[U108] JS：随机整数
来源：http://rd.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qu.hnjuh.cn

[U109] JS：数组分组
来源：http://wf.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://fh.nszjky.cn

[U110] JS：数组分块
来源：http://rr.gzmigu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://kz.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://ko.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://xh.yuexingan06.cn

[U112] JS：字符串补位
来源：http://vn.muxihuayi.cn

"7".padStart(3, "0")
来源：http://zm.521024.cn

[U113] JS：正则替换全部
来源：http://hd.huixinmuqiang.cn

s.replaceAll("a", "b")
来源：http://zz.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://rb.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://vl.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://fk.szxytkj.cn

crypto.randomUUID()
来源：http://dl.szxytkj.cn

[U116] JS：类型检查（JSDoc）
来源：http://so.gzmigu.cn

/** @param {string} name */ function f(name) {}
来源：http://ta.bjjhwx.cn

[U117] JS：单元测试
来源：http://to.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://ts.colortex.cn

[U118] JS：开发服务器
来源：http://ii.9csxet.cn

npm i -D vite;  npx vite
来源：http://ta.newstarts.cn

[U119] JS：生产构建
来源：http://sg.yuntaijiaju.cn

npx vite build
来源：http://wp.shxzukj.cn

[U120] JS：读取环境变量（Vite）
来源：http://yo.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://zu.huixinmuqiang.cn

================================================================================
来源：http://nl.shxzukj.cn

统计汇总
来源：http://zm.chemitech.net.cn

================================================================================
来源：http://vj.jianghongdianzi.cn

按语言统计（条）：
来源：http://zd.szsharing.cn

Python ......... 252
来源：http://su.hnjuh.cn

PHP ............ 252
来源：http://jp.szxytkj.cn

JavaScript ..... 252
来源：http://to.huixinmuqiang.cn

TypeScript ..... 212
来源：http://mz.muxihuayi.cn

Java ........... 212
来源：http://xe.gzmigu.cn

Go ............. 212
来源：http://tf.bjjhwx.cn

Ruby ........... 212
来源：http://op.huanxung.cn

C# ............. 212
来源：http://kb.huanxung.cn

C .............. 30
来源：http://kj.jianghongdianzi.cn

C++ ............ 30
来源：http://qo.jctech888.com.cn

SQL ............ 90
来源：http://su.huanxung.cn

Bash ........... 80
来源：http://om.nicolike.cn

Kotlin ......... 15
来源：http://qa.huixinmuqiang.cn

Swift .......... 15
来源：http://ob.muxihuayi.cn

Lua ............ 10
来源：http://us.panjiajie.cn

Perl ........... 10
来源：http://qc.nicolike.cn

Scala .......... 10
来源：http://zy.bjjhwx.cn

------------------------------------
来源：http://kp.nszjky.cn

合计 ........... 2106 条
来源：http://cj.muxihuayi.cn

按章节统计：
来源：http://gv.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qg.asd995.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cn.szsharing.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://br.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zh.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://li.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xc.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://zk.huixiangedu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wi.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://so.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pm.521024.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dv.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qp.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sn.asd995.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dt.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zx.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ej.asd995.cn

Q SQL 专题                              90
来源：http://lg.wgjwhj.cn

R Bash 专题                             80
来源：http://md.nszjky.cn

S C / C++ 专题                          60
来源：http://is.gzmigu.cn

T 其他语言补充                          60
来源：http://df.yuexingan06.cn

U 高频实用片段                         120
来源：http://qa.huanxung.cn

------------------------------------
来源：http://gt.newstarts.cn

合计                                  2106 条
来源：http://vs.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://wq.yuexingan06.cn

使用提醒
来源：http://tn.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zy.jctech888.com.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fz.yuntaijiaju.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vn.shtwfgs.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yi.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gz.colortex.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oi.bookmarksfly.cn

—— 文件结束 ——
来源：http://nn.shxzukj.cn

================================================================================
来源：http://qk.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://sk.hnjuh.cn

Common Programming Examples Cheat Book
来源：http://zn.nicolike.cn

================================================================================
来源：http://ar.huixiangedu.cn

【收录内容】
来源：http://zq.yuexingan06.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tn.lnxyls.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jw.asd995.cn

SQL · Bash · C · C++
来源：http://lf.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://to.colortex.cn

【使用说明】
来源：http://ge.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://az.colortex.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://jh.muxihuayi.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wl.9csxet.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pj.hnjuh.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ul.yuntaijiaju.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://eh.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wp.asd995.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://oa.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jk.newstarts.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ay.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://td.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ui.chemitech.net.cn

【文件统计】
来源：http://rp.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qj.huanxung.cn

--------------------------------------------------------------------------------
来源：http://hz.szsharing.cn

目  录
来源：http://bu.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://xe.jctech888.com.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sk.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tk.jctech888.com.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yd.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dp.lnxyls.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nu.shxzskj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mk.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://xc.panjiajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://zm.bookmarksfly.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ai.nicolike.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pi.asd995.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ws.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://eb.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ms.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xr.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://so.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wt.bookmarksfly.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yd.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wi.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://bb.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sn.9csxet.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ij.jctech888.com.cn

================================================================================
来源：http://iv.yuntaijiaju.cn

A. 基础语法与类型
来源：http://nz.panjiajie.cn

================================================================================
来源：http://ya.panjiajie.cn

[A01] Hello World
来源：http://qz.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://zs.colortex.cn

PHP:  echo "Hello, World!";
来源：http://zx.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://sz.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xo.hnjuh.cn

Java: System.out.println("Hello, World!");
来源：http://jl.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://xh.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://zq.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://py.shtwfgs.cn

[A02] 变量声明与赋值
来源：http://lh.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iq.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sv.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hw.asd995.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://cw.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://mx.panjiajie.cn

Go:   name := "Alex"; age := 20
来源：http://os.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://me.521024.cn

C#:   string name = "Alex"; int age = 20;
来源：http://uq.bookmarksfly.cn

[A03] 常量定义
来源：http://in.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://kn.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://vh.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://yp.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://pg.asd995.cn

Java: static final double PI = 3.14159;
来源：http://lk.lnxyls.cn

Go:   const PI = 3.14159
来源：http://tq.colortex.cn

Ruby: PI = 3.14159
来源：http://do.bjjhwx.cn

C#:   const double PI = 3.14159;
来源：http://eo.wgjwhj.cn

[A04] 判断变量类型
来源：http://kk.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qi.shtwfgs.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ds.521024.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xw.hnjuh.cn

TS:   typeof x; x instanceof Date
来源：http://yo.bookmarksfly.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vh.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://cx.huixinmuqiang.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://gf.bookmarksfly.cn

C#:   x.GetType().Name; x is int
来源：http://uu.newstarts.cn

[A05] 整数除法与取模
来源：http://pm.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://up.newstarts.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://rf.huixiangedu.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pv.jctech888.com.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pi.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://ih.shxzukj.cn

Go:   7 / 2; 7 % 2
来源：http://fj.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://is.huanxung.cn

C#:   7 / 2; 7 % 2
来源：http://oi.muxihuayi.cn

[A06] 字符串转数字
来源：http://ew.hahajie.cn

Py:   int("42"); float("3.14")
来源：http://eb.muxihuayi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://yw.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://gs.521024.cn

TS:   parseInt("42", 10); Number("42")
来源：http://uj.bjjhwx.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://nd.bookmarksfly.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://fc.gzmigu.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fy.yuntaijiaju.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://oy.bjjhwx.cn

[A07] 数字转字符串
来源：http://ok.9csxet.cn

Py:   str(42)
来源：http://hr.wgjwhj.cn

PHP:  (string) 42; strval(42)
来源：http://np.wgjwhj.cn


<!-- 参考信息 -->