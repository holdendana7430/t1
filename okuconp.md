代发 wailian999

[U51] PHP：数组解构
来源：http://dz.huixiangedu.cn

[$a, $b] = $arr;
来源：http://ur.shxzskj.cn

[U52] PHP：箭头函数
来源：http://ct.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://oc.asd995.cn

[U53] PHP：空合并运算符
来源：http://nl.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://hw.nszjky.cn

[U54] PHP：空安全调用
来源：http://al.chemitech.net.cn

$obj?->method()
来源：http://xz.521024.cn

[U55] PHP：match 表达式
来源：http://ug.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ir.szsharing.cn

[U56] PHP：命名参数
来源：http://ip.szxytkj.cn

f(a: 1, b: 2)
来源：http://bq.shtwfgs.cn

[U57] PHP：字符串插值
来源：http://hq.wgjwhj.cn

"值: {$a}"
来源：http://ry.colortex.cn

[U58] PHP：数组三件套
来源：http://kc.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ml.muxihuayi.cn

[U59] PHP：自定义排序
来源：http://ic.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dd.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://fn.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://os.521024.cn

[U61] PHP：正则
来源：http://pk.jianghongdianzi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qw.521024.cn

[U62] PHP：日期对象
来源：http://vd.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zf.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://gz.muxihuayi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rb.gzmigu.cn

[U64] PHP：目录遍历
来源：http://kj.nicolike.cn

glob("dir/*.php");  scandir("dir");
来源：http://od.jianghongdianzi.cn

[U65] PHP：会话
来源：http://hw.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://do.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://qp.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://be.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://yf.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ja.nszjky.cn

[U68] PHP：PDO 连接
来源：http://yk.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://pt.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://te.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jn.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://kq.gzmigu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dh.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://xc.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://te.shxzskj.cn

[U72] PHP：写错误日志
来源：http://ve.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://ot.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://zx.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://tc.asd995.cn

[U74] PHP：读取环境变量
来源：http://ml.521024.cn

getenv("APP_ENV") ?: "production"
来源：http://xg.szsharing.cn

[U75] PHP：依赖注入
来源：http://pe.nicolike.cn

composer require psr/container
来源：http://gx.9csxet.cn

[U76] PHP：简单路由
来源：http://xi.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oz.hnjuh.cn

[U77] PHP：模板渲染
来源：http://yp.huanxung.cn

composer require twig/twig
来源：http://qz.wgjwhj.cn

[U78] PHP：单元测试
来源：http://yw.haigaiapp.cn

composer require --dev phpunit/phpunit
来源：http://kp.colortex.cn

[U79] PHP：静态分析
来源：http://ml.chemitech.net.cn

composer require --dev phpstan/phpstan
来源：http://gq.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://tv.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kt.9csxet.cn

[U81] JS：初始化项目
来源：http://zy.newstarts.cn

npm init -y;  npm i express
来源：http://fm.szsharing.cn

[U82] JS：package.json 脚本
来源：http://on.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ri.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://yi.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://lj.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://kl.hnjuh.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ny.shxzskj.cn

[U85] JS：可选链
来源：http://sa.huixinmuqiang.cn

a?.b?.c
来源：http://iq.shxzskj.cn

[U86] JS：空值合并
来源：http://gr.bookmarksfly.cn

a ?? b
来源：http://jn.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://ap.szxytkj.cn

const { a = 1, b = 2 } = obj;
来源：http://ik.newstarts.cn

[U88] JS：对象展开合并
来源：http://jx.huixinmuqiang.cn

{ ...a, ...b }
来源：http://nv.9csxet.cn

[U89] JS：数组去重
来源：http://sd.521024.cn

[...new Set(arr)]
来源：http://yf.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://lm.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://tn.hnjuh.cn

[U91] JS：对象键值遍历
来源：http://tx.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sg.haigaiapp.cn

[U92] JS：深拷贝
来源：http://nh.huanxung.cn

structuredClone(obj)
来源：http://gn.newstarts.cn

[U93] JS：模板字符串
来源：http://fb.hnjuh.cn

`共 ${n} 条`
来源：http://ie.haigaiapp.cn

[U94] JS：箭头函数
来源：http://os.hahajie.cn

const double = x => x * 2;
来源：http://bu.newstarts.cn

[U95] JS：Promise 包装
来源：http://eq.gzmigu.cn

new Promise((resolve, reject) => {})
来源：http://om.hnjuh.cn

[U96] JS：async/await 与异常
来源：http://lq.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ew.hahajie.cn

[U97] JS：并发请求
来源：http://bt.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ob.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://bz.wgjwhj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://io.wgjwhj.cn

[U99] JS：事件监听
来源：http://jq.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://xi.szsharing.cn

[U100] JS：DOM 查询
来源：http://pk.chemitech.net.cn

document.querySelector(".item")
来源：http://uz.shxzukj.cn

[U101] JS：classList 操作
来源：http://xl.panjiajie.cn

el.classList.toggle("active")
来源：http://yx.gzmigu.cn

[U102] JS：本地存储
来源：http://fi.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rm.bjjhwx.cn

[U103] JS：定时器
来源：http://oq.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lt.521024.cn

[U104] JS：防抖
来源：http://in.szsharing.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xp.huixiangedu.cn

[U105] JS：节流
来源：http://rt.muxihuayi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qh.colortex.cn

[U106] JS：日期格式化
来源：http://ca.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bl.yuexingan06.cn

[U107] JS：数字千分位
来源：http://yn.yuntaijiaju.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://lq.haigaiapp.cn

[U108] JS：随机整数
来源：http://xm.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bi.colortex.cn

[U109] JS：数组分组
来源：http://cp.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://gr.yuntaijiaju.cn

[U110] JS：数组分块
来源：http://ox.szxytkj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qj.yuntaijiaju.cn

[U111] JS：对象转 Map
来源：http://fz.haigaiapp.cn

new Map(Object.entries(obj))
来源：http://br.bjjhwx.cn

[U112] JS：字符串补位
来源：http://ig.bookmarksfly.cn

"7".padStart(3, "0")
来源：http://eu.bookmarksfly.cn

[U113] JS：正则替换全部
来源：http://kl.bjjhwx.cn

s.replaceAll("a", "b")
来源：http://rd.nicolike.cn

[U114] JS：JSON 深比较
来源：http://ap.panjiajie.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hy.nszjky.cn

[U115] JS：生成 UUID
来源：http://vs.muxihuayi.cn

crypto.randomUUID()
来源：http://ge.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://ki.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://uz.lnxyls.cn

[U117] JS：单元测试
来源：http://rg.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://lk.gzmigu.cn

[U118] JS：开发服务器
来源：http://gg.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://tt.hnjuh.cn

[U119] JS：生产构建
来源：http://au.hnjuh.cn

npx vite build
来源：http://hv.huixiangedu.cn

[U120] JS：读取环境变量（Vite）
来源：http://sj.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://ye.bookmarksfly.cn

================================================================================
来源：http://yh.huanxung.cn

统计汇总
来源：http://rk.hnjuh.cn

================================================================================
来源：http://cx.shxzukj.cn

按语言统计（条）：
来源：http://xs.yuntaijiaju.cn

Python ......... 252
来源：http://hd.nicolike.cn

PHP ............ 252
来源：http://ge.szsharing.cn

JavaScript ..... 252
来源：http://vc.nicolike.cn

TypeScript ..... 212
来源：http://on.szsharing.cn

Java ........... 212
来源：http://mt.shtwfgs.cn

Go ............. 212
来源：http://rg.jianghongdianzi.cn

Ruby ........... 212
来源：http://yw.colortex.cn

C# ............. 212
来源：http://oz.hahajie.cn

C .............. 30
来源：http://re.huixinmuqiang.cn

C++ ............ 30
来源：http://zp.jctech888.com.cn

SQL ............ 90
来源：http://tb.bookmarksfly.cn

Bash ........... 80
来源：http://rx.szsharing.cn

Kotlin ......... 15
来源：http://oc.szsharing.cn

Swift .......... 15
来源：http://vq.asd995.cn

Lua ............ 10
来源：http://rt.hahajie.cn

Perl ........... 10
来源：http://gm.521024.cn

Scala .......... 10
来源：http://or.nszjky.cn

------------------------------------
来源：http://vi.szsharing.cn

合计 ........... 2106 条
来源：http://xm.jianghongdianzi.cn

按章节统计：
来源：http://kd.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ox.huixinmuqiang.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://st.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zj.asd995.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pm.wgjwhj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ca.muxihuayi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://zr.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jv.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://dg.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gs.bjjhwx.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://km.asd995.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ie.huanxung.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://jz.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://in.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ed.gzmigu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hf.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ov.haigaiapp.cn

Q SQL 专题                              90
来源：http://lo.nicolike.cn

R Bash 专题                             80
来源：http://kn.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://bo.panjiajie.cn

T 其他语言补充                          60
来源：http://ok.hnjuh.cn

U 高频实用片段                         120
来源：http://fq.colortex.cn

------------------------------------
来源：http://rn.shtwfgs.cn

合计                                  2106 条
来源：http://ml.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ni.shxzskj.cn

使用提醒
来源：http://ap.newstarts.cn

--------------------------------------------------------------------------------
来源：http://cf.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ao.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ej.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://fa.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://yw.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://kj.asd995.cn

—— 文件结束 ——
来源：http://cv.colortex.cn

================================================================================
来源：http://bm.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://xh.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://xb.chemitech.net.cn

================================================================================
来源：http://wf.bookmarksfly.cn

【收录内容】
来源：http://pe.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jg.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://cd.hnjuh.cn

SQL · Bash · C · C++
来源：http://yw.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xz.521024.cn

【使用说明】
来源：http://iy.521024.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sq.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yq.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://fo.gzmigu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dd.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ih.hnjuh.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zb.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://en.colortex.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gq.panjiajie.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rp.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://tl.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mi.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uw.huixinmuqiang.cn

【文件统计】
来源：http://ve.chemitech.net.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tb.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ys.szxytkj.cn

目  录
来源：http://hu.hahajie.cn

--------------------------------------------------------------------------------
来源：http://hg.wgjwhj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vv.hahajie.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qw.bookmarksfly.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xi.szxytkj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://av.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ms.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lg.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://so.bjjhwx.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://sn.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aq.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mp.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://by.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hl.newstarts.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://eg.jianghongdianzi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ei.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cd.muxihuayi.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lt.shxzskj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dw.colortex.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zp.asd995.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oa.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fg.jctech888.com.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://jg.bjjhwx.cn

================================================================================
来源：http://ua.hahajie.cn

A. 基础语法与类型
来源：http://ti.colortex.cn

================================================================================
来源：http://yj.huixinmuqiang.cn

[A01] Hello World
来源：http://rx.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ut.szxytkj.cn

PHP:  echo "Hello, World!";
来源：http://rw.szxytkj.cn

JS:   console.log("Hello, World!");
来源：http://pq.shxzukj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cl.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://mx.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://yu.huanxung.cn

Ruby: puts "Hello, World!"
来源：http://go.nicolike.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ft.colortex.cn

[A02] 变量声明与赋值
来源：http://gk.yuntaijiaju.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gw.shxzukj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sq.lnxyls.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ki.9csxet.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bm.521024.cn

Java: String name = "Alex"; int age = 20;
来源：http://iz.wgjwhj.cn

Go:   name := "Alex"; age := 20
来源：http://ys.shtwfgs.cn

Ruby: name = "Alex"; age = 20
来源：http://uz.chemitech.net.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ut.nicolike.cn

[A03] 常量定义
来源：http://xd.wgjwhj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://qd.yuntaijiaju.cn

PHP:  const PI = 3.14159;
来源：http://yu.colortex.cn

JS:   const PI = 3.14159;
来源：http://ye.shxzukj.cn

TS:   const PI: number = 3.14159;
来源：http://ds.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://qv.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://qj.gzmigu.cn

Ruby: PI = 3.14159
来源：http://pk.hnjuh.cn

C#:   const double PI = 3.14159;
来源：http://qa.huanxung.cn

[A04] 判断变量类型
来源：http://pf.9csxet.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jm.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ga.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zp.jianghongdianzi.cn

TS:   typeof x; x instanceof Date
来源：http://ij.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://hx.9csxet.cn

Go:   reflect.TypeOf(x).Name()
来源：http://rm.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://oy.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://kd.yuntaijiaju.cn

[A05] 整数除法与取模
来源：http://aw.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://al.yuntaijiaju.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ii.shxzukj.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://hv.bjjhwx.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gf.521024.cn

Java: 7 / 2; 7 % 2
来源：http://lj.nszjky.cn

Go:   7 / 2; 7 % 2
来源：http://nf.lnxyls.cn

Ruby: 7 / 2; 7 % 2
来源：http://eu.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://vy.szsharing.cn

[A06] 字符串转数字
来源：http://pc.shxzukj.cn

Py:   int("42"); float("3.14")
来源：http://fx.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://dd.yuexingan06.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://fg.szsharing.cn

TS:   parseInt("42", 10); Number("42")
来源：http://gp.newstarts.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wf.huanxung.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://iq.hnjuh.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://df.nszjky.cn


<!-- 参考信息 -->