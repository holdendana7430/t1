代发 wailian999

[U31] Py：单测
来源：http://vo.bjjhwx.cn

python -m pytest -q
来源：http://vu.shxzskj.cn

[U32] Py：代码格式化
来源：http://kv.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://nj.bookmarksfly.cn

[U33] Py：打包发布
来源：http://ao.nicolike.cn

python -m build  （依赖 pyproject.toml）
来源：http://os.wgjwhj.cn

[U34] Py：判断编码
来源：http://jd.wgjwhj.cn

chardet.detect(raw)
来源：http://xc.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://lg.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tr.colortex.cn

[U36] Py：定时任务
来源：http://nt.9csxet.cn

schedule.every(10).minutes.do(job)
来源：http://us.nicolike.cn

[U37] Py：读写 Excel
来源：http://yt.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ug.yuexingan06.cn

[U38] Py：获取脚本所在目录
来源：http://qt.asd995.cn

Path(__file__).resolve().parent
来源：http://gn.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://zi.haigaiapp.cn

sys.stdout.isatty()
来源：http://nu.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://eq.colortex.cn

print("err", file=sys.stderr)
来源：http://or.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ne.9csxet.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vk.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://qq.huixiangedu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://sr.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://zr.yuntaijiaju.cn

namespace App\Http;
来源：http://ob.szsharing.cn

[U44] PHP：开启严格类型
来源：http://qk.huixinmuqiang.cn

declare(strict_types=1);
来源：http://kf.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://wy.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cj.szxytkj.cn

[U46] PHP：可空类型
来源：http://ae.chemitech.net.cn

?string $name = null
来源：http://aw.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://zp.huixiangedu.cn

int|string $id
来源：http://ot.huanxung.cn

[U48] PHP：纯枚举
来源：http://lj.nicolike.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qn.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://cw.chemitech.net.cn

public readonly string $name
来源：http://ec.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://gs.szsharing.cn

public function __construct(private int $id) {}
来源：http://rd.9csxet.cn

[U51] PHP：数组解构
来源：http://rx.shxzukj.cn

[$a, $b] = $arr;
来源：http://hy.nszjky.cn

[U52] PHP：箭头函数
来源：http://wi.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://kl.jctech888.com.cn

[U53] PHP：空合并运算符
来源：http://wp.newstarts.cn

$v = $a ?? $b ?? "default";
来源：http://ti.yuntaijiaju.cn

[U54] PHP：空安全调用
来源：http://pf.hahajie.cn

$obj?->method()
来源：http://fj.panjiajie.cn

[U55] PHP：match 表达式
来源：http://nd.szxytkj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://of.gzmigu.cn

[U56] PHP：命名参数
来源：http://ha.szxytkj.cn

f(a: 1, b: 2)
来源：http://gr.jianghongdianzi.cn

[U57] PHP：字符串插值
来源：http://pa.huixinmuqiang.cn

"值: {$a}"
来源：http://bf.lnxyls.cn

[U58] PHP：数组三件套
来源：http://zu.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ix.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://vu.nszjky.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gh.bookmarksfly.cn

[U60] PHP：JSON 编解码
来源：http://qr.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jy.hnjuh.cn

[U61] PHP：正则
来源：http://pq.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jo.chemitech.net.cn

[U62] PHP：日期对象
来源：http://kd.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ru.gzmigu.cn

[U63] PHP：文件读写
来源：http://rm.shxzukj.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xy.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://xl.9csxet.cn

glob("dir/*.php");  scandir("dir");
来源：http://sh.muxihuayi.cn

[U65] PHP：会话
来源：http://ew.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://qq.jctech888.com.cn

[U66] PHP：设置 Cookie
来源：http://fl.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gq.jctech888.com.cn

[U67] PHP：处理文件上传
来源：http://gc.hahajie.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://le.colortex.cn

[U68] PHP：PDO 连接
来源：http://zo.panjiajie.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://iv.yuntaijiaju.cn

[U69] PHP：PDO 预处理
来源：http://bp.jianghongdianzi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lo.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://jm.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vh.muxihuayi.cn

[U71] PHP：抛出异常
来源：http://pk.nszjky.cn

throw new RuntimeException("失败", 500);
来源：http://nh.panjiajie.cn

[U72] PHP：写错误日志
来源：http://lw.huixiangedu.cn

error_log("失败: " . $e->getMessage());
来源：http://mw.colortex.cn

[U73] PHP：读取 ini 配置
来源：http://wu.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://od.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://oe.gzmigu.cn

getenv("APP_ENV") ?: "production"
来源：http://rg.colortex.cn

[U75] PHP：依赖注入
来源：http://xo.yuexingan06.cn

composer require psr/container
来源：http://uc.muxihuayi.cn

[U76] PHP：简单路由
来源：http://ci.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wt.nicolike.cn

[U77] PHP：模板渲染
来源：http://sy.yuntaijiaju.cn

composer require twig/twig
来源：http://ap.lnxyls.cn

[U78] PHP：单元测试
来源：http://pr.huixinmuqiang.cn

composer require --dev phpunit/phpunit
来源：http://ox.huixinmuqiang.cn

[U79] PHP：静态分析
来源：http://jg.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://ww.521024.cn

[U80] PHP：代码规范修复
来源：http://eq.bjjhwx.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://lu.yuexingan06.cn

[U81] JS：初始化项目
来源：http://ey.shtwfgs.cn

npm init -y;  npm i express
来源：http://mi.shtwfgs.cn

[U82] JS：package.json 脚本
来源：http://lm.szsharing.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ni.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://bm.yuntaijiaju.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zv.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://jq.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ps.shtwfgs.cn

[U85] JS：可选链
来源：http://kk.shxzskj.cn

a?.b?.c
来源：http://gq.hnjuh.cn

[U86] JS：空值合并
来源：http://fq.9csxet.cn

a ?? b
来源：http://ri.shxzskj.cn

[U87] JS：解构默认值
来源：http://pq.panjiajie.cn

const { a = 1, b = 2 } = obj;
来源：http://xf.szsharing.cn

[U88] JS：对象展开合并
来源：http://kz.yuexingan06.cn

{ ...a, ...b }
来源：http://nf.shxzskj.cn

[U89] JS：数组去重
来源：http://ra.9csxet.cn

[...new Set(arr)]
来源：http://ti.lnxyls.cn

[U90] JS：数字数组排序
来源：http://ah.jctech888.com.cn

[...arr].sort((a, b) => a - b)
来源：http://dx.muxihuayi.cn

[U91] JS：对象键值遍历
来源：http://wo.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://fu.panjiajie.cn

[U92] JS：深拷贝
来源：http://dk.wgjwhj.cn

structuredClone(obj)
来源：http://co.yuntaijiaju.cn

[U93] JS：模板字符串
来源：http://vn.jianghongdianzi.cn

`共 ${n} 条`
来源：http://fd.9csxet.cn

[U94] JS：箭头函数
来源：http://zj.lnxyls.cn

const double = x => x * 2;
来源：http://ye.yuexingan06.cn

[U95] JS：Promise 包装
来源：http://nc.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://ty.bookmarksfly.cn

[U96] JS：async/await 与异常
来源：http://ss.yuexingan06.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rc.hnjuh.cn

[U97] JS：并发请求
来源：http://zp.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ez.gzmigu.cn

[U98] JS：fetch 带 JSON
来源：http://qb.521024.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pn.colortex.cn

[U99] JS：事件监听
来源：http://nr.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://fk.huanxung.cn

[U100] JS：DOM 查询
来源：http://vq.huixiangedu.cn

document.querySelector(".item")
来源：http://lu.bjjhwx.cn

[U101] JS：classList 操作
来源：http://jg.shtwfgs.cn

el.classList.toggle("active")
来源：http://vn.nszjky.cn

[U102] JS：本地存储
来源：http://qb.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ub.bjjhwx.cn

[U103] JS：定时器
来源：http://bu.shtwfgs.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ed.jctech888.com.cn

[U104] JS：防抖
来源：http://qf.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nf.panjiajie.cn

[U105] JS：节流
来源：http://ok.jianghongdianzi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ur.hahajie.cn

[U106] JS：日期格式化
来源：http://jn.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://je.szsharing.cn

[U107] JS：数字千分位
来源：http://uo.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ki.shxzukj.cn

[U108] JS：随机整数
来源：http://nn.szsharing.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pe.haigaiapp.cn

[U109] JS：数组分组
来源：http://ip.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://ly.nicolike.cn

[U110] JS：数组分块
来源：http://jh.hahajie.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ke.haigaiapp.cn

[U111] JS：对象转 Map
来源：http://nr.lnxyls.cn

new Map(Object.entries(obj))
来源：http://rg.521024.cn

[U112] JS：字符串补位
来源：http://aq.chemitech.net.cn

"7".padStart(3, "0")
来源：http://hx.hnjuh.cn

[U113] JS：正则替换全部
来源：http://av.yuntaijiaju.cn

s.replaceAll("a", "b")
来源：http://by.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://fg.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://mm.bookmarksfly.cn

[U115] JS：生成 UUID
来源：http://xp.521024.cn

crypto.randomUUID()
来源：http://tk.jctech888.com.cn

[U116] JS：类型检查（JSDoc）
来源：http://zs.colortex.cn

/** @param {string} name */ function f(name) {}
来源：http://lw.wgjwhj.cn

[U117] JS：单元测试
来源：http://ce.chemitech.net.cn

npm i -D vitest;  npx vitest
来源：http://vr.lnxyls.cn

[U118] JS：开发服务器
来源：http://vx.asd995.cn

npm i -D vite;  npx vite
来源：http://nu.shxzukj.cn

[U119] JS：生产构建
来源：http://ql.bookmarksfly.cn

npx vite build
来源：http://pp.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://ar.hahajie.cn

import.meta.env.VITE_API_URL
来源：http://jw.haigaiapp.cn

================================================================================
来源：http://hh.yuntaijiaju.cn

统计汇总
来源：http://xt.chemitech.net.cn

================================================================================
来源：http://wf.bookmarksfly.cn

按语言统计（条）：
来源：http://ip.yuntaijiaju.cn

Python ......... 252
来源：http://wp.chemitech.net.cn

PHP ............ 252
来源：http://pr.nicolike.cn

JavaScript ..... 252
来源：http://jd.newstarts.cn

TypeScript ..... 212
来源：http://ih.gzmigu.cn

Java ........... 212
来源：http://gu.shxzskj.cn

Go ............. 212
来源：http://ca.shxzskj.cn

Ruby ........... 212
来源：http://ch.bookmarksfly.cn

C# ............. 212
来源：http://ey.jianghongdianzi.cn

C .............. 30
来源：http://yr.panjiajie.cn

C++ ............ 30
来源：http://go.huixinmuqiang.cn

SQL ............ 90
来源：http://yt.shxzukj.cn

Bash ........... 80
来源：http://cm.wgjwhj.cn

Kotlin ......... 15
来源：http://pa.haigaiapp.cn

Swift .......... 15
来源：http://cy.colortex.cn

Lua ............ 10
来源：http://al.huixinmuqiang.cn

Perl ........... 10
来源：http://fq.nicolike.cn

Scala .......... 10
来源：http://ap.nszjky.cn

------------------------------------
来源：http://vt.lnxyls.cn

合计 ........... 2106 条
来源：http://qf.521024.cn

按章节统计：
来源：http://br.gzmigu.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gp.bjjhwx.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wj.521024.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ez.wgjwhj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://id.muxihuayi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ov.bookmarksfly.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://gn.bookmarksfly.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://nv.bookmarksfly.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ek.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://vn.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yh.huixiangedu.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xq.hahajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ou.hnjuh.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sw.bookmarksfly.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zx.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://bm.hnjuh.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://df.nicolike.cn

Q SQL 专题                              90
来源：http://xf.wgjwhj.cn

R Bash 专题                             80
来源：http://gl.newstarts.cn

S C / C++ 专题                          60
来源：http://ug.shxzukj.cn

T 其他语言补充                          60
来源：http://uk.nicolike.cn

U 高频实用片段                         120
来源：http://ld.chemitech.net.cn

------------------------------------
来源：http://cl.wgjwhj.cn

合计                                  2106 条
来源：http://nh.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://dg.huixinmuqiang.cn

使用提醒
来源：http://ez.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://vd.panjiajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ow.szsharing.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pa.gzmigu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://eo.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://py.wgjwhj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ls.nicolike.cn

—— 文件结束 ——
来源：http://xc.huixinmuqiang.cn

================================================================================
来源：http://xe.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://mi.521024.cn

Common Programming Examples Cheat Book
来源：http://yj.gzmigu.cn

================================================================================
来源：http://zo.nszjky.cn

【收录内容】
来源：http://is.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xa.chemitech.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yo.521024.cn

SQL · Bash · C · C++
来源：http://sx.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://pe.nszjky.cn

【使用说明】
来源：http://yo.wgjwhj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pj.gzmigu.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yu.shxzskj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yc.bjjhwx.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://yz.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dn.newstarts.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ym.szxytkj.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://kb.shtwfgs.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mu.nicolike.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nz.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uu.nicolike.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nd.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xs.asd995.cn

【文件统计】
来源：http://gf.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cx.nicolike.cn

--------------------------------------------------------------------------------
来源：http://lq.huanxung.cn

目  录
来源：http://ls.nszjky.cn

--------------------------------------------------------------------------------
来源：http://no.bjjhwx.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://vj.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oj.yuexingan06.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tm.hahajie.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://dw.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mk.bjjhwx.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://qf.gzmigu.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uw.haigaiapp.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ed.hahajie.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://sp.521024.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ui.bjjhwx.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://ks.muxihuayi.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wa.muxihuayi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wp.shxzukj.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yp.huixinmuqiang.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ks.chemitech.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://qa.521024.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ib.hahajie.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://hl.szsharing.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hb.shxzukj.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zl.shxzukj.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bx.shxzukj.cn

================================================================================
来源：http://ci.newstarts.cn

A. 基础语法与类型
来源：http://vz.chemitech.net.cn

================================================================================
来源：http://gs.asd995.cn

[A01] Hello World
来源：http://ha.wgjwhj.cn

Py:   print("Hello, World!")
来源：http://as.521024.cn

PHP:  echo "Hello, World!";
来源：http://jf.chemitech.net.cn

JS:   console.log("Hello, World!");
来源：http://vc.wgjwhj.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://rx.nszjky.cn

Java: System.out.println("Hello, World!");
来源：http://kw.521024.cn

Go:   fmt.Println("Hello, World!")
来源：http://rm.jctech888.com.cn

Ruby: puts "Hello, World!"
来源：http://ux.bjjhwx.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jn.chemitech.net.cn

[A02] 变量声明与赋值
来源：http://gf.nicolike.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://gg.yuntaijiaju.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://pk.nszjky.cn

JS:   let name = "Alex"; const age = 20;
来源：http://hq.shxzskj.cn


<!-- 参考信息 -->