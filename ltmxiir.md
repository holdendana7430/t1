代发 wailian999

[U47] PHP：联合类型
来源：http://zr.bjjhwx.cn

int|string $id
来源：http://zy.nicolike.cn

[U48] PHP：纯枚举
来源：http://be.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xy.huixiangedu.cn

[U49] PHP：只读属性
来源：http://ze.hnjuh.cn

public readonly string $name
来源：http://fk.shtwfgs.cn

[U50] PHP：构造器属性提升
来源：http://ed.9csxet.cn

public function __construct(private int $id) {}
来源：http://yy.nszjky.cn

[U51] PHP：数组解构
来源：http://dh.panjiajie.cn

[$a, $b] = $arr;
来源：http://fc.chemitech.net.cn

[U52] PHP：箭头函数
来源：http://ip.jctech888.com.cn

$double = fn($x) => $x * 2;
来源：http://my.lnxyls.cn

[U53] PHP：空合并运算符
来源：http://sl.muxihuayi.cn

$v = $a ?? $b ?? "default";
来源：http://ol.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://pa.nicolike.cn

$obj?->method()
来源：http://ba.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://vb.hahajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nr.szsharing.cn

[U56] PHP：命名参数
来源：http://mr.szxytkj.cn

f(a: 1, b: 2)
来源：http://hm.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://nf.bookmarksfly.cn

"值: {$a}"
来源：http://ms.yuntaijiaju.cn

[U58] PHP：数组三件套
来源：http://zh.panjiajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ha.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://fq.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ut.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://hf.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ek.jianghongdianzi.cn

[U61] PHP：正则
来源：http://re.haigaiapp.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ry.szxytkj.cn

[U62] PHP：日期对象
来源：http://lh.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ef.bjjhwx.cn

[U63] PHP：文件读写
来源：http://zl.bjjhwx.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yb.gzmigu.cn

[U64] PHP：目录遍历
来源：http://bd.shxzskj.cn

glob("dir/*.php");  scandir("dir");
来源：http://xv.yuexingan06.cn

[U65] PHP：会话
来源：http://ql.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kj.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://eu.newstarts.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hs.muxihuayi.cn

[U67] PHP：处理文件上传
来源：http://uk.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tr.wgjwhj.cn

[U68] PHP：PDO 连接
来源：http://gj.muxihuayi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kq.asd995.cn

[U69] PHP：PDO 预处理
来源：http://yz.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rn.huixinmuqiang.cn

[U70] PHP：PDO 事务
来源：http://af.asd995.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jb.nicolike.cn

[U71] PHP：抛出异常
来源：http://nr.jctech888.com.cn

throw new RuntimeException("失败", 500);
来源：http://nz.521024.cn

[U72] PHP：写错误日志
来源：http://df.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://bz.hahajie.cn

[U73] PHP：读取 ini 配置
来源：http://rk.bjjhwx.cn

parse_ini_file("config.ini", true)
来源：http://bb.szsharing.cn

[U74] PHP：读取环境变量
来源：http://gd.nicolike.cn

getenv("APP_ENV") ?: "production"
来源：http://lt.shxzskj.cn

[U75] PHP：依赖注入
来源：http://xd.hahajie.cn

composer require psr/container
来源：http://yg.huanxung.cn

[U76] PHP：简单路由
来源：http://al.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gn.szxytkj.cn

[U77] PHP：模板渲染
来源：http://nk.yuexingan06.cn

composer require twig/twig
来源：http://hh.jctech888.com.cn

[U78] PHP：单元测试
来源：http://hf.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://mh.yuntaijiaju.cn

[U79] PHP：静态分析
来源：http://ru.jianghongdianzi.cn

composer require --dev phpstan/phpstan
来源：http://sr.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://cv.muxihuayi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wb.yuexingan06.cn

[U81] JS：初始化项目
来源：http://ik.9csxet.cn

npm init -y;  npm i express
来源：http://ir.hahajie.cn

[U82] JS：package.json 脚本
来源：http://rq.colortex.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gf.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://hg.bjjhwx.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kt.lnxyls.cn

[U84] JS：CommonJS 写法
来源：http://mr.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wj.hahajie.cn

[U85] JS：可选链
来源：http://bi.shtwfgs.cn

a?.b?.c
来源：http://yx.huixiangedu.cn

[U86] JS：空值合并
来源：http://sq.huixinmuqiang.cn

a ?? b
来源：http://et.panjiajie.cn

[U87] JS：解构默认值
来源：http://cr.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://vc.hnjuh.cn

[U88] JS：对象展开合并
来源：http://it.huixiangedu.cn

{ ...a, ...b }
来源：http://mc.9csxet.cn

[U89] JS：数组去重
来源：http://ro.huanxung.cn

[...new Set(arr)]
来源：http://sx.huixiangedu.cn

[U90] JS：数字数组排序
来源：http://qq.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://cb.hahajie.cn

[U91] JS：对象键值遍历
来源：http://vz.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pr.hahajie.cn

[U92] JS：深拷贝
来源：http://tn.szxytkj.cn

structuredClone(obj)
来源：http://gl.huixiangedu.cn

[U93] JS：模板字符串
来源：http://rd.hahajie.cn

`共 ${n} 条`
来源：http://hi.colortex.cn

[U94] JS：箭头函数
来源：http://eg.nicolike.cn

const double = x => x * 2;
来源：http://rm.huanxung.cn

[U95] JS：Promise 包装
来源：http://my.521024.cn

new Promise((resolve, reject) => {})
来源：http://mf.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://wk.bjjhwx.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qv.shxzukj.cn

[U97] JS：并发请求
来源：http://dd.shxzukj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://un.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://df.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vq.chemitech.net.cn

[U99] JS：事件监听
来源：http://ag.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://as.jctech888.com.cn

[U100] JS：DOM 查询
来源：http://fe.wgjwhj.cn

document.querySelector(".item")
来源：http://eh.hnjuh.cn

[U101] JS：classList 操作
来源：http://xk.bookmarksfly.cn

el.classList.toggle("active")
来源：http://ax.shxzskj.cn

[U102] JS：本地存储
来源：http://au.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jb.bjjhwx.cn

[U103] JS：定时器
来源：http://qe.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://nu.asd995.cn

[U104] JS：防抖
来源：http://pd.9csxet.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ey.521024.cn

[U105] JS：节流
来源：http://hg.bookmarksfly.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ll.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://ae.shxzukj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zb.nszjky.cn

[U107] JS：数字千分位
来源：http://ck.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ez.huixiangedu.cn

[U108] JS：随机整数
来源：http://cm.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://na.lnxyls.cn

[U109] JS：数组分组
来源：http://zl.shxzskj.cn

Object.groupBy(arr, x => x.type)
来源：http://xh.szsharing.cn

[U110] JS：数组分块
来源：http://lc.shtwfgs.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hu.521024.cn

[U111] JS：对象转 Map
来源：http://hj.hahajie.cn

new Map(Object.entries(obj))
来源：http://ld.bookmarksfly.cn

[U112] JS：字符串补位
来源：http://ew.szsharing.cn

"7".padStart(3, "0")
来源：http://iy.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://gg.asd995.cn

s.replaceAll("a", "b")
来源：http://pi.szsharing.cn

[U114] JS：JSON 深比较
来源：http://up.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kz.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://ow.jianghongdianzi.cn

crypto.randomUUID()
来源：http://ss.colortex.cn

[U116] JS：类型检查（JSDoc）
来源：http://il.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://nw.hahajie.cn

[U117] JS：单元测试
来源：http://xw.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://pk.shxzukj.cn

[U118] JS：开发服务器
来源：http://xg.colortex.cn

npm i -D vite;  npx vite
来源：http://yk.shtwfgs.cn

[U119] JS：生产构建
来源：http://to.nszjky.cn

npx vite build
来源：http://ed.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://vf.chemitech.net.cn

import.meta.env.VITE_API_URL
来源：http://il.wgjwhj.cn

================================================================================
来源：http://zb.haigaiapp.cn

统计汇总
来源：http://gw.shtwfgs.cn

================================================================================
来源：http://sd.yuntaijiaju.cn

按语言统计（条）：
来源：http://ba.yuexingan06.cn

Python ......... 252
来源：http://hn.muxihuayi.cn

PHP ............ 252
来源：http://bf.colortex.cn

JavaScript ..... 252
来源：http://ru.bookmarksfly.cn

TypeScript ..... 212
来源：http://ba.panjiajie.cn

Java ........... 212
来源：http://wu.huanxung.cn

Go ............. 212
来源：http://fi.shxzskj.cn

Ruby ........... 212
来源：http://dk.muxihuayi.cn

C# ............. 212
来源：http://mu.huixiangedu.cn

C .............. 30
来源：http://ds.shxzukj.cn

C++ ............ 30
来源：http://zf.szsharing.cn

SQL ............ 90
来源：http://tw.yuexingan06.cn

Bash ........... 80
来源：http://pq.gzmigu.cn

Kotlin ......... 15
来源：http://qm.panjiajie.cn

Swift .......... 15
来源：http://ea.hahajie.cn

Lua ............ 10
来源：http://jy.huanxung.cn

Perl ........... 10
来源：http://oj.hahajie.cn

Scala .......... 10
来源：http://hk.9csxet.cn

------------------------------------
来源：http://er.wgjwhj.cn

合计 ........... 2106 条
来源：http://ca.shxzukj.cn

按章节统计：
来源：http://eb.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ui.yuntaijiaju.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://yg.9csxet.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zn.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ng.newstarts.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gv.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ec.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ir.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://hm.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cc.shxzukj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xv.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ir.asd995.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yq.colortex.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://la.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ec.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xm.haigaiapp.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rf.521024.cn

Q SQL 专题                              90
来源：http://bm.gzmigu.cn

R Bash 专题                             80
来源：http://qb.nicolike.cn

S C / C++ 专题                          60
来源：http://vc.bookmarksfly.cn

T 其他语言补充                          60
来源：http://be.muxihuayi.cn

U 高频实用片段                         120
来源：http://gr.shxzukj.cn

------------------------------------
来源：http://yq.521024.cn

合计                                  2106 条
来源：http://sm.gzmigu.cn

--------------------------------------------------------------------------------
来源：http://wc.yuexingan06.cn

使用提醒
来源：http://jo.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://pm.nszjky.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://jf.jctech888.com.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kw.shxzskj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qi.chemitech.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://dt.muxihuayi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://th.muxihuayi.cn

—— 文件结束 ——
来源：http://uq.muxihuayi.cn

================================================================================
来源：http://tp.haigaiapp.cn

程序语言常见例子速查手册（2024 版）
来源：http://ks.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://yw.yuexingan06.cn

================================================================================
来源：http://qs.shxzukj.cn

【收录内容】
来源：http://qs.haigaiapp.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://fj.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ke.nszjky.cn

SQL · Bash · C · C++
来源：http://sn.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://vc.hnjuh.cn

【使用说明】
来源：http://hn.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://hk.szsharing.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oq.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wj.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ap.haigaiapp.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://af.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qs.nszjky.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wh.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kt.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sl.yuntaijiaju.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pg.panjiajie.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://zd.hnjuh.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://by.huixinmuqiang.cn

【文件统计】
来源：http://pn.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qi.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://xc.hnjuh.cn

目  录
来源：http://dh.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://kw.nicolike.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://yn.9csxet.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xi.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ns.hnjuh.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qy.shxzukj.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kl.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qi.chemitech.net.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dq.huixiangedu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://qa.bjjhwx.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ay.shxzukj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ra.hnjuh.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://eh.bookmarksfly.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wu.lnxyls.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://vw.shtwfgs.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://rr.shtwfgs.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://rr.wgjwhj.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rf.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dd.huixiangedu.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qb.nicolike.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://my.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rp.colortex.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://rf.shxzskj.cn

================================================================================
来源：http://lt.jctech888.com.cn

A. 基础语法与类型
来源：http://zh.bjjhwx.cn

================================================================================
来源：http://fw.nszjky.cn

[A01] Hello World
来源：http://qk.bookmarksfly.cn

Py:   print("Hello, World!")
来源：http://xt.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://el.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://bm.shxzskj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yx.jianghongdianzi.cn

Java: System.out.println("Hello, World!");
来源：http://hc.szxytkj.cn

Go:   fmt.Println("Hello, World!")
来源：http://mf.asd995.cn

Ruby: puts "Hello, World!"
来源：http://id.newstarts.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xi.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://hq.szxytkj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sm.bjjhwx.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://of.hahajie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ir.lnxyls.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mx.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://ql.jctech888.com.cn

Go:   name := "Alex"; age := 20
来源：http://vj.yuexingan06.cn

Ruby: name = "Alex"; age = 20
来源：http://oc.newstarts.cn

C#:   string name = "Alex"; int age = 20;
来源：http://rr.colortex.cn

[A03] 常量定义
来源：http://ns.lnxyls.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ff.szsharing.cn

PHP:  const PI = 3.14159;
来源：http://cf.haigaiapp.cn

JS:   const PI = 3.14159;
来源：http://mn.muxihuayi.cn

TS:   const PI: number = 3.14159;
来源：http://xd.shxzskj.cn

Java: static final double PI = 3.14159;
来源：http://fz.huixiangedu.cn

Go:   const PI = 3.14159
来源：http://ak.szxytkj.cn

Ruby: PI = 3.14159
来源：http://ob.shxzukj.cn

C#:   const double PI = 3.14159;
来源：http://kj.huanxung.cn

[A04] 判断变量类型
来源：http://ve.hahajie.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://dk.huixinmuqiang.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fa.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://xu.panjiajie.cn

TS:   typeof x; x instanceof Date
来源：http://wh.newstarts.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ml.panjiajie.cn

Go:   reflect.TypeOf(x).Name()
来源：http://im.hnjuh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://av.huixinmuqiang.cn

C#:   x.GetType().Name; x is int
来源：http://to.gzmigu.cn

[A05] 整数除法与取模
来源：http://rf.huanxung.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ul.huixinmuqiang.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://au.jctech888.com.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wp.newstarts.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://lj.chemitech.net.cn

Java: 7 / 2; 7 % 2
来源：http://gv.colortex.cn

Go:   7 / 2; 7 % 2
来源：http://ep.wgjwhj.cn

Ruby: 7 / 2; 7 % 2
来源：http://hr.yuntaijiaju.cn

C#:   7 / 2; 7 % 2
来源：http://aw.newstarts.cn


<!-- 参考信息 -->