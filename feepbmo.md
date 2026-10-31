代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://vt.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://vw.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://ai.521024.cn

?string $name = null
来源：http://jb.newstarts.cn

[U47] PHP：联合类型
来源：http://zl.nszjky.cn

int|string $id
来源：http://en.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://bw.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://em.huixinmuqiang.cn

[U49] PHP：只读属性
来源：http://pd.bookmarksfly.cn

public readonly string $name
来源：http://rj.bookmarksfly.cn

[U50] PHP：构造器属性提升
来源：http://ty.newstarts.cn

public function __construct(private int $id) {}
来源：http://yf.szxytkj.cn

[U51] PHP：数组解构
来源：http://sf.jianghongdianzi.cn

[$a, $b] = $arr;
来源：http://cy.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://zm.lnxyls.cn

$double = fn($x) => $x * 2;
来源：http://jk.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://oi.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://wv.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ua.hahajie.cn

$obj?->method()
来源：http://jq.chemitech.net.cn

[U55] PHP：match 表达式
来源：http://lp.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://cg.nicolike.cn

[U56] PHP：命名参数
来源：http://yc.colortex.cn

f(a: 1, b: 2)
来源：http://kq.newstarts.cn

[U57] PHP：字符串插值
来源：http://ol.bjjhwx.cn

"值: {$a}"
来源：http://dh.lnxyls.cn

[U58] PHP：数组三件套
来源：http://zq.nszjky.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jj.521024.cn

[U59] PHP：自定义排序
来源：http://xb.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rn.lnxyls.cn

[U60] PHP：JSON 编解码
来源：http://iv.nicolike.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lk.huixinmuqiang.cn

[U61] PHP：正则
来源：http://bi.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fn.haigaiapp.cn

[U62] PHP：日期对象
来源：http://ez.bookmarksfly.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pr.bookmarksfly.cn

[U63] PHP：文件读写
来源：http://nz.szxytkj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://af.haigaiapp.cn

[U64] PHP：目录遍历
来源：http://ei.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://hl.chemitech.net.cn

[U65] PHP：会话
来源：http://ze.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://lx.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://lw.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ls.jianghongdianzi.cn

[U67] PHP：处理文件上传
来源：http://es.szxytkj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bi.yuntaijiaju.cn

[U68] PHP：PDO 连接
来源：http://ci.shxzukj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iy.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://zi.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zr.shxzskj.cn

[U70] PHP：PDO 事务
来源：http://zl.shxzukj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nr.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://iy.huixiangedu.cn

throw new RuntimeException("失败", 500);
来源：http://io.colortex.cn

[U72] PHP：写错误日志
来源：http://fk.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://ps.huixinmuqiang.cn

[U73] PHP：读取 ini 配置
来源：http://si.lnxyls.cn

parse_ini_file("config.ini", true)
来源：http://ta.yuntaijiaju.cn

[U74] PHP：读取环境变量
来源：http://ht.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://gb.521024.cn

[U75] PHP：依赖注入
来源：http://lz.jianghongdianzi.cn

composer require psr/container
来源：http://op.jctech888.com.cn

[U76] PHP：简单路由
来源：http://jy.asd995.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ik.panjiajie.cn

[U77] PHP：模板渲染
来源：http://cf.9csxet.cn

composer require twig/twig
来源：http://dy.muxihuayi.cn

[U78] PHP：单元测试
来源：http://zx.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://vk.szsharing.cn

[U79] PHP：静态分析
来源：http://kv.hahajie.cn

composer require --dev phpstan/phpstan
来源：http://dp.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://qh.shtwfgs.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://zz.hnjuh.cn

[U81] JS：初始化项目
来源：http://mf.huanxung.cn

npm init -y;  npm i express
来源：http://wj.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://sz.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qo.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://gt.521024.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fv.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://ei.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kd.521024.cn

[U85] JS：可选链
来源：http://uh.muxihuayi.cn

a?.b?.c
来源：http://ko.szxytkj.cn

[U86] JS：空值合并
来源：http://pc.muxihuayi.cn

a ?? b
来源：http://bm.hnjuh.cn

[U87] JS：解构默认值
来源：http://uq.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://ut.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://kq.yuexingan06.cn

{ ...a, ...b }
来源：http://wm.shxzskj.cn

[U89] JS：数组去重
来源：http://fr.nicolike.cn

[...new Set(arr)]
来源：http://ya.szsharing.cn

[U90] JS：数字数组排序
来源：http://bh.huanxung.cn

[...arr].sort((a, b) => a - b)
来源：http://yz.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://no.lnxyls.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pj.huixiangedu.cn

[U92] JS：深拷贝
来源：http://cr.huixinmuqiang.cn

structuredClone(obj)
来源：http://op.szxytkj.cn

[U93] JS：模板字符串
来源：http://vc.bookmarksfly.cn

`共 ${n} 条`
来源：http://gz.chemitech.net.cn

[U94] JS：箭头函数
来源：http://ax.shxzskj.cn

const double = x => x * 2;
来源：http://ae.szxytkj.cn

[U95] JS：Promise 包装
来源：http://to.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://qb.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://sm.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://sg.panjiajie.cn

[U97] JS：并发请求
来源：http://om.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://la.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://rn.panjiajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jw.bookmarksfly.cn

[U99] JS：事件监听
来源：http://mz.hahajie.cn

el.addEventListener("click", e => {})
来源：http://gr.bookmarksfly.cn

[U100] JS：DOM 查询
来源：http://jy.szxytkj.cn

document.querySelector(".item")
来源：http://db.asd995.cn

[U101] JS：classList 操作
来源：http://nm.haigaiapp.cn

el.classList.toggle("active")
来源：http://up.jctech888.com.cn

[U102] JS：本地存储
来源：http://co.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ad.newstarts.cn

[U103] JS：定时器
来源：http://wc.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fr.gzmigu.cn

[U104] JS：防抖
来源：http://fg.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bn.bjjhwx.cn

[U105] JS：节流
来源：http://ye.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hn.colortex.cn

[U106] JS：日期格式化
来源：http://yh.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ty.nszjky.cn

[U107] JS：数字千分位
来源：http://rl.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yf.bjjhwx.cn

[U108] JS：随机整数
来源：http://xr.bjjhwx.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hx.bookmarksfly.cn

[U109] JS：数组分组
来源：http://at.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://sf.szsharing.cn

[U110] JS：数组分块
来源：http://te.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ok.yuexingan06.cn

[U111] JS：对象转 Map
来源：http://lj.nicolike.cn

new Map(Object.entries(obj))
来源：http://nv.jctech888.com.cn

[U112] JS：字符串补位
来源：http://no.shxzukj.cn

"7".padStart(3, "0")
来源：http://zi.yuexingan06.cn

[U113] JS：正则替换全部
来源：http://tw.nszjky.cn

s.replaceAll("a", "b")
来源：http://rg.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://ao.9csxet.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://aw.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://tv.521024.cn

crypto.randomUUID()
来源：http://us.huixiangedu.cn

[U116] JS：类型检查（JSDoc）
来源：http://os.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://si.nszjky.cn

[U117] JS：单元测试
来源：http://ce.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://tq.9csxet.cn

[U118] JS：开发服务器
来源：http://dj.panjiajie.cn

npm i -D vite;  npx vite
来源：http://to.wgjwhj.cn

[U119] JS：生产构建
来源：http://ip.newstarts.cn

npx vite build
来源：http://xm.huixinmuqiang.cn

[U120] JS：读取环境变量（Vite）
来源：http://lz.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://nv.nicolike.cn

================================================================================
来源：http://et.shxzukj.cn

统计汇总
来源：http://si.haigaiapp.cn

================================================================================
来源：http://ld.shxzskj.cn

按语言统计（条）：
来源：http://py.9csxet.cn

Python ......... 252
来源：http://tx.huixinmuqiang.cn

PHP ............ 252
来源：http://qy.hahajie.cn

JavaScript ..... 252
来源：http://pq.colortex.cn

TypeScript ..... 212
来源：http://kb.newstarts.cn

Java ........... 212
来源：http://kg.szxytkj.cn

Go ............. 212
来源：http://nh.haigaiapp.cn

Ruby ........... 212
来源：http://ur.huixiangedu.cn

C# ............. 212
来源：http://fr.9csxet.cn

C .............. 30
来源：http://mn.bjjhwx.cn

C++ ............ 30
来源：http://jw.newstarts.cn

SQL ............ 90
来源：http://qe.huixinmuqiang.cn

Bash ........... 80
来源：http://ak.hnjuh.cn

Kotlin ......... 15
来源：http://xy.521024.cn

Swift .......... 15
来源：http://de.bjjhwx.cn

Lua ............ 10
来源：http://ra.hnjuh.cn

Perl ........... 10
来源：http://lt.jianghongdianzi.cn

Scala .......... 10
来源：http://xw.hahajie.cn

------------------------------------
来源：http://wo.wgjwhj.cn

合计 ........... 2106 条
来源：http://zb.huixinmuqiang.cn

按章节统计：
来源：http://ek.szxytkj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rq.szsharing.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yo.yuexingan06.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ww.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://an.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ts.wgjwhj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://lo.szxytkj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://py.panjiajie.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pe.9csxet.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xh.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ll.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ps.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ft.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://tb.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bw.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nc.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://uw.panjiajie.cn

Q SQL 专题                              90
来源：http://sl.bookmarksfly.cn

R Bash 专题                             80
来源：http://vh.gzmigu.cn

S C / C++ 专题                          60
来源：http://pe.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://ix.jctech888.com.cn

U 高频实用片段                         120
来源：http://bl.newstarts.cn

------------------------------------
来源：http://zr.wgjwhj.cn

合计                                  2106 条
来源：http://wd.hahajie.cn

--------------------------------------------------------------------------------
来源：http://li.muxihuayi.cn

使用提醒
来源：http://sa.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://yy.huixiangedu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://us.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cr.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://gd.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ev.gzmigu.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vd.huixinmuqiang.cn

—— 文件结束 ——
来源：http://os.muxihuayi.cn

================================================================================
来源：http://sj.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://hj.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://tg.yuntaijiaju.cn

================================================================================
来源：http://dd.panjiajie.cn

【收录内容】
来源：http://dx.gzmigu.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jl.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ul.huixiangedu.cn

SQL · Bash · C · C++
来源：http://jb.panjiajie.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nr.521024.cn

【使用说明】
来源：http://dx.chemitech.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ow.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ue.asd995.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wy.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://no.szsharing.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://fm.jianghongdianzi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wu.jctech888.com.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vi.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wc.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pr.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ed.shxzskj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://at.newstarts.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wa.huixiangedu.cn

【文件统计】
来源：http://yb.nszjky.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gt.huixiangedu.cn

--------------------------------------------------------------------------------
来源：http://ho.gzmigu.cn

目  录
来源：http://pz.asd995.cn

--------------------------------------------------------------------------------
来源：http://se.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mg.nicolike.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tg.huanxung.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vp.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://eu.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bm.haigaiapp.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mk.colortex.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hb.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://dm.szsharing.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ez.huanxung.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ec.chemitech.net.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://js.9csxet.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://jb.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lw.haigaiapp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xo.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ip.shxzskj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gz.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://om.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xt.wgjwhj.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://qm.colortex.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zp.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://zw.panjiajie.cn

================================================================================
来源：http://bf.jianghongdianzi.cn

A. 基础语法与类型
来源：http://hi.9csxet.cn

================================================================================
来源：http://dj.panjiajie.cn

[A01] Hello World
来源：http://sq.chemitech.net.cn

Py:   print("Hello, World!")
来源：http://bb.wgjwhj.cn

PHP:  echo "Hello, World!";
来源：http://td.szsharing.cn

JS:   console.log("Hello, World!");
来源：http://yg.jianghongdianzi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://po.gzmigu.cn

Java: System.out.println("Hello, World!");
来源：http://gq.colortex.cn

Go:   fmt.Println("Hello, World!")
来源：http://vp.lnxyls.cn

Ruby: puts "Hello, World!"
来源：http://ea.9csxet.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://lf.muxihuayi.cn

[A02] 变量声明与赋值
来源：http://vx.asd995.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qb.nicolike.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://bc.wgjwhj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://wv.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xw.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://ml.hahajie.cn

Go:   name := "Alex"; age := 20
来源：http://zp.chemitech.net.cn

Ruby: name = "Alex"; age = 20
来源：http://rb.huixinmuqiang.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ae.yuexingan06.cn

[A03] 常量定义
来源：http://sb.jianghongdianzi.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://pv.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://ww.huixinmuqiang.cn

JS:   const PI = 3.14159;
来源：http://co.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://uq.lnxyls.cn

Java: static final double PI = 3.14159;
来源：http://ib.wgjwhj.cn

Go:   const PI = 3.14159
来源：http://tr.szxytkj.cn

Ruby: PI = 3.14159
来源：http://fo.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://bd.muxihuayi.cn

[A04] 判断变量类型
来源：http://ey.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://lp.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oa.haigaiapp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rr.colortex.cn

TS:   typeof x; x instanceof Date
来源：http://ly.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://fc.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://qb.newstarts.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://si.newstarts.cn

C#:   x.GetType().Name; x is int
来源：http://qh.szsharing.cn

[A05] 整数除法与取模
来源：http://ff.lnxyls.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ml.nicolike.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://oq.huixinmuqiang.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://fn.bookmarksfly.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://vf.521024.cn


<!-- 参考信息 -->