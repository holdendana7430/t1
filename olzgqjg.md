代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://vq.bjjhwx.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wa.lnxyls.cn

[U46] PHP：可空类型
来源：http://ne.asd995.cn

?string $name = null
来源：http://go.colortex.cn

[U47] PHP：联合类型
来源：http://ld.jianghongdianzi.cn

int|string $id
来源：http://lg.huixiangedu.cn

[U48] PHP：纯枚举
来源：http://zv.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tl.jctech888.com.cn

[U49] PHP：只读属性
来源：http://jk.chemitech.net.cn

public readonly string $name
来源：http://xt.nicolike.cn

[U50] PHP：构造器属性提升
来源：http://wy.lnxyls.cn

public function __construct(private int $id) {}
来源：http://sp.szsharing.cn

[U51] PHP：数组解构
来源：http://uk.nicolike.cn

[$a, $b] = $arr;
来源：http://bl.yuexingan06.cn

[U52] PHP：箭头函数
来源：http://iu.colortex.cn

$double = fn($x) => $x * 2;
来源：http://ht.haigaiapp.cn

[U53] PHP：空合并运算符
来源：http://dg.nicolike.cn

$v = $a ?? $b ?? "default";
来源：http://ty.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://jt.gzmigu.cn

$obj?->method()
来源：http://bb.jctech888.com.cn

[U55] PHP：match 表达式
来源：http://jb.chemitech.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://th.521024.cn

[U56] PHP：命名参数
来源：http://mq.huixiangedu.cn

f(a: 1, b: 2)
来源：http://gm.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://ld.asd995.cn

"值: {$a}"
来源：http://am.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://ve.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://le.szxytkj.cn

[U59] PHP：自定义排序
来源：http://dv.huanxung.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uy.yuntaijiaju.cn

[U60] PHP：JSON 编解码
来源：http://po.haigaiapp.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://yn.nicolike.cn

[U61] PHP：正则
来源：http://wp.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jd.shtwfgs.cn

[U62] PHP：日期对象
来源：http://xj.panjiajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xn.asd995.cn

[U63] PHP：文件读写
来源：http://as.asd995.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fo.newstarts.cn

[U64] PHP：目录遍历
来源：http://el.bjjhwx.cn

glob("dir/*.php");  scandir("dir");
来源：http://pn.9csxet.cn

[U65] PHP：会话
来源：http://ff.shxzskj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zj.yuexingan06.cn

[U66] PHP：设置 Cookie
来源：http://ef.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vk.lnxyls.cn

[U67] PHP：处理文件上传
来源：http://eu.bookmarksfly.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bm.nszjky.cn

[U68] PHP：PDO 连接
来源：http://xd.wgjwhj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rc.lnxyls.cn

[U69] PHP：PDO 预处理
来源：http://tu.szsharing.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://co.colortex.cn

[U70] PHP：PDO 事务
来源：http://gu.nicolike.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ym.hnjuh.cn

[U71] PHP：抛出异常
来源：http://km.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://vm.panjiajie.cn

[U72] PHP：写错误日志
来源：http://to.muxihuayi.cn

error_log("失败: " . $e->getMessage());
来源：http://yx.hnjuh.cn

[U73] PHP：读取 ini 配置
来源：http://em.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://nz.shtwfgs.cn

[U74] PHP：读取环境变量
来源：http://rc.9csxet.cn

getenv("APP_ENV") ?: "production"
来源：http://ci.szsharing.cn

[U75] PHP：依赖注入
来源：http://qo.shxzskj.cn

composer require psr/container
来源：http://bt.yuntaijiaju.cn

[U76] PHP：简单路由
来源：http://tf.nszjky.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qh.huixinmuqiang.cn

[U77] PHP：模板渲染
来源：http://bh.bookmarksfly.cn

composer require twig/twig
来源：http://zh.panjiajie.cn

[U78] PHP：单元测试
来源：http://ur.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://md.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://sq.bjjhwx.cn

composer require --dev phpstan/phpstan
来源：http://qq.asd995.cn

[U80] PHP：代码规范修复
来源：http://iq.yuexingan06.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kw.newstarts.cn

[U81] JS：初始化项目
来源：http://ib.shxzukj.cn

npm init -y;  npm i express
来源：http://ce.huixinmuqiang.cn

[U82] JS：package.json 脚本
来源：http://xy.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xh.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://mu.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://gw.521024.cn

[U84] JS：CommonJS 写法
来源：http://bx.huixinmuqiang.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kc.colortex.cn

[U85] JS：可选链
来源：http://in.newstarts.cn

a?.b?.c
来源：http://hx.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://ph.9csxet.cn

a ?? b
来源：http://aq.shtwfgs.cn

[U87] JS：解构默认值
来源：http://no.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://xj.lnxyls.cn

[U88] JS：对象展开合并
来源：http://ra.bjjhwx.cn

{ ...a, ...b }
来源：http://sm.nszjky.cn

[U89] JS：数组去重
来源：http://mt.asd995.cn

[...new Set(arr)]
来源：http://bg.chemitech.net.cn

[U90] JS：数字数组排序
来源：http://yu.hnjuh.cn

[...arr].sort((a, b) => a - b)
来源：http://uu.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://ut.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lo.muxihuayi.cn

[U92] JS：深拷贝
来源：http://bd.yuntaijiaju.cn

structuredClone(obj)
来源：http://dm.521024.cn

[U93] JS：模板字符串
来源：http://pw.521024.cn

`共 ${n} 条`
来源：http://jy.asd995.cn

[U94] JS：箭头函数
来源：http://ah.nszjky.cn

const double = x => x * 2;
来源：http://yc.colortex.cn

[U95] JS：Promise 包装
来源：http://zw.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://iy.huixiangedu.cn

[U96] JS：async/await 与异常
来源：http://lq.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pk.huanxung.cn

[U97] JS：并发请求
来源：http://mi.gzmigu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fh.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://ve.huixiangedu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://if.shtwfgs.cn

[U99] JS：事件监听
来源：http://ni.shxzukj.cn

el.addEventListener("click", e => {})
来源：http://ei.lnxyls.cn

[U100] JS：DOM 查询
来源：http://xm.hnjuh.cn

document.querySelector(".item")
来源：http://cw.9csxet.cn

[U101] JS：classList 操作
来源：http://hl.huixiangedu.cn

el.classList.toggle("active")
来源：http://tw.szsharing.cn

[U102] JS：本地存储
来源：http://np.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cm.521024.cn

[U103] JS：定时器
来源：http://cj.hnjuh.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zv.chemitech.net.cn

[U104] JS：防抖
来源：http://xa.szxytkj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://os.nicolike.cn

[U105] JS：节流
来源：http://pq.jctech888.com.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://rl.asd995.cn

[U106] JS：日期格式化
来源：http://vp.huanxung.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://es.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://dk.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ii.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://ht.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ii.shxzukj.cn

[U109] JS：数组分组
来源：http://wc.lnxyls.cn

Object.groupBy(arr, x => x.type)
来源：http://jg.yuexingan06.cn

[U110] JS：数组分块
来源：http://ad.panjiajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://jt.shxzskj.cn

[U111] JS：对象转 Map
来源：http://lp.521024.cn

new Map(Object.entries(obj))
来源：http://ax.huixinmuqiang.cn

[U112] JS：字符串补位
来源：http://ec.colortex.cn

"7".padStart(3, "0")
来源：http://ld.panjiajie.cn

[U113] JS：正则替换全部
来源：http://je.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://qr.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://kx.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://nr.9csxet.cn

[U115] JS：生成 UUID
来源：http://lc.muxihuayi.cn

crypto.randomUUID()
来源：http://ko.shxzskj.cn

[U116] JS：类型检查（JSDoc）
来源：http://jc.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ra.muxihuayi.cn

[U117] JS：单元测试
来源：http://cu.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://sn.muxihuayi.cn

[U118] JS：开发服务器
来源：http://cq.wgjwhj.cn

npm i -D vite;  npx vite
来源：http://zf.9csxet.cn

[U119] JS：生产构建
来源：http://qz.szxytkj.cn

npx vite build
来源：http://mo.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://kp.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://lx.huixiangedu.cn

================================================================================
来源：http://gu.huixinmuqiang.cn

统计汇总
来源：http://kf.haigaiapp.cn

================================================================================
来源：http://gz.muxihuayi.cn

按语言统计（条）：
来源：http://fj.nszjky.cn

Python ......... 252
来源：http://ai.jctech888.com.cn

PHP ............ 252
来源：http://di.yuntaijiaju.cn

JavaScript ..... 252
来源：http://zp.panjiajie.cn

TypeScript ..... 212
来源：http://qt.huixinmuqiang.cn

Java ........... 212
来源：http://rd.szsharing.cn

Go ............. 212
来源：http://th.hahajie.cn

Ruby ........... 212
来源：http://zk.bjjhwx.cn

C# ............. 212
来源：http://gi.nszjky.cn

C .............. 30
来源：http://ya.gzmigu.cn

C++ ............ 30
来源：http://hw.yuntaijiaju.cn

SQL ............ 90
来源：http://bz.shxzskj.cn

Bash ........... 80
来源：http://ic.asd995.cn

Kotlin ......... 15
来源：http://bx.chemitech.net.cn

Swift .......... 15
来源：http://cx.lnxyls.cn

Lua ............ 10
来源：http://xb.szxytkj.cn

Perl ........... 10
来源：http://tn.jctech888.com.cn

Scala .......... 10
来源：http://av.jctech888.com.cn

------------------------------------
来源：http://ou.shtwfgs.cn

合计 ........... 2106 条
来源：http://yx.lnxyls.cn

按章节统计：
来源：http://nr.bjjhwx.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://he.yuexingan06.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mc.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://jy.chemitech.net.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://vb.gzmigu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ie.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pp.muxihuayi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bo.shxzukj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ic.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vt.521024.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ab.nszjky.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ls.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xp.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nx.nszjky.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ll.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://og.gzmigu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ah.shxzskj.cn

Q SQL 专题                              90
来源：http://vr.huixinmuqiang.cn

R Bash 专题                             80
来源：http://ji.yuntaijiaju.cn

S C / C++ 专题                          60
来源：http://na.panjiajie.cn

T 其他语言补充                          60
来源：http://jo.jctech888.com.cn

U 高频实用片段                         120
来源：http://cy.yuexingan06.cn

------------------------------------
来源：http://fe.bjjhwx.cn

合计                                  2106 条
来源：http://rs.newstarts.cn

--------------------------------------------------------------------------------
来源：http://rn.hnjuh.cn

使用提醒
来源：http://qj.asd995.cn

--------------------------------------------------------------------------------
来源：http://ml.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ty.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xv.521024.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vj.nicolike.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hr.lnxyls.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://fn.lnxyls.cn

—— 文件结束 ——
来源：http://rv.shxzukj.cn

================================================================================
来源：http://ex.muxihuayi.cn

程序语言常见例子速查手册（2024 版）
来源：http://lj.huixinmuqiang.cn

Common Programming Examples Cheat Book
来源：http://fs.chemitech.net.cn

================================================================================
来源：http://xc.bjjhwx.cn

【收录内容】
来源：http://jb.shtwfgs.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://em.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ux.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://qx.muxihuayi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zo.shtwfgs.cn

【使用说明】
来源：http://gi.gzmigu.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://je.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zs.szxytkj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xh.jctech888.com.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hs.bjjhwx.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ip.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mf.huixinmuqiang.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://jm.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://dx.9csxet.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://xa.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nl.jctech888.com.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ip.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jk.huanxung.cn

【文件统计】
来源：http://hb.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://vs.newstarts.cn

--------------------------------------------------------------------------------
来源：http://na.bookmarksfly.cn

目  录
来源：http://xt.nicolike.cn

--------------------------------------------------------------------------------
来源：http://qg.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kc.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://lk.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mw.shxzukj.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ov.muxihuayi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ed.szsharing.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://tm.newstarts.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zf.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ri.gzmigu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ai.wgjwhj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jn.jctech888.com.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fr.jctech888.com.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://br.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ym.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yg.wgjwhj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yx.bjjhwx.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wf.yuntaijiaju.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wo.gzmigu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://vt.gzmigu.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hg.panjiajie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ha.haigaiapp.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://gp.gzmigu.cn

================================================================================
来源：http://de.lnxyls.cn

A. 基础语法与类型
来源：http://iw.lnxyls.cn

================================================================================
来源：http://jf.yuntaijiaju.cn

[A01] Hello World
来源：http://tl.hnjuh.cn

Py:   print("Hello, World!")
来源：http://ic.huixinmuqiang.cn

PHP:  echo "Hello, World!";
来源：http://rz.huixinmuqiang.cn

JS:   console.log("Hello, World!");
来源：http://pi.bookmarksfly.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://sm.shxzskj.cn

Java: System.out.println("Hello, World!");
来源：http://tp.yuntaijiaju.cn

Go:   fmt.Println("Hello, World!")
来源：http://nd.9csxet.cn

Ruby: puts "Hello, World!"
来源：http://pf.chemitech.net.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ne.lnxyls.cn

[A02] 变量声明与赋值
来源：http://zc.szsharing.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ko.hahajie.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ja.yuexingan06.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lf.panjiajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://to.asd995.cn

Java: String name = "Alex"; int age = 20;
来源：http://rn.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://ko.wgjwhj.cn

Ruby: name = "Alex"; age = 20
来源：http://ym.asd995.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xk.yuntaijiaju.cn

[A03] 常量定义
来源：http://an.bookmarksfly.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://an.newstarts.cn

PHP:  const PI = 3.14159;
来源：http://lg.huixiangedu.cn

JS:   const PI = 3.14159;
来源：http://bq.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://fl.shxzukj.cn

Java: static final double PI = 3.14159;
来源：http://xd.jianghongdianzi.cn

Go:   const PI = 3.14159
来源：http://gi.wgjwhj.cn

Ruby: PI = 3.14159
来源：http://pf.muxihuayi.cn

C#:   const double PI = 3.14159;
来源：http://xt.muxihuayi.cn

[A04] 判断变量类型
来源：http://xz.yuexingan06.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://um.newstarts.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ms.wgjwhj.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rn.szsharing.cn

TS:   typeof x; x instanceof Date
来源：http://yp.szsharing.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nz.hnjuh.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pz.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://iz.chemitech.net.cn

C#:   x.GetType().Name; x is int
来源：http://sx.newstarts.cn

[A05] 整数除法与取模
来源：http://ju.colortex.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://yj.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://tl.521024.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ct.hnjuh.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xd.nszjky.cn


<!-- 参考信息 -->