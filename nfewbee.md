代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://rs.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.521024.cn

[U46] PHP：可空类型
来源：http://yb.hahajie.cn

?string $name = null
来源：http://dv.shtwfgs.cn

[U47] PHP：联合类型
来源：http://gp.huixinmuqiang.cn

int|string $id
来源：http://cf.shxzukj.cn

[U48] PHP：纯枚举
来源：http://tj.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vk.nicolike.cn

[U49] PHP：只读属性
来源：http://zs.yuexingan06.cn

public readonly string $name
来源：http://xu.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://xf.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://qb.hahajie.cn

[U51] PHP：数组解构
来源：http://mi.521024.cn

[$a, $b] = $arr;
来源：http://zt.shxzukj.cn

[U52] PHP：箭头函数
来源：http://yo.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://yi.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://no.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://gy.nszjky.cn

[U54] PHP：空安全调用
来源：http://ly.jianghongdianzi.cn

$obj?->method()
来源：http://ti.nszjky.cn

[U55] PHP：match 表达式
来源：http://ga.newstarts.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gs.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://tb.panjiajie.cn

f(a: 1, b: 2)
来源：http://wh.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://il.hnjuh.cn

"值: {$a}"
来源：http://jw.asd995.cn

[U58] PHP：数组三件套
来源：http://cf.muxihuayi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rs.yuexingan06.cn

[U59] PHP：自定义排序
来源：http://vp.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://al.wgjwhj.cn

[U60] PHP：JSON 编解码
来源：http://hn.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ju.hnjuh.cn

[U61] PHP：正则
来源：http://np.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tn.muxihuayi.cn

[U62] PHP：日期对象
来源：http://fr.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gb.jianghongdianzi.cn

[U63] PHP：文件读写
来源：http://wv.panjiajie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ea.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://gx.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://yr.jctech888.com.cn

[U65] PHP：会话
来源：http://vn.bookmarksfly.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pc.lnxyls.cn

[U66] PHP：设置 Cookie
来源：http://br.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zn.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://or.muxihuayi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nh.huixinmuqiang.cn

[U68] PHP：PDO 连接
来源：http://eb.huixinmuqiang.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bz.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://hq.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kx.yuexingan06.cn

[U70] PHP：PDO 事务
来源：http://jy.hnjuh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ng.szxytkj.cn

[U71] PHP：抛出异常
来源：http://vd.panjiajie.cn

throw new RuntimeException("失败", 500);
来源：http://jv.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://ci.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://bk.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://ws.yuntaijiaju.cn

parse_ini_file("config.ini", true)
来源：http://kn.nicolike.cn

[U74] PHP：读取环境变量
来源：http://vg.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://zg.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://el.nszjky.cn

composer require psr/container
来源：http://ov.muxihuayi.cn

[U76] PHP：简单路由
来源：http://uz.haigaiapp.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tj.muxihuayi.cn

[U77] PHP：模板渲染
来源：http://by.shxzskj.cn

composer require twig/twig
来源：http://xw.huanxung.cn

[U78] PHP：单元测试
来源：http://hh.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://fo.newstarts.cn

[U79] PHP：静态分析
来源：http://bt.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://fi.gzmigu.cn

[U80] PHP：代码规范修复
来源：http://na.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wo.shxzskj.cn

[U81] JS：初始化项目
来源：http://kd.huanxung.cn

npm init -y;  npm i express
来源：http://di.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://fh.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pe.9csxet.cn

[U83] JS：ES Module 导入导出
来源：http://xm.shxzskj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iw.shtwfgs.cn

[U84] JS：CommonJS 写法
来源：http://cn.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ka.bjjhwx.cn

[U85] JS：可选链
来源：http://fj.bjjhwx.cn

a?.b?.c
来源：http://xy.bookmarksfly.cn

[U86] JS：空值合并
来源：http://kb.huixiangedu.cn

a ?? b
来源：http://ir.huanxung.cn

[U87] JS：解构默认值
来源：http://oh.bookmarksfly.cn

const { a = 1, b = 2 } = obj;
来源：http://tv.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://vs.asd995.cn

{ ...a, ...b }
来源：http://fx.hnjuh.cn

[U89] JS：数组去重
来源：http://jh.bookmarksfly.cn

[...new Set(arr)]
来源：http://rj.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://ol.haigaiapp.cn

[...arr].sort((a, b) => a - b)
来源：http://ok.hahajie.cn

[U91] JS：对象键值遍历
来源：http://yj.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tb.wgjwhj.cn

[U92] JS：深拷贝
来源：http://lj.muxihuayi.cn

structuredClone(obj)
来源：http://ok.chemitech.net.cn

[U93] JS：模板字符串
来源：http://ws.szsharing.cn

`共 ${n} 条`
来源：http://mg.muxihuayi.cn

[U94] JS：箭头函数
来源：http://xg.yuntaijiaju.cn

const double = x => x * 2;
来源：http://rn.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://wc.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://zu.jianghongdianzi.cn

[U96] JS：async/await 与异常
来源：http://eb.huixinmuqiang.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fm.newstarts.cn

[U97] JS：并发请求
来源：http://uc.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qn.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://kt.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lh.yuntaijiaju.cn

[U99] JS：事件监听
来源：http://xe.szsharing.cn

el.addEventListener("click", e => {})
来源：http://nb.hahajie.cn

[U100] JS：DOM 查询
来源：http://vt.huixiangedu.cn

document.querySelector(".item")
来源：http://as.muxihuayi.cn

[U101] JS：classList 操作
来源：http://cm.muxihuayi.cn

el.classList.toggle("active")
来源：http://an.nicolike.cn

[U102] JS：本地存储
来源：http://rp.yuexingan06.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dl.szsharing.cn

[U103] JS：定时器
来源：http://pd.szsharing.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zd.haigaiapp.cn

[U104] JS：防抖
来源：http://cl.hnjuh.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dy.colortex.cn

[U105] JS：节流
来源：http://om.huixinmuqiang.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fg.huanxung.cn

[U106] JS：日期格式化
来源：http://eb.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ro.panjiajie.cn

[U107] JS：数字千分位
来源：http://dp.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://no.szsharing.cn

[U108] JS：随机整数
来源：http://lr.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dy.asd995.cn

[U109] JS：数组分组
来源：http://cm.huixiangedu.cn

Object.groupBy(arr, x => x.type)
来源：http://kr.wgjwhj.cn

[U110] JS：数组分块
来源：http://al.szsharing.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://cu.szxytkj.cn

[U111] JS：对象转 Map
来源：http://qh.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://pl.asd995.cn

[U112] JS：字符串补位
来源：http://tw.hahajie.cn

"7".padStart(3, "0")
来源：http://ol.gzmigu.cn

[U113] JS：正则替换全部
来源：http://cx.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://ii.huanxung.cn

[U114] JS：JSON 深比较
来源：http://le.bookmarksfly.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mb.nicolike.cn

[U115] JS：生成 UUID
来源：http://ry.muxihuayi.cn

crypto.randomUUID()
来源：http://tg.panjiajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://cn.jianghongdianzi.cn

/** @param {string} name */ function f(name) {}
来源：http://zq.wgjwhj.cn

[U117] JS：单元测试
来源：http://ep.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://qe.newstarts.cn

[U118] JS：开发服务器
来源：http://ju.lnxyls.cn

npm i -D vite;  npx vite
来源：http://gh.lnxyls.cn

[U119] JS：生产构建
来源：http://ax.asd995.cn

npx vite build
来源：http://wu.bookmarksfly.cn

[U120] JS：读取环境变量（Vite）
来源：http://ok.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://vs.nszjky.cn

================================================================================
来源：http://mp.huixinmuqiang.cn

统计汇总
来源：http://za.yuexingan06.cn

================================================================================
来源：http://hv.bookmarksfly.cn

按语言统计（条）：
来源：http://iy.bjjhwx.cn

Python ......... 252
来源：http://jx.shtwfgs.cn

PHP ............ 252
来源：http://xz.haigaiapp.cn

JavaScript ..... 252
来源：http://nc.shxzukj.cn

TypeScript ..... 212
来源：http://wp.huanxung.cn

Java ........... 212
来源：http://ju.gzmigu.cn

Go ............. 212
来源：http://fh.gzmigu.cn

Ruby ........... 212
来源：http://aw.huanxung.cn

C# ............. 212
来源：http://sx.szxytkj.cn

C .............. 30
来源：http://aq.huixiangedu.cn

C++ ............ 30
来源：http://ft.gzmigu.cn

SQL ............ 90
来源：http://cj.jctech888.com.cn

Bash ........... 80
来源：http://sp.shtwfgs.cn

Kotlin ......... 15
来源：http://dn.huixinmuqiang.cn

Swift .......... 15
来源：http://kk.nicolike.cn

Lua ............ 10
来源：http://rj.huixiangedu.cn

Perl ........... 10
来源：http://uj.yuexingan06.cn

Scala .......... 10
来源：http://yh.chemitech.net.cn

------------------------------------
来源：http://jf.lnxyls.cn

合计 ........... 2106 条
来源：http://og.yuntaijiaju.cn

按章节统计：
来源：http://at.wgjwhj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zf.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ab.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nx.bjjhwx.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jq.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ej.nicolike.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://aq.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tm.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://cr.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fz.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nn.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ch.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kc.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mh.wgjwhj.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pt.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wh.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mi.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://im.gzmigu.cn

R Bash 专题                             80
来源：http://ah.bjjhwx.cn

S C / C++ 专题                          60
来源：http://cm.newstarts.cn

T 其他语言补充                          60
来源：http://bn.nicolike.cn

U 高频实用片段                         120
来源：http://dk.chemitech.net.cn

------------------------------------
来源：http://hi.bjjhwx.cn

合计                                  2106 条
来源：http://wj.9csxet.cn

--------------------------------------------------------------------------------
来源：http://if.huixinmuqiang.cn

使用提醒
来源：http://gl.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://qv.huanxung.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://kl.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://hs.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ec.lnxyls.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bo.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wl.shxzskj.cn

—— 文件结束 ——
来源：http://kj.nszjky.cn

================================================================================
来源：http://st.jctech888.com.cn

程序语言常见例子速查手册（2024 版）
来源：http://eu.jctech888.com.cn

Common Programming Examples Cheat Book
来源：http://uo.jianghongdianzi.cn

================================================================================
来源：http://ah.muxihuayi.cn

【收录内容】
来源：http://zd.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yz.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vb.nszjky.cn

SQL · Bash · C · C++
来源：http://vj.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pt.gzmigu.cn

【使用说明】
来源：http://my.bjjhwx.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://oe.chemitech.net.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bn.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xi.huanxung.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uy.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dr.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pj.9csxet.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://yx.bjjhwx.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ky.jctech888.com.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ta.nicolike.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://df.szsharing.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jf.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://go.haigaiapp.cn

【文件统计】
来源：http://gi.szxytkj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://gy.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zp.jctech888.com.cn

目  录
来源：http://mt.asd995.cn

--------------------------------------------------------------------------------
来源：http://cu.panjiajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vf.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vx.huixiangedu.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ou.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wr.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hf.9csxet.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bg.bookmarksfly.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bw.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://xa.huixinmuqiang.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dg.haigaiapp.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ur.panjiajie.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://td.asd995.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ft.nszjky.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wi.lnxyls.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jn.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://oh.newstarts.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dc.chemitech.net.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://gi.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://do.jianghongdianzi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://fr.nicolike.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hc.jianghongdianzi.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://fw.panjiajie.cn

================================================================================
来源：http://mv.gzmigu.cn

A. 基础语法与类型
来源：http://df.szsharing.cn

================================================================================
来源：http://pn.panjiajie.cn

[A01] Hello World
来源：http://sp.huanxung.cn

Py:   print("Hello, World!")
来源：http://jg.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://dt.huanxung.cn

JS:   console.log("Hello, World!");
来源：http://zw.chemitech.net.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xv.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://mb.nicolike.cn

Go:   fmt.Println("Hello, World!")
来源：http://ki.shtwfgs.cn

Ruby: puts "Hello, World!"
来源：http://yf.hahajie.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://uy.szsharing.cn

[A02] 变量声明与赋值
来源：http://nk.9csxet.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://qe.9csxet.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://lh.huanxung.cn

JS:   let name = "Alex"; const age = 20;
来源：http://vv.nszjky.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mm.huixiangedu.cn

Java: String name = "Alex"; int age = 20;
来源：http://xd.bookmarksfly.cn

Go:   name := "Alex"; age := 20
来源：http://qe.shxzskj.cn

Ruby: name = "Alex"; age = 20
来源：http://un.szsharing.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hs.lnxyls.cn

[A03] 常量定义
来源：http://ut.nicolike.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tp.yuexingan06.cn

PHP:  const PI = 3.14159;
来源：http://cj.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://jd.shxzskj.cn

TS:   const PI: number = 3.14159;
来源：http://kp.bookmarksfly.cn

Java: static final double PI = 3.14159;
来源：http://ke.haigaiapp.cn

Go:   const PI = 3.14159
来源：http://ke.huixinmuqiang.cn

Ruby: PI = 3.14159
来源：http://be.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://ga.yuexingan06.cn

[A04] 判断变量类型
来源：http://al.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ty.jctech888.com.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bd.hahajie.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ef.chemitech.net.cn

TS:   typeof x; x instanceof Date
来源：http://tm.jctech888.com.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://sk.colortex.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sz.nszjky.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://xk.huanxung.cn

C#:   x.GetType().Name; x is int
来源：http://pr.yuexingan06.cn

[A05] 整数除法与取模
来源：http://kj.shxzukj.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://li.yuexingan06.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://pb.bjjhwx.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://kl.shtwfgs.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mj.wgjwhj.cn


<!-- 参考信息 -->