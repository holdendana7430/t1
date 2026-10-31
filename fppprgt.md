代发 wailian999

[U51] PHP：数组解构
来源：http://jh.muxihuayi.cn

[$a, $b] = $arr;
来源：http://wt.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://zg.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://yv.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://fl.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://xv.nicolike.cn

[U54] PHP：空安全调用
来源：http://to.newstarts.cn

$obj?->method()
来源：http://mx.521024.cn

[U55] PHP：match 表达式
来源：http://lw.bjjhwx.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fg.muxihuayi.cn

[U56] PHP：命名参数
来源：http://ur.hahajie.cn

f(a: 1, b: 2)
来源：http://tp.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://ng.gzmigu.cn

"值: {$a}"
来源：http://yo.shxzskj.cn

[U58] PHP：数组三件套
来源：http://dq.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kq.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://gd.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dc.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://xn.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qi.bjjhwx.cn

[U61] PHP：正则
来源：http://bl.9csxet.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ip.muxihuayi.cn

[U62] PHP：日期对象
来源：http://ay.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://at.nicolike.cn

[U63] PHP：文件读写
来源：http://ii.yuntaijiaju.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aa.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://yg.huixiangedu.cn

glob("dir/*.php");  scandir("dir");
来源：http://un.nszjky.cn

[U65] PHP：会话
来源：http://jg.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qn.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://az.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zu.gzmigu.cn

[U67] PHP：处理文件上传
来源：http://sx.hnjuh.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://cv.chemitech.net.cn

[U68] PHP：PDO 连接
来源：http://nr.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lb.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://tt.hnjuh.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sq.szxytkj.cn

[U70] PHP：PDO 事务
来源：http://pa.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://br.panjiajie.cn

[U71] PHP：抛出异常
来源：http://bo.hnjuh.cn

throw new RuntimeException("失败", 500);
来源：http://pm.hnjuh.cn

[U72] PHP：写错误日志
来源：http://ap.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://tl.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://us.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://bt.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://is.shxzskj.cn

getenv("APP_ENV") ?: "production"
来源：http://cb.szsharing.cn

[U75] PHP：依赖注入
来源：http://mt.newstarts.cn

composer require psr/container
来源：http://dm.asd995.cn

[U76] PHP：简单路由
来源：http://uc.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://my.colortex.cn

[U77] PHP：模板渲染
来源：http://jq.huixinmuqiang.cn

composer require twig/twig
来源：http://rb.newstarts.cn

[U78] PHP：单元测试
来源：http://yk.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://fz.yuexingan06.cn

[U79] PHP：静态分析
来源：http://yt.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://ez.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://pj.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yy.asd995.cn

[U81] JS：初始化项目
来源：http://pg.shxzukj.cn

npm init -y;  npm i express
来源：http://al.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://ox.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bt.jctech888.com.cn

[U83] JS：ES Module 导入导出
来源：http://vk.jctech888.com.cn

export const a = 1;  import { a } from "./m.js";
来源：http://xl.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://cw.asd995.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lf.shtwfgs.cn

[U85] JS：可选链
来源：http://dd.bjjhwx.cn

a?.b?.c
来源：http://bg.521024.cn

[U86] JS：空值合并
来源：http://tv.nicolike.cn

a ?? b
来源：http://ho.panjiajie.cn

[U87] JS：解构默认值
来源：http://vr.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://yq.shxzukj.cn

[U88] JS：对象展开合并
来源：http://uz.newstarts.cn

{ ...a, ...b }
来源：http://lf.521024.cn

[U89] JS：数组去重
来源：http://bj.gzmigu.cn

[...new Set(arr)]
来源：http://to.9csxet.cn

[U90] JS：数字数组排序
来源：http://iv.nicolike.cn

[...arr].sort((a, b) => a - b)
来源：http://es.huixinmuqiang.cn

[U91] JS：对象键值遍历
来源：http://ky.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ow.nszjky.cn

[U92] JS：深拷贝
来源：http://vq.huixiangedu.cn

structuredClone(obj)
来源：http://df.chemitech.net.cn

[U93] JS：模板字符串
来源：http://uu.nicolike.cn

`共 ${n} 条`
来源：http://bm.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://ho.lnxyls.cn

const double = x => x * 2;
来源：http://sw.nszjky.cn

[U95] JS：Promise 包装
来源：http://ao.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://qi.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://fx.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zc.bookmarksfly.cn

[U97] JS：并发请求
来源：http://qe.haigaiapp.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pf.asd995.cn

[U98] JS：fetch 带 JSON
来源：http://nb.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://il.panjiajie.cn

[U99] JS：事件监听
来源：http://zw.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://dz.521024.cn

[U100] JS：DOM 查询
来源：http://wr.wgjwhj.cn

document.querySelector(".item")
来源：http://ip.asd995.cn

[U101] JS：classList 操作
来源：http://rn.521024.cn

el.classList.toggle("active")
来源：http://pe.newstarts.cn

[U102] JS：本地存储
来源：http://bs.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ye.chemitech.net.cn

[U103] JS：定时器
来源：http://kp.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://uk.hahajie.cn

[U104] JS：防抖
来源：http://qi.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ar.chemitech.net.cn

[U105] JS：节流
来源：http://lz.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://df.shtwfgs.cn

[U106] JS：日期格式化
来源：http://vd.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ho.yuexingan06.cn

[U107] JS：数字千分位
来源：http://wk.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pe.haigaiapp.cn

[U108] JS：随机整数
来源：http://lm.nicolike.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://nw.szsharing.cn

[U109] JS：数组分组
来源：http://dz.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://me.newstarts.cn

[U110] JS：数组分块
来源：http://yr.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ey.nicolike.cn

[U111] JS：对象转 Map
来源：http://wt.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://ax.muxihuayi.cn

[U112] JS：字符串补位
来源：http://no.hahajie.cn

"7".padStart(3, "0")
来源：http://or.nicolike.cn

[U113] JS：正则替换全部
来源：http://eq.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://wd.lnxyls.cn

[U114] JS：JSON 深比较
来源：http://tj.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qx.nszjky.cn

[U115] JS：生成 UUID
来源：http://tr.lnxyls.cn

crypto.randomUUID()
来源：http://jm.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://ne.huanxung.cn

/** @param {string} name */ function f(name) {}
来源：http://hz.hnjuh.cn

[U117] JS：单元测试
来源：http://ql.wgjwhj.cn

npm i -D vitest;  npx vitest
来源：http://zs.newstarts.cn

[U118] JS：开发服务器
来源：http://ja.lnxyls.cn

npm i -D vite;  npx vite
来源：http://gd.bookmarksfly.cn

[U119] JS：生产构建
来源：http://ha.wgjwhj.cn

npx vite build
来源：http://sp.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://me.bookmarksfly.cn

import.meta.env.VITE_API_URL
来源：http://eu.521024.cn

================================================================================
来源：http://nj.shxzukj.cn

统计汇总
来源：http://ss.bookmarksfly.cn

================================================================================
来源：http://eo.colortex.cn

按语言统计（条）：
来源：http://hw.9csxet.cn

Python ......... 252
来源：http://ot.szxytkj.cn

PHP ............ 252
来源：http://xj.panjiajie.cn

JavaScript ..... 252
来源：http://ak.shtwfgs.cn

TypeScript ..... 212
来源：http://ei.panjiajie.cn

Java ........... 212
来源：http://vl.bjjhwx.cn

Go ............. 212
来源：http://kf.jianghongdianzi.cn

Ruby ........... 212
来源：http://tn.szxytkj.cn

C# ............. 212
来源：http://pz.shtwfgs.cn

C .............. 30
来源：http://wg.shxzskj.cn

C++ ............ 30
来源：http://qd.colortex.cn

SQL ............ 90
来源：http://kf.hnjuh.cn

Bash ........... 80
来源：http://bc.szxytkj.cn

Kotlin ......... 15
来源：http://ej.lnxyls.cn

Swift .......... 15
来源：http://jc.yuexingan06.cn

Lua ............ 10
来源：http://zt.shxzukj.cn

Perl ........... 10
来源：http://yg.nicolike.cn

Scala .......... 10
来源：http://ij.gzmigu.cn

------------------------------------
来源：http://hd.lnxyls.cn

合计 ........... 2106 条
来源：http://xn.bookmarksfly.cn

按章节统计：
来源：http://zm.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vp.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dd.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lz.yuntaijiaju.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ly.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ne.gzmigu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hp.szsharing.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nj.nszjky.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pr.hahajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ao.shtwfgs.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sx.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://va.shxzskj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qq.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://he.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ui.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://om.wgjwhj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fg.asd995.cn

Q SQL 专题                              90
来源：http://iy.hnjuh.cn

R Bash 专题                             80
来源：http://tc.wgjwhj.cn

S C / C++ 专题                          60
来源：http://yk.521024.cn

T 其他语言补充                          60
来源：http://dq.9csxet.cn

U 高频实用片段                         120
来源：http://dp.huixinmuqiang.cn

------------------------------------
来源：http://mo.asd995.cn

合计                                  2106 条
来源：http://td.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://cp.lnxyls.cn

使用提醒
来源：http://ah.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://kq.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rj.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fw.szxytkj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ky.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://cp.9csxet.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zh.hahajie.cn

—— 文件结束 ——
来源：http://vo.yuexingan06.cn

================================================================================
来源：http://fd.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://ea.haigaiapp.cn

Common Programming Examples Cheat Book
来源：http://td.jctech888.com.cn

================================================================================
来源：http://en.bookmarksfly.cn

【收录内容】
来源：http://dt.bjjhwx.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://oz.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://au.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://ut.wgjwhj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vj.panjiajie.cn

【使用说明】
来源：http://es.bookmarksfly.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nn.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bf.hnjuh.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pk.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sy.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://li.panjiajie.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://oz.yuexingan06.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jm.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://cv.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ab.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://lf.hnjuh.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://uw.yuntaijiaju.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://st.lnxyls.cn

【文件统计】
来源：http://qa.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vb.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ew.jianghongdianzi.cn

目  录
来源：http://wq.shxzukj.cn

--------------------------------------------------------------------------------
来源：http://ve.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://sx.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qd.nicolike.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qu.huixiangedu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://oi.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gc.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://jg.jianghongdianzi.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rh.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://au.hnjuh.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://le.hnjuh.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pe.muxihuayi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sz.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://uh.szsharing.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dn.muxihuayi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://fr.hnjuh.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rp.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://xu.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jc.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://do.huanxung.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qt.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://tn.nszjky.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://cp.muxihuayi.cn

================================================================================
来源：http://yx.jctech888.com.cn

A. 基础语法与类型
来源：http://hm.szxytkj.cn

================================================================================
来源：http://dx.panjiajie.cn

[A01] Hello World
来源：http://mj.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://hm.nicolike.cn

PHP:  echo "Hello, World!";
来源：http://jg.muxihuayi.cn

JS:   console.log("Hello, World!");
来源：http://gp.lnxyls.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pd.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://jl.nszjky.cn

Go:   fmt.Println("Hello, World!")
来源：http://mk.colortex.cn

Ruby: puts "Hello, World!"
来源：http://lh.shtwfgs.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://kj.huanxung.cn

[A02] 变量声明与赋值
来源：http://zn.huixiangedu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://bh.bookmarksfly.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://dc.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://sr.shxzukj.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hd.9csxet.cn

Java: String name = "Alex"; int age = 20;
来源：http://bf.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ok.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://hf.lnxyls.cn

C#:   string name = "Alex"; int age = 20;
来源：http://vm.haigaiapp.cn

[A03] 常量定义
来源：http://dq.shxzskj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pq.shxzskj.cn

PHP:  const PI = 3.14159;
来源：http://fk.shtwfgs.cn

JS:   const PI = 3.14159;
来源：http://my.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://wu.jctech888.com.cn

Java: static final double PI = 3.14159;
来源：http://ip.huixinmuqiang.cn

Go:   const PI = 3.14159
来源：http://at.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://el.haigaiapp.cn

C#:   const double PI = 3.14159;
来源：http://oo.colortex.cn

[A04] 判断变量类型
来源：http://sx.muxihuayi.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ia.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wk.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fh.bookmarksfly.cn

TS:   typeof x; x instanceof Date
来源：http://tg.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ez.lnxyls.cn

Go:   reflect.TypeOf(x).Name()
来源：http://vs.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lp.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://kn.szxytkj.cn

[A05] 整数除法与取模
来源：http://ap.jianghongdianzi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://sz.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://qq.nicolike.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://uv.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jg.lnxyls.cn

Java: 7 / 2; 7 % 2
来源：http://mw.huixiangedu.cn

Go:   7 / 2; 7 % 2
来源：http://zt.szxytkj.cn

Ruby: 7 / 2; 7 % 2
来源：http://qb.huixiangedu.cn

C#:   7 / 2; 7 % 2
来源：http://ue.szxytkj.cn

[A06] 字符串转数字
来源：http://iq.szxytkj.cn

Py:   int("42"); float("3.14")
来源：http://uz.jianghongdianzi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://hb.chemitech.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://vn.nszjky.cn

TS:   parseInt("42", 10); Number("42")
来源：http://as.bookmarksfly.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fs.hahajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zx.yuexingan06.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fi.haigaiapp.cn


<!-- 参考信息 -->