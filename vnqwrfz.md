代发 wailian999

[U53] PHP：空合并运算符
来源：http://te.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://xz.colortex.cn

[U54] PHP：空安全调用
来源：http://hq.newstarts.cn

$obj?->method()
来源：http://vh.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://ps.yuntaijiaju.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nd.huanxung.cn

[U56] PHP：命名参数
来源：http://tn.lnxyls.cn

f(a: 1, b: 2)
来源：http://un.hahajie.cn

[U57] PHP：字符串插值
来源：http://bu.haigaiapp.cn

"值: {$a}"
来源：http://lq.shxzskj.cn

[U58] PHP：数组三件套
来源：http://ox.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qh.szsharing.cn

[U59] PHP：自定义排序
来源：http://tf.asd995.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rz.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://tz.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://hx.chemitech.net.cn

[U61] PHP：正则
来源：http://aj.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sl.chemitech.net.cn

[U62] PHP：日期对象
来源：http://ee.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ug.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://pg.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hs.yuntaijiaju.cn

[U64] PHP：目录遍历
来源：http://tm.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://be.yuntaijiaju.cn

[U65] PHP：会话
来源：http://xu.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ca.szsharing.cn

[U66] PHP：设置 Cookie
来源：http://qb.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ex.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://vq.huanxung.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://us.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://va.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ys.newstarts.cn

[U69] PHP：PDO 预处理
来源：http://ur.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hb.521024.cn

[U70] PHP：PDO 事务
来源：http://ms.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dy.huanxung.cn

[U71] PHP：抛出异常
来源：http://dg.haigaiapp.cn

throw new RuntimeException("失败", 500);
来源：http://se.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://iu.shxzukj.cn

error_log("失败: " . $e->getMessage());
来源：http://sz.bookmarksfly.cn

[U73] PHP：读取 ini 配置
来源：http://mz.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://bh.huixinmuqiang.cn

[U74] PHP：读取环境变量
来源：http://ar.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://xa.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://dw.nszjky.cn

composer require psr/container
来源：http://xh.9csxet.cn

[U76] PHP：简单路由
来源：http://bi.huanxung.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://am.nicolike.cn

[U77] PHP：模板渲染
来源：http://tl.521024.cn

composer require twig/twig
来源：http://cs.asd995.cn

[U78] PHP：单元测试
来源：http://oj.9csxet.cn

composer require --dev phpunit/phpunit
来源：http://pa.yuexingan06.cn

[U79] PHP：静态分析
来源：http://ci.panjiajie.cn

composer require --dev phpstan/phpstan
来源：http://wg.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://dv.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://uy.shtwfgs.cn

[U81] JS：初始化项目
来源：http://or.newstarts.cn

npm init -y;  npm i express
来源：http://eg.nszjky.cn

[U82] JS：package.json 脚本
来源：http://kv.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ps.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://by.huixinmuqiang.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ao.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://yp.yuexingan06.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gi.gzmigu.cn

[U85] JS：可选链
来源：http://jr.shxzskj.cn

a?.b?.c
来源：http://nz.huixiangedu.cn

[U86] JS：空值合并
来源：http://br.bjjhwx.cn

a ?? b
来源：http://cx.haigaiapp.cn

[U87] JS：解构默认值
来源：http://ph.huixinmuqiang.cn

const { a = 1, b = 2 } = obj;
来源：http://fj.newstarts.cn

[U88] JS：对象展开合并
来源：http://qv.yuntaijiaju.cn

{ ...a, ...b }
来源：http://ku.yuexingan06.cn

[U89] JS：数组去重
来源：http://bf.shxzukj.cn

[...new Set(arr)]
来源：http://ms.huanxung.cn

[U90] JS：数字数组排序
来源：http://ap.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://ej.9csxet.cn

[U91] JS：对象键值遍历
来源：http://ru.bjjhwx.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gn.hnjuh.cn

[U92] JS：深拷贝
来源：http://la.muxihuayi.cn

structuredClone(obj)
来源：http://hu.colortex.cn

[U93] JS：模板字符串
来源：http://li.colortex.cn

`共 ${n} 条`
来源：http://dn.yuexingan06.cn

[U94] JS：箭头函数
来源：http://co.lnxyls.cn

const double = x => x * 2;
来源：http://nn.521024.cn

[U95] JS：Promise 包装
来源：http://pv.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://cb.colortex.cn

[U96] JS：async/await 与异常
来源：http://zr.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qd.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://iz.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ib.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://cv.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://di.nszjky.cn

[U99] JS：事件监听
来源：http://vq.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://yo.huanxung.cn

[U100] JS：DOM 查询
来源：http://je.wgjwhj.cn

document.querySelector(".item")
来源：http://gz.9csxet.cn

[U101] JS：classList 操作
来源：http://kz.wgjwhj.cn

el.classList.toggle("active")
来源：http://tc.huanxung.cn

[U102] JS：本地存储
来源：http://ab.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lu.nszjky.cn

[U103] JS：定时器
来源：http://ny.shxzukj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://oq.gzmigu.cn

[U104] JS：防抖
来源：http://vi.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ft.asd995.cn

[U105] JS：节流
来源：http://ms.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wb.newstarts.cn

[U106] JS：日期格式化
来源：http://kx.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://xs.nszjky.cn

[U107] JS：数字千分位
来源：http://zg.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://hb.yuexingan06.cn

[U108] JS：随机整数
来源：http://lk.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mi.hahajie.cn

[U109] JS：数组分组
来源：http://lu.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://gt.chemitech.net.cn

[U110] JS：数组分块
来源：http://om.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yd.muxihuayi.cn

[U111] JS：对象转 Map
来源：http://ok.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://cr.panjiajie.cn

[U112] JS：字符串补位
来源：http://ef.newstarts.cn

"7".padStart(3, "0")
来源：http://mm.shxzukj.cn

[U113] JS：正则替换全部
来源：http://co.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://dv.shxzukj.cn

[U114] JS：JSON 深比较
来源：http://pn.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ao.shxzskj.cn

[U115] JS：生成 UUID
来源：http://iu.gzmigu.cn

crypto.randomUUID()
来源：http://rm.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://mc.huixiangedu.cn

/** @param {string} name */ function f(name) {}
来源：http://he.huixinmuqiang.cn

[U117] JS：单元测试
来源：http://dt.shtwfgs.cn

npm i -D vitest;  npx vitest
来源：http://pt.jianghongdianzi.cn

[U118] JS：开发服务器
来源：http://rr.lnxyls.cn

npm i -D vite;  npx vite
来源：http://el.9csxet.cn

[U119] JS：生产构建
来源：http://xh.gzmigu.cn

npx vite build
来源：http://qk.nszjky.cn

[U120] JS：读取环境变量（Vite）
来源：http://dk.hnjuh.cn

import.meta.env.VITE_API_URL
来源：http://yf.shxzskj.cn

================================================================================
来源：http://tb.9csxet.cn

统计汇总
来源：http://zk.nicolike.cn

================================================================================
来源：http://ix.haigaiapp.cn

按语言统计（条）：
来源：http://gw.wgjwhj.cn

Python ......... 252
来源：http://ty.shxzukj.cn

PHP ............ 252
来源：http://zm.521024.cn

JavaScript ..... 252
来源：http://af.jctech888.com.cn

TypeScript ..... 212
来源：http://kw.szsharing.cn

Java ........... 212
来源：http://pt.nicolike.cn

Go ............. 212
来源：http://nv.shxzskj.cn

Ruby ........... 212
来源：http://uo.nszjky.cn

C# ............. 212
来源：http://xi.panjiajie.cn

C .............. 30
来源：http://ju.yuexingan06.cn

C++ ............ 30
来源：http://qm.shtwfgs.cn

SQL ............ 90
来源：http://ps.nszjky.cn

Bash ........... 80
来源：http://ds.chemitech.net.cn

Kotlin ......... 15
来源：http://nb.jianghongdianzi.cn

Swift .......... 15
来源：http://hi.nszjky.cn

Lua ............ 10
来源：http://jk.huixinmuqiang.cn

Perl ........... 10
来源：http://ei.lnxyls.cn

Scala .......... 10
来源：http://wn.shxzukj.cn

------------------------------------
来源：http://rv.9csxet.cn

合计 ........... 2106 条
来源：http://te.bjjhwx.cn

按章节统计：
来源：http://at.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yu.9csxet.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hc.wgjwhj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nf.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wx.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://of.lnxyls.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mp.panjiajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wq.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://fs.colortex.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zo.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zz.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rp.521024.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://rw.szsharing.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://yu.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mi.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ip.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://cz.yuexingan06.cn

Q SQL 专题                              90
来源：http://oe.nicolike.cn

R Bash 专题                             80
来源：http://rg.jctech888.com.cn

S C / C++ 专题                          60
来源：http://dt.huixiangedu.cn

T 其他语言补充                          60
来源：http://mw.huixiangedu.cn

U 高频实用片段                         120
来源：http://ak.yuntaijiaju.cn

------------------------------------
来源：http://rb.lnxyls.cn

合计                                  2106 条
来源：http://ed.huanxung.cn

--------------------------------------------------------------------------------
来源：http://pu.szxytkj.cn

使用提醒
来源：http://yo.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ae.szsharing.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rb.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://we.panjiajie.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://dz.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xs.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://oa.gzmigu.cn

—— 文件结束 ——
来源：http://ce.muxihuayi.cn

================================================================================
来源：http://rk.wgjwhj.cn

程序语言常见例子速查手册（2024 版）
来源：http://lz.szsharing.cn

Common Programming Examples Cheat Book
来源：http://tb.9csxet.cn

================================================================================
来源：http://cn.nszjky.cn

【收录内容】
来源：http://ra.nicolike.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fh.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rm.jianghongdianzi.cn

SQL · Bash · C · C++
来源：http://vc.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zv.huanxung.cn

【使用说明】
来源：http://vk.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://so.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yi.chemitech.net.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iy.bookmarksfly.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sp.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ib.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://bn.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jd.521024.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dv.asd995.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cc.huixiangedu.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ns.yuntaijiaju.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rt.jctech888.com.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zy.jctech888.com.cn

【文件统计】
来源：http://ys.jianghongdianzi.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://fi.huanxung.cn

--------------------------------------------------------------------------------
来源：http://rb.nszjky.cn

目  录
来源：http://ao.asd995.cn

--------------------------------------------------------------------------------
来源：http://bh.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tm.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fc.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://oq.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dc.newstarts.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://av.muxihuayi.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qr.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qz.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uj.chemitech.net.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://bb.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wg.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ft.nicolike.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dq.szxytkj.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ty.521024.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sw.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jd.9csxet.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sx.9csxet.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wd.bookmarksfly.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://oe.shxzukj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://uh.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://js.nicolike.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://dw.muxihuayi.cn

================================================================================
来源：http://pd.huixiangedu.cn

A. 基础语法与类型
来源：http://hw.521024.cn

================================================================================
来源：http://cw.nicolike.cn

[A01] Hello World
来源：http://un.yuntaijiaju.cn

Py:   print("Hello, World!")
来源：http://eg.521024.cn

PHP:  echo "Hello, World!";
来源：http://ci.jctech888.com.cn

JS:   console.log("Hello, World!");
来源：http://iz.panjiajie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rl.bookmarksfly.cn

Java: System.out.println("Hello, World!");
来源：http://go.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://wc.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://nb.yuntaijiaju.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ar.asd995.cn

[A02] 变量声明与赋值
来源：http://pl.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ik.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ad.shxzskj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qq.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fd.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://uk.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://ox.9csxet.cn

Ruby: name = "Alex"; age = 20
来源：http://dp.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fy.jctech888.com.cn

[A03] 常量定义
来源：http://ac.newstarts.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tm.wgjwhj.cn

PHP:  const PI = 3.14159;
来源：http://fs.gzmigu.cn

JS:   const PI = 3.14159;
来源：http://im.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://zk.nszjky.cn

Java: static final double PI = 3.14159;
来源：http://ke.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://qt.muxihuayi.cn

Ruby: PI = 3.14159
来源：http://wn.huanxung.cn

C#:   const double PI = 3.14159;
来源：http://oi.nicolike.cn

[A04] 判断变量类型
来源：http://to.wgjwhj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://bl.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qm.huixiangedu.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hc.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://xd.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://am.haigaiapp.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ec.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nj.panjiajie.cn

C#:   x.GetType().Name; x is int
来源：http://ot.huanxung.cn

[A05] 整数除法与取模
来源：http://uf.bookmarksfly.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ca.gzmigu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://jj.9csxet.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://of.muxihuayi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://dl.huixiangedu.cn

Java: 7 / 2; 7 % 2
来源：http://gu.lnxyls.cn

Go:   7 / 2; 7 % 2
来源：http://qi.asd995.cn

Ruby: 7 / 2; 7 % 2
来源：http://wh.jctech888.com.cn

C#:   7 / 2; 7 % 2
来源：http://cc.bjjhwx.cn

[A06] 字符串转数字
来源：http://gj.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://qa.newstarts.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://tu.hnjuh.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kq.9csxet.cn

TS:   parseInt("42", 10); Number("42")
来源：http://xw.lnxyls.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fl.muxihuayi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zh.lnxyls.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://uu.yuexingan06.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qr.asd995.cn

[A07] 数字转字符串
来源：http://ly.hahajie.cn

Py:   str(42)
来源：http://tw.hnjuh.cn

PHP:  (string) 42; strval(42)
来源：http://zd.wgjwhj.cn


<!-- 参考信息 -->