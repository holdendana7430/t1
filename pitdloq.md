代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://ut.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jp.szsharing.cn

[U46] PHP：可空类型
来源：http://ls.huanxung.cn

?string $name = null
来源：http://iv.haigaiapp.cn

[U47] PHP：联合类型
来源：http://yc.yuntaijiaju.cn

int|string $id
来源：http://cr.jctech888.com.cn

[U48] PHP：纯枚举
来源：http://xy.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zp.nszjky.cn

[U49] PHP：只读属性
来源：http://sl.huixinmuqiang.cn

public readonly string $name
来源：http://iq.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://tj.chemitech.net.cn

public function __construct(private int $id) {}
来源：http://ie.chemitech.net.cn

[U51] PHP：数组解构
来源：http://jg.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://ex.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://sm.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ek.asd995.cn

[U53] PHP：空合并运算符
来源：http://vd.shtwfgs.cn

$v = $a ?? $b ?? "default";
来源：http://br.nicolike.cn

[U54] PHP：空安全调用
来源：http://wi.jianghongdianzi.cn

$obj?->method()
来源：http://cr.shtwfgs.cn

[U55] PHP：match 表达式
来源：http://ej.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wl.szsharing.cn

[U56] PHP：命名参数
来源：http://av.huixiangedu.cn

f(a: 1, b: 2)
来源：http://ba.szxytkj.cn

[U57] PHP：字符串插值
来源：http://oa.haigaiapp.cn

"值: {$a}"
来源：http://cc.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://ff.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yf.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://sp.bjjhwx.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xd.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://hp.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bq.newstarts.cn

[U61] PHP：正则
来源：http://wl.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qg.jctech888.com.cn

[U62] PHP：日期对象
来源：http://pv.colortex.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ha.panjiajie.cn

[U63] PHP：文件读写
来源：http://bb.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pa.9csxet.cn

[U64] PHP：目录遍历
来源：http://iv.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://jb.szsharing.cn

[U65] PHP：会话
来源：http://id.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ei.bjjhwx.cn

[U66] PHP：设置 Cookie
来源：http://nl.colortex.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zm.hnjuh.cn

[U67] PHP：处理文件上传
来源：http://gl.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tv.shxzskj.cn

[U68] PHP：PDO 连接
来源：http://ti.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://zt.bjjhwx.cn

[U69] PHP：PDO 预处理
来源：http://ad.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ip.newstarts.cn

[U70] PHP：PDO 事务
来源：http://no.9csxet.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kp.lnxyls.cn

[U71] PHP：抛出异常
来源：http://hb.newstarts.cn

throw new RuntimeException("失败", 500);
来源：http://rr.lnxyls.cn

[U72] PHP：写错误日志
来源：http://sz.hahajie.cn

error_log("失败: " . $e->getMessage());
来源：http://wc.panjiajie.cn

[U73] PHP：读取 ini 配置
来源：http://xp.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://lr.szxytkj.cn

[U74] PHP：读取环境变量
来源：http://ha.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://ai.jctech888.com.cn

[U75] PHP：依赖注入
来源：http://ug.hnjuh.cn

composer require psr/container
来源：http://cd.gzmigu.cn

[U76] PHP：简单路由
来源：http://fk.muxihuayi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lk.hnjuh.cn

[U77] PHP：模板渲染
来源：http://uw.colortex.cn

composer require twig/twig
来源：http://rc.shtwfgs.cn

[U78] PHP：单元测试
来源：http://td.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://cg.huixiangedu.cn

[U79] PHP：静态分析
来源：http://rz.colortex.cn

composer require --dev phpstan/phpstan
来源：http://rz.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://pd.yuntaijiaju.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wt.wgjwhj.cn

[U81] JS：初始化项目
来源：http://xf.shxzskj.cn

npm init -y;  npm i express
来源：http://jr.colortex.cn

[U82] JS：package.json 脚本
来源：http://is.wgjwhj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bp.huixiangedu.cn

[U83] JS：ES Module 导入导出
来源：http://fo.huanxung.cn

export const a = 1;  import { a } from "./m.js";
来源：http://af.gzmigu.cn

[U84] JS：CommonJS 写法
来源：http://yc.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mw.jianghongdianzi.cn

[U85] JS：可选链
来源：http://kw.szsharing.cn

a?.b?.c
来源：http://uh.yuntaijiaju.cn

[U86] JS：空值合并
来源：http://qe.lnxyls.cn

a ?? b
来源：http://fc.huanxung.cn

[U87] JS：解构默认值
来源：http://ql.hahajie.cn

const { a = 1, b = 2 } = obj;
来源：http://te.9csxet.cn

[U88] JS：对象展开合并
来源：http://ea.yuntaijiaju.cn

{ ...a, ...b }
来源：http://cl.shxzskj.cn

[U89] JS：数组去重
来源：http://sf.gzmigu.cn

[...new Set(arr)]
来源：http://nj.bjjhwx.cn

[U90] JS：数字数组排序
来源：http://ou.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://lv.asd995.cn

[U91] JS：对象键值遍历
来源：http://gg.chemitech.net.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://xc.shxzskj.cn

[U92] JS：深拷贝
来源：http://if.yuexingan06.cn

structuredClone(obj)
来源：http://ly.bjjhwx.cn

[U93] JS：模板字符串
来源：http://ln.huanxung.cn

`共 ${n} 条`
来源：http://xh.shxzukj.cn

[U94] JS：箭头函数
来源：http://sb.colortex.cn

const double = x => x * 2;
来源：http://np.shxzukj.cn

[U95] JS：Promise 包装
来源：http://sq.huanxung.cn

new Promise((resolve, reject) => {})
来源：http://vq.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://qh.colortex.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ul.asd995.cn

[U97] JS：并发请求
来源：http://nb.9csxet.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rz.yuexingan06.cn

[U98] JS：fetch 带 JSON
来源：http://lb.hnjuh.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://sp.huanxung.cn

[U99] JS：事件监听
来源：http://du.newstarts.cn

el.addEventListener("click", e => {})
来源：http://rb.shxzukj.cn

[U100] JS：DOM 查询
来源：http://wg.wgjwhj.cn

document.querySelector(".item")
来源：http://zi.lnxyls.cn

[U101] JS：classList 操作
来源：http://kg.9csxet.cn

el.classList.toggle("active")
来源：http://xc.huanxung.cn

[U102] JS：本地存储
来源：http://hp.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ye.huixinmuqiang.cn

[U103] JS：定时器
来源：http://nh.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dj.shtwfgs.cn

[U104] JS：防抖
来源：http://gt.newstarts.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nn.hahajie.cn

[U105] JS：节流
来源：http://kc.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ca.gzmigu.cn

[U106] JS：日期格式化
来源：http://ru.bookmarksfly.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://if.shtwfgs.cn

[U107] JS：数字千分位
来源：http://jj.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://du.panjiajie.cn

[U108] JS：随机整数
来源：http://yu.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://gp.yuexingan06.cn

[U109] JS：数组分组
来源：http://ka.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://zf.haigaiapp.cn

[U110] JS：数组分块
来源：http://le.nszjky.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tb.asd995.cn

[U111] JS：对象转 Map
来源：http://hk.szxytkj.cn

new Map(Object.entries(obj))
来源：http://bb.bjjhwx.cn

[U112] JS：字符串补位
来源：http://jz.szxytkj.cn

"7".padStart(3, "0")
来源：http://mq.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://bn.szxytkj.cn

s.replaceAll("a", "b")
来源：http://iw.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://ls.asd995.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cy.lnxyls.cn

[U115] JS：生成 UUID
来源：http://lg.521024.cn

crypto.randomUUID()
来源：http://hy.shtwfgs.cn

[U116] JS：类型检查（JSDoc）
来源：http://sz.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://kt.bookmarksfly.cn

[U117] JS：单元测试
来源：http://wd.9csxet.cn

npm i -D vitest;  npx vitest
来源：http://wz.shxzskj.cn

[U118] JS：开发服务器
来源：http://kl.huanxung.cn

npm i -D vite;  npx vite
来源：http://sn.nicolike.cn

[U119] JS：生产构建
来源：http://bj.szxytkj.cn

npx vite build
来源：http://sc.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://rw.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://yp.szxytkj.cn

================================================================================
来源：http://jp.szsharing.cn

统计汇总
来源：http://hr.shxzskj.cn

================================================================================
来源：http://mf.bjjhwx.cn

按语言统计（条）：
来源：http://li.521024.cn

Python ......... 252
来源：http://qn.szsharing.cn

PHP ............ 252
来源：http://sz.gzmigu.cn

JavaScript ..... 252
来源：http://gk.shtwfgs.cn

TypeScript ..... 212
来源：http://ij.wgjwhj.cn

Java ........... 212
来源：http://ye.newstarts.cn

Go ............. 212
来源：http://xu.jctech888.com.cn

Ruby ........... 212
来源：http://kt.huixiangedu.cn

C# ............. 212
来源：http://ty.shtwfgs.cn

C .............. 30
来源：http://ci.panjiajie.cn

C++ ............ 30
来源：http://mu.gzmigu.cn

SQL ............ 90
来源：http://co.gzmigu.cn

Bash ........... 80
来源：http://qs.newstarts.cn

Kotlin ......... 15
来源：http://lr.nszjky.cn

Swift .......... 15
来源：http://hw.colortex.cn

Lua ............ 10
来源：http://qf.wgjwhj.cn

Perl ........... 10
来源：http://ba.huanxung.cn

Scala .......... 10
来源：http://bp.chemitech.net.cn

------------------------------------
来源：http://fv.panjiajie.cn

合计 ........... 2106 条
来源：http://fk.9csxet.cn

按章节统计：
来源：http://ca.bookmarksfly.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xc.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://zn.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cq.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ki.shxzskj.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://bb.szsharing.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vm.nszjky.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mq.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xe.gzmigu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ix.jianghongdianzi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://fk.panjiajie.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tf.yuntaijiaju.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ee.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ve.colortex.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eh.shxzukj.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dl.shxzukj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mb.nszjky.cn

Q SQL 专题                              90
来源：http://wh.jctech888.com.cn

R Bash 专题                             80
来源：http://he.shxzskj.cn

S C / C++ 专题                          60
来源：http://wb.haigaiapp.cn

T 其他语言补充                          60
来源：http://vh.bjjhwx.cn

U 高频实用片段                         120
来源：http://ix.shxzskj.cn

------------------------------------
来源：http://vi.muxihuayi.cn

合计                                  2106 条
来源：http://jf.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://pc.hahajie.cn

使用提醒
来源：http://kb.newstarts.cn

--------------------------------------------------------------------------------
来源：http://ch.bjjhwx.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hg.jianghongdianzi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://rr.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://md.colortex.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xy.asd995.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ui.shxzukj.cn

—— 文件结束 ——
来源：http://hn.hahajie.cn

================================================================================
来源：http://gp.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://ie.nszjky.cn

Common Programming Examples Cheat Book
来源：http://wg.muxihuayi.cn

================================================================================
来源：http://op.haigaiapp.cn

【收录内容】
来源：http://qx.9csxet.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xn.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://il.colortex.cn

SQL · Bash · C · C++
来源：http://zu.huanxung.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jq.yuexingan06.cn

【使用说明】
来源：http://go.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jq.huanxung.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ne.shtwfgs.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ec.yuexingan06.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://zr.nicolike.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dw.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://zd.newstarts.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cv.hahajie.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ga.yuexingan06.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fh.haigaiapp.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sx.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vo.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ov.colortex.cn

【文件统计】
来源：http://is.shxzukj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rm.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://ca.nszjky.cn

目  录
来源：http://fa.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://ip.yuexingan06.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://eg.chemitech.net.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yp.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ve.newstarts.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jf.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vt.huanxung.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ei.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://lv.lnxyls.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rc.yuexingan06.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mj.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bp.bookmarksfly.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://le.lnxyls.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://dk.panjiajie.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gd.nicolike.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://sz.huanxung.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://nn.nszjky.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://hq.huanxung.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://qe.521024.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://qy.bookmarksfly.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mo.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://jp.szxytkj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://hn.huixiangedu.cn

================================================================================
来源：http://uq.nicolike.cn

A. 基础语法与类型
来源：http://za.lnxyls.cn

================================================================================
来源：http://pk.wgjwhj.cn

[A01] Hello World
来源：http://qx.yuexingan06.cn

Py:   print("Hello, World!")
来源：http://ko.chemitech.net.cn

PHP:  echo "Hello, World!";
来源：http://kq.jianghongdianzi.cn

JS:   console.log("Hello, World!");
来源：http://qy.jctech888.com.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://qi.muxihuayi.cn

Java: System.out.println("Hello, World!");
来源：http://un.huixinmuqiang.cn

Go:   fmt.Println("Hello, World!")
来源：http://rp.yuexingan06.cn

Ruby: puts "Hello, World!"
来源：http://zq.colortex.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://cf.shxzukj.cn

[A02] 变量声明与赋值
来源：http://lh.hahajie.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sr.huixinmuqiang.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://yw.9csxet.cn

JS:   let name = "Alex"; const age = 20;
来源：http://fe.bjjhwx.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kn.chemitech.net.cn

Java: String name = "Alex"; int age = 20;
来源：http://ju.szxytkj.cn

Go:   name := "Alex"; age := 20
来源：http://pl.lnxyls.cn

Ruby: name = "Alex"; age = 20
来源：http://vi.huanxung.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ly.lnxyls.cn

[A03] 常量定义
来源：http://dj.hnjuh.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://dg.muxihuayi.cn

PHP:  const PI = 3.14159;
来源：http://nl.bookmarksfly.cn

JS:   const PI = 3.14159;
来源：http://bp.huixiangedu.cn

TS:   const PI: number = 3.14159;
来源：http://vd.9csxet.cn

Java: static final double PI = 3.14159;
来源：http://hc.yuexingan06.cn

Go:   const PI = 3.14159
来源：http://ct.haigaiapp.cn

Ruby: PI = 3.14159
来源：http://tq.shtwfgs.cn

C#:   const double PI = 3.14159;
来源：http://qr.newstarts.cn

[A04] 判断变量类型
来源：http://jh.shxzukj.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://je.panjiajie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gh.yuntaijiaju.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://bu.nicolike.cn

TS:   typeof x; x instanceof Date
来源：http://ex.gzmigu.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://gf.muxihuayi.cn

Go:   reflect.TypeOf(x).Name()
来源：http://jd.yuntaijiaju.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://dk.huixiangedu.cn

C#:   x.GetType().Name; x is int
来源：http://zn.shxzukj.cn

[A05] 整数除法与取模
来源：http://kp.panjiajie.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bd.nszjky.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ls.nszjky.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://gh.hahajie.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://fb.chemitech.net.cn


<!-- 参考信息 -->