代发 wailian999

[U27] Py：异步 HTTP
来源：http://sl.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://ip.gzmigu.cn

[U28] Py：类型别名
来源：http://vb.huixiangedu.cn

UserId = int
来源：http://my.lnxyls.cn

[U29] Py：属性校验
来源：http://fs.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://dg.szxytkj.cn

[U30] Py：数据类
来源：http://sa.muxihuayi.cn

@dataclass(slots=True)
来源：http://vo.gzmigu.cn

[U31] Py：单测
来源：http://dr.jctech888.com.cn

python -m pytest -q
来源：http://tl.9csxet.cn

[U32] Py：代码格式化
来源：http://kx.panjiajie.cn

ruff format . && ruff check --fix .
来源：http://no.shxzukj.cn

[U33] Py：打包发布
来源：http://po.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://tx.wgjwhj.cn

[U34] Py：判断编码
来源：http://hq.jctech888.com.cn

chardet.detect(raw)
来源：http://ru.chemitech.net.cn

[U35] Py：发送邮件
来源：http://tj.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oc.muxihuayi.cn

[U36] Py：定时任务
来源：http://pn.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://ke.huanxung.cn

[U37] Py：读写 Excel
来源：http://df.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kz.huixinmuqiang.cn

[U38] Py：获取脚本所在目录
来源：http://jl.huanxung.cn

Path(__file__).resolve().parent
来源：http://hb.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://fm.hnjuh.cn

sys.stdout.isatty()
来源：http://pe.9csxet.cn

[U40] Py：打印到标准错误
来源：http://tf.huixinmuqiang.cn

print("err", file=sys.stderr)
来源：http://fg.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://jd.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kp.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://ha.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zx.colortex.cn

[U43] PHP：声明命名空间
来源：http://nf.szsharing.cn

namespace App\Http;
来源：http://ee.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://tx.asd995.cn

declare(strict_types=1);
来源：http://pl.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://pq.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://uf.nicolike.cn

[U46] PHP：可空类型
来源：http://kn.shxzukj.cn

?string $name = null
来源：http://rn.bookmarksfly.cn

[U47] PHP：联合类型
来源：http://mj.lnxyls.cn

int|string $id
来源：http://dj.newstarts.cn

[U48] PHP：纯枚举
来源：http://zj.chemitech.net.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pz.bjjhwx.cn

[U49] PHP：只读属性
来源：http://sn.bjjhwx.cn

public readonly string $name
来源：http://nk.wgjwhj.cn

[U50] PHP：构造器属性提升
来源：http://fg.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://cy.panjiajie.cn

[U51] PHP：数组解构
来源：http://ih.yuntaijiaju.cn

[$a, $b] = $arr;
来源：http://bl.nicolike.cn

[U52] PHP：箭头函数
来源：http://ef.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://mi.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://ur.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://rd.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://yq.hnjuh.cn

$obj?->method()
来源：http://qm.jianghongdianzi.cn

[U55] PHP：match 表达式
来源：http://dx.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qg.szsharing.cn

[U56] PHP：命名参数
来源：http://zy.chemitech.net.cn

f(a: 1, b: 2)
来源：http://jv.yuntaijiaju.cn

[U57] PHP：字符串插值
来源：http://zn.nicolike.cn

"值: {$a}"
来源：http://qw.bjjhwx.cn

[U58] PHP：数组三件套
来源：http://df.nicolike.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://om.lnxyls.cn

[U59] PHP：自定义排序
来源：http://vb.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ei.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://gu.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jh.hahajie.cn

[U61] PHP：正则
来源：http://ha.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://el.bjjhwx.cn

[U62] PHP：日期对象
来源：http://oy.hahajie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ph.lnxyls.cn

[U63] PHP：文件读写
来源：http://xq.yuexingan06.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rq.szsharing.cn

[U64] PHP：目录遍历
来源：http://az.hahajie.cn

glob("dir/*.php");  scandir("dir");
来源：http://ft.yuexingan06.cn

[U65] PHP：会话
来源：http://go.colortex.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://td.nicolike.cn

[U66] PHP：设置 Cookie
来源：http://jk.nicolike.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sx.nicolike.cn

[U67] PHP：处理文件上传
来源：http://bd.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zb.huanxung.cn

[U68] PHP：PDO 连接
来源：http://ql.shxzskj.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lk.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://xy.lnxyls.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sc.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://pz.huixiangedu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ru.shxzukj.cn

[U71] PHP：抛出异常
来源：http://sf.huixinmuqiang.cn

throw new RuntimeException("失败", 500);
来源：http://sz.nszjky.cn

[U72] PHP：写错误日志
来源：http://lr.shtwfgs.cn

error_log("失败: " . $e->getMessage());
来源：http://dt.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://vu.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://pj.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://tu.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://at.huixinmuqiang.cn

[U75] PHP：依赖注入
来源：http://yj.9csxet.cn

composer require psr/container
来源：http://mh.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://lj.bookmarksfly.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qx.521024.cn

[U77] PHP：模板渲染
来源：http://aj.shxzskj.cn

composer require twig/twig
来源：http://hf.haigaiapp.cn

[U78] PHP：单元测试
来源：http://bt.yuntaijiaju.cn

composer require --dev phpunit/phpunit
来源：http://sx.9csxet.cn

[U79] PHP：静态分析
来源：http://lg.asd995.cn

composer require --dev phpstan/phpstan
来源：http://bj.haigaiapp.cn

[U80] PHP：代码规范修复
来源：http://se.newstarts.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xs.lnxyls.cn

[U81] JS：初始化项目
来源：http://rr.hahajie.cn

npm init -y;  npm i express
来源：http://fs.lnxyls.cn

[U82] JS：package.json 脚本
来源：http://wp.jctech888.com.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://os.wgjwhj.cn

[U83] JS：ES Module 导入导出
来源：http://ld.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iz.huanxung.cn

[U84] JS：CommonJS 写法
来源：http://tw.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://up.asd995.cn

[U85] JS：可选链
来源：http://jk.huixinmuqiang.cn

a?.b?.c
来源：http://yv.521024.cn

[U86] JS：空值合并
来源：http://gb.panjiajie.cn

a ?? b
来源：http://oo.bookmarksfly.cn

[U87] JS：解构默认值
来源：http://ry.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://sp.lnxyls.cn

[U88] JS：对象展开合并
来源：http://gh.lnxyls.cn

{ ...a, ...b }
来源：http://on.szxytkj.cn

[U89] JS：数组去重
来源：http://hj.jctech888.com.cn

[...new Set(arr)]
来源：http://di.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://pe.szxytkj.cn

[...arr].sort((a, b) => a - b)
来源：http://ga.szxytkj.cn

[U91] JS：对象键值遍历
来源：http://xn.yuntaijiaju.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://kl.haigaiapp.cn

[U92] JS：深拷贝
来源：http://mc.huixinmuqiang.cn

structuredClone(obj)
来源：http://nf.haigaiapp.cn

[U93] JS：模板字符串
来源：http://sj.newstarts.cn

`共 ${n} 条`
来源：http://xe.huixiangedu.cn

[U94] JS：箭头函数
来源：http://se.hahajie.cn

const double = x => x * 2;
来源：http://hx.muxihuayi.cn

[U95] JS：Promise 包装
来源：http://uf.nszjky.cn

new Promise((resolve, reject) => {})
来源：http://pm.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://id.nicolike.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cq.shxzukj.cn

[U97] JS：并发请求
来源：http://za.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://id.bjjhwx.cn

[U98] JS：fetch 带 JSON
来源：http://el.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://yv.chemitech.net.cn

[U99] JS：事件监听
来源：http://mi.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://qd.panjiajie.cn

[U100] JS：DOM 查询
来源：http://yl.asd995.cn

document.querySelector(".item")
来源：http://ye.9csxet.cn

[U101] JS：classList 操作
来源：http://nu.jctech888.com.cn

el.classList.toggle("active")
来源：http://cy.521024.cn

[U102] JS：本地存储
来源：http://pe.wgjwhj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://bz.hnjuh.cn

[U103] JS：定时器
来源：http://wd.bjjhwx.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://lv.huixiangedu.cn

[U104] JS：防抖
来源：http://li.huixiangedu.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lk.yuexingan06.cn

[U105] JS：节流
来源：http://rh.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://uf.huixiangedu.cn

[U106] JS：日期格式化
来源：http://za.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://vv.muxihuayi.cn

[U107] JS：数字千分位
来源：http://yh.hnjuh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://qh.jianghongdianzi.cn

[U108] JS：随机整数
来源：http://mh.szxytkj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://xc.huixiangedu.cn

[U109] JS：数组分组
来源：http://pt.hnjuh.cn

Object.groupBy(arr, x => x.type)
来源：http://xi.nicolike.cn

[U110] JS：数组分块
来源：http://uc.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://hs.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://qq.hahajie.cn

new Map(Object.entries(obj))
来源：http://kj.colortex.cn

[U112] JS：字符串补位
来源：http://ln.asd995.cn

"7".padStart(3, "0")
来源：http://fm.shtwfgs.cn

[U113] JS：正则替换全部
来源：http://va.panjiajie.cn

s.replaceAll("a", "b")
来源：http://sh.gzmigu.cn

[U114] JS：JSON 深比较
来源：http://uk.newstarts.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bn.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://fc.chemitech.net.cn

crypto.randomUUID()
来源：http://oa.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://yb.szsharing.cn

/** @param {string} name */ function f(name) {}
来源：http://na.haigaiapp.cn

[U117] JS：单元测试
来源：http://xk.newstarts.cn

npm i -D vitest;  npx vitest
来源：http://dv.yuntaijiaju.cn

[U118] JS：开发服务器
来源：http://am.hahajie.cn

npm i -D vite;  npx vite
来源：http://xi.lnxyls.cn

[U119] JS：生产构建
来源：http://qu.yuntaijiaju.cn

npx vite build
来源：http://tj.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://sj.haigaiapp.cn

import.meta.env.VITE_API_URL
来源：http://ak.gzmigu.cn

================================================================================
来源：http://jz.shtwfgs.cn

统计汇总
来源：http://ua.asd995.cn

================================================================================
来源：http://bg.newstarts.cn

按语言统计（条）：
来源：http://kx.yuntaijiaju.cn

Python ......... 252
来源：http://us.9csxet.cn

PHP ............ 252
来源：http://xs.shxzskj.cn

JavaScript ..... 252
来源：http://vg.bookmarksfly.cn

TypeScript ..... 212
来源：http://cm.colortex.cn

Java ........... 212
来源：http://er.newstarts.cn

Go ............. 212
来源：http://ji.colortex.cn

Ruby ........... 212
来源：http://tc.yuexingan06.cn

C# ............. 212
来源：http://ak.nszjky.cn

C .............. 30
来源：http://gg.9csxet.cn

C++ ............ 30
来源：http://uf.chemitech.net.cn

SQL ............ 90
来源：http://ir.asd995.cn

Bash ........... 80
来源：http://zr.yuexingan06.cn

Kotlin ......... 15
来源：http://xk.szxytkj.cn

Swift .......... 15
来源：http://vy.chemitech.net.cn

Lua ............ 10
来源：http://ua.nszjky.cn

Perl ........... 10
来源：http://bq.9csxet.cn

Scala .......... 10
来源：http://eu.wgjwhj.cn

------------------------------------
来源：http://zp.gzmigu.cn

合计 ........... 2106 条
来源：http://an.huanxung.cn

按章节统计：
来源：http://xg.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://my.muxihuayi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wk.huanxung.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ek.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gh.shtwfgs.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://dx.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://le.jianghongdianzi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://tc.9csxet.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://rb.szsharing.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xo.huanxung.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://av.yuexingan06.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://yx.jianghongdianzi.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://xv.newstarts.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://eb.jianghongdianzi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hy.huixiangedu.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ip.jianghongdianzi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xe.huixinmuqiang.cn

Q SQL 专题                              90
来源：http://dh.shxzukj.cn

R Bash 专题                             80
来源：http://uu.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://uk.521024.cn

T 其他语言补充                          60
来源：http://ea.hnjuh.cn

U 高频实用片段                         120
来源：http://bl.jctech888.com.cn

------------------------------------
来源：http://bx.gzmigu.cn

合计                                  2106 条
来源：http://ao.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ya.gzmigu.cn

使用提醒
来源：http://nw.huixinmuqiang.cn

--------------------------------------------------------------------------------
来源：http://kr.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zz.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://sp.nszjky.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://zd.gzmigu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ip.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zq.huixinmuqiang.cn

—— 文件结束 ——
来源：http://ak.shtwfgs.cn

================================================================================
来源：http://wl.yuexingan06.cn

程序语言常见例子速查手册（2024 版）
来源：http://sg.shxzukj.cn

Common Programming Examples Cheat Book
来源：http://ej.newstarts.cn

================================================================================
来源：http://kj.huanxung.cn

【收录内容】
来源：http://xr.jctech888.com.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kw.hnjuh.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ci.colortex.cn

SQL · Bash · C · C++
来源：http://zf.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wk.newstarts.cn

【使用说明】
来源：http://qs.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://it.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ws.haigaiapp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://me.colortex.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://jt.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ge.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://gd.muxihuayi.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://oe.gzmigu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://si.hnjuh.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pa.nszjky.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xg.szxytkj.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jb.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vb.haigaiapp.cn

【文件统计】
来源：http://jv.shxzskj.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rn.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://ne.nicolike.cn

目  录
来源：http://uk.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://em.colortex.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lv.gzmigu.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://oo.wgjwhj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gn.haigaiapp.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xs.haigaiapp.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://te.shtwfgs.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://li.szxytkj.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://my.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://cj.jianghongdianzi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://rj.newstarts.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fx.szxytkj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://sf.newstarts.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://go.9csxet.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nf.9csxet.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yh.521024.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jw.huixinmuqiang.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://zx.szxytkj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://fn.muxihuayi.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://bs.9csxet.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://hc.muxihuayi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cf.bookmarksfly.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://lp.yuexingan06.cn

================================================================================
来源：http://gr.huixinmuqiang.cn

A. 基础语法与类型
来源：http://oq.nicolike.cn

================================================================================
来源：http://ib.yuexingan06.cn

[A01] Hello World
来源：http://ed.haigaiapp.cn

Py:   print("Hello, World!")
来源：http://wc.asd995.cn

PHP:  echo "Hello, World!";
来源：http://wq.bookmarksfly.cn

JS:   console.log("Hello, World!");
来源：http://jm.yuexingan06.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wb.huanxung.cn


<!-- 参考信息 -->