代发 wailian999

[U43] PHP：声明命名空间
来源：http://io.shxzukj.cn

namespace App\Http;
来源：http://ke.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://iq.shxzukj.cn

declare(strict_types=1);
来源：http://ft.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://pz.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gc.jianghongdianzi.cn

[U46] PHP：可空类型
来源：http://ix.nicolike.cn

?string $name = null
来源：http://es.newstarts.cn

[U47] PHP：联合类型
来源：http://db.szxytkj.cn

int|string $id
来源：http://ef.nszjky.cn

[U48] PHP：纯枚举
来源：http://wn.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fy.9csxet.cn

[U49] PHP：只读属性
来源：http://qq.9csxet.cn

public readonly string $name
来源：http://ka.asd995.cn

[U50] PHP：构造器属性提升
来源：http://fp.bookmarksfly.cn

public function __construct(private int $id) {}
来源：http://kj.szsharing.cn

[U51] PHP：数组解构
来源：http://gu.521024.cn

[$a, $b] = $arr;
来源：http://qr.9csxet.cn

[U52] PHP：箭头函数
来源：http://fg.gzmigu.cn

$double = fn($x) => $x * 2;
来源：http://fm.shtwfgs.cn

[U53] PHP：空合并运算符
来源：http://op.szxytkj.cn

$v = $a ?? $b ?? "default";
来源：http://wl.newstarts.cn

[U54] PHP：空安全调用
来源：http://jf.shxzukj.cn

$obj?->method()
来源：http://mo.shxzukj.cn

[U55] PHP：match 表达式
来源：http://vy.szsharing.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hy.nicolike.cn

[U56] PHP：命名参数
来源：http://yf.szxytkj.cn

f(a: 1, b: 2)
来源：http://al.huixinmuqiang.cn

[U57] PHP：字符串插值
来源：http://lm.nszjky.cn

"值: {$a}"
来源：http://fh.szsharing.cn

[U58] PHP：数组三件套
来源：http://cc.hahajie.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://na.9csxet.cn

[U59] PHP：自定义排序
来源：http://ah.szsharing.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uu.bjjhwx.cn

[U60] PHP：JSON 编解码
来源：http://pr.521024.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://po.huixinmuqiang.cn

[U61] PHP：正则
来源：http://jh.jctech888.com.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nv.9csxet.cn

[U62] PHP：日期对象
来源：http://nl.gzmigu.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vu.lnxyls.cn

[U63] PHP：文件读写
来源：http://im.lnxyls.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yx.nszjky.cn

[U64] PHP：目录遍历
来源：http://ns.huixinmuqiang.cn

glob("dir/*.php");  scandir("dir");
来源：http://nx.gzmigu.cn

[U65] PHP：会话
来源：http://ve.panjiajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://pi.521024.cn

[U66] PHP：设置 Cookie
来源：http://ai.bookmarksfly.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jf.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://kg.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dd.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://eq.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zk.muxihuayi.cn

[U69] PHP：PDO 预处理
来源：http://an.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://at.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://qq.chemitech.net.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://sf.yuexingan06.cn

[U71] PHP：抛出异常
来源：http://iy.szxytkj.cn

throw new RuntimeException("失败", 500);
来源：http://pe.newstarts.cn

[U72] PHP：写错误日志
来源：http://rn.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://li.521024.cn

[U73] PHP：读取 ini 配置
来源：http://ip.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://tr.colortex.cn

[U74] PHP：读取环境变量
来源：http://hf.jctech888.com.cn

getenv("APP_ENV") ?: "production"
来源：http://nw.huanxung.cn

[U75] PHP：依赖注入
来源：http://nt.wgjwhj.cn

composer require psr/container
来源：http://nm.muxihuayi.cn

[U76] PHP：简单路由
来源：http://ln.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ep.colortex.cn

[U77] PHP：模板渲染
来源：http://fl.asd995.cn

composer require twig/twig
来源：http://xq.jctech888.com.cn

[U78] PHP：单元测试
来源：http://zp.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://ls.muxihuayi.cn

[U79] PHP：静态分析
来源：http://lu.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://yf.asd995.cn

[U80] PHP：代码规范修复
来源：http://xx.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sl.jctech888.com.cn

[U81] JS：初始化项目
来源：http://rg.huixiangedu.cn

npm init -y;  npm i express
来源：http://rx.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://dw.shtwfgs.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://cb.newstarts.cn

[U83] JS：ES Module 导入导出
来源：http://yt.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://tu.521024.cn

[U84] JS：CommonJS 写法
来源：http://ew.haigaiapp.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ve.shxzukj.cn

[U85] JS：可选链
来源：http://an.521024.cn

a?.b?.c
来源：http://sx.muxihuayi.cn

[U86] JS：空值合并
来源：http://oq.chemitech.net.cn

a ?? b
来源：http://zs.szsharing.cn

[U87] JS：解构默认值
来源：http://cz.bjjhwx.cn

const { a = 1, b = 2 } = obj;
来源：http://jh.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://up.nicolike.cn

{ ...a, ...b }
来源：http://zi.muxihuayi.cn

[U89] JS：数组去重
来源：http://tl.newstarts.cn

[...new Set(arr)]
来源：http://rm.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://tf.9csxet.cn

[...arr].sort((a, b) => a - b)
来源：http://pv.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://yh.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pu.haigaiapp.cn

[U92] JS：深拷贝
来源：http://ug.huanxung.cn

structuredClone(obj)
来源：http://pa.colortex.cn

[U93] JS：模板字符串
来源：http://og.nszjky.cn

`共 ${n} 条`
来源：http://vf.hnjuh.cn

[U94] JS：箭头函数
来源：http://ao.haigaiapp.cn

const double = x => x * 2;
来源：http://wj.huixinmuqiang.cn

[U95] JS：Promise 包装
来源：http://rl.huixinmuqiang.cn

new Promise((resolve, reject) => {})
来源：http://vl.lnxyls.cn

[U96] JS：async/await 与异常
来源：http://gp.yuntaijiaju.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://fs.huixiangedu.cn

[U97] JS：并发请求
来源：http://rp.bookmarksfly.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ay.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://qy.shxzukj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://tm.521024.cn

[U99] JS：事件监听
来源：http://ly.shxzskj.cn

el.addEventListener("click", e => {})
来源：http://ru.szsharing.cn

[U100] JS：DOM 查询
来源：http://ay.huixiangedu.cn

document.querySelector(".item")
来源：http://cb.shxzskj.cn

[U101] JS：classList 操作
来源：http://gn.bookmarksfly.cn

el.classList.toggle("active")
来源：http://na.yuexingan06.cn

[U102] JS：本地存储
来源：http://wk.yuntaijiaju.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zm.nszjky.cn

[U103] JS：定时器
来源：http://gf.colortex.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eo.haigaiapp.cn

[U104] JS：防抖
来源：http://bn.lnxyls.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://au.szxytkj.cn

[U105] JS：节流
来源：http://oq.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://kw.521024.cn

[U106] JS：日期格式化
来源：http://za.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nw.colortex.cn

[U107] JS：数字千分位
来源：http://nh.hahajie.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ro.huanxung.cn

[U108] JS：随机整数
来源：http://ir.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://hn.muxihuayi.cn

[U109] JS：数组分组
来源：http://sm.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://bq.chemitech.net.cn

[U110] JS：数组分块
来源：http://qu.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vz.hahajie.cn

[U111] JS：对象转 Map
来源：http://vz.hahajie.cn

new Map(Object.entries(obj))
来源：http://ad.yuntaijiaju.cn

[U112] JS：字符串补位
来源：http://dn.jctech888.com.cn

"7".padStart(3, "0")
来源：http://zz.nicolike.cn

[U113] JS：正则替换全部
来源：http://ac.panjiajie.cn

s.replaceAll("a", "b")
来源：http://ws.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://zx.haigaiapp.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://hz.hahajie.cn

[U115] JS：生成 UUID
来源：http://vb.szsharing.cn

crypto.randomUUID()
来源：http://fh.hahajie.cn

[U116] JS：类型检查（JSDoc）
来源：http://qf.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://rh.hahajie.cn

[U117] JS：单元测试
来源：http://wo.szxytkj.cn

npm i -D vitest;  npx vitest
来源：http://lv.huanxung.cn

[U118] JS：开发服务器
来源：http://dj.muxihuayi.cn

npm i -D vite;  npx vite
来源：http://st.shxzskj.cn

[U119] JS：生产构建
来源：http://nv.huixinmuqiang.cn

npx vite build
来源：http://yh.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://sm.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://ql.huanxung.cn

================================================================================
来源：http://dz.newstarts.cn

统计汇总
来源：http://te.szsharing.cn

================================================================================
来源：http://iu.nicolike.cn

按语言统计（条）：
来源：http://vy.gzmigu.cn

Python ......... 252
来源：http://ut.jctech888.com.cn

PHP ............ 252
来源：http://ic.521024.cn

JavaScript ..... 252
来源：http://uu.chemitech.net.cn

TypeScript ..... 212
来源：http://tn.shxzukj.cn

Java ........... 212
来源：http://nc.hahajie.cn

Go ............. 212
来源：http://gv.hnjuh.cn

Ruby ........... 212
来源：http://hd.asd995.cn

C# ............. 212
来源：http://kj.huixinmuqiang.cn

C .............. 30
来源：http://wo.newstarts.cn

C++ ............ 30
来源：http://br.gzmigu.cn

SQL ............ 90
来源：http://iu.shxzukj.cn

Bash ........... 80
来源：http://dz.jianghongdianzi.cn

Kotlin ......... 15
来源：http://sx.shtwfgs.cn

Swift .......... 15
来源：http://jv.lnxyls.cn

Lua ............ 10
来源：http://bw.yuexingan06.cn

Perl ........... 10
来源：http://mn.haigaiapp.cn

Scala .......... 10
来源：http://qn.asd995.cn

------------------------------------
来源：http://at.szxytkj.cn

合计 ........... 2106 条
来源：http://xk.jianghongdianzi.cn

按章节统计：
来源：http://wm.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ho.521024.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tf.shxzskj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sd.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mo.asd995.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fw.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://fc.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yi.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://nt.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://dk.szsharing.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://my.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://st.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zi.szxytkj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://gi.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ug.shxzskj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://vs.521024.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pv.yuexingan06.cn

Q SQL 专题                              90
来源：http://fp.bookmarksfly.cn

R Bash 专题                             80
来源：http://yn.lnxyls.cn

S C / C++ 专题                          60
来源：http://dw.yuntaijiaju.cn

T 其他语言补充                          60
来源：http://dt.shxzskj.cn

U 高频实用片段                         120
来源：http://gf.hahajie.cn

------------------------------------
来源：http://oy.panjiajie.cn

合计                                  2106 条
来源：http://wd.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://dm.bookmarksfly.cn

使用提醒
来源：http://pj.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://oq.haigaiapp.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yh.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rc.9csxet.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wm.shxzskj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://sl.szxytkj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cu.9csxet.cn

—— 文件结束 ——
来源：http://yw.muxihuayi.cn

================================================================================
来源：http://hq.panjiajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://ch.shtwfgs.cn

Common Programming Examples Cheat Book
来源：http://og.colortex.cn

================================================================================
来源：http://nm.gzmigu.cn

【收录内容】
来源：http://mb.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kx.jianghongdianzi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://lz.521024.cn

SQL · Bash · C · C++
来源：http://ml.szsharing.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://yj.bjjhwx.cn

【使用说明】
来源：http://ii.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://vm.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rc.gzmigu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dc.chemitech.net.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://an.jctech888.com.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://to.muxihuayi.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qw.bookmarksfly.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fl.wgjwhj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://es.shtwfgs.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://eq.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://fd.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wf.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://bv.muxihuayi.cn

【文件统计】
来源：http://dv.asd995.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://je.newstarts.cn

--------------------------------------------------------------------------------
来源：http://zz.yuntaijiaju.cn

目  录
来源：http://uy.hahajie.cn

--------------------------------------------------------------------------------
来源：http://mp.nszjky.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gu.jctech888.com.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qg.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wc.panjiajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://sb.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://li.huixiangedu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hz.panjiajie.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ui.yuntaijiaju.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://iv.muxihuayi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vp.shxzskj.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hk.jianghongdianzi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ko.521024.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tj.gzmigu.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wo.shxzskj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oz.haigaiapp.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://th.nicolike.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://dw.hnjuh.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wi.huixinmuqiang.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tk.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://zi.shxzskj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://uq.hahajie.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://go.hahajie.cn

================================================================================
来源：http://bu.shxzskj.cn

A. 基础语法与类型
来源：http://yi.nicolike.cn

================================================================================
来源：http://kc.panjiajie.cn

[A01] Hello World
来源：http://vf.panjiajie.cn

Py:   print("Hello, World!")
来源：http://qq.asd995.cn

PHP:  echo "Hello, World!";
来源：http://du.newstarts.cn

JS:   console.log("Hello, World!");
来源：http://fb.muxihuayi.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bs.shtwfgs.cn

Java: System.out.println("Hello, World!");
来源：http://qr.lnxyls.cn

Go:   fmt.Println("Hello, World!")
来源：http://ec.nicolike.cn

Ruby: puts "Hello, World!"
来源：http://qz.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://ij.shxzukj.cn

[A02] 变量声明与赋值
来源：http://rm.lnxyls.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://tv.szsharing.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://rb.huixinmuqiang.cn

JS:   let name = "Alex"; const age = 20;
来源：http://or.hahajie.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://yq.huixinmuqiang.cn

Java: String name = "Alex"; int age = 20;
来源：http://aj.shxzskj.cn

Go:   name := "Alex"; age := 20
来源：http://ib.521024.cn

Ruby: name = "Alex"; age = 20
来源：http://rf.hnjuh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://xw.muxihuayi.cn

[A03] 常量定义
来源：http://be.9csxet.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://el.gzmigu.cn

PHP:  const PI = 3.14159;
来源：http://kn.shxzskj.cn

JS:   const PI = 3.14159;
来源：http://va.colortex.cn

TS:   const PI: number = 3.14159;
来源：http://im.panjiajie.cn

Java: static final double PI = 3.14159;
来源：http://sa.chemitech.net.cn

Go:   const PI = 3.14159
来源：http://fc.szsharing.cn

Ruby: PI = 3.14159
来源：http://wq.9csxet.cn

C#:   const double PI = 3.14159;
来源：http://hh.bjjhwx.cn

[A04] 判断变量类型
来源：http://ki.huixinmuqiang.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://fm.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yj.9csxet.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://os.shtwfgs.cn

TS:   typeof x; x instanceof Date
来源：http://ei.shxzskj.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ts.521024.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ui.huanxung.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ex.nicolike.cn

C#:   x.GetType().Name; x is int
来源：http://un.shtwfgs.cn

[A05] 整数除法与取模
来源：http://ky.shxzukj.cn


<!-- 参考信息 -->