代发 wailian999

[U33] Py：打包发布
来源：http://nz.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://fn.newstarts.cn

[U34] Py：判断编码
来源：http://sj.haigaiapp.cn

chardet.detect(raw)
来源：http://aq.hahajie.cn

[U35] Py：发送邮件
来源：http://qf.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ji.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://in.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://ul.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://ic.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fw.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://wg.hnjuh.cn

Path(__file__).resolve().parent
来源：http://cl.asd995.cn

[U39] Py：判断是否在交互环境
来源：http://fy.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://uw.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://nt.wgjwhj.cn

print("err", file=sys.stderr)
来源：http://kj.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://ec.521024.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://lq.shxzskj.cn

[U42] PHP：PSR-4 自动加载
来源：http://jn.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ff.newstarts.cn

[U43] PHP：声明命名空间
来源：http://mu.asd995.cn

namespace App\Http;
来源：http://gu.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://fd.huixinmuqiang.cn

declare(strict_types=1);
来源：http://yg.asd995.cn

[U45] PHP：类型声明与返回类型
来源：http://mr.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://to.yuexingan06.cn

[U46] PHP：可空类型
来源：http://ey.haigaiapp.cn

?string $name = null
来源：http://dx.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://gq.asd995.cn

int|string $id
来源：http://xo.shxzukj.cn

[U48] PHP：纯枚举
来源：http://bw.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ay.gzmigu.cn

[U49] PHP：只读属性
来源：http://xv.bjjhwx.cn

public readonly string $name
来源：http://cw.yuexingan06.cn

[U50] PHP：构造器属性提升
来源：http://dy.huanxung.cn

public function __construct(private int $id) {}
来源：http://us.huanxung.cn

[U51] PHP：数组解构
来源：http://uk.muxihuayi.cn

[$a, $b] = $arr;
来源：http://qd.shtwfgs.cn

[U52] PHP：箭头函数
来源：http://qi.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://si.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://wc.521024.cn

$v = $a ?? $b ?? "default";
来源：http://qk.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://eg.yuntaijiaju.cn

$obj?->method()
来源：http://ff.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://ys.jctech888.com.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fy.shxzukj.cn

[U56] PHP：命名参数
来源：http://ul.muxihuayi.cn

f(a: 1, b: 2)
来源：http://hm.muxihuayi.cn

[U57] PHP：字符串插值
来源：http://bp.yuntaijiaju.cn

"值: {$a}"
来源：http://th.9csxet.cn

[U58] PHP：数组三件套
来源：http://zm.yuexingan06.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://kn.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://bm.wgjwhj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uf.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://qy.bookmarksfly.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://zg.huixiangedu.cn

[U61] PHP：正则
来源：http://ak.huixinmuqiang.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qh.wgjwhj.cn

[U62] PHP：日期对象
来源：http://hl.hnjuh.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zo.haigaiapp.cn

[U63] PHP：文件读写
来源：http://bx.9csxet.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ky.hahajie.cn

[U64] PHP：目录遍历
来源：http://id.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://ir.521024.cn

[U65] PHP：会话
来源：http://cy.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://dg.huanxung.cn

[U66] PHP：设置 Cookie
来源：http://le.muxihuayi.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jw.newstarts.cn

[U67] PHP：处理文件上传
来源：http://mj.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://om.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://pb.huixiangedu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ct.panjiajie.cn

[U69] PHP：PDO 预处理
来源：http://jj.wgjwhj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://dn.9csxet.cn

[U70] PHP：PDO 事务
来源：http://oj.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ce.hahajie.cn

[U71] PHP：抛出异常
来源：http://us.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://zz.szsharing.cn

[U72] PHP：写错误日志
来源：http://st.huanxung.cn

error_log("失败: " . $e->getMessage());
来源：http://qq.huanxung.cn

[U73] PHP：读取 ini 配置
来源：http://zh.shxzukj.cn

parse_ini_file("config.ini", true)
来源：http://qa.huanxung.cn

[U74] PHP：读取环境变量
来源：http://sp.szsharing.cn

getenv("APP_ENV") ?: "production"
来源：http://da.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://tn.newstarts.cn

composer require psr/container
来源：http://pd.szsharing.cn

[U76] PHP：简单路由
来源：http://sh.shtwfgs.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yf.9csxet.cn

[U77] PHP：模板渲染
来源：http://ch.521024.cn

composer require twig/twig
来源：http://oz.gzmigu.cn

[U78] PHP：单元测试
来源：http://nn.lnxyls.cn

composer require --dev phpunit/phpunit
来源：http://hs.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://lx.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://gy.huixiangedu.cn

[U80] PHP：代码规范修复
来源：http://nq.huanxung.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ul.nicolike.cn

[U81] JS：初始化项目
来源：http://qk.panjiajie.cn

npm init -y;  npm i express
来源：http://kw.hahajie.cn

[U82] JS：package.json 脚本
来源：http://sb.muxihuayi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://xq.yuexingan06.cn

[U83] JS：ES Module 导入导出
来源：http://hg.9csxet.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qj.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://vv.hahajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://my.jctech888.com.cn

[U85] JS：可选链
来源：http://bj.521024.cn

a?.b?.c
来源：http://kg.lnxyls.cn

[U86] JS：空值合并
来源：http://mf.yuntaijiaju.cn

a ?? b
来源：http://gc.szsharing.cn

[U87] JS：解构默认值
来源：http://cj.nszjky.cn

const { a = 1, b = 2 } = obj;
来源：http://bw.bookmarksfly.cn

[U88] JS：对象展开合并
来源：http://ib.yuexingan06.cn

{ ...a, ...b }
来源：http://wd.hahajie.cn

[U89] JS：数组去重
来源：http://kz.panjiajie.cn

[...new Set(arr)]
来源：http://ig.asd995.cn

[U90] JS：数字数组排序
来源：http://yd.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://if.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://wu.panjiajie.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mu.gzmigu.cn

[U92] JS：深拷贝
来源：http://wx.lnxyls.cn

structuredClone(obj)
来源：http://ba.nszjky.cn

[U93] JS：模板字符串
来源：http://vh.nicolike.cn

`共 ${n} 条`
来源：http://ab.gzmigu.cn

[U94] JS：箭头函数
来源：http://fd.wgjwhj.cn

const double = x => x * 2;
来源：http://db.shxzukj.cn

[U95] JS：Promise 包装
来源：http://sr.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://ct.9csxet.cn

[U96] JS：async/await 与异常
来源：http://er.huixiangedu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dc.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://vf.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ba.chemitech.net.cn

[U98] JS：fetch 带 JSON
来源：http://vt.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wy.jianghongdianzi.cn

[U99] JS：事件监听
来源：http://qw.shtwfgs.cn

el.addEventListener("click", e => {})
来源：http://xv.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://rh.muxihuayi.cn

document.querySelector(".item")
来源：http://lu.panjiajie.cn

[U101] JS：classList 操作
来源：http://tv.huixiangedu.cn

el.classList.toggle("active")
来源：http://fg.9csxet.cn

[U102] JS：本地存储
来源：http://eg.haigaiapp.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://rg.nszjky.cn

[U103] JS：定时器
来源：http://xg.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fp.hnjuh.cn

[U104] JS：防抖
来源：http://pi.wgjwhj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qa.huixinmuqiang.cn

[U105] JS：节流
来源：http://uh.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cb.shxzskj.cn

[U106] JS：日期格式化
来源：http://oz.jctech888.com.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fo.asd995.cn

[U107] JS：数字千分位
来源：http://eg.bookmarksfly.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ti.colortex.cn

[U108] JS：随机整数
来源：http://fl.asd995.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ru.panjiajie.cn

[U109] JS：数组分组
来源：http://gy.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://pj.yuexingan06.cn

[U110] JS：数组分块
来源：http://ln.yuntaijiaju.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tv.nicolike.cn

[U111] JS：对象转 Map
来源：http://wq.shxzskj.cn

new Map(Object.entries(obj))
来源：http://kd.muxihuayi.cn

[U112] JS：字符串补位
来源：http://aa.szxytkj.cn

"7".padStart(3, "0")
来源：http://gz.hahajie.cn

[U113] JS：正则替换全部
来源：http://jg.huixiangedu.cn

s.replaceAll("a", "b")
来源：http://xn.521024.cn

[U114] JS：JSON 深比较
来源：http://ct.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://xm.huixiangedu.cn

[U115] JS：生成 UUID
来源：http://to.bookmarksfly.cn

crypto.randomUUID()
来源：http://re.gzmigu.cn

[U116] JS：类型检查（JSDoc）
来源：http://uf.newstarts.cn

/** @param {string} name */ function f(name) {}
来源：http://pq.colortex.cn

[U117] JS：单元测试
来源：http://kg.huanxung.cn

npm i -D vitest;  npx vitest
来源：http://lx.haigaiapp.cn

[U118] JS：开发服务器
来源：http://qv.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://pw.gzmigu.cn

[U119] JS：生产构建
来源：http://zt.yuexingan06.cn

npx vite build
来源：http://zv.nicolike.cn

[U120] JS：读取环境变量（Vite）
来源：http://he.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://hl.haigaiapp.cn

================================================================================
来源：http://cr.huixiangedu.cn

统计汇总
来源：http://iz.nszjky.cn

================================================================================
来源：http://jh.wgjwhj.cn

按语言统计（条）：
来源：http://hn.wgjwhj.cn

Python ......... 252
来源：http://tb.szxytkj.cn

PHP ............ 252
来源：http://fn.szxytkj.cn

JavaScript ..... 252
来源：http://wi.9csxet.cn

TypeScript ..... 212
来源：http://ur.huixiangedu.cn

Java ........... 212
来源：http://it.nicolike.cn

Go ............. 212
来源：http://fh.nicolike.cn

Ruby ........... 212
来源：http://qq.wgjwhj.cn

C# ............. 212
来源：http://wi.yuexingan06.cn

C .............. 30
来源：http://vg.huanxung.cn

C++ ............ 30
来源：http://lr.shxzskj.cn

SQL ............ 90
来源：http://nv.hnjuh.cn

Bash ........... 80
来源：http://mw.jianghongdianzi.cn

Kotlin ......... 15
来源：http://mj.jctech888.com.cn

Swift .......... 15
来源：http://gv.huixinmuqiang.cn

Lua ............ 10
来源：http://ei.shxzskj.cn

Perl ........... 10
来源：http://wq.huixinmuqiang.cn

Scala .......... 10
来源：http://zg.521024.cn

------------------------------------
来源：http://mw.szxytkj.cn

合计 ........... 2106 条
来源：http://ns.9csxet.cn

按章节统计：
来源：http://vl.shxzukj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ww.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hy.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://od.nszjky.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://od.huixiangedu.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iv.panjiajie.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nh.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://si.nicolike.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://eu.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jq.yuntaijiaju.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://iu.newstarts.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://bc.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ou.bjjhwx.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://vb.jctech888.com.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://os.9csxet.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hs.colortex.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://fr.hahajie.cn

Q SQL 专题                              90
来源：http://tn.panjiajie.cn

R Bash 专题                             80
来源：http://ji.shxzukj.cn

S C / C++ 专题                          60
来源：http://ib.9csxet.cn

T 其他语言补充                          60
来源：http://gi.521024.cn

U 高频实用片段                         120
来源：http://dz.chemitech.net.cn

------------------------------------
来源：http://my.yuntaijiaju.cn

合计                                  2106 条
来源：http://co.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://mi.shxzskj.cn

使用提醒
来源：http://ve.szsharing.cn

--------------------------------------------------------------------------------
来源：http://se.bookmarksfly.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://uk.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sr.yuntaijiaju.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://rj.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://vj.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ci.colortex.cn

—— 文件结束 ——
来源：http://ki.nszjky.cn

================================================================================
来源：http://sb.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://wj.jianghongdianzi.cn

Common Programming Examples Cheat Book
来源：http://kq.szxytkj.cn

================================================================================
来源：http://mt.shxzskj.cn

【收录内容】
来源：http://zk.chemitech.net.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://lc.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wv.szxytkj.cn

SQL · Bash · C · C++
来源：http://jh.lnxyls.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zd.shtwfgs.cn

【使用说明】
来源：http://dt.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qj.521024.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yp.yuntaijiaju.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jc.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://kn.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://er.asd995.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://om.yuntaijiaju.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ws.yuexingan06.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://lv.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ap.shxzskj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sx.muxihuayi.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://hl.shxzskj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vt.colortex.cn

【文件统计】
来源：http://cb.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tq.newstarts.cn

--------------------------------------------------------------------------------
来源：http://cz.chemitech.net.cn

目  录
来源：http://sh.nicolike.cn

--------------------------------------------------------------------------------
来源：http://zz.jianghongdianzi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fx.nszjky.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rv.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qi.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ki.bookmarksfly.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://an.gzmigu.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://bq.huixiangedu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mg.huixinmuqiang.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tt.nszjky.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://di.jctech888.com.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hl.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://nh.huanxung.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iz.yuexingan06.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://lq.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jj.hahajie.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://gc.gzmigu.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://gf.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ja.shxzskj.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://cj.huixinmuqiang.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ze.9csxet.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ga.huixinmuqiang.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://vw.haigaiapp.cn

================================================================================
来源：http://fb.nszjky.cn

A. 基础语法与类型
来源：http://yn.huixinmuqiang.cn

================================================================================
来源：http://qk.bookmarksfly.cn

[A01] Hello World
来源：http://mi.muxihuayi.cn

Py:   print("Hello, World!")
来源：http://fz.asd995.cn

PHP:  echo "Hello, World!";
来源：http://pa.hahajie.cn

JS:   console.log("Hello, World!");
来源：http://uj.huixiangedu.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://un.szsharing.cn

Java: System.out.println("Hello, World!");
来源：http://sx.gzmigu.cn

Go:   fmt.Println("Hello, World!")
来源：http://sa.haigaiapp.cn

Ruby: puts "Hello, World!"
来源：http://yt.muxihuayi.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vq.gzmigu.cn

[A02] 变量声明与赋值
来源：http://lq.huixinmuqiang.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://md.huixiangedu.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kn.yuntaijiaju.cn

JS:   let name = "Alex"; const age = 20;
来源：http://uv.haigaiapp.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://jf.bjjhwx.cn

Java: String name = "Alex"; int age = 20;
来源：http://um.shxzukj.cn

Go:   name := "Alex"; age := 20
来源：http://as.huixinmuqiang.cn

Ruby: name = "Alex"; age = 20
来源：http://nr.chemitech.net.cn


<!-- 参考信息 -->