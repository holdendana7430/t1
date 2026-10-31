代发 wailian999

[U55] PHP：match 表达式
来源：http://tt.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ss.newstarts.cn

[U56] PHP：命名参数
来源：http://nu.asd995.cn

f(a: 1, b: 2)
来源：http://uh.nicolike.cn

[U57] PHP：字符串插值
来源：http://yi.yuexingan06.cn

"值: {$a}"
来源：http://am.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://zi.shxzukj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ck.hahajie.cn

[U59] PHP：自定义排序
来源：http://dy.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://el.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://kq.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qw.nszjky.cn

[U61] PHP：正则
来源：http://jc.muxihuayi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lx.jctech888.com.cn

[U62] PHP：日期对象
来源：http://rx.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ph.wgjwhj.cn

[U63] PHP：文件读写
来源：http://pv.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fq.yuexingan06.cn

[U64] PHP：目录遍历
来源：http://in.colortex.cn

glob("dir/*.php");  scandir("dir");
来源：http://iq.hahajie.cn

[U65] PHP：会话
来源：http://bm.hnjuh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tw.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://ng.chemitech.net.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ns.huixiangedu.cn

[U67] PHP：处理文件上传
来源：http://rl.shxzskj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hx.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://hw.hnjuh.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xx.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ro.yuntaijiaju.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rc.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://bk.newstarts.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qo.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://pm.bjjhwx.cn

throw new RuntimeException("失败", 500);
来源：http://ob.newstarts.cn

[U72] PHP：写错误日志
来源：http://fj.nszjky.cn

error_log("失败: " . $e->getMessage());
来源：http://eu.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://tt.szxytkj.cn

parse_ini_file("config.ini", true)
来源：http://hh.colortex.cn

[U74] PHP：读取环境变量
来源：http://di.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://vo.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://wf.shxzukj.cn

composer require psr/container
来源：http://gd.gzmigu.cn

[U76] PHP：简单路由
来源：http://zy.chemitech.net.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xt.gzmigu.cn

[U77] PHP：模板渲染
来源：http://kb.bjjhwx.cn

composer require twig/twig
来源：http://hw.shtwfgs.cn

[U78] PHP：单元测试
来源：http://lu.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://pz.szxytkj.cn

[U79] PHP：静态分析
来源：http://jg.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://pf.shtwfgs.cn

[U80] PHP：代码规范修复
来源：http://ie.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ec.newstarts.cn

[U81] JS：初始化项目
来源：http://yb.muxihuayi.cn

npm init -y;  npm i express
来源：http://eu.hnjuh.cn

[U82] JS：package.json 脚本
来源：http://nu.bjjhwx.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xm.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://wr.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uj.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://yc.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://id.newstarts.cn

[U85] JS：可选链
来源：http://dd.bookmarksfly.cn

a?.b?.c
来源：http://cz.haigaiapp.cn

[U86] JS：空值合并
来源：http://zm.shxzukj.cn

a ?? b
来源：http://et.colortex.cn

[U87] JS：解构默认值
来源：http://pk.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://ah.shtwfgs.cn

[U88] JS：对象展开合并
来源：http://rn.colortex.cn

{ ...a, ...b }
来源：http://hl.asd995.cn

[U89] JS：数组去重
来源：http://vi.shxzukj.cn

[...new Set(arr)]
来源：http://wk.nszjky.cn

[U90] JS：数字数组排序
来源：http://xo.shxzskj.cn

[...arr].sort((a, b) => a - b)
来源：http://pt.bjjhwx.cn

[U91] JS：对象键值遍历
来源：http://ci.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://dh.colortex.cn

[U92] JS：深拷贝
来源：http://yg.hahajie.cn

structuredClone(obj)
来源：http://qx.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://fr.newstarts.cn

`共 ${n} 条`
来源：http://cq.nicolike.cn

[U94] JS：箭头函数
来源：http://de.newstarts.cn

const double = x => x * 2;
来源：http://gd.asd995.cn

[U95] JS：Promise 包装
来源：http://lx.muxihuayi.cn

new Promise((resolve, reject) => {})
来源：http://ix.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://km.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gv.shxzukj.cn

[U97] JS：并发请求
来源：http://cq.newstarts.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ej.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://kn.huanxung.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mc.chemitech.net.cn

[U99] JS：事件监听
来源：http://xl.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://mt.huixinmuqiang.cn

[U100] JS：DOM 查询
来源：http://vn.bjjhwx.cn

document.querySelector(".item")
来源：http://jv.shtwfgs.cn

[U101] JS：classList 操作
来源：http://lb.shxzukj.cn

el.classList.toggle("active")
来源：http://fy.lnxyls.cn

[U102] JS：本地存储
来源：http://or.nszjky.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hh.yuntaijiaju.cn

[U103] JS：定时器
来源：http://mz.shxzskj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://yf.panjiajie.cn

[U104] JS：防抖
来源：http://zz.bjjhwx.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://la.szsharing.cn

[U105] JS：节流
来源：http://qm.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nj.chemitech.net.cn

[U106] JS：日期格式化
来源：http://po.colortex.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dt.521024.cn

[U107] JS：数字千分位
来源：http://hz.colortex.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bh.9csxet.cn

[U108] JS：随机整数
来源：http://lb.wgjwhj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mr.nicolike.cn

[U109] JS：数组分组
来源：http://cf.muxihuayi.cn

Object.groupBy(arr, x => x.type)
来源：http://ki.jctech888.com.cn

[U110] JS：数组分块
来源：http://or.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cx.shxzskj.cn

[U111] JS：对象转 Map
来源：http://xv.gzmigu.cn

new Map(Object.entries(obj))
来源：http://ff.hahajie.cn

[U112] JS：字符串补位
来源：http://tk.haigaiapp.cn

"7".padStart(3, "0")
来源：http://cm.gzmigu.cn

[U113] JS：正则替换全部
来源：http://db.521024.cn

s.replaceAll("a", "b")
来源：http://if.nicolike.cn

[U114] JS：JSON 深比较
来源：http://al.nszjky.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dw.nicolike.cn

[U115] JS：生成 UUID
来源：http://ol.nszjky.cn

crypto.randomUUID()
来源：http://um.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://qj.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ll.wgjwhj.cn

[U117] JS：单元测试
来源：http://qj.nicolike.cn

npm i -D vitest;  npx vitest
来源：http://yr.shxzskj.cn

[U118] JS：开发服务器
来源：http://pr.nicolike.cn

npm i -D vite;  npx vite
来源：http://do.lnxyls.cn

[U119] JS：生产构建
来源：http://ro.bjjhwx.cn

npx vite build
来源：http://uq.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://bp.asd995.cn

import.meta.env.VITE_API_URL
来源：http://iu.9csxet.cn

================================================================================
来源：http://yo.jianghongdianzi.cn

统计汇总
来源：http://jp.bjjhwx.cn

================================================================================
来源：http://lt.asd995.cn

按语言统计（条）：
来源：http://zb.hahajie.cn

Python ......... 252
来源：http://gq.colortex.cn

PHP ............ 252
来源：http://cj.nszjky.cn

JavaScript ..... 252
来源：http://ra.newstarts.cn

TypeScript ..... 212
来源：http://ef.huanxung.cn

Java ........... 212
来源：http://nz.hahajie.cn

Go ............. 212
来源：http://at.huanxung.cn

Ruby ........... 212
来源：http://cv.haigaiapp.cn

C# ............. 212
来源：http://it.bjjhwx.cn

C .............. 30
来源：http://tg.newstarts.cn

C++ ............ 30
来源：http://si.haigaiapp.cn

SQL ............ 90
来源：http://fk.muxihuayi.cn

Bash ........... 80
来源：http://ou.hnjuh.cn

Kotlin ......... 15
来源：http://fp.bjjhwx.cn

Swift .......... 15
来源：http://pb.haigaiapp.cn

Lua ............ 10
来源：http://bw.szsharing.cn

Perl ........... 10
来源：http://ck.bookmarksfly.cn

Scala .......... 10
来源：http://sv.yuntaijiaju.cn

------------------------------------
来源：http://xs.colortex.cn

合计 ........... 2106 条
来源：http://be.yuntaijiaju.cn

按章节统计：
来源：http://bk.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://za.haigaiapp.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vt.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xo.huixinmuqiang.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xx.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yc.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://if.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://he.yuexingan06.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ic.chemitech.net.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://yl.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rs.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ww.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nd.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vz.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://el.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bv.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rx.jctech888.com.cn

Q SQL 专题                              90
来源：http://qm.521024.cn

R Bash 专题                             80
来源：http://qu.huanxung.cn

S C / C++ 专题                          60
来源：http://lz.521024.cn

T 其他语言补充                          60
来源：http://jz.yuexingan06.cn

U 高频实用片段                         120
来源：http://wx.gzmigu.cn

------------------------------------
来源：http://cx.nicolike.cn

合计                                  2106 条
来源：http://am.szsharing.cn

--------------------------------------------------------------------------------
来源：http://ou.chemitech.net.cn

使用提醒
来源：http://kd.asd995.cn

--------------------------------------------------------------------------------
来源：http://ao.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ct.hahajie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tb.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uq.szxytkj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hp.huanxung.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://pu.gzmigu.cn

—— 文件结束 ——
来源：http://mx.newstarts.cn

================================================================================
来源：http://vp.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://ur.gzmigu.cn

Common Programming Examples Cheat Book
来源：http://cm.hnjuh.cn

================================================================================
来源：http://mu.szxytkj.cn

【收录内容】
来源：http://tg.huixiangedu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://hg.shxzukj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wq.wgjwhj.cn

SQL · Bash · C · C++
来源：http://rh.asd995.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://eg.wgjwhj.cn

【使用说明】
来源：http://cm.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hc.muxihuayi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zn.lnxyls.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uw.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vf.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vf.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mz.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ij.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xj.yuntaijiaju.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://lf.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nr.wgjwhj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ja.colortex.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cz.yuexingan06.cn

【文件统计】
来源：http://oa.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jl.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://fc.jctech888.com.cn

目  录
来源：http://nc.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://xq.gzmigu.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://st.yuexingan06.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jy.shtwfgs.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://hu.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zh.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://oo.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ha.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://qu.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://gh.shtwfgs.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gg.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://vg.huixiangedu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mx.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://re.hahajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cp.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ir.lnxyls.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wj.huixiangedu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dp.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://as.shtwfgs.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://iy.colortex.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mo.bookmarksfly.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qc.wgjwhj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wc.jianghongdianzi.cn

================================================================================
来源：http://gb.chemitech.net.cn

A. 基础语法与类型
来源：http://nd.bjjhwx.cn

================================================================================
来源：http://hu.hnjuh.cn

[A01] Hello World
来源：http://xh.shxzukj.cn

Py:   print("Hello, World!")
来源：http://wu.shtwfgs.cn

PHP:  echo "Hello, World!";
来源：http://zk.panjiajie.cn

JS:   console.log("Hello, World!");
来源：http://zo.9csxet.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rf.colortex.cn

Java: System.out.println("Hello, World!");
来源：http://jl.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://rb.bookmarksfly.cn

Ruby: puts "Hello, World!"
来源：http://or.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ef.yuexingan06.cn

[A02] 变量声明与赋值
来源：http://bx.shtwfgs.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xo.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xx.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wj.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://eo.yuntaijiaju.cn

Java: String name = "Alex"; int age = 20;
来源：http://mu.jianghongdianzi.cn

Go:   name := "Alex"; age := 20
来源：http://hw.newstarts.cn

Ruby: name = "Alex"; age = 20
来源：http://fk.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ho.szxytkj.cn

[A03] 常量定义
来源：http://sn.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://oc.bookmarksfly.cn

PHP:  const PI = 3.14159;
来源：http://ec.muxihuayi.cn

JS:   const PI = 3.14159;
来源：http://br.yuntaijiaju.cn

TS:   const PI: number = 3.14159;
来源：http://wd.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://ue.shxzukj.cn

Go:   const PI = 3.14159
来源：http://hx.huanxung.cn

Ruby: PI = 3.14159
来源：http://nj.yuexingan06.cn

C#:   const double PI = 3.14159;
来源：http://nr.yuexingan06.cn

[A04] 判断变量类型
来源：http://ej.shtwfgs.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://jw.lnxyls.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ql.shxzukj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://qh.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://zj.colortex.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zk.szxytkj.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bf.huixiangedu.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://rh.wgjwhj.cn

C#:   x.GetType().Name; x is int
来源：http://kk.huanxung.cn

[A05] 整数除法与取模
来源：http://nd.szsharing.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://db.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://kl.lnxyls.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yp.shxzukj.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://oy.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://fc.bjjhwx.cn

Go:   7 / 2; 7 % 2
来源：http://da.9csxet.cn

Ruby: 7 / 2; 7 % 2
来源：http://hr.bjjhwx.cn

C#:   7 / 2; 7 % 2
来源：http://re.wgjwhj.cn

[A06] 字符串转数字
来源：http://ph.wgjwhj.cn

Py:   int("42"); float("3.14")
来源：http://ke.huixiangedu.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://jj.wgjwhj.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://sa.yuntaijiaju.cn

TS:   parseInt("42", 10); Number("42")
来源：http://dv.hahajie.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://gu.panjiajie.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nw.szsharing.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rm.chemitech.net.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://zg.yuexingan06.cn

[A07] 数字转字符串
来源：http://ri.panjiajie.cn

Py:   str(42)
来源：http://vh.521024.cn

PHP:  (string) 42; strval(42)
来源：http://xi.huixiangedu.cn

JS:   String(42); (42).toString()
来源：http://gd.asd995.cn

TS:   String(42)
来源：http://yw.szsharing.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://gb.521024.cn

Go:   strconv.Itoa(42)
来源：http://ls.nicolike.cn


<!-- 参考信息 -->