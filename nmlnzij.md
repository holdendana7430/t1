代发 wailian999

[U35] Py：发送邮件
来源：http://uo.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mj.lnxyls.cn

[U36] Py：定时任务
来源：http://ux.panjiajie.cn

schedule.every(10).minutes.do(job)
来源：http://vb.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://bc.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ed.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://rx.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://cm.yuntaijiaju.cn

[U39] Py：判断是否在交互环境
来源：http://st.nszjky.cn

sys.stdout.isatty()
来源：http://or.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ja.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://oq.muxihuayi.cn

[U41] PHP：初始化 Composer 项目
来源：http://qr.wgjwhj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://us.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://db.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ss.szsharing.cn

[U43] PHP：声明命名空间
来源：http://md.bjjhwx.cn

namespace App\Http;
来源：http://ds.panjiajie.cn

[U44] PHP：开启严格类型
来源：http://af.nszjky.cn

declare(strict_types=1);
来源：http://mj.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://if.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://gr.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://si.bookmarksfly.cn

?string $name = null
来源：http://ak.haigaiapp.cn

[U47] PHP：联合类型
来源：http://nj.colortex.cn

int|string $id
来源：http://fg.hahajie.cn

[U48] PHP：纯枚举
来源：http://bt.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rq.panjiajie.cn

[U49] PHP：只读属性
来源：http://nj.nicolike.cn

public readonly string $name
来源：http://co.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://he.9csxet.cn

public function __construct(private int $id) {}
来源：http://fm.shxzskj.cn

[U51] PHP：数组解构
来源：http://fx.chemitech.net.cn

[$a, $b] = $arr;
来源：http://sh.bjjhwx.cn

[U52] PHP：箭头函数
来源：http://my.newstarts.cn

$double = fn($x) => $x * 2;
来源：http://sp.nicolike.cn

[U53] PHP：空合并运算符
来源：http://sc.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://rl.haigaiapp.cn

[U54] PHP：空安全调用
来源：http://ij.bjjhwx.cn

$obj?->method()
来源：http://bn.huanxung.cn

[U55] PHP：match 表达式
来源：http://ux.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qv.szxytkj.cn

[U56] PHP：命名参数
来源：http://pz.haigaiapp.cn

f(a: 1, b: 2)
来源：http://ix.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://pp.shxzskj.cn

"值: {$a}"
来源：http://wr.hahajie.cn

[U58] PHP：数组三件套
来源：http://xd.colortex.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://gw.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://di.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cn.shtwfgs.cn

[U60] PHP：JSON 编解码
来源：http://yr.gzmigu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cm.huixiangedu.cn

[U61] PHP：正则
来源：http://iw.bjjhwx.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://fa.shxzskj.cn

[U62] PHP：日期对象
来源：http://bf.muxihuayi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lv.shxzukj.cn

[U63] PHP：文件读写
来源：http://ti.shtwfgs.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dz.newstarts.cn

[U64] PHP：目录遍历
来源：http://on.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://bn.colortex.cn

[U65] PHP：会话
来源：http://rs.chemitech.net.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kb.jianghongdianzi.cn

[U66] PHP：设置 Cookie
来源：http://wb.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fe.shtwfgs.cn

[U67] PHP：处理文件上传
来源：http://an.9csxet.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mw.colortex.cn

[U68] PHP：PDO 连接
来源：http://mk.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xo.521024.cn

[U69] PHP：PDO 预处理
来源：http://ea.shxzukj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wo.nszjky.cn

[U70] PHP：PDO 事务
来源：http://vm.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vw.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://vn.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://ud.colortex.cn

[U72] PHP：写错误日志
来源：http://gh.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://xi.bjjhwx.cn

[U73] PHP：读取 ini 配置
来源：http://tp.9csxet.cn

parse_ini_file("config.ini", true)
来源：http://fn.asd995.cn

[U74] PHP：读取环境变量
来源：http://ay.yuntaijiaju.cn

getenv("APP_ENV") ?: "production"
来源：http://va.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://cb.panjiajie.cn

composer require psr/container
来源：http://fw.szxytkj.cn

[U76] PHP：简单路由
来源：http://to.colortex.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jw.colortex.cn

[U77] PHP：模板渲染
来源：http://pb.bjjhwx.cn

composer require twig/twig
来源：http://wo.chemitech.net.cn

[U78] PHP：单元测试
来源：http://re.jianghongdianzi.cn

composer require --dev phpunit/phpunit
来源：http://cg.szsharing.cn

[U79] PHP：静态分析
来源：http://uy.wgjwhj.cn

composer require --dev phpstan/phpstan
来源：http://qi.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://qj.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ps.asd995.cn

[U81] JS：初始化项目
来源：http://qp.huanxung.cn

npm init -y;  npm i express
来源：http://dt.huanxung.cn

[U82] JS：package.json 脚本
来源：http://cl.9csxet.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://gj.shxzskj.cn

[U83] JS：ES Module 导入导出
来源：http://rc.gzmigu.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vl.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://he.9csxet.cn

module.exports = { a };  const { a } = require("./m");
来源：http://vi.bjjhwx.cn

[U85] JS：可选链
来源：http://pa.chemitech.net.cn

a?.b?.c
来源：http://wx.shxzukj.cn

[U86] JS：空值合并
来源：http://bl.yuntaijiaju.cn

a ?? b
来源：http://sq.colortex.cn

[U87] JS：解构默认值
来源：http://fg.jianghongdianzi.cn

const { a = 1, b = 2 } = obj;
来源：http://py.huixiangedu.cn

[U88] JS：对象展开合并
来源：http://di.panjiajie.cn

{ ...a, ...b }
来源：http://cp.jctech888.com.cn

[U89] JS：数组去重
来源：http://cp.muxihuayi.cn

[...new Set(arr)]
来源：http://ct.shxzukj.cn

[U90] JS：数字数组排序
来源：http://kz.yuexingan06.cn

[...arr].sort((a, b) => a - b)
来源：http://fg.shxzukj.cn

[U91] JS：对象键值遍历
来源：http://bl.hnjuh.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ji.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://hz.huixiangedu.cn

structuredClone(obj)
来源：http://mu.shxzukj.cn

[U93] JS：模板字符串
来源：http://oq.shxzskj.cn

`共 ${n} 条`
来源：http://rb.huixiangedu.cn

[U94] JS：箭头函数
来源：http://ky.nszjky.cn

const double = x => x * 2;
来源：http://db.shxzskj.cn

[U95] JS：Promise 包装
来源：http://vh.shxzskj.cn

new Promise((resolve, reject) => {})
来源：http://uy.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://fn.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hi.lnxyls.cn

[U97] JS：并发请求
来源：http://gk.nszjky.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://fc.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://pf.yuntaijiaju.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gk.521024.cn

[U99] JS：事件监听
来源：http://zu.colortex.cn

el.addEventListener("click", e => {})
来源：http://hx.panjiajie.cn

[U100] JS：DOM 查询
来源：http://lx.muxihuayi.cn

document.querySelector(".item")
来源：http://oe.haigaiapp.cn

[U101] JS：classList 操作
来源：http://sw.nicolike.cn

el.classList.toggle("active")
来源：http://ye.chemitech.net.cn

[U102] JS：本地存储
来源：http://ws.szsharing.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://wm.huixiangedu.cn

[U103] JS：定时器
来源：http://pj.huixiangedu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://xd.nicolike.cn

[U104] JS：防抖
来源：http://kl.gzmigu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://za.shxzskj.cn

[U105] JS：节流
来源：http://vv.hnjuh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://bv.shtwfgs.cn

[U106] JS：日期格式化
来源：http://yr.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yz.lnxyls.cn

[U107] JS：数字千分位
来源：http://gz.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gu.haigaiapp.cn

[U108] JS：随机整数
来源：http://sr.colortex.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pf.huixinmuqiang.cn

[U109] JS：数组分组
来源：http://kr.asd995.cn

Object.groupBy(arr, x => x.type)
来源：http://xe.lnxyls.cn

[U110] JS：数组分块
来源：http://ps.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ho.521024.cn

[U111] JS：对象转 Map
来源：http://cd.huixiangedu.cn

new Map(Object.entries(obj))
来源：http://xv.huixiangedu.cn

[U112] JS：字符串补位
来源：http://jf.szxytkj.cn

"7".padStart(3, "0")
来源：http://hr.asd995.cn

[U113] JS：正则替换全部
来源：http://bq.jianghongdianzi.cn

s.replaceAll("a", "b")
来源：http://wt.hahajie.cn

[U114] JS：JSON 深比较
来源：http://wj.huixinmuqiang.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://fh.yuntaijiaju.cn

[U115] JS：生成 UUID
来源：http://rj.wgjwhj.cn

crypto.randomUUID()
来源：http://je.shxzukj.cn

[U116] JS：类型检查（JSDoc）
来源：http://jf.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://le.nicolike.cn

[U117] JS：单元测试
来源：http://kx.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://vm.huixiangedu.cn

[U118] JS：开发服务器
来源：http://xa.szsharing.cn

npm i -D vite;  npx vite
来源：http://nf.szxytkj.cn

[U119] JS：生产构建
来源：http://uu.huixiangedu.cn

npx vite build
来源：http://xt.gzmigu.cn

[U120] JS：读取环境变量（Vite）
来源：http://pl.asd995.cn

import.meta.env.VITE_API_URL
来源：http://bx.szsharing.cn

================================================================================
来源：http://uw.asd995.cn

统计汇总
来源：http://mx.521024.cn

================================================================================
来源：http://be.chemitech.net.cn

按语言统计（条）：
来源：http://jd.panjiajie.cn

Python ......... 252
来源：http://vg.wgjwhj.cn

PHP ............ 252
来源：http://mh.hahajie.cn

JavaScript ..... 252
来源：http://fb.wgjwhj.cn

TypeScript ..... 212
来源：http://bn.hahajie.cn

Java ........... 212
来源：http://oq.haigaiapp.cn

Go ............. 212
来源：http://sv.jctech888.com.cn

Ruby ........... 212
来源：http://cb.bjjhwx.cn

C# ............. 212
来源：http://rk.chemitech.net.cn

C .............. 30
来源：http://id.muxihuayi.cn

C++ ............ 30
来源：http://se.jctech888.com.cn

SQL ............ 90
来源：http://fo.szsharing.cn

Bash ........... 80
来源：http://uj.hnjuh.cn

Kotlin ......... 15
来源：http://se.huixinmuqiang.cn

Swift .......... 15
来源：http://as.panjiajie.cn

Lua ............ 10
来源：http://ct.asd995.cn

Perl ........... 10
来源：http://uw.shxzskj.cn

Scala .......... 10
来源：http://ka.bjjhwx.cn

------------------------------------
来源：http://wi.shtwfgs.cn

合计 ........... 2106 条
来源：http://ql.bookmarksfly.cn

按章节统计：
来源：http://fz.haigaiapp.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://oh.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gk.bookmarksfly.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xf.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://za.huixinmuqiang.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://cl.bjjhwx.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://xr.shxzskj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ca.chemitech.net.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ow.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fo.panjiajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://bw.9csxet.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wo.huixinmuqiang.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kb.huixinmuqiang.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vw.9csxet.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ka.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://tc.nszjky.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://br.wgjwhj.cn

Q SQL 专题                              90
来源：http://dv.shxzskj.cn

R Bash 专题                             80
来源：http://ao.szsharing.cn

S C / C++ 专题                          60
来源：http://dz.asd995.cn

T 其他语言补充                          60
来源：http://hq.chemitech.net.cn

U 高频实用片段                         120
来源：http://tg.jianghongdianzi.cn

------------------------------------
来源：http://dn.jianghongdianzi.cn

合计                                  2106 条
来源：http://sz.huanxung.cn

--------------------------------------------------------------------------------
来源：http://bt.yuntaijiaju.cn

使用提醒
来源：http://bx.hahajie.cn

--------------------------------------------------------------------------------
来源：http://vr.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lu.gzmigu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fb.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vl.newstarts.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://wn.panjiajie.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ln.hnjuh.cn

—— 文件结束 ——
来源：http://ll.shxzskj.cn

================================================================================
来源：http://im.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://tn.yuntaijiaju.cn

Common Programming Examples Cheat Book
来源：http://cb.shtwfgs.cn

================================================================================
来源：http://ye.nicolike.cn

【收录内容】
来源：http://iq.newstarts.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jq.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://fz.521024.cn

SQL · Bash · C · C++
来源：http://hh.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gv.nicolike.cn

【使用说明】
来源：http://ai.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pw.nszjky.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://la.wgjwhj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dl.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://cd.szxytkj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ci.szsharing.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mw.huixiangedu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nc.chemitech.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ht.newstarts.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://jl.huanxung.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://rd.colortex.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yd.bjjhwx.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ee.huanxung.cn

【文件统计】
来源：http://op.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bk.asd995.cn

--------------------------------------------------------------------------------
来源：http://ie.jianghongdianzi.cn

目  录
来源：http://hu.lnxyls.cn

--------------------------------------------------------------------------------
来源：http://ly.bookmarksfly.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gz.huanxung.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://vs.nszjky.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://dm.bookmarksfly.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://pf.shtwfgs.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://so.newstarts.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zg.jctech888.com.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://hl.wgjwhj.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://co.9csxet.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://lc.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dv.yuexingan06.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tt.shtwfgs.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://xo.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cx.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wx.yuntaijiaju.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ik.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cb.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://aa.hnjuh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ly.muxihuayi.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rr.shtwfgs.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cj.yuntaijiaju.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ls.yuexingan06.cn

================================================================================
来源：http://xr.9csxet.cn

A. 基础语法与类型
来源：http://vz.shxzskj.cn

================================================================================
来源：http://jx.lnxyls.cn

[A01] Hello World
来源：http://ns.shxzskj.cn

Py:   print("Hello, World!")
来源：http://xv.gzmigu.cn

PHP:  echo "Hello, World!";
来源：http://oa.hnjuh.cn

JS:   console.log("Hello, World!");
来源：http://ac.colortex.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bf.huixinmuqiang.cn

Java: System.out.println("Hello, World!");
来源：http://pi.shxzskj.cn

Go:   fmt.Println("Hello, World!")
来源：http://om.muxihuayi.cn

Ruby: puts "Hello, World!"
来源：http://zq.gzmigu.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://aa.9csxet.cn

[A02] 变量声明与赋值
来源：http://ku.jianghongdianzi.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://hb.nszjky.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ke.jianghongdianzi.cn

JS:   let name = "Alex"; const age = 20;
来源：http://nh.huanxung.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zs.hnjuh.cn

Java: String name = "Alex"; int age = 20;
来源：http://xl.bjjhwx.cn

Go:   name := "Alex"; age := 20
来源：http://cn.muxihuayi.cn

Ruby: name = "Alex"; age = 20
来源：http://xl.shxzukj.cn

C#:   string name = "Alex"; int age = 20;
来源：http://sk.colortex.cn

[A03] 常量定义
来源：http://mz.shxzukj.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gj.nszjky.cn

PHP:  const PI = 3.14159;
来源：http://dc.gzmigu.cn


<!-- 参考信息 -->