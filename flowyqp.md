代发 wailian999

[U53] PHP：空合并运算符
来源：http://ob.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://ey.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://ez.shxzukj.cn

$obj?->method()
来源：http://hl.szxytkj.cn

[U55] PHP：match 表达式
来源：http://rr.gzmigu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wn.gzmigu.cn

[U56] PHP：命名参数
来源：http://yx.gzmigu.cn

f(a: 1, b: 2)
来源：http://ac.newstarts.cn

[U57] PHP：字符串插值
来源：http://bg.shxzskj.cn

"值: {$a}"
来源：http://cx.9csxet.cn

[U58] PHP：数组三件套
来源：http://xc.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://aa.shxzukj.cn

[U59] PHP：自定义排序
来源：http://pd.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ow.gzmigu.cn

[U60] PHP：JSON 编解码
来源：http://lm.jianghongdianzi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jv.gzmigu.cn

[U61] PHP：正则
来源：http://wu.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hy.szsharing.cn

[U62] PHP：日期对象
来源：http://kb.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bd.hnjuh.cn

[U63] PHP：文件读写
来源：http://tq.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vs.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://ug.shtwfgs.cn

glob("dir/*.php");  scandir("dir");
来源：http://qw.panjiajie.cn

[U65] PHP：会话
来源：http://nj.szsharing.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://xn.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://cs.lnxyls.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vw.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://gi.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kt.newstarts.cn

[U68] PHP：PDO 连接
来源：http://is.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rd.chemitech.net.cn

[U69] PHP：PDO 预处理
来源：http://qx.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gq.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://fs.jianghongdianzi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ad.szxytkj.cn

[U71] PHP：抛出异常
来源：http://bm.bookmarksfly.cn

throw new RuntimeException("失败", 500);
来源：http://qf.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://lu.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://el.szsharing.cn

[U73] PHP：读取 ini 配置
来源：http://zk.colortex.cn

parse_ini_file("config.ini", true)
来源：http://jo.nicolike.cn

[U74] PHP：读取环境变量
来源：http://bm.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://nk.wgjwhj.cn

[U75] PHP：依赖注入
来源：http://pr.bjjhwx.cn

composer require psr/container
来源：http://yq.nszjky.cn

[U76] PHP：简单路由
来源：http://eg.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bs.colortex.cn

[U77] PHP：模板渲染
来源：http://jd.gzmigu.cn

composer require twig/twig
来源：http://gt.shxzskj.cn

[U78] PHP：单元测试
来源：http://xf.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://hv.shxzskj.cn

[U79] PHP：静态分析
来源：http://cl.szxytkj.cn

composer require --dev phpstan/phpstan
来源：http://px.asd995.cn

[U80] PHP：代码规范修复
来源：http://aq.hahajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qn.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ji.nszjky.cn

npm init -y;  npm i express
来源：http://rp.bookmarksfly.cn

[U82] JS：package.json 脚本
来源：http://vl.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yt.nicolike.cn

[U83] JS：ES Module 导入导出
来源：http://si.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tk.shxzskj.cn

[U84] JS：CommonJS 写法
来源：http://rg.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://nl.bookmarksfly.cn

[U85] JS：可选链
来源：http://pc.colortex.cn

a?.b?.c
来源：http://hc.bjjhwx.cn

[U86] JS：空值合并
来源：http://bn.shxzukj.cn

a ?? b
来源：http://jg.muxihuayi.cn

[U87] JS：解构默认值
来源：http://ul.gzmigu.cn

const { a = 1, b = 2 } = obj;
来源：http://tk.haigaiapp.cn

[U88] JS：对象展开合并
来源：http://ge.jctech888.com.cn

{ ...a, ...b }
来源：http://wt.asd995.cn

[U89] JS：数组去重
来源：http://hl.gzmigu.cn

[...new Set(arr)]
来源：http://ga.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://ox.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://pq.9csxet.cn

[U91] JS：对象键值遍历
来源：http://lw.huanxung.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qg.jctech888.com.cn

[U92] JS：深拷贝
来源：http://go.panjiajie.cn

structuredClone(obj)
来源：http://wu.hnjuh.cn

[U93] JS：模板字符串
来源：http://ls.nszjky.cn

`共 ${n} 条`
来源：http://sm.haigaiapp.cn

[U94] JS：箭头函数
来源：http://zg.huixinmuqiang.cn

const double = x => x * 2;
来源：http://hc.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://ij.lnxyls.cn

new Promise((resolve, reject) => {})
来源：http://vh.huanxung.cn

[U96] JS：async/await 与异常
来源：http://xa.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hj.huanxung.cn

[U97] JS：并发请求
来源：http://xk.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ea.yuntaijiaju.cn

[U98] JS：fetch 带 JSON
来源：http://kx.bookmarksfly.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://qz.gzmigu.cn

[U99] JS：事件监听
来源：http://au.bjjhwx.cn

el.addEventListener("click", e => {})
来源：http://oj.nszjky.cn

[U100] JS：DOM 查询
来源：http://ml.bjjhwx.cn

document.querySelector(".item")
来源：http://sb.huanxung.cn

[U101] JS：classList 操作
来源：http://ee.hahajie.cn

el.classList.toggle("active")
来源：http://np.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://vk.nicolike.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://hx.chemitech.net.cn

[U103] JS：定时器
来源：http://rj.9csxet.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ng.huixiangedu.cn

[U104] JS：防抖
来源：http://cn.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nw.colortex.cn

[U105] JS：节流
来源：http://uc.bjjhwx.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fl.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://mn.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fq.gzmigu.cn

[U107] JS：数字千分位
来源：http://cz.shxzskj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rc.hahajie.cn

[U108] JS：随机整数
来源：http://os.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pq.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://bx.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://hj.521024.cn

[U110] JS：数组分块
来源：http://xh.521024.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tt.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://qk.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://uk.hahajie.cn

[U112] JS：字符串补位
来源：http://ul.jctech888.com.cn

"7".padStart(3, "0")
来源：http://va.asd995.cn

[U113] JS：正则替换全部
来源：http://jo.panjiajie.cn

s.replaceAll("a", "b")
来源：http://bb.yuexingan06.cn

[U114] JS：JSON 深比较
来源：http://di.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pd.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://aw.gzmigu.cn

crypto.randomUUID()
来源：http://lz.nszjky.cn

[U116] JS：类型检查（JSDoc）
来源：http://dq.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://uj.lnxyls.cn

[U117] JS：单元测试
来源：http://cz.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://cn.bookmarksfly.cn

[U118] JS：开发服务器
来源：http://fj.shxzskj.cn

npm i -D vite;  npx vite
来源：http://wy.lnxyls.cn

[U119] JS：生产构建
来源：http://zp.jctech888.com.cn

npx vite build
来源：http://dg.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://se.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://ye.huanxung.cn

================================================================================
来源：http://et.nicolike.cn

统计汇总
来源：http://rq.yuexingan06.cn

================================================================================
来源：http://ej.muxihuayi.cn

按语言统计（条）：
来源：http://cj.huanxung.cn

Python ......... 252
来源：http://qe.panjiajie.cn

PHP ............ 252
来源：http://su.chemitech.net.cn

JavaScript ..... 252
来源：http://ne.jctech888.com.cn

TypeScript ..... 212
来源：http://ii.yuexingan06.cn

Java ........... 212
来源：http://ez.huixinmuqiang.cn

Go ............. 212
来源：http://cq.bookmarksfly.cn

Ruby ........... 212
来源：http://br.9csxet.cn

C# ............. 212
来源：http://nl.9csxet.cn

C .............. 30
来源：http://or.asd995.cn

C++ ............ 30
来源：http://iq.jianghongdianzi.cn

SQL ............ 90
来源：http://kb.jctech888.com.cn

Bash ........... 80
来源：http://fm.huixiangedu.cn

Kotlin ......... 15
来源：http://pe.jianghongdianzi.cn

Swift .......... 15
来源：http://vq.bjjhwx.cn

Lua ............ 10
来源：http://ue.bjjhwx.cn

Perl ........... 10
来源：http://cn.yuntaijiaju.cn

Scala .......... 10
来源：http://gi.wgjwhj.cn

------------------------------------
来源：http://gl.szxytkj.cn

合计 ........... 2106 条
来源：http://oa.huanxung.cn

按章节统计：
来源：http://or.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ll.nszjky.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ey.shxzukj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kg.shxzskj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://zu.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gc.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gy.colortex.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ao.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ks.yuntaijiaju.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ji.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xj.chemitech.net.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pm.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tw.jctech888.com.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ee.huixinmuqiang.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ye.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qn.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://hu.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://hx.shxzukj.cn

R Bash 专题                             80
来源：http://iq.9csxet.cn

S C / C++ 专题                          60
来源：http://ep.colortex.cn

T 其他语言补充                          60
来源：http://tv.gzmigu.cn

U 高频实用片段                         120
来源：http://rf.bjjhwx.cn

------------------------------------
来源：http://dv.9csxet.cn

合计                                  2106 条
来源：http://mr.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://gz.colortex.cn

使用提醒
来源：http://hb.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://cx.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://vj.chemitech.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pp.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pv.haigaiapp.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xa.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://go.lnxyls.cn

—— 文件结束 ——
来源：http://ye.colortex.cn

================================================================================
来源：http://ow.nszjky.cn

程序语言常见例子速查手册（2024 版）
来源：http://tt.panjiajie.cn

Common Programming Examples Cheat Book
来源：http://tt.bookmarksfly.cn

================================================================================
来源：http://gp.lnxyls.cn

【收录内容】
来源：http://xg.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ce.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gt.9csxet.cn

SQL · Bash · C · C++
来源：http://lq.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hn.bookmarksfly.cn

【使用说明】
来源：http://co.jctech888.com.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wv.yuntaijiaju.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bt.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ih.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rm.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://uo.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ba.nicolike.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://lz.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qb.bookmarksfly.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ge.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fi.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hu.huixiangedu.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ya.huixinmuqiang.cn

【文件统计】
来源：http://ss.huixinmuqiang.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tv.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://aw.muxihuayi.cn

目  录
来源：http://my.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://rh.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://po.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cu.jianghongdianzi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ol.muxihuayi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://he.huixinmuqiang.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://xi.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wd.521024.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ej.jctech888.com.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pc.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gj.hahajie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jj.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nv.jianghongdianzi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://vi.huanxung.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ji.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gr.bjjhwx.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qi.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ir.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ss.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ns.yuexingan06.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://jt.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uq.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vx.huixiangedu.cn

================================================================================
来源：http://xi.hahajie.cn

A. 基础语法与类型
来源：http://hx.hnjuh.cn

================================================================================
来源：http://ij.bjjhwx.cn

[A01] Hello World
来源：http://os.nicolike.cn

Py:   print("Hello, World!")
来源：http://bd.yuntaijiaju.cn

PHP:  echo "Hello, World!";
来源：http://qd.wgjwhj.cn

JS:   console.log("Hello, World!");
来源：http://np.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pk.hahajie.cn

Java: System.out.println("Hello, World!");
来源：http://vb.hahajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://bh.wgjwhj.cn

Ruby: puts "Hello, World!"
来源：http://vw.lnxyls.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lf.521024.cn

[A02] 变量声明与赋值
来源：http://ha.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eu.shxzskj.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://tk.hnjuh.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tx.521024.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gg.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://qm.asd995.cn

Go:   name := "Alex"; age := 20
来源：http://ek.nszjky.cn

Ruby: name = "Alex"; age = 20
来源：http://rr.yuntaijiaju.cn

C#:   string name = "Alex"; int age = 20;
来源：http://dz.muxihuayi.cn

[A03] 常量定义
来源：http://uk.asd995.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://vq.shxzukj.cn

PHP:  const PI = 3.14159;
来源：http://vb.9csxet.cn

JS:   const PI = 3.14159;
来源：http://wi.jianghongdianzi.cn

TS:   const PI: number = 3.14159;
来源：http://ss.asd995.cn

Java: static final double PI = 3.14159;
来源：http://hs.shxzskj.cn

Go:   const PI = 3.14159
来源：http://gw.huanxung.cn

Ruby: PI = 3.14159
来源：http://nq.bookmarksfly.cn

C#:   const double PI = 3.14159;
来源：http://ka.gzmigu.cn

[A04] 判断变量类型
来源：http://bo.asd995.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://gn.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xn.panjiajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://zu.huixiangedu.cn

TS:   typeof x; x instanceof Date
来源：http://du.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ct.bjjhwx.cn

Go:   reflect.TypeOf(x).Name()
来源：http://nx.521024.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://qc.lnxyls.cn

C#:   x.GetType().Name; x is int
来源：http://ll.chemitech.net.cn

[A05] 整数除法与取模
来源：http://bs.wgjwhj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://cg.hnjuh.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ho.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://np.jianghongdianzi.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nf.hahajie.cn

Java: 7 / 2; 7 % 2
来源：http://ag.shxzskj.cn

Go:   7 / 2; 7 % 2
来源：http://ad.huanxung.cn

Ruby: 7 / 2; 7 % 2
来源：http://ww.hahajie.cn

C#:   7 / 2; 7 % 2
来源：http://jb.shxzskj.cn

[A06] 字符串转数字
来源：http://vl.szsharing.cn

Py:   int("42"); float("3.14")
来源：http://iv.haigaiapp.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://cr.asd995.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xe.nicolike.cn

TS:   parseInt("42", 10); Number("42")
来源：http://df.hnjuh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://hp.hnjuh.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ns.shxzskj.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://kv.huixinmuqiang.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://gi.muxihuayi.cn

[A07] 数字转字符串
来源：http://al.521024.cn

Py:   str(42)
来源：http://gw.nszjky.cn

PHP:  (string) 42; strval(42)
来源：http://qr.szsharing.cn


<!-- 参考信息 -->