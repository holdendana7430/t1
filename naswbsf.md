代发 wailian999

[U51] PHP：数组解构
来源：http://vj.muxihuayi.cn

[$a, $b] = $arr;
来源：http://ac.szsharing.cn

[U52] PHP：箭头函数
来源：http://al.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://et.hahajie.cn

[U53] PHP：空合并运算符
来源：http://dr.lnxyls.cn

$v = $a ?? $b ?? "default";
来源：http://kl.nszjky.cn

[U54] PHP：空安全调用
来源：http://fh.hahajie.cn

$obj?->method()
来源：http://me.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://jl.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://to.shxzskj.cn

[U56] PHP：命名参数
来源：http://aw.colortex.cn

f(a: 1, b: 2)
来源：http://lp.nicolike.cn

[U57] PHP：字符串插值
来源：http://ov.szxytkj.cn

"值: {$a}"
来源：http://ki.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://lw.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jv.jctech888.com.cn

[U59] PHP：自定义排序
来源：http://re.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ti.jctech888.com.cn

[U60] PHP：JSON 编解码
来源：http://hq.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ou.521024.cn

[U61] PHP：正则
来源：http://vn.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hz.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://gy.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ik.yuntaijiaju.cn

[U63] PHP：文件读写
来源：http://fj.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zw.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://vg.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://vv.yuexingan06.cn

[U65] PHP：会话
来源：http://bp.yuntaijiaju.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dv.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://sa.huanxung.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://kq.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://jv.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zo.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://nd.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://gt.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://wk.nszjky.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fz.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://hh.yuntaijiaju.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mh.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://hp.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://ax.nicolike.cn

[U72] PHP：写错误日志
来源：http://rd.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://qi.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://wj.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://pw.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://xc.newstarts.cn

getenv("APP_ENV") ?: "production"
来源：http://vx.chemitech.net.cn

[U75] PHP：依赖注入
来源：http://gl.huixiangedu.cn

composer require psr/container
来源：http://yc.szsharing.cn

[U76] PHP：简单路由
来源：http://dg.jianghongdianzi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kf.lnxyls.cn

[U77] PHP：模板渲染
来源：http://qn.nicolike.cn

composer require twig/twig
来源：http://mn.yuexingan06.cn

[U78] PHP：单元测试
来源：http://ej.shxzskj.cn

composer require --dev phpunit/phpunit
来源：http://mw.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://eo.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://lc.colortex.cn

[U80] PHP：代码规范修复
来源：http://yq.jianghongdianzi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hz.jctech888.com.cn

[U81] JS：初始化项目
来源：http://tt.nszjky.cn

npm init -y;  npm i express
来源：http://gt.521024.cn

[U82] JS：package.json 脚本
来源：http://tw.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wm.nszjky.cn

[U83] JS：ES Module 导入导出
来源：http://ir.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fj.hahajie.cn

[U84] JS：CommonJS 写法
来源：http://cx.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ii.shxzskj.cn

[U85] JS：可选链
来源：http://qu.9csxet.cn

a?.b?.c
来源：http://zp.9csxet.cn

[U86] JS：空值合并
来源：http://xf.chemitech.net.cn

a ?? b
来源：http://xb.hnjuh.cn

[U87] JS：解构默认值
来源：http://qz.haigaiapp.cn

const { a = 1, b = 2 } = obj;
来源：http://cm.521024.cn

[U88] JS：对象展开合并
来源：http://ks.hahajie.cn

{ ...a, ...b }
来源：http://vo.hnjuh.cn

[U89] JS：数组去重
来源：http://pb.nszjky.cn

[...new Set(arr)]
来源：http://ee.jianghongdianzi.cn

[U90] JS：数字数组排序
来源：http://iq.wgjwhj.cn

[...arr].sort((a, b) => a - b)
来源：http://to.bookmarksfly.cn

[U91] JS：对象键值遍历
来源：http://xm.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ho.hnjuh.cn

[U92] JS：深拷贝
来源：http://ei.huanxung.cn

structuredClone(obj)
来源：http://dk.shxzskj.cn

[U93] JS：模板字符串
来源：http://gn.jctech888.com.cn

`共 ${n} 条`
来源：http://jg.9csxet.cn

[U94] JS：箭头函数
来源：http://wa.9csxet.cn

const double = x => x * 2;
来源：http://ax.shtwfgs.cn

[U95] JS：Promise 包装
来源：http://cl.bjjhwx.cn

new Promise((resolve, reject) => {})
来源：http://dd.panjiajie.cn

[U96] JS：async/await 与异常
来源：http://ni.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lv.huixiangedu.cn

[U97] JS：并发请求
来源：http://yr.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fv.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://mp.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bw.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://ar.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://es.asd995.cn

[U100] JS：DOM 查询
来源：http://vw.szsharing.cn

document.querySelector(".item")
来源：http://lt.lnxyls.cn

[U101] JS：classList 操作
来源：http://av.muxihuayi.cn

el.classList.toggle("active")
来源：http://in.hahajie.cn

[U102] JS：本地存储
来源：http://wl.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://so.panjiajie.cn

[U103] JS：定时器
来源：http://od.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ag.huixiangedu.cn

[U104] JS：防抖
来源：http://sy.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ps.panjiajie.cn

[U105] JS：节流
来源：http://py.newstarts.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qe.nicolike.cn

[U106] JS：日期格式化
来源：http://mu.szxytkj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xn.jctech888.com.cn

[U107] JS：数字千分位
来源：http://tn.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ad.yuexingan06.cn

[U108] JS：随机整数
来源：http://dq.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tt.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://fy.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://ly.9csxet.cn

[U110] JS：数组分块
来源：http://qx.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rl.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://yy.521024.cn

new Map(Object.entries(obj))
来源：http://jp.huanxung.cn

[U112] JS：字符串补位
来源：http://uc.szxytkj.cn

"7".padStart(3, "0")
来源：http://ar.shxzukj.cn

[U113] JS：正则替换全部
来源：http://bl.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://ca.panjiajie.cn

[U114] JS：JSON 深比较
来源：http://qs.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qy.shxzukj.cn

[U115] JS：生成 UUID
来源：http://nm.chemitech.net.cn

crypto.randomUUID()
来源：http://ag.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://by.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://cg.asd995.cn

[U117] JS：单元测试
来源：http://gf.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://gi.colortex.cn

[U118] JS：开发服务器
来源：http://qw.lnxyls.cn

npm i -D vite;  npx vite
来源：http://li.bjjhwx.cn

[U119] JS：生产构建
来源：http://oh.yuntaijiaju.cn

npx vite build
来源：http://ko.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://mn.bjjhwx.cn

import.meta.env.VITE_API_URL
来源：http://em.yuexingan06.cn

================================================================================
来源：http://rn.huanxung.cn

统计汇总
来源：http://ks.bjjhwx.cn

================================================================================
来源：http://bi.yuexingan06.cn

按语言统计（条）：
来源：http://na.muxihuayi.cn

Python ......... 252
来源：http://jj.shtwfgs.cn

PHP ............ 252
来源：http://ej.shxzukj.cn

JavaScript ..... 252
来源：http://bo.bjjhwx.cn

TypeScript ..... 212
来源：http://tz.yuexingan06.cn

Java ........... 212
来源：http://fd.huanxung.cn

Go ............. 212
来源：http://tf.hnjuh.cn

Ruby ........... 212
来源：http://ry.yuntaijiaju.cn

C# ............. 212
来源：http://sl.yuntaijiaju.cn

C .............. 30
来源：http://ng.lnxyls.cn

C++ ............ 30
来源：http://nd.wgjwhj.cn

SQL ............ 90
来源：http://re.szsharing.cn

Bash ........... 80
来源：http://sl.colortex.cn

Kotlin ......... 15
来源：http://bc.wgjwhj.cn

Swift .......... 15
来源：http://ty.chemitech.net.cn

Lua ............ 10
来源：http://tl.gzmigu.cn

Perl ........... 10
来源：http://dh.yuntaijiaju.cn

Scala .......... 10
来源：http://di.szxytkj.cn

------------------------------------
来源：http://ux.hahajie.cn

合计 ........... 2106 条
来源：http://xn.bookmarksfly.cn

按章节统计：
来源：http://il.huixinmuqiang.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ki.chemitech.net.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ye.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fz.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ww.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ba.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sz.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xp.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://of.521024.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ou.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://es.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oi.colortex.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xf.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://dq.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vi.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://on.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hc.lnxyls.cn

Q SQL 专题                              90
来源：http://ra.9csxet.cn

R Bash 专题                             80
来源：http://vq.hahajie.cn

S C / C++ 专题                          60
来源：http://vf.chemitech.net.cn

T 其他语言补充                          60
来源：http://mu.newstarts.cn

U 高频实用片段                         120
来源：http://tb.nicolike.cn

------------------------------------
来源：http://br.shxzskj.cn

合计                                  2106 条
来源：http://go.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://qv.gzmigu.cn

使用提醒
来源：http://fy.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ga.gzmigu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hs.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ry.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://af.bjjhwx.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ca.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mo.yuntaijiaju.cn

—— 文件结束 ——
来源：http://id.haigaiapp.cn

================================================================================
来源：http://ia.szsharing.cn

程序语言常见例子速查手册（2024 版）
来源：http://ru.chemitech.net.cn

Common Programming Examples Cheat Book
来源：http://yw.yuexingan06.cn

================================================================================
来源：http://iz.bookmarksfly.cn

【收录内容】
来源：http://sq.hahajie.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zr.asd995.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gj.hahajie.cn

SQL · Bash · C · C++
来源：http://mt.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pq.huixiangedu.cn

【使用说明】
来源：http://qp.nszjky.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gr.jianghongdianzi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://nu.szsharing.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://or.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tx.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://cl.hahajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://is.hnjuh.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vq.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://io.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://di.szsharing.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tl.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oe.shtwfgs.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mo.9csxet.cn

【文件统计】
来源：http://kj.yuntaijiaju.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ti.521024.cn

--------------------------------------------------------------------------------
来源：http://ux.bjjhwx.cn

目  录
来源：http://xr.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://rx.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://uo.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://dk.szxytkj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tz.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dn.bjjhwx.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dm.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://sv.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dq.asd995.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mm.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jd.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jy.nszjky.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://bu.hahajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ar.hnjuh.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ed.panjiajie.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://tg.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ca.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mu.nszjky.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pb.nszjky.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://pt.huixiangedu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ug.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pv.szsharing.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ak.jctech888.com.cn

================================================================================
来源：http://vt.shxzukj.cn

A. 基础语法与类型
来源：http://rq.chemitech.net.cn

================================================================================
来源：http://td.huixiangedu.cn

[A01] Hello World
来源：http://xt.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ue.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://ms.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://ez.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://am.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://yv.hnjuh.cn

Go:   fmt.Println("Hello, World!")
来源：http://gs.jianghongdianzi.cn

Ruby: puts "Hello, World!"
来源：http://qj.huixinmuqiang.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://bz.huixinmuqiang.cn

[A02] 变量声明与赋值
来源：http://lc.huanxung.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://td.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://np.muxihuayi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ow.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xe.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://az.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://kq.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://tc.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xl.nicolike.cn

[A03] 常量定义
来源：http://qs.huixinmuqiang.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://hb.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://tb.jctech888.com.cn

JS:   const PI = 3.14159;
来源：http://hy.asd995.cn

TS:   const PI: number = 3.14159;
来源：http://et.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://ig.521024.cn

Go:   const PI = 3.14159
来源：http://vw.yuntaijiaju.cn

Ruby: PI = 3.14159
来源：http://px.nicolike.cn

C#:   const double PI = 3.14159;
来源：http://js.shxzukj.cn

[A04] 判断变量类型
来源：http://ul.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://iz.shxzukj.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tb.lnxyls.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hv.huixinmuqiang.cn

TS:   typeof x; x instanceof Date
来源：http://az.wgjwhj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mq.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ae.nicolike.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xn.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://lz.bookmarksfly.cn

[A05] 整数除法与取模
来源：http://un.muxihuayi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://az.521024.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://lo.yuntaijiaju.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cc.haigaiapp.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gj.wgjwhj.cn

Java: 7 / 2; 7 % 2
来源：http://bb.gzmigu.cn

Go:   7 / 2; 7 % 2
来源：http://dt.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://wj.nszjky.cn

C#:   7 / 2; 7 % 2
来源：http://gy.hnjuh.cn

[A06] 字符串转数字
来源：http://fc.hnjuh.cn

Py:   int("42"); float("3.14")
来源：http://sw.bookmarksfly.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://et.shxzukj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wr.jianghongdianzi.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vt.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://it.bjjhwx.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://qy.huanxung.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://qi.szsharing.cn


<!-- 参考信息 -->