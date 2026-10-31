代发 wailian999

[U53] PHP：空合并运算符
来源：http://bp.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://ug.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://oi.muxihuayi.cn

$obj?->method()
来源：http://ar.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://qb.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jg.nicolike.cn

[U56] PHP：命名参数
来源：http://ko.wgjwhj.cn

f(a: 1, b: 2)
来源：http://xh.panjiajie.cn

[U57] PHP：字符串插值
来源：http://ru.huixiangedu.cn

"值: {$a}"
来源：http://wz.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://ok.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yd.shtwfgs.cn

[U59] PHP：自定义排序
来源：http://eg.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://do.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://vj.muxihuayi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cg.haigaiapp.cn

[U61] PHP：正则
来源：http://yx.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cv.jctech888.com.cn

[U62] PHP：日期对象
来源：http://xx.yuntaijiaju.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://as.panjiajie.cn

[U63] PHP：文件读写
来源：http://ca.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xv.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://zq.gzmigu.cn

glob("dir/*.php");  scandir("dir");
来源：http://wu.szsharing.cn

[U65] PHP：会话
来源：http://ph.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ti.nszjky.cn

[U66] PHP：设置 Cookie
来源：http://ju.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mi.bjjhwx.cn

[U67] PHP：处理文件上传
来源：http://tw.bjjhwx.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://im.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://ev.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hd.shxzskj.cn

[U69] PHP：PDO 预处理
来源：http://wl.haigaiapp.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://io.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://rn.wgjwhj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ul.panjiajie.cn

[U71] PHP：抛出异常
来源：http://dk.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://kr.huanxung.cn

[U72] PHP：写错误日志
来源：http://oo.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://lt.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://vy.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://xt.szsharing.cn

[U74] PHP：读取环境变量
来源：http://im.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://of.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://hf.huixinmuqiang.cn

composer require psr/container
来源：http://xp.huanxung.cn

[U76] PHP：简单路由
来源：http://yj.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fv.lnxyls.cn

[U77] PHP：模板渲染
来源：http://tw.colortex.cn

composer require twig/twig
来源：http://cx.haigaiapp.cn

[U78] PHP：单元测试
来源：http://xt.hnjuh.cn

composer require --dev phpunit/phpunit
来源：http://vm.huixiangedu.cn

[U79] PHP：静态分析
来源：http://cd.haigaiapp.cn

composer require --dev phpstan/phpstan
来源：http://zi.hahajie.cn

[U80] PHP：代码规范修复
来源：http://us.shxzukj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dx.colortex.cn

[U81] JS：初始化项目
来源：http://wz.huanxung.cn

npm init -y;  npm i express
来源：http://wk.newstarts.cn

[U82] JS：package.json 脚本
来源：http://of.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pd.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://pc.szsharing.cn

export const a = 1;  import { a } from "./m.js";
来源：http://sn.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://lj.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nl.lnxyls.cn

[U85] JS：可选链
来源：http://gj.newstarts.cn

a?.b?.c
来源：http://db.yuexingan06.cn

[U86] JS：空值合并
来源：http://hl.chemitech.net.cn

a ?? b
来源：http://ur.asd995.cn

[U87] JS：解构默认值
来源：http://ex.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://kh.hnjuh.cn

[U88] JS：对象展开合并
来源：http://gj.szxytkj.cn

{ ...a, ...b }
来源：http://oz.521024.cn

[U89] JS：数组去重
来源：http://ih.nicolike.cn

[...new Set(arr)]
来源：http://qp.szxytkj.cn

[U90] JS：数字数组排序
来源：http://vu.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://ag.yuexingan06.cn

[U91] JS：对象键值遍历
来源：http://uy.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://rj.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://ba.hnjuh.cn

structuredClone(obj)
来源：http://nv.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://hx.shxzskj.cn

`共 ${n} 条`
来源：http://qs.bookmarksfly.cn

[U94] JS：箭头函数
来源：http://pg.lnxyls.cn

const double = x => x * 2;
来源：http://nr.9csxet.cn

[U95] JS：Promise 包装
来源：http://kt.jctech888.com.cn

new Promise((resolve, reject) => {})
来源：http://yu.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://xu.newstarts.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xv.chemitech.net.cn

[U97] JS：并发请求
来源：http://ub.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ro.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://wp.newstarts.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lb.szxytkj.cn

[U99] JS：事件监听
来源：http://se.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://mp.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ev.asd995.cn

document.querySelector(".item")
来源：http://nh.gzmigu.cn

[U101] JS：classList 操作
来源：http://gl.jianghongdianzi.cn

el.classList.toggle("active")
来源：http://fc.muxihuayi.cn

[U102] JS：本地存储
来源：http://nz.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ro.bookmarksfly.cn

[U103] JS：定时器
来源：http://nq.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ys.newstarts.cn

[U104] JS：防抖
来源：http://pl.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pm.shxzskj.cn

[U105] JS：节流
来源：http://hh.chemitech.net.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zt.panjiajie.cn

[U106] JS：日期格式化
来源：http://kk.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pz.bjjhwx.cn

[U107] JS：数字千分位
来源：http://ia.huixinmuqiang.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://id.newstarts.cn

[U108] JS：随机整数
来源：http://dw.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fa.szsharing.cn

[U109] JS：数组分组
来源：http://gi.newstarts.cn

Object.groupBy(arr, x => x.type)
来源：http://lw.shxzukj.cn

[U110] JS：数组分块
来源：http://pw.bookmarksfly.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://zd.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://ie.hnjuh.cn

new Map(Object.entries(obj))
来源：http://vs.shxzskj.cn

[U112] JS：字符串补位
来源：http://ek.gzmigu.cn

"7".padStart(3, "0")
来源：http://xw.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://fr.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://lr.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://ia.huixiangedu.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yu.521024.cn

[U115] JS：生成 UUID
来源：http://qq.yuntaijiaju.cn

crypto.randomUUID()
来源：http://dg.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://aj.yuntaijiaju.cn

/** @param {string} name */ function f(name) {}
来源：http://yz.hahajie.cn

[U117] JS：单元测试
来源：http://aa.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://ey.nicolike.cn

[U118] JS：开发服务器
来源：http://qm.9csxet.cn

npm i -D vite;  npx vite
来源：http://zh.hnjuh.cn

[U119] JS：生产构建
来源：http://od.shtwfgs.cn

npx vite build
来源：http://dd.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://pp.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://vn.hnjuh.cn

================================================================================
来源：http://sq.panjiajie.cn

统计汇总
来源：http://bs.lnxyls.cn

================================================================================
来源：http://zw.hnjuh.cn

按语言统计（条）：
来源：http://jh.szxytkj.cn

Python ......... 252
来源：http://tb.colortex.cn

PHP ............ 252
来源：http://pc.szsharing.cn

JavaScript ..... 252
来源：http://qt.bookmarksfly.cn

TypeScript ..... 212
来源：http://rq.huixinmuqiang.cn

Java ........... 212
来源：http://fj.huixiangedu.cn

Go ............. 212
来源：http://pz.panjiajie.cn

Ruby ........... 212
来源：http://am.lnxyls.cn

C# ............. 212
来源：http://ji.9csxet.cn

C .............. 30
来源：http://fb.huixinmuqiang.cn

C++ ............ 30
来源：http://nd.bookmarksfly.cn

SQL ............ 90
来源：http://vw.newstarts.cn

Bash ........... 80
来源：http://gd.9csxet.cn

Kotlin ......... 15
来源：http://il.szxytkj.cn

Swift .......... 15
来源：http://ua.shtwfgs.cn

Lua ............ 10
来源：http://ia.huanxung.cn

Perl ........... 10
来源：http://hr.jctech888.com.cn

Scala .......... 10
来源：http://iv.shxzskj.cn

------------------------------------
来源：http://ag.hnjuh.cn

合计 ........... 2106 条
来源：http://qs.szsharing.cn

按章节统计：
来源：http://pn.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ty.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fw.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vj.bookmarksfly.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xk.yuntaijiaju.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zd.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jl.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nv.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ka.shxzukj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tq.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://en.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://si.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cl.panjiajie.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ax.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://py.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wb.bookmarksfly.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jr.asd995.cn

Q SQL 专题                              90
来源：http://vw.asd995.cn

R Bash 专题                             80
来源：http://xg.newstarts.cn

S C / C++ 专题                          60
来源：http://sb.hnjuh.cn

T 其他语言补充                          60
来源：http://mf.huixinmuqiang.cn

U 高频实用片段                         120
来源：http://op.nszjky.cn

------------------------------------
来源：http://tm.bookmarksfly.cn

合计                                  2106 条
来源：http://ny.newstarts.cn

--------------------------------------------------------------------------------
来源：http://dl.hnjuh.cn

使用提醒
来源：http://pv.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://vi.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://id.hnjuh.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pl.colortex.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://or.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://pg.shxzskj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ag.yuexingan06.cn

—— 文件结束 ——
来源：http://gh.huanxung.cn

================================================================================
来源：http://zp.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://vs.bjjhwx.cn

Common Programming Examples Cheat Book
来源：http://mh.shxzskj.cn

================================================================================
来源：http://ri.haigaiapp.cn

【收录内容】
来源：http://wk.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ju.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://kn.haigaiapp.cn

SQL · Bash · C · C++
来源：http://tx.shxzskj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://km.bookmarksfly.cn

【使用说明】
来源：http://ot.yuexingan06.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wj.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yk.nszjky.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wf.szsharing.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oz.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://kk.huixiangedu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qf.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ni.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://jz.hahajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xb.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lh.asd995.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vx.hahajie.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zs.gzmigu.cn

【文件统计】
来源：http://ow.newstarts.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://pc.colortex.cn

--------------------------------------------------------------------------------
来源：http://yd.muxihuayi.cn

目  录
来源：http://bm.9csxet.cn

--------------------------------------------------------------------------------
来源：http://fi.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zt.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ak.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ju.nszjky.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sk.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xs.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tw.wgjwhj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fu.shxzskj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bp.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ok.panjiajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ua.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pw.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ef.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lm.bookmarksfly.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pw.chemitech.net.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nx.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://nr.hahajie.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bz.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://mu.szxytkj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nj.haigaiapp.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://yz.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cz.jctech888.com.cn

================================================================================
来源：http://sf.jctech888.com.cn

A. 基础语法与类型
来源：http://do.yuntaijiaju.cn

================================================================================
来源：http://nv.hnjuh.cn

[A01] Hello World
来源：http://aj.nszjky.cn

Py:   print("Hello, World!")
来源：http://qd.haigaiapp.cn

PHP:  echo "Hello, World!";
来源：http://iz.shxzukj.cn

JS:   console.log("Hello, World!");
来源：http://vj.huixinmuqiang.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rn.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://hs.muxihuayi.cn

Go:   fmt.Println("Hello, World!")
来源：http://ky.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://at.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://do.szxytkj.cn

[A02] 变量声明与赋值
来源：http://gb.bjjhwx.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ob.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://gt.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://st.nicolike.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gs.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://ei.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://bm.huanxung.cn

Ruby: name = "Alex"; age = 20
来源：http://gl.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zl.bjjhwx.cn

[A03] 常量定义
来源：http://gk.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ja.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://fz.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://ko.jctech888.com.cn

TS:   const PI: number = 3.14159;
来源：http://wk.szsharing.cn

Java: static final double PI = 3.14159;
来源：http://ad.szsharing.cn

Go:   const PI = 3.14159
来源：http://vu.chemitech.net.cn

Ruby: PI = 3.14159
来源：http://gs.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://du.szxytkj.cn

[A04] 判断变量类型
来源：http://uq.huanxung.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jo.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://du.huanxung.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ea.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://an.hahajie.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://pz.chemitech.net.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sd.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://mc.jianghongdianzi.cn

C#:   x.GetType().Name; x is int
来源：http://zl.huixinmuqiang.cn

[A05] 整数除法与取模
来源：http://fc.huixinmuqiang.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mr.asd995.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ck.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ys.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gp.nszjky.cn

Java: 7 / 2; 7 % 2
来源：http://ox.huixinmuqiang.cn

Go:   7 / 2; 7 % 2
来源：http://xr.hahajie.cn

Ruby: 7 / 2; 7 % 2
来源：http://nn.shxzskj.cn

C#:   7 / 2; 7 % 2
来源：http://xr.yuntaijiaju.cn

[A06] 字符串转数字
来源：http://rl.bjjhwx.cn

Py:   int("42"); float("3.14")
来源：http://lr.chemitech.net.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wl.huixiangedu.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dw.panjiajie.cn

TS:   parseInt("42", 10); Number("42")
来源：http://bk.jianghongdianzi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://sk.huixiangedu.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tu.haigaiapp.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://lr.szsharing.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://el.huixinmuqiang.cn

[A07] 数字转字符串
来源：http://pm.hahajie.cn

Py:   str(42)
来源：http://yj.shxzukj.cn

PHP:  (string) 42; strval(42)
来源：http://eg.bookmarksfly.cn


<!-- 参考信息 -->