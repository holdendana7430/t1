代发 wailian999

[U53] PHP：空合并运算符
来源：http://cj.bookmarksfly.cn

$v = $a ?? $b ?? "default";
来源：http://pg.shxzukj.cn

[U54] PHP：空安全调用
来源：http://vi.newstarts.cn

$obj?->method()
来源：http://kh.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://oy.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://un.szxytkj.cn

[U56] PHP：命名参数
来源：http://ea.521024.cn

f(a: 1, b: 2)
来源：http://px.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://wg.shxzskj.cn

"值: {$a}"
来源：http://dv.szxytkj.cn

[U58] PHP：数组三件套
来源：http://qy.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ua.lnxyls.cn

[U59] PHP：自定义排序
来源：http://bu.9csxet.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.yuexingan06.cn

[U60] PHP：JSON 编解码
来源：http://ia.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://iu.hahajie.cn

[U61] PHP：正则
来源：http://iy.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://er.huixiangedu.cn

[U62] PHP：日期对象
来源：http://ex.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fi.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://dz.hnjuh.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bj.muxihuayi.cn

[U64] PHP：目录遍历
来源：http://ko.yuexingan06.cn

glob("dir/*.php");  scandir("dir");
来源：http://fe.asd995.cn

[U65] PHP：会话
来源：http://zs.lnxyls.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://he.colortex.cn

[U66] PHP：设置 Cookie
来源：http://yq.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://uw.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://wp.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fg.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://cg.bjjhwx.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://km.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://aq.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dj.9csxet.cn

[U70] PHP：PDO 事务
来源：http://rj.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ee.jianghongdianzi.cn

[U71] PHP：抛出异常
来源：http://em.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://uy.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://vl.nicolike.cn

error_log("失败: " . $e->getMessage());
来源：http://ll.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://ir.521024.cn

parse_ini_file("config.ini", true)
来源：http://uq.huanxung.cn

[U74] PHP：读取环境变量
来源：http://xa.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://nt.colortex.cn

[U75] PHP：依赖注入
来源：http://ky.huanxung.cn

composer require psr/container
来源：http://ny.nszjky.cn

[U76] PHP：简单路由
来源：http://sj.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cy.chemitech.net.cn

[U77] PHP：模板渲染
来源：http://sf.muxihuayi.cn

composer require twig/twig
来源：http://tx.shxzskj.cn

[U78] PHP：单元测试
来源：http://na.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://lb.szsharing.cn

[U79] PHP：静态分析
来源：http://tk.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://le.szsharing.cn

[U80] PHP：代码规范修复
来源：http://se.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lt.muxihuayi.cn

[U81] JS：初始化项目
来源：http://cy.bookmarksfly.cn

npm init -y;  npm i express
来源：http://bd.huixiangedu.cn

[U82] JS：package.json 脚本
来源：http://fq.szxytkj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pl.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://lf.haigaiapp.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fe.panjiajie.cn

[U84] JS：CommonJS 写法
来源：http://gr.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xn.szxytkj.cn

[U85] JS：可选链
来源：http://ti.9csxet.cn

a?.b?.c
来源：http://wl.hahajie.cn

[U86] JS：空值合并
来源：http://cg.nszjky.cn

a ?? b
来源：http://vf.wgjwhj.cn

[U87] JS：解构默认值
来源：http://lz.wgjwhj.cn

const { a = 1, b = 2 } = obj;
来源：http://ui.wgjwhj.cn

[U88] JS：对象展开合并
来源：http://xs.bjjhwx.cn

{ ...a, ...b }
来源：http://ly.hnjuh.cn

[U89] JS：数组去重
来源：http://yl.wgjwhj.cn

[...new Set(arr)]
来源：http://cx.asd995.cn

[U90] JS：数字数组排序
来源：http://hs.huixinmuqiang.cn

[...arr].sort((a, b) => a - b)
来源：http://bh.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://wc.szxytkj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ca.asd995.cn

[U92] JS：深拷贝
来源：http://hp.huanxung.cn

structuredClone(obj)
来源：http://wj.jianghongdianzi.cn

[U93] JS：模板字符串
来源：http://nn.jctech888.com.cn

`共 ${n} 条`
来源：http://ri.haigaiapp.cn

[U94] JS：箭头函数
来源：http://sh.asd995.cn

const double = x => x * 2;
来源：http://oy.hnjuh.cn

[U95] JS：Promise 包装
来源：http://gx.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://rx.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://wc.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://og.huixiangedu.cn

[U97] JS：并发请求
来源：http://xi.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://iu.huixiangedu.cn

[U98] JS：fetch 带 JSON
来源：http://wn.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ew.huixinmuqiang.cn

[U99] JS：事件监听
来源：http://te.panjiajie.cn

el.addEventListener("click", e => {})
来源：http://rb.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://sm.shtwfgs.cn

document.querySelector(".item")
来源：http://mm.bookmarksfly.cn

[U101] JS：classList 操作
来源：http://bi.nicolike.cn

el.classList.toggle("active")
来源：http://sy.huanxung.cn

[U102] JS：本地存储
来源：http://wl.9csxet.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ub.haigaiapp.cn

[U103] JS：定时器
来源：http://it.lnxyls.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ro.bjjhwx.cn

[U104] JS：防抖
来源：http://ij.nicolike.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kg.521024.cn

[U105] JS：节流
来源：http://zh.9csxet.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mq.panjiajie.cn

[U106] JS：日期格式化
来源：http://sr.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lv.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://yz.jctech888.com.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rj.bookmarksfly.cn

[U108] JS：随机整数
来源：http://yt.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://lp.huixiangedu.cn

[U109] JS：数组分组
来源：http://uf.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://vy.szsharing.cn

[U110] JS：数组分块
来源：http://se.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iv.9csxet.cn

[U111] JS：对象转 Map
来源：http://yw.muxihuayi.cn

new Map(Object.entries(obj))
来源：http://ir.huanxung.cn

[U112] JS：字符串补位
来源：http://mh.jianghongdianzi.cn

"7".padStart(3, "0")
来源：http://ai.asd995.cn

[U113] JS：正则替换全部
来源：http://fm.szsharing.cn

s.replaceAll("a", "b")
来源：http://pg.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://wa.jctech888.com.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://rd.jianghongdianzi.cn

[U115] JS：生成 UUID
来源：http://xt.9csxet.cn

crypto.randomUUID()
来源：http://cq.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://ko.yuexingan06.cn

/** @param {string} name */ function f(name) {}
来源：http://hj.gzmigu.cn

[U117] JS：单元测试
来源：http://rw.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://zx.muxihuayi.cn

[U118] JS：开发服务器
来源：http://dl.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://hx.huixiangedu.cn

[U119] JS：生产构建
来源：http://zt.9csxet.cn

npx vite build
来源：http://kj.jctech888.com.cn

[U120] JS：读取环境变量（Vite）
来源：http://zj.lnxyls.cn

import.meta.env.VITE_API_URL
来源：http://yj.bjjhwx.cn

================================================================================
来源：http://ft.nicolike.cn

统计汇总
来源：http://tt.shxzskj.cn

================================================================================
来源：http://pf.hahajie.cn

按语言统计（条）：
来源：http://ri.nszjky.cn

Python ......... 252
来源：http://dd.shxzskj.cn

PHP ............ 252
来源：http://rz.chemitech.net.cn

JavaScript ..... 252
来源：http://wh.bjjhwx.cn

TypeScript ..... 212
来源：http://dt.jianghongdianzi.cn

Java ........... 212
来源：http://wa.yuntaijiaju.cn

Go ............. 212
来源：http://jy.asd995.cn

Ruby ........... 212
来源：http://ce.shtwfgs.cn

C# ............. 212
来源：http://ld.521024.cn

C .............. 30
来源：http://iy.asd995.cn

C++ ............ 30
来源：http://sr.gzmigu.cn

SQL ............ 90
来源：http://fi.haigaiapp.cn

Bash ........... 80
来源：http://hv.hnjuh.cn

Kotlin ......... 15
来源：http://qv.bjjhwx.cn

Swift .......... 15
来源：http://mj.shxzukj.cn

Lua ............ 10
来源：http://tz.shxzskj.cn

Perl ........... 10
来源：http://nr.yuntaijiaju.cn

Scala .......... 10
来源：http://st.nszjky.cn

------------------------------------
来源：http://iz.nicolike.cn

合计 ........... 2106 条
来源：http://yv.huixiangedu.cn

按章节统计：
来源：http://ji.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gj.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://kr.huixinmuqiang.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nj.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vg.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zw.shxzskj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vs.hahajie.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cu.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://il.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pw.colortex.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zf.gzmigu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qv.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ut.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://by.gzmigu.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ir.hahajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://eo.huanxung.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mc.newstarts.cn

Q SQL 专题                              90
来源：http://ez.colortex.cn

R Bash 专题                             80
来源：http://uh.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://ss.lnxyls.cn

T 其他语言补充                          60
来源：http://we.yuexingan06.cn

U 高频实用片段                         120
来源：http://qw.521024.cn

------------------------------------
来源：http://qp.nicolike.cn

合计                                  2106 条
来源：http://iz.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://cu.nszjky.cn

使用提醒
来源：http://gv.nicolike.cn

--------------------------------------------------------------------------------
来源：http://tm.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://at.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://vk.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://sh.jctech888.com.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fc.bookmarksfly.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mp.yuexingan06.cn

—— 文件结束 ——
来源：http://ir.bjjhwx.cn

================================================================================
来源：http://jh.shxzskj.cn

程序语言常见例子速查手册（2024 版）
来源：http://gh.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://qt.haigaiapp.cn

================================================================================
来源：http://tc.szsharing.cn

【收录内容】
来源：http://gx.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://af.wgjwhj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wc.wgjwhj.cn

SQL · Bash · C · C++
来源：http://nu.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://fw.9csxet.cn

【使用说明】
来源：http://yh.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ij.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://iq.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://py.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ws.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://nc.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://us.shxzskj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qc.nszjky.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lh.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ad.hnjuh.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yp.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nd.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vw.shxzskj.cn

【文件统计】
来源：http://tz.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wo.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://uv.hnjuh.cn

目  录
来源：http://yc.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ga.muxihuayi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zf.szsharing.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ws.hahajie.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hc.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cx.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://qk.bookmarksfly.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://fd.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://sa.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bk.wgjwhj.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://yy.gzmigu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://pp.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gh.huixiangedu.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vc.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fv.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ui.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gq.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cz.lnxyls.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pz.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ga.newstarts.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zc.huixiangedu.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://oo.lnxyls.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://th.jianghongdianzi.cn

================================================================================
来源：http://ir.huixinmuqiang.cn

A. 基础语法与类型
来源：http://vt.nszjky.cn

================================================================================
来源：http://sy.yuexingan06.cn

[A01] Hello World
来源：http://dz.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://az.huanxung.cn

PHP:  echo "Hello, World!";
来源：http://kv.shxzskj.cn

JS:   console.log("Hello, World!");
来源：http://od.gzmigu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qe.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://ic.9csxet.cn

Go:   fmt.Println("Hello, World!")
来源：http://dv.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://iu.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xi.bookmarksfly.cn

[A02] 变量声明与赋值
来源：http://zk.gzmigu.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://yu.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://wr.jctech888.com.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gz.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ci.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://nk.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://la.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://hd.shtwfgs.cn

C#:   string name = "Alex"; int age = 20;
来源：http://qo.nicolike.cn

[A03] 常量定义
来源：http://hk.jctech888.com.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bg.huanxung.cn

PHP:  const PI = 3.14159;
来源：http://hy.9csxet.cn

JS:   const PI = 3.14159;
来源：http://iu.newstarts.cn

TS:   const PI: number = 3.14159;
来源：http://lg.szxytkj.cn

Java: static final double PI = 3.14159;
来源：http://ou.lnxyls.cn

Go:   const PI = 3.14159
来源：http://vf.bookmarksfly.cn

Ruby: PI = 3.14159
来源：http://lf.521024.cn

C#:   const double PI = 3.14159;
来源：http://uc.yuntaijiaju.cn

[A04] 判断变量类型
来源：http://nz.nicolike.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ij.nicolike.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://pu.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://vb.wgjwhj.cn

TS:   typeof x; x instanceof Date
来源：http://ld.yuntaijiaju.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ti.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wv.jianghongdianzi.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vj.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://xq.bjjhwx.cn

[A05] 整数除法与取模
来源：http://vz.shxzskj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xt.wgjwhj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cz.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://sz.521024.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://sb.shxzukj.cn

Java: 7 / 2; 7 % 2
来源：http://bl.huanxung.cn

Go:   7 / 2; 7 % 2
来源：http://ud.nszjky.cn

Ruby: 7 / 2; 7 % 2
来源：http://sd.wgjwhj.cn

C#:   7 / 2; 7 % 2
来源：http://gp.bjjhwx.cn

[A06] 字符串转数字
来源：http://gx.nicolike.cn

Py:   int("42"); float("3.14")
来源：http://bi.huanxung.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://nx.szsharing.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ft.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vm.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://jk.szsharing.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://om.newstarts.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://be.szxytkj.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vo.gzmigu.cn

[A07] 数字转字符串
来源：http://tn.huanxung.cn

Py:   str(42)
来源：http://dd.hahajie.cn

PHP:  (string) 42; strval(42)
来源：http://ws.yuexingan06.cn


<!-- 参考信息 -->