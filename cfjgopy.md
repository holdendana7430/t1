代发 wailian999

[U53] PHP：空合并运算符
来源：http://cc.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://jv.hnjuh.cn

[U54] PHP：空安全调用
来源：http://wr.nszjky.cn

$obj?->method()
来源：http://lj.szxytkj.cn

[U55] PHP：match 表达式
来源：http://wo.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://py.shtwfgs.cn

[U56] PHP：命名参数
来源：http://kx.shtwfgs.cn

f(a: 1, b: 2)
来源：http://ex.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://sd.521024.cn

"值: {$a}"
来源：http://os.shxzskj.cn

[U58] PHP：数组三件套
来源：http://fa.bookmarksfly.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lx.colortex.cn

[U59] PHP：自定义排序
来源：http://lm.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sz.9csxet.cn

[U60] PHP：JSON 编解码
来源：http://xv.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lv.huanxung.cn

[U61] PHP：正则
来源：http://nh.nicolike.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wl.yuexingan06.cn

[U62] PHP：日期对象
来源：http://rv.haigaiapp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://yr.bjjhwx.cn

[U63] PHP：文件读写
来源：http://rt.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ia.hahajie.cn

[U64] PHP：目录遍历
来源：http://kr.jctech888.com.cn

glob("dir/*.php");  scandir("dir");
来源：http://zb.521024.cn

[U65] PHP：会话
来源：http://mq.jianghongdianzi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ch.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://wf.bjjhwx.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oh.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://xp.chemitech.net.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ro.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://wf.asd995.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tl.521024.cn

[U69] PHP：PDO 预处理
来源：http://gd.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://un.jianghongdianzi.cn

[U70] PHP：PDO 事务
来源：http://of.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tj.colortex.cn

[U71] PHP：抛出异常
来源：http://xi.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://hw.hahajie.cn

[U72] PHP：写错误日志
来源：http://oh.haigaiapp.cn

error_log("失败: " . $e->getMessage());
来源：http://cj.muxihuayi.cn

[U73] PHP：读取 ini 配置
来源：http://hh.jianghongdianzi.cn

parse_ini_file("config.ini", true)
来源：http://zz.bjjhwx.cn

[U74] PHP：读取环境变量
来源：http://kb.hahajie.cn

getenv("APP_ENV") ?: "production"
来源：http://db.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://xb.shxzskj.cn

composer require psr/container
来源：http://pq.yuexingan06.cn

[U76] PHP：简单路由
来源：http://yl.huixiangedu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jr.haigaiapp.cn

[U77] PHP：模板渲染
来源：http://uk.bjjhwx.cn

composer require twig/twig
来源：http://ph.asd995.cn

[U78] PHP：单元测试
来源：http://yo.shxzukj.cn

composer require --dev phpunit/phpunit
来源：http://cp.huixiangedu.cn

[U79] PHP：静态分析
来源：http://yc.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://gz.jianghongdianzi.cn

[U80] PHP：代码规范修复
来源：http://aq.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pg.bjjhwx.cn

[U81] JS：初始化项目
来源：http://kk.huixinmuqiang.cn

npm init -y;  npm i express
来源：http://pc.chemitech.net.cn

[U82] JS：package.json 脚本
来源：http://ah.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fg.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://ic.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://bt.bjjhwx.cn

[U84] JS：CommonJS 写法
来源：http://kd.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bh.shxzskj.cn

[U85] JS：可选链
来源：http://pc.jianghongdianzi.cn

a?.b?.c
来源：http://cv.colortex.cn

[U86] JS：空值合并
来源：http://dv.huixinmuqiang.cn

a ?? b
来源：http://ci.colortex.cn

[U87] JS：解构默认值
来源：http://ee.shxzukj.cn

const { a = 1, b = 2 } = obj;
来源：http://tu.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://lk.bjjhwx.cn

{ ...a, ...b }
来源：http://la.shxzukj.cn

[U89] JS：数组去重
来源：http://gd.yuexingan06.cn

[...new Set(arr)]
来源：http://rx.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://aj.panjiajie.cn

[...arr].sort((a, b) => a - b)
来源：http://bt.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://cj.9csxet.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nm.asd995.cn

[U92] JS：深拷贝
来源：http://fc.hnjuh.cn

structuredClone(obj)
来源：http://yy.wgjwhj.cn

[U93] JS：模板字符串
来源：http://ny.shtwfgs.cn

`共 ${n} 条`
来源：http://as.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://rb.colortex.cn

const double = x => x * 2;
来源：http://bt.shxzskj.cn

[U95] JS：Promise 包装
来源：http://ij.nicolike.cn

new Promise((resolve, reject) => {})
来源：http://lf.yuntaijiaju.cn

[U96] JS：async/await 与异常
来源：http://yg.shtwfgs.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yo.9csxet.cn

[U97] JS：并发请求
来源：http://sp.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ik.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://dc.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dk.bookmarksfly.cn

[U99] JS：事件监听
来源：http://rk.nszjky.cn

el.addEventListener("click", e => {})
来源：http://yd.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://eo.jianghongdianzi.cn

document.querySelector(".item")
来源：http://zy.szsharing.cn

[U101] JS：classList 操作
来源：http://uo.shxzskj.cn

el.classList.toggle("active")
来源：http://op.jctech888.com.cn

[U102] JS：本地存储
来源：http://ed.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jk.asd995.cn

[U103] JS：定时器
来源：http://ai.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ux.wgjwhj.cn

[U104] JS：防抖
来源：http://nn.521024.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vg.shxzukj.cn

[U105] JS：节流
来源：http://rh.nszjky.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fq.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ym.chemitech.net.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dy.shxzukj.cn

[U107] JS：数字千分位
来源：http://pb.nicolike.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rk.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://yr.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ip.huixiangedu.cn

[U109] JS：数组分组
来源：http://ap.haigaiapp.cn

Object.groupBy(arr, x => x.type)
来源：http://fo.asd995.cn

[U110] JS：数组分块
来源：http://zf.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://qi.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://aa.yuntaijiaju.cn

new Map(Object.entries(obj))
来源：http://nu.yuexingan06.cn

[U112] JS：字符串补位
来源：http://sf.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://jj.nicolike.cn

[U113] JS：正则替换全部
来源：http://vi.haigaiapp.cn

s.replaceAll("a", "b")
来源：http://ri.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://qg.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lh.wgjwhj.cn

[U115] JS：生成 UUID
来源：http://iv.chemitech.net.cn

crypto.randomUUID()
来源：http://xz.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://ww.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://ym.newstarts.cn

[U117] JS：单元测试
来源：http://fc.shxzskj.cn

npm i -D vitest;  npx vitest
来源：http://go.haigaiapp.cn

[U118] JS：开发服务器
来源：http://ku.9csxet.cn

npm i -D vite;  npx vite
来源：http://hp.huanxung.cn

[U119] JS：生产构建
来源：http://aw.shxzukj.cn

npx vite build
来源：http://zo.lnxyls.cn

[U120] JS：读取环境变量（Vite）
来源：http://mo.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://ng.huanxung.cn

================================================================================
来源：http://sy.szxytkj.cn

统计汇总
来源：http://yt.jctech888.com.cn

================================================================================
来源：http://jk.chemitech.net.cn

按语言统计（条）：
来源：http://mz.gzmigu.cn

Python ......... 252
来源：http://ju.gzmigu.cn

PHP ............ 252
来源：http://va.shxzukj.cn

JavaScript ..... 252
来源：http://sy.szsharing.cn

TypeScript ..... 212
来源：http://dq.shtwfgs.cn

Java ........... 212
来源：http://cq.yuexingan06.cn

Go ............. 212
来源：http://pr.521024.cn

Ruby ........... 212
来源：http://bg.yuexingan06.cn

C# ............. 212
来源：http://sn.haigaiapp.cn

C .............. 30
来源：http://jl.bookmarksfly.cn

C++ ............ 30
来源：http://zg.chemitech.net.cn

SQL ............ 90
来源：http://vs.jctech888.com.cn

Bash ........... 80
来源：http://yb.szsharing.cn

Kotlin ......... 15
来源：http://pd.huixinmuqiang.cn

Swift .......... 15
来源：http://nh.9csxet.cn

Lua ............ 10
来源：http://xn.yuexingan06.cn

Perl ........... 10
来源：http://rv.shxzukj.cn

Scala .......... 10
来源：http://bk.hahajie.cn

------------------------------------
来源：http://pn.wgjwhj.cn

合计 ........... 2106 条
来源：http://hi.huixinmuqiang.cn

按章节统计：
来源：http://su.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vx.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mr.chemitech.net.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://gx.shxzukj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ch.szxytkj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wv.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ig.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qk.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rk.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vu.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wy.haigaiapp.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tm.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hq.9csxet.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://lo.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://vq.wgjwhj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xe.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qj.gzmigu.cn

Q SQL 专题                              90
来源：http://ru.panjiajie.cn

R Bash 专题                             80
来源：http://ne.jctech888.com.cn

S C / C++ 专题                          60
来源：http://fa.colortex.cn

T 其他语言补充                          60
来源：http://pk.shxzskj.cn

U 高频实用片段                         120
来源：http://pq.huixinmuqiang.cn

------------------------------------
来源：http://fa.521024.cn

合计                                  2106 条
来源：http://ca.9csxet.cn

--------------------------------------------------------------------------------
来源：http://er.9csxet.cn

使用提醒
来源：http://fp.9csxet.cn

--------------------------------------------------------------------------------
来源：http://ln.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ek.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ea.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://po.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xo.bjjhwx.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fd.bookmarksfly.cn

—— 文件结束 ——
来源：http://st.panjiajie.cn

================================================================================
来源：http://wt.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://ba.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://go.yuexingan06.cn

================================================================================
来源：http://iz.jianghongdianzi.cn

【收录内容】
来源：http://gt.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://qp.huixiangedu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://pm.lnxyls.cn

SQL · Bash · C · C++
来源：http://qh.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://bb.muxihuayi.cn

【使用说明】
来源：http://ng.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vk.nicolike.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://il.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iv.panjiajie.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ew.huixinmuqiang.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ph.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mm.hahajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://he.shxzskj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ra.huanxung.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cv.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rd.gzmigu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cf.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://uq.szxytkj.cn

【文件统计】
来源：http://ib.haigaiapp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://nt.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://wz.colortex.cn

目  录
来源：http://cr.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://tg.9csxet.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://he.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ih.chemitech.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wr.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://lq.asd995.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kg.szxytkj.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://xa.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vy.newstarts.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://kl.521024.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ub.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ij.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fw.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ta.yuntaijiaju.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pe.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pg.shxzukj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ng.yuexingan06.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gm.shtwfgs.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://im.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xr.chemitech.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://we.huanxung.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hy.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xg.asd995.cn

================================================================================
来源：http://rb.szxytkj.cn

A. 基础语法与类型
来源：http://ic.bookmarksfly.cn

================================================================================
来源：http://mv.wgjwhj.cn

[A01] Hello World
来源：http://rw.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://ul.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://rz.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://yf.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vl.asd995.cn

Java: System.out.println("Hello, World!");
来源：http://fn.jctech888.com.cn

Go:   fmt.Println("Hello, World!")
来源：http://gk.521024.cn

Ruby: puts "Hello, World!"
来源：http://ii.jctech888.com.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vx.shxzskj.cn

[A02] 变量声明与赋值
来源：http://eh.panjiajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qv.521024.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://sm.bookmarksfly.cn

JS:   let name = "Alex"; const age = 20;
来源：http://rc.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ax.szxytkj.cn

Java: String name = "Alex"; int age = 20;
来源：http://he.newstarts.cn

Go:   name := "Alex"; age := 20
来源：http://fu.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://lr.nszjky.cn

C#:   string name = "Alex"; int age = 20;
来源：http://eo.jctech888.com.cn

[A03] 常量定义
来源：http://dc.gzmigu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bu.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://xs.yuexingan06.cn

JS:   const PI = 3.14159;
来源：http://qu.nszjky.cn

TS:   const PI: number = 3.14159;
来源：http://bo.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://jt.hnjuh.cn

Go:   const PI = 3.14159
来源：http://kd.hnjuh.cn

Ruby: PI = 3.14159
来源：http://dy.huixiangedu.cn

C#:   const double PI = 3.14159;
来源：http://ac.huixinmuqiang.cn

[A04] 判断变量类型
来源：http://id.nszjky.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qm.chemitech.net.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ib.jctech888.com.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ck.huanxung.cn

TS:   typeof x; x instanceof Date
来源：http://wr.huixinmuqiang.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://vq.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gz.bookmarksfly.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ac.jctech888.com.cn

C#:   x.GetType().Name; x is int
来源：http://zd.shtwfgs.cn

[A05] 整数除法与取模
来源：http://xp.yuntaijiaju.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kl.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zz.huanxung.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jx.lnxyls.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://ub.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://kk.hahajie.cn

Go:   7 / 2; 7 % 2
来源：http://ep.gzmigu.cn

Ruby: 7 / 2; 7 % 2
来源：http://if.chemitech.net.cn

C#:   7 / 2; 7 % 2
来源：http://xh.hnjuh.cn

[A06] 字符串转数字
来源：http://jg.newstarts.cn

Py:   int("42"); float("3.14")
来源：http://pk.huixinmuqiang.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xr.lnxyls.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://bn.hnjuh.cn

TS:   parseInt("42", 10); Number("42")
来源：http://yq.shxzukj.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://me.shxzukj.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ql.nszjky.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://sr.muxihuayi.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://te.yuexingan06.cn

[A07] 数字转字符串
来源：http://lt.shxzukj.cn

Py:   str(42)
来源：http://dk.haigaiapp.cn

PHP:  (string) 42; strval(42)
来源：http://uu.huixinmuqiang.cn


<!-- 参考信息 -->