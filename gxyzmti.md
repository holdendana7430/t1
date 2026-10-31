代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://ef.chemitech.net.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nb.hahajie.cn

[U46] PHP：可空类型
来源：http://of.chemitech.net.cn

?string $name = null
来源：http://rh.szxytkj.cn

[U47] PHP：联合类型
来源：http://vf.lnxyls.cn

int|string $id
来源：http://ix.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://xg.jianghongdianzi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://us.521024.cn

[U49] PHP：只读属性
来源：http://cm.szxytkj.cn

public readonly string $name
来源：http://lw.nszjky.cn

[U50] PHP：构造器属性提升
来源：http://cs.muxihuayi.cn

public function __construct(private int $id) {}
来源：http://vg.chemitech.net.cn

[U51] PHP：数组解构
来源：http://el.yuexingan06.cn

[$a, $b] = $arr;
来源：http://ik.hahajie.cn

[U52] PHP：箭头函数
来源：http://vq.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://hf.huixiangedu.cn

[U53] PHP：空合并运算符
来源：http://ng.hahajie.cn

$v = $a ?? $b ?? "default";
来源：http://ay.wgjwhj.cn

[U54] PHP：空安全调用
来源：http://jm.shxzukj.cn

$obj?->method()
来源：http://dd.wgjwhj.cn

[U55] PHP：match 表达式
来源：http://tk.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jv.jctech888.com.cn

[U56] PHP：命名参数
来源：http://sn.521024.cn

f(a: 1, b: 2)
来源：http://gv.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://vi.shxzukj.cn

"值: {$a}"
来源：http://ih.9csxet.cn

[U58] PHP：数组三件套
来源：http://md.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ce.szsharing.cn

[U59] PHP：自定义排序
来源：http://kk.szxytkj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vb.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://nc.yuexingan06.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mz.hahajie.cn

[U61] PHP：正则
来源：http://rt.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ca.muxihuayi.cn

[U62] PHP：日期对象
来源：http://gc.nicolike.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cr.9csxet.cn

[U63] PHP：文件读写
来源：http://wc.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lk.bookmarksfly.cn

[U64] PHP：目录遍历
来源：http://es.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://ns.huanxung.cn

[U65] PHP：会话
来源：http://jy.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://od.9csxet.cn

[U66] PHP：设置 Cookie
来源：http://zq.panjiajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zu.chemitech.net.cn

[U67] PHP：处理文件上传
来源：http://xa.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zz.shtwfgs.cn

[U68] PHP：PDO 连接
来源：http://aq.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dz.szxytkj.cn

[U69] PHP：PDO 预处理
来源：http://um.shxzskj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oh.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://gf.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wx.shtwfgs.cn

[U71] PHP：抛出异常
来源：http://sk.wgjwhj.cn

throw new RuntimeException("失败", 500);
来源：http://jz.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://fe.chemitech.net.cn

error_log("失败: " . $e->getMessage());
来源：http://in.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://hp.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://xk.wgjwhj.cn

[U74] PHP：读取环境变量
来源：http://hb.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://xj.huixiangedu.cn

[U75] PHP：依赖注入
来源：http://gy.jianghongdianzi.cn

composer require psr/container
来源：http://vg.gzmigu.cn

[U76] PHP：简单路由
来源：http://uy.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cg.bookmarksfly.cn

[U77] PHP：模板渲染
来源：http://an.nszjky.cn

composer require twig/twig
来源：http://ht.shxzukj.cn

[U78] PHP：单元测试
来源：http://gk.jctech888.com.cn

composer require --dev phpunit/phpunit
来源：http://zg.nicolike.cn

[U79] PHP：静态分析
来源：http://lu.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://ef.521024.cn

[U80] PHP：代码规范修复
来源：http://rb.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gz.bookmarksfly.cn

[U81] JS：初始化项目
来源：http://qr.muxihuayi.cn

npm init -y;  npm i express
来源：http://lv.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://il.nszjky.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sa.hnjuh.cn

[U83] JS：ES Module 导入导出
来源：http://pn.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://wa.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://uy.bookmarksfly.cn

module.exports = { a };  const { a } = require("./m");
来源：http://dk.521024.cn

[U85] JS：可选链
来源：http://nb.nszjky.cn

a?.b?.c
来源：http://sf.huanxung.cn

[U86] JS：空值合并
来源：http://ud.nicolike.cn

a ?? b
来源：http://gz.hahajie.cn

[U87] JS：解构默认值
来源：http://yn.nicolike.cn

const { a = 1, b = 2 } = obj;
来源：http://zo.jctech888.com.cn

[U88] JS：对象展开合并
来源：http://wu.521024.cn

{ ...a, ...b }
来源：http://qv.huixinmuqiang.cn

[U89] JS：数组去重
来源：http://ik.haigaiapp.cn

[...new Set(arr)]
来源：http://xk.asd995.cn

[U90] JS：数字数组排序
来源：http://le.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://av.gzmigu.cn

[U91] JS：对象键值遍历
来源：http://nt.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hu.haigaiapp.cn

[U92] JS：深拷贝
来源：http://rt.521024.cn

structuredClone(obj)
来源：http://bf.szsharing.cn

[U93] JS：模板字符串
来源：http://aa.szxytkj.cn

`共 ${n} 条`
来源：http://bu.asd995.cn

[U94] JS：箭头函数
来源：http://ay.panjiajie.cn

const double = x => x * 2;
来源：http://pt.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://vg.newstarts.cn

new Promise((resolve, reject) => {})
来源：http://rw.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://nl.shxzukj.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ja.jianghongdianzi.cn

[U97] JS：并发请求
来源：http://cv.shtwfgs.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://os.jctech888.com.cn

[U98] JS：fetch 带 JSON
来源：http://fq.hahajie.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ow.gzmigu.cn

[U99] JS：事件监听
来源：http://zt.hnjuh.cn

el.addEventListener("click", e => {})
来源：http://mz.521024.cn

[U100] JS：DOM 查询
来源：http://ho.jianghongdianzi.cn

document.querySelector(".item")
来源：http://oj.nicolike.cn

[U101] JS：classList 操作
来源：http://pe.chemitech.net.cn

el.classList.toggle("active")
来源：http://jx.hnjuh.cn

[U102] JS：本地存储
来源：http://xs.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://jq.asd995.cn

[U103] JS：定时器
来源：http://vq.yuntaijiaju.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ab.szsharing.cn

[U104] JS：防抖
来源：http://fq.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ke.asd995.cn

[U105] JS：节流
来源：http://gp.asd995.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://dw.chemitech.net.cn

[U106] JS：日期格式化
来源：http://pv.muxihuayi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ud.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://ed.lnxyls.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vl.asd995.cn

[U108] JS：随机整数
来源：http://vl.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gb.haigaiapp.cn

[U109] JS：数组分组
来源：http://vv.9csxet.cn

Object.groupBy(arr, x => x.type)
来源：http://ie.panjiajie.cn

[U110] JS：数组分块
来源：http://dz.nicolike.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ik.huixinmuqiang.cn

[U111] JS：对象转 Map
来源：http://dh.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://gk.bjjhwx.cn

[U112] JS：字符串补位
来源：http://de.chemitech.net.cn

"7".padStart(3, "0")
来源：http://zg.521024.cn

[U113] JS：正则替换全部
来源：http://gt.newstarts.cn

s.replaceAll("a", "b")
来源：http://oj.wgjwhj.cn

[U114] JS：JSON 深比较
来源：http://mz.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wa.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://wo.asd995.cn

crypto.randomUUID()
来源：http://ko.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://gr.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://fs.chemitech.net.cn

[U117] JS：单元测试
来源：http://vo.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://hw.9csxet.cn

[U118] JS：开发服务器
来源：http://be.shxzukj.cn

npm i -D vite;  npx vite
来源：http://in.muxihuayi.cn

[U119] JS：生产构建
来源：http://ic.gzmigu.cn

npx vite build
来源：http://lg.yuntaijiaju.cn

[U120] JS：读取环境变量（Vite）
来源：http://lw.huanxung.cn

import.meta.env.VITE_API_URL
来源：http://rq.haigaiapp.cn

================================================================================
来源：http://aw.yuntaijiaju.cn

统计汇总
来源：http://wp.muxihuayi.cn

================================================================================
来源：http://gt.szxytkj.cn

按语言统计（条）：
来源：http://yg.nszjky.cn

Python ......... 252
来源：http://zq.bjjhwx.cn

PHP ............ 252
来源：http://ah.shtwfgs.cn

JavaScript ..... 252
来源：http://yl.huanxung.cn

TypeScript ..... 212
来源：http://fi.shxzskj.cn

Java ........... 212
来源：http://ts.jctech888.com.cn

Go ............. 212
来源：http://xr.9csxet.cn

Ruby ........... 212
来源：http://wk.hnjuh.cn

C# ............. 212
来源：http://bz.gzmigu.cn

C .............. 30
来源：http://my.nicolike.cn

C++ ............ 30
来源：http://fs.panjiajie.cn

SQL ............ 90
来源：http://cb.panjiajie.cn

Bash ........... 80
来源：http://ak.szsharing.cn

Kotlin ......... 15
来源：http://il.shxzskj.cn

Swift .......... 15
来源：http://sg.gzmigu.cn

Lua ............ 10
来源：http://az.huixinmuqiang.cn

Perl ........... 10
来源：http://zw.jctech888.com.cn

Scala .......... 10
来源：http://sq.chemitech.net.cn

------------------------------------
来源：http://hx.colortex.cn

合计 ........... 2106 条
来源：http://ty.shtwfgs.cn

按章节统计：
来源：http://mi.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://hu.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nd.lnxyls.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mu.muxihuayi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://hk.haigaiapp.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sp.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bg.yuexingan06.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ue.colortex.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gl.huixinmuqiang.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ks.jctech888.com.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xr.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://el.bookmarksfly.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://vi.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mb.hnjuh.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://sk.asd995.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ih.hahajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yq.jctech888.com.cn

Q SQL 专题                              90
来源：http://ia.huixiangedu.cn

R Bash 专题                             80
来源：http://zi.wgjwhj.cn

S C / C++ 专题                          60
来源：http://rn.bjjhwx.cn

T 其他语言补充                          60
来源：http://ye.lnxyls.cn

U 高频实用片段                         120
来源：http://jc.muxihuayi.cn

------------------------------------
来源：http://ue.yuexingan06.cn

合计                                  2106 条
来源：http://tx.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://uz.yuexingan06.cn

使用提醒
来源：http://vp.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://pi.shtwfgs.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nr.shxzukj.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ik.szsharing.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://pq.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gn.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ou.panjiajie.cn

—— 文件结束 ——
来源：http://vj.muxihuayi.cn

================================================================================
来源：http://eu.shxzukj.cn

程序语言常见例子速查手册（2024 版）
来源：http://od.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://kt.yuntaijiaju.cn

================================================================================
来源：http://zg.muxihuayi.cn

【收录内容】
来源：http://sx.521024.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rd.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://be.newstarts.cn

SQL · Bash · C · C++
来源：http://bw.haigaiapp.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xv.nicolike.cn

【使用说明】
来源：http://ek.muxihuayi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://st.szxytkj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qe.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://xf.asd995.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vi.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ri.jctech888.com.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pz.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bv.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zi.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yx.9csxet.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dt.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dn.lnxyls.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dz.gzmigu.cn

【文件统计】
来源：http://lo.panjiajie.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mm.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://it.hnjuh.cn

目  录
来源：http://wx.bjjhwx.cn

--------------------------------------------------------------------------------
来源：http://hy.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://og.shtwfgs.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kk.asd995.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ya.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ey.yuexingan06.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yu.hnjuh.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ss.szsharing.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ql.gzmigu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rv.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cs.huixinmuqiang.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://zd.huixinmuqiang.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ub.wgjwhj.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://sn.bjjhwx.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://pk.huixinmuqiang.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mc.shxzskj.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ch.shtwfgs.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sq.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zb.9csxet.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://an.haigaiapp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lm.szxytkj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gd.huanxung.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lw.haigaiapp.cn

================================================================================
来源：http://uy.asd995.cn

A. 基础语法与类型
来源：http://go.nicolike.cn

================================================================================
来源：http://fr.9csxet.cn

[A01] Hello World
来源：http://zf.lnxyls.cn

Py:   print("Hello, World!")
来源：http://lu.hnjuh.cn

PHP:  echo "Hello, World!";
来源：http://hn.nicolike.cn

JS:   console.log("Hello, World!");
来源：http://qx.bjjhwx.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yz.chemitech.net.cn

Java: System.out.println("Hello, World!");
来源：http://lf.panjiajie.cn

Go:   fmt.Println("Hello, World!")
来源：http://iu.hnjuh.cn

Ruby: puts "Hello, World!"
来源：http://or.shxzukj.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://sc.huixiangedu.cn

[A02] 变量声明与赋值
来源：http://hj.yuexingan06.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rj.asd995.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://zl.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hg.chemitech.net.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dx.gzmigu.cn

Java: String name = "Alex"; int age = 20;
来源：http://zy.szsharing.cn

Go:   name := "Alex"; age := 20
来源：http://pm.szsharing.cn

Ruby: name = "Alex"; age = 20
来源：http://cc.hahajie.cn

C#:   string name = "Alex"; int age = 20;
来源：http://nu.shtwfgs.cn

[A03] 常量定义
来源：http://ja.colortex.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mn.bjjhwx.cn

PHP:  const PI = 3.14159;
来源：http://vr.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://xt.9csxet.cn

TS:   const PI: number = 3.14159;
来源：http://zp.yuexingan06.cn

Java: static final double PI = 3.14159;
来源：http://nv.muxihuayi.cn

Go:   const PI = 3.14159
来源：http://hx.newstarts.cn

Ruby: PI = 3.14159
来源：http://tx.jctech888.com.cn

C#:   const double PI = 3.14159;
来源：http://rg.yuexingan06.cn

[A04] 判断变量类型
来源：http://dg.newstarts.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ol.huanxung.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://cc.shtwfgs.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ts.gzmigu.cn

TS:   typeof x; x instanceof Date
来源：http://ra.jianghongdianzi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://so.jianghongdianzi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://bl.bjjhwx.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://lc.yuntaijiaju.cn

C#:   x.GetType().Name; x is int
来源：http://yd.muxihuayi.cn

[A05] 整数除法与取模
来源：http://nc.bjjhwx.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pe.shxzskj.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://zd.jianghongdianzi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pp.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://js.jianghongdianzi.cn


<!-- 参考信息 -->