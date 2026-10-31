代发 wailian999

[U47] PHP：联合类型
来源：http://qz.yuntaijiaju.cn

int|string $id
来源：http://qz.asd995.cn

[U48] PHP：纯枚举
来源：http://wc.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tl.shxzskj.cn

[U49] PHP：只读属性
来源：http://ux.wgjwhj.cn

public readonly string $name
来源：http://eb.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://cy.bjjhwx.cn

public function __construct(private int $id) {}
来源：http://fq.lnxyls.cn

[U51] PHP：数组解构
来源：http://mq.gzmigu.cn

[$a, $b] = $arr;
来源：http://th.szxytkj.cn

[U52] PHP：箭头函数
来源：http://af.521024.cn

$double = fn($x) => $x * 2;
来源：http://sd.huanxung.cn

[U53] PHP：空合并运算符
来源：http://fo.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://bz.nszjky.cn

[U54] PHP：空安全调用
来源：http://mn.colortex.cn

$obj?->method()
来源：http://uf.huixinmuqiang.cn

[U55] PHP：match 表达式
来源：http://dt.shtwfgs.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fm.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://tp.newstarts.cn

f(a: 1, b: 2)
来源：http://et.bookmarksfly.cn

[U57] PHP：字符串插值
来源：http://jq.521024.cn

"值: {$a}"
来源：http://ql.nszjky.cn

[U58] PHP：数组三件套
来源：http://zw.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dp.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://oq.jctech888.com.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nr.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://ux.newstarts.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tf.9csxet.cn

[U61] PHP：正则
来源：http://lb.asd995.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ng.szsharing.cn

[U62] PHP：日期对象
来源：http://vm.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ks.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://cu.huanxung.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://cv.nszjky.cn

[U64] PHP：目录遍历
来源：http://bo.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://ly.jianghongdianzi.cn

[U65] PHP：会话
来源：http://bi.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rm.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://io.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vr.shxzskj.cn

[U67] PHP：处理文件上传
来源：http://ml.nszjky.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ib.521024.cn

[U68] PHP：PDO 连接
来源：http://wg.shtwfgs.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://oy.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://vn.bookmarksfly.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wy.yuntaijiaju.cn

[U70] PHP：PDO 事务
来源：http://qb.huanxung.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sm.shxzukj.cn

[U71] PHP：抛出异常
来源：http://bo.yuexingan06.cn

throw new RuntimeException("失败", 500);
来源：http://ur.newstarts.cn

[U72] PHP：写错误日志
来源：http://gs.lnxyls.cn

error_log("失败: " . $e->getMessage());
来源：http://ot.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://aj.hahajie.cn

parse_ini_file("config.ini", true)
来源：http://ta.9csxet.cn

[U74] PHP：读取环境变量
来源：http://wx.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://vb.bjjhwx.cn

[U75] PHP：依赖注入
来源：http://ub.panjiajie.cn

composer require psr/container
来源：http://ag.nszjky.cn

[U76] PHP：简单路由
来源：http://cn.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://oi.9csxet.cn

[U77] PHP：模板渲染
来源：http://dt.colortex.cn

composer require twig/twig
来源：http://yd.chemitech.net.cn

[U78] PHP：单元测试
来源：http://xk.nicolike.cn

composer require --dev phpunit/phpunit
来源：http://hw.jctech888.com.cn

[U79] PHP：静态分析
来源：http://ur.yuexingan06.cn

composer require --dev phpstan/phpstan
来源：http://fh.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://ct.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ex.hahajie.cn

[U81] JS：初始化项目
来源：http://tz.shxzukj.cn

npm init -y;  npm i express
来源：http://zl.jianghongdianzi.cn

[U82] JS：package.json 脚本
来源：http://pe.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zu.521024.cn

[U83] JS：ES Module 导入导出
来源：http://dh.nszjky.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ua.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://vg.shxzskj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://qz.jianghongdianzi.cn

[U85] JS：可选链
来源：http://jo.muxihuayi.cn

a?.b?.c
来源：http://te.gzmigu.cn

[U86] JS：空值合并
来源：http://ko.szxytkj.cn

a ?? b
来源：http://wu.nicolike.cn

[U87] JS：解构默认值
来源：http://nv.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://ze.huixinmuqiang.cn

[U88] JS：对象展开合并
来源：http://iq.chemitech.net.cn

{ ...a, ...b }
来源：http://da.szsharing.cn

[U89] JS：数组去重
来源：http://av.jctech888.com.cn

[...new Set(arr)]
来源：http://eh.asd995.cn

[U90] JS：数字数组排序
来源：http://bc.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://qr.haigaiapp.cn

[U91] JS：对象键值遍历
来源：http://zs.shtwfgs.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lr.nszjky.cn

[U92] JS：深拷贝
来源：http://dw.szsharing.cn

structuredClone(obj)
来源：http://zl.gzmigu.cn

[U93] JS：模板字符串
来源：http://fn.hnjuh.cn

`共 ${n} 条`
来源：http://hi.hahajie.cn

[U94] JS：箭头函数
来源：http://nr.huanxung.cn

const double = x => x * 2;
来源：http://dw.asd995.cn

[U95] JS：Promise 包装
来源：http://ss.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://sc.wgjwhj.cn

[U96] JS：async/await 与异常
来源：http://ld.521024.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://no.hahajie.cn

[U97] JS：并发请求
来源：http://hn.bjjhwx.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://dl.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://il.gzmigu.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nh.jctech888.com.cn

[U99] JS：事件监听
来源：http://yz.muxihuayi.cn

el.addEventListener("click", e => {})
来源：http://dk.hnjuh.cn

[U100] JS：DOM 查询
来源：http://gv.gzmigu.cn

document.querySelector(".item")
来源：http://ll.huixiangedu.cn

[U101] JS：classList 操作
来源：http://bw.wgjwhj.cn

el.classList.toggle("active")
来源：http://kp.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://eu.huanxung.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://sr.chemitech.net.cn

[U103] JS：定时器
来源：http://oi.newstarts.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zd.hnjuh.cn

[U104] JS：防抖
来源：http://sq.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ua.huixinmuqiang.cn

[U105] JS：节流
来源：http://yg.lnxyls.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hk.panjiajie.cn

[U106] JS：日期格式化
来源：http://wa.nszjky.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fj.yuexingan06.cn

[U107] JS：数字千分位
来源：http://rl.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gz.huanxung.cn

[U108] JS：随机整数
来源：http://ku.huixinmuqiang.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dy.haigaiapp.cn

[U109] JS：数组分组
来源：http://hc.colortex.cn

Object.groupBy(arr, x => x.type)
来源：http://cb.9csxet.cn

[U110] JS：数组分块
来源：http://de.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ci.521024.cn

[U111] JS：对象转 Map
来源：http://rg.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://cn.asd995.cn

[U112] JS：字符串补位
来源：http://pq.huixinmuqiang.cn

"7".padStart(3, "0")
来源：http://yr.newstarts.cn

[U113] JS：正则替换全部
来源：http://py.hahajie.cn

s.replaceAll("a", "b")
来源：http://nn.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://vf.bjjhwx.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qy.shxzukj.cn

[U115] JS：生成 UUID
来源：http://ki.nszjky.cn

crypto.randomUUID()
来源：http://rv.lnxyls.cn

[U116] JS：类型检查（JSDoc）
来源：http://rh.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://bn.shxzskj.cn

[U117] JS：单元测试
来源：http://si.lnxyls.cn

npm i -D vitest;  npx vitest
来源：http://ce.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://hd.haigaiapp.cn

npm i -D vite;  npx vite
来源：http://mq.shxzukj.cn

[U119] JS：生产构建
来源：http://ap.newstarts.cn

npx vite build
来源：http://cj.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://oo.521024.cn

import.meta.env.VITE_API_URL
来源：http://xo.shxzukj.cn

================================================================================
来源：http://vt.wgjwhj.cn

统计汇总
来源：http://pa.haigaiapp.cn

================================================================================
来源：http://yh.asd995.cn

按语言统计（条）：
来源：http://uw.colortex.cn

Python ......... 252
来源：http://eo.nicolike.cn

PHP ............ 252
来源：http://kl.huixiangedu.cn

JavaScript ..... 252
来源：http://uh.9csxet.cn

TypeScript ..... 212
来源：http://oo.jianghongdianzi.cn

Java ........... 212
来源：http://jn.szsharing.cn

Go ............. 212
来源：http://em.yuntaijiaju.cn

Ruby ........... 212
来源：http://bs.nszjky.cn

C# ............. 212
来源：http://jy.huanxung.cn

C .............. 30
来源：http://fh.szxytkj.cn

C++ ............ 30
来源：http://gj.huixiangedu.cn

SQL ............ 90
来源：http://ub.bjjhwx.cn

Bash ........... 80
来源：http://ri.muxihuayi.cn

Kotlin ......... 15
来源：http://pc.chemitech.net.cn

Swift .......... 15
来源：http://fb.jctech888.com.cn

Lua ............ 10
来源：http://oa.colortex.cn

Perl ........... 10
来源：http://rk.jctech888.com.cn

Scala .......... 10
来源：http://pj.nicolike.cn

------------------------------------
来源：http://kw.jianghongdianzi.cn

合计 ........... 2106 条
来源：http://ya.huixiangedu.cn

按章节统计：
来源：http://ob.521024.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://pl.bookmarksfly.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ub.colortex.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://za.hahajie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rw.szsharing.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://yw.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://id.newstarts.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://na.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wf.muxihuayi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sg.asd995.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wy.bjjhwx.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xd.jctech888.com.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://tv.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rc.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ot.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://yi.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://au.asd995.cn

Q SQL 专题                              90
来源：http://wh.yuntaijiaju.cn

R Bash 专题                             80
来源：http://ls.521024.cn

S C / C++ 专题                          60
来源：http://ki.shxzukj.cn

T 其他语言补充                          60
来源：http://zx.nszjky.cn

U 高频实用片段                         120
来源：http://zk.huixiangedu.cn

------------------------------------
来源：http://mt.yuntaijiaju.cn

合计                                  2106 条
来源：http://sv.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://hn.shxzukj.cn

使用提醒
来源：http://sd.asd995.cn

--------------------------------------------------------------------------------
来源：http://zz.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://sc.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ll.nicolike.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xn.shxzukj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://mj.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qm.jianghongdianzi.cn

—— 文件结束 ——
来源：http://kj.haigaiapp.cn

================================================================================
来源：http://zs.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://te.shxzskj.cn

Common Programming Examples Cheat Book
来源：http://ch.chemitech.net.cn

================================================================================
来源：http://hi.wgjwhj.cn

【收录内容】
来源：http://ia.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://rc.yuexingan06.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://jh.521024.cn

SQL · Bash · C · C++
来源：http://fa.bjjhwx.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ru.huixiangedu.cn

【使用说明】
来源：http://ap.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://un.9csxet.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qa.yuexingan06.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://be.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ut.521024.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://pi.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://na.haigaiapp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nq.hnjuh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://un.huixinmuqiang.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://rd.jianghongdianzi.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hv.9csxet.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gu.wgjwhj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://hr.shxzskj.cn

【文件统计】
来源：http://mi.huixiangedu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wu.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ev.hnjuh.cn

目  录
来源：http://pv.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://ju.huanxung.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ai.haigaiapp.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://cj.szsharing.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nc.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ox.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ks.panjiajie.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ph.huanxung.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gu.muxihuayi.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cb.jctech888.com.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sn.muxihuayi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jm.newstarts.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ji.szsharing.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://io.chemitech.net.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://fw.asd995.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zy.nszjky.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vk.huanxung.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ib.shxzukj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wa.lnxyls.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xg.nszjky.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rn.nszjky.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zh.bjjhwx.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://yc.bjjhwx.cn

================================================================================
来源：http://bw.521024.cn

A. 基础语法与类型
来源：http://pe.asd995.cn

================================================================================
来源：http://kv.nicolike.cn

[A01] Hello World
来源：http://mr.lnxyls.cn

Py:   print("Hello, World!")
来源：http://ul.colortex.cn

PHP:  echo "Hello, World!";
来源：http://kd.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://aa.hnjuh.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vj.huixiangedu.cn

Java: System.out.println("Hello, World!");
来源：http://lb.jianghongdianzi.cn

Go:   fmt.Println("Hello, World!")
来源：http://at.huixiangedu.cn

Ruby: puts "Hello, World!"
来源：http://eh.yuexingan06.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://xk.haigaiapp.cn

[A02] 变量声明与赋值
来源：http://yl.shxzukj.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://cz.jianghongdianzi.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://qx.shxzukj.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jr.jctech888.com.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rp.muxihuayi.cn

Java: String name = "Alex"; int age = 20;
来源：http://vq.yuexingan06.cn

Go:   name := "Alex"; age := 20
来源：http://is.panjiajie.cn

Ruby: name = "Alex"; age = 20
来源：http://pu.gzmigu.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jw.szsharing.cn

[A03] 常量定义
来源：http://kn.panjiajie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wu.9csxet.cn

PHP:  const PI = 3.14159;
来源：http://df.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://wl.gzmigu.cn

TS:   const PI: number = 3.14159;
来源：http://lo.nicolike.cn

Java: static final double PI = 3.14159;
来源：http://bu.asd995.cn

Go:   const PI = 3.14159
来源：http://iz.jianghongdianzi.cn

Ruby: PI = 3.14159
来源：http://up.asd995.cn

C#:   const double PI = 3.14159;
来源：http://vp.jctech888.com.cn

[A04] 判断变量类型
来源：http://uw.shxzskj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://wp.huixiangedu.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://uh.hnjuh.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bg.szxytkj.cn

TS:   typeof x; x instanceof Date
来源：http://oo.521024.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://di.huixiangedu.cn

Go:   reflect.TypeOf(x).Name()
来源：http://gy.szsharing.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://nt.nszjky.cn

C#:   x.GetType().Name; x is int
来源：http://np.nszjky.cn

[A05] 整数除法与取模
来源：http://im.nicolike.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://rf.huixiangedu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://cq.asd995.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://bu.huixiangedu.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://eg.9csxet.cn

Java: 7 / 2; 7 % 2
来源：http://sz.chemitech.net.cn

Go:   7 / 2; 7 % 2
来源：http://sb.muxihuayi.cn

Ruby: 7 / 2; 7 % 2
来源：http://sb.shxzukj.cn

C#:   7 / 2; 7 % 2
来源：http://et.huixinmuqiang.cn


<!-- 参考信息 -->