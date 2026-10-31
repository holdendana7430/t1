代发 wailian999

[U51] PHP：数组解构
来源：http://lw.szxytkj.cn

[$a, $b] = $arr;
来源：http://as.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://eo.panjiajie.cn

$double = fn($x) => $x * 2;
来源：http://tl.9csxet.cn

[U53] PHP：空合并运算符
来源：http://ss.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://zl.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://zp.shxzskj.cn

$obj?->method()
来源：http://lk.haigaiapp.cn

[U55] PHP：match 表达式
来源：http://cb.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://id.newstarts.cn

[U56] PHP：命名参数
来源：http://ns.hahajie.cn

f(a: 1, b: 2)
来源：http://oa.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ln.szsharing.cn

"值: {$a}"
来源：http://pw.yuexingan06.cn

[U58] PHP：数组三件套
来源：http://ds.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xz.hnjuh.cn

[U59] PHP：自定义排序
来源：http://aq.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uz.panjiajie.cn

[U60] PHP：JSON 编解码
来源：http://er.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ic.huixinmuqiang.cn

[U61] PHP：正则
来源：http://mw.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ks.colortex.cn

[U62] PHP：日期对象
来源：http://oa.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kv.muxihuayi.cn

[U63] PHP：文件读写
来源：http://ni.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qr.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://xz.asd995.cn

glob("dir/*.php");  scandir("dir");
来源：http://rb.yuexingan06.cn

[U65] PHP：会话
来源：http://yq.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wp.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://mx.huixiangedu.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://js.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://yf.shxzukj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ye.szsharing.cn

[U68] PHP：PDO 连接
来源：http://oz.yuexingan06.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hz.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://dl.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iz.muxihuayi.cn

[U70] PHP：PDO 事务
来源：http://ne.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pp.9csxet.cn

[U71] PHP：抛出异常
来源：http://zd.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://tj.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://xe.jianghongdianzi.cn

error_log("失败: " . $e->getMessage());
来源：http://bp.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://iy.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://yz.jianghongdianzi.cn

[U74] PHP：读取环境变量
来源：http://xo.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://eg.muxihuayi.cn

[U75] PHP：依赖注入
来源：http://la.yuexingan06.cn

composer require psr/container
来源：http://lg.hahajie.cn

[U76] PHP：简单路由
来源：http://rs.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ec.yuntaijiaju.cn

[U77] PHP：模板渲染
来源：http://kf.yuntaijiaju.cn

composer require twig/twig
来源：http://lg.szxytkj.cn

[U78] PHP：单元测试
来源：http://rt.colortex.cn

composer require --dev phpunit/phpunit
来源：http://yo.muxihuayi.cn

[U79] PHP：静态分析
来源：http://ce.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://qu.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://od.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pq.bjjhwx.cn

[U81] JS：初始化项目
来源：http://yu.lnxyls.cn

npm init -y;  npm i express
来源：http://gw.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://lm.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://th.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://hn.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rn.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://am.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lp.shtwfgs.cn

[U85] JS：可选链
来源：http://ty.yuntaijiaju.cn

a?.b?.c
来源：http://jk.asd995.cn

[U86] JS：空值合并
来源：http://lh.9csxet.cn

a ?? b
来源：http://rf.hahajie.cn

[U87] JS：解构默认值
来源：http://sj.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://rk.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://ce.chemitech.net.cn

{ ...a, ...b }
来源：http://fd.jianghongdianzi.cn

[U89] JS：数组去重
来源：http://mq.huixiangedu.cn

[...new Set(arr)]
来源：http://mu.bookmarksfly.cn

[U90] JS：数字数组排序
来源：http://vy.huixiangedu.cn

[...arr].sort((a, b) => a - b)
来源：http://qq.colortex.cn

[U91] JS：对象键值遍历
来源：http://tr.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://uu.nszjky.cn

[U92] JS：深拷贝
来源：http://me.shtwfgs.cn

structuredClone(obj)
来源：http://bc.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://vu.hnjuh.cn

`共 ${n} 条`
来源：http://xu.shxzskj.cn

[U94] JS：箭头函数
来源：http://oo.yuntaijiaju.cn

const double = x => x * 2;
来源：http://qp.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://zl.yuexingan06.cn

new Promise((resolve, reject) => {})
来源：http://wg.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://rl.muxihuayi.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dc.bjjhwx.cn

[U97] JS：并发请求
来源：http://pf.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://kc.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://se.chemitech.net.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bx.haigaiapp.cn

[U99] JS：事件监听
来源：http://yu.nszjky.cn

el.addEventListener("click", e => {})
来源：http://wh.nicolike.cn

[U100] JS：DOM 查询
来源：http://pn.huixinmuqiang.cn

document.querySelector(".item")
来源：http://uz.huixiangedu.cn

[U101] JS：classList 操作
来源：http://gc.szxytkj.cn

el.classList.toggle("active")
来源：http://dv.hahajie.cn

[U102] JS：本地存储
来源：http://ly.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uk.shtwfgs.cn

[U103] JS：定时器
来源：http://bm.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://st.nicolike.cn

[U104] JS：防抖
来源：http://zy.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ig.bjjhwx.cn

[U105] JS：节流
来源：http://ty.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ux.colortex.cn

[U106] JS：日期格式化
来源：http://in.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vz.521024.cn

[U107] JS：数字千分位
来源：http://em.jianghongdianzi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://di.huixiangedu.cn

[U108] JS：随机整数
来源：http://qy.9csxet.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bl.huixiangedu.cn

[U109] JS：数组分组
来源：http://as.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://oy.huixinmuqiang.cn

[U110] JS：数组分块
来源：http://dc.huixinmuqiang.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zm.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://hs.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://xj.muxihuayi.cn

[U112] JS：字符串补位
来源：http://cq.wgjwhj.cn

"7".padStart(3, "0")
来源：http://cw.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://yz.hnjuh.cn

s.replaceAll("a", "b")
来源：http://jl.jctech888.com.cn

[U114] JS：JSON 深比较
来源：http://jx.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dy.huanxung.cn

[U115] JS：生成 UUID
来源：http://vz.jianghongdianzi.cn

crypto.randomUUID()
来源：http://ar.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://te.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://tq.yuexingan06.cn

[U117] JS：单元测试
来源：http://vw.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://iy.colortex.cn

[U118] JS：开发服务器
来源：http://ws.jianghongdianzi.cn

npm i -D vite;  npx vite
来源：http://xc.shxzukj.cn

[U119] JS：生产构建
来源：http://lo.gzmigu.cn

npx vite build
来源：http://ha.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://eb.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://bs.hahajie.cn

================================================================================
来源：http://ie.521024.cn

统计汇总
来源：http://vx.lnxyls.cn

================================================================================
来源：http://qp.panjiajie.cn

按语言统计（条）：
来源：http://lm.lnxyls.cn

Python ......... 252
来源：http://af.bookmarksfly.cn

PHP ............ 252
来源：http://ck.9csxet.cn

JavaScript ..... 252
来源：http://vq.newstarts.cn

TypeScript ..... 212
来源：http://ir.szsharing.cn

Java ........... 212
来源：http://jg.jianghongdianzi.cn

Go ............. 212
来源：http://aj.huixiangedu.cn

Ruby ........... 212
来源：http://pf.yuntaijiaju.cn

C# ............. 212
来源：http://ze.szsharing.cn

C .............. 30
来源：http://yn.wgjwhj.cn

C++ ............ 30
来源：http://uy.nszjky.cn

SQL ............ 90
来源：http://dq.szsharing.cn

Bash ........... 80
来源：http://cb.asd995.cn

Kotlin ......... 15
来源：http://cp.bjjhwx.cn

Swift .......... 15
来源：http://la.wgjwhj.cn

Lua ............ 10
来源：http://mj.yuntaijiaju.cn

Perl ........... 10
来源：http://yd.yuexingan06.cn

Scala .......... 10
来源：http://un.haigaiapp.cn

------------------------------------
来源：http://ul.shxzskj.cn

合计 ........... 2106 条
来源：http://lp.jianghongdianzi.cn

按章节统计：
来源：http://uk.huanxung.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://va.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://li.asd995.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ct.nicolike.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ho.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ww.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xm.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hx.yuntaijiaju.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mz.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nw.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fb.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qc.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kb.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hn.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mj.szxytkj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ay.yuntaijiaju.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://zm.haigaiapp.cn

Q SQL 专题                              90
来源：http://yw.szxytkj.cn

R Bash 专题                             80
来源：http://rj.huixinmuqiang.cn

S C / C++ 专题                          60
来源：http://am.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://ml.yuexingan06.cn

U 高频实用片段                         120
来源：http://kl.jianghongdianzi.cn

------------------------------------
来源：http://yp.shtwfgs.cn

合计                                  2106 条
来源：http://wy.nicolike.cn

--------------------------------------------------------------------------------
来源：http://rf.lnxyls.cn

使用提醒
来源：http://oh.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://sm.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kq.9csxet.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://na.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ws.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://na.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hi.chemitech.net.cn

—— 文件结束 ——
来源：http://nd.bjjhwx.cn

================================================================================
来源：http://nz.huanxung.cn

程序语言常见例子速查手册（2024 版）
来源：http://nq.szsharing.cn

Common Programming Examples Cheat Book
来源：http://cn.jctech888.com.cn

================================================================================
来源：http://jw.szsharing.cn

【收录内容】
来源：http://zy.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://gk.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tl.shxzskj.cn

SQL · Bash · C · C++
来源：http://rr.bookmarksfly.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dn.muxihuayi.cn

【使用说明】
来源：http://vf.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cm.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cp.huanxung.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vx.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cj.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://yt.shxzukj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dl.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rw.szxytkj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://pn.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://qc.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sb.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hz.szsharing.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ro.huanxung.cn

【文件统计】
来源：http://xt.bookmarksfly.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://le.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://hm.bookmarksfly.cn

目  录
来源：http://ir.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://kj.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yz.panjiajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ft.9csxet.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qi.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://he.shxzskj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://fj.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mo.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ba.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lb.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ic.shtwfgs.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://la.wgjwhj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gh.chemitech.net.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://qy.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://si.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pk.newstarts.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://me.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cn.asd995.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zq.bjjhwx.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://li.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://vl.wgjwhj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mp.521024.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mm.wgjwhj.cn

================================================================================
来源：http://ao.muxihuayi.cn

A. 基础语法与类型
来源：http://bq.jctech888.com.cn

================================================================================
来源：http://ni.jctech888.com.cn

[A01] Hello World
来源：http://fq.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://mk.yuexingan06.cn

PHP:  echo "Hello, World!";
来源：http://ai.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://oj.nszjky.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pf.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://kc.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://xl.yuntaijiaju.cn

Ruby: puts "Hello, World!"
来源：http://ej.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://oh.shxzukj.cn

[A02] 变量声明与赋值
来源：http://jn.chemitech.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vs.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://fs.haigaiapp.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sq.jianghongdianzi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dd.haigaiapp.cn

Java: String name = "Alex"; int age = 20;
来源：http://iw.hnjuh.cn

Go:   name := "Alex"; age := 20
来源：http://sd.huixiangedu.cn

Ruby: name = "Alex"; age = 20
来源：http://ed.haigaiapp.cn

C#:   string name = "Alex"; int age = 20;
来源：http://he.gzmigu.cn

[A03] 常量定义
来源：http://zd.yuntaijiaju.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oh.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://gp.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://cd.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://im.huanxung.cn

Java: static final double PI = 3.14159;
来源：http://qe.yuntaijiaju.cn

Go:   const PI = 3.14159
来源：http://rm.hahajie.cn

Ruby: PI = 3.14159
来源：http://dh.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://mv.newstarts.cn

[A04] 判断变量类型
来源：http://qc.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wj.jianghongdianzi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tz.gzmigu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://pn.asd995.cn

TS:   typeof x; x instanceof Date
来源：http://sq.bjjhwx.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sq.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ry.muxihuayi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nq.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://qk.szsharing.cn

[A05] 整数除法与取模
来源：http://ao.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cb.lnxyls.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yk.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tb.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eu.huixinmuqiang.cn

Java: 7 / 2; 7 % 2
来源：http://ac.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://wr.hnjuh.cn

Ruby: 7 / 2; 7 % 2
来源：http://pq.gzmigu.cn

C#:   7 / 2; 7 % 2
来源：http://au.shxzukj.cn

[A06] 字符串转数字
来源：http://ta.haigaiapp.cn

Py:   int("42"); float("3.14")
来源：http://sl.nicolike.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tf.yuntaijiaju.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fl.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ib.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://aw.521024.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://xr.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://zz.szxytkj.cn


<!-- 参考信息 -->