代发 wailian999

[U23] Py：分块读取大文件
来源：http://cs.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://be.szxytkj.cn

[U24] Py：路径操作
来源：http://fz.nicolike.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bp.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://oq.nicolike.cn

csv.DictReader(f)
来源：http://gm.szxytkj.cn

[U26] Py：并发下载
来源：http://jw.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ut.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://cb.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://nx.szsharing.cn

[U28] Py：类型别名
来源：http://my.wgjwhj.cn

UserId = int
来源：http://kd.hnjuh.cn

[U29] Py：属性校验
来源：http://hy.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://zw.jianghongdianzi.cn

[U30] Py：数据类
来源：http://za.shtwfgs.cn

@dataclass(slots=True)
来源：http://sj.521024.cn

[U31] Py：单测
来源：http://lv.hnjuh.cn

python -m pytest -q
来源：http://ey.muxihuayi.cn

[U32] Py：代码格式化
来源：http://oe.bookmarksfly.cn

ruff format . && ruff check --fix .
来源：http://fs.yuexingan06.cn

[U33] Py：打包发布
来源：http://zn.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://bz.wgjwhj.cn

[U34] Py：判断编码
来源：http://qv.colortex.cn

chardet.detect(raw)
来源：http://nx.nszjky.cn

[U35] Py：发送邮件
来源：http://ug.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jw.bjjhwx.cn

[U36] Py：定时任务
来源：http://hd.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://pe.huanxung.cn

[U37] Py：读写 Excel
来源：http://us.nicolike.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qn.wgjwhj.cn

[U38] Py：获取脚本所在目录
来源：http://ld.panjiajie.cn

Path(__file__).resolve().parent
来源：http://bb.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://de.newstarts.cn

sys.stdout.isatty()
来源：http://qj.nicolike.cn

[U40] Py：打印到标准错误
来源：http://lc.yuexingan06.cn

print("err", file=sys.stderr)
来源：http://rj.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://lk.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://uu.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://xa.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hm.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://ns.gzmigu.cn

namespace App\Http;
来源：http://vp.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://cp.shtwfgs.cn

declare(strict_types=1);
来源：http://dv.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://rx.huixiangedu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ou.lnxyls.cn

[U46] PHP：可空类型
来源：http://uh.panjiajie.cn

?string $name = null
来源：http://vo.asd995.cn

[U47] PHP：联合类型
来源：http://ks.newstarts.cn

int|string $id
来源：http://es.yuntaijiaju.cn

[U48] PHP：纯枚举
来源：http://xp.lnxyls.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zh.chemitech.net.cn

[U49] PHP：只读属性
来源：http://ln.jianghongdianzi.cn

public readonly string $name
来源：http://kj.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://nv.shxzukj.cn

public function __construct(private int $id) {}
来源：http://ve.yuntaijiaju.cn

[U51] PHP：数组解构
来源：http://cq.lnxyls.cn

[$a, $b] = $arr;
来源：http://df.wgjwhj.cn

[U52] PHP：箭头函数
来源：http://ep.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://wf.shxzskj.cn

[U53] PHP：空合并运算符
来源：http://ik.chemitech.net.cn

$v = $a ?? $b ?? "default";
来源：http://am.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://qq.hnjuh.cn

$obj?->method()
来源：http://vo.huixiangedu.cn

[U55] PHP：match 表达式
来源：http://zz.muxihuayi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://yq.colortex.cn

[U56] PHP：命名参数
来源：http://rw.newstarts.cn

f(a: 1, b: 2)
来源：http://yt.shxzukj.cn

[U57] PHP：字符串插值
来源：http://ao.bookmarksfly.cn

"值: {$a}"
来源：http://rg.haigaiapp.cn

[U58] PHP：数组三件套
来源：http://zm.huixinmuqiang.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fc.yuntaijiaju.cn

[U59] PHP：自定义排序
来源：http://pf.muxihuayi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://do.shxzukj.cn

[U60] PHP：JSON 编解码
来源：http://hg.yuntaijiaju.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qx.huixiangedu.cn

[U61] PHP：正则
来源：http://lp.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aq.hnjuh.cn

[U62] PHP：日期对象
来源：http://jg.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zj.asd995.cn

[U63] PHP：文件读写
来源：http://qq.szsharing.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mp.shtwfgs.cn

[U64] PHP：目录遍历
来源：http://vj.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ie.lnxyls.cn

[U65] PHP：会话
来源：http://gf.muxihuayi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gm.yuntaijiaju.cn

[U66] PHP：设置 Cookie
来源：http://ay.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wp.huixinmuqiang.cn

[U67] PHP：处理文件上传
来源：http://im.huixinmuqiang.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sq.nszjky.cn

[U68] PHP：PDO 连接
来源：http://nn.haigaiapp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lt.521024.cn

[U69] PHP：PDO 预处理
来源：http://hh.szxytkj.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ua.huixiangedu.cn

[U70] PHP：PDO 事务
来源：http://si.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yj.gzmigu.cn

[U71] PHP：抛出异常
来源：http://ef.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://qo.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://xq.gzmigu.cn

error_log("失败: " . $e->getMessage());
来源：http://om.shtwfgs.cn

[U73] PHP：读取 ini 配置
来源：http://vr.nszjky.cn

parse_ini_file("config.ini", true)
来源：http://ne.nszjky.cn

[U74] PHP：读取环境变量
来源：http://wo.panjiajie.cn

getenv("APP_ENV") ?: "production"
来源：http://lw.shxzukj.cn

[U75] PHP：依赖注入
来源：http://jw.colortex.cn

composer require psr/container
来源：http://hp.nicolike.cn

[U76] PHP：简单路由
来源：http://vp.nicolike.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://al.szsharing.cn

[U77] PHP：模板渲染
来源：http://xu.521024.cn

composer require twig/twig
来源：http://db.asd995.cn

[U78] PHP：单元测试
来源：http://rr.wgjwhj.cn

composer require --dev phpunit/phpunit
来源：http://es.yuexingan06.cn

[U79] PHP：静态分析
来源：http://lt.hnjuh.cn

composer require --dev phpstan/phpstan
来源：http://eo.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://ub.nszjky.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fw.shxzskj.cn

[U81] JS：初始化项目
来源：http://bk.muxihuayi.cn

npm init -y;  npm i express
来源：http://kr.colortex.cn

[U82] JS：package.json 脚本
来源：http://em.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zd.huanxung.cn

[U83] JS：ES Module 导入导出
来源：http://ot.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cy.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://tq.521024.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wx.shxzskj.cn

[U85] JS：可选链
来源：http://il.nszjky.cn

a?.b?.c
来源：http://fm.chemitech.net.cn

[U86] JS：空值合并
来源：http://oj.gzmigu.cn

a ?? b
来源：http://gu.huanxung.cn

[U87] JS：解构默认值
来源：http://yf.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://ta.hnjuh.cn

[U88] JS：对象展开合并
来源：http://ce.shtwfgs.cn

{ ...a, ...b }
来源：http://fj.chemitech.net.cn

[U89] JS：数组去重
来源：http://ny.szsharing.cn

[...new Set(arr)]
来源：http://nx.colortex.cn

[U90] JS：数字数组排序
来源：http://cn.521024.cn

[...arr].sort((a, b) => a - b)
来源：http://ny.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://ml.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://sc.chemitech.net.cn

[U92] JS：深拷贝
来源：http://gy.panjiajie.cn

structuredClone(obj)
来源：http://ho.huixinmuqiang.cn

[U93] JS：模板字符串
来源：http://xh.wgjwhj.cn

`共 ${n} 条`
来源：http://dv.jianghongdianzi.cn

[U94] JS：箭头函数
来源：http://bg.haigaiapp.cn

const double = x => x * 2;
来源：http://qq.shxzskj.cn

[U95] JS：Promise 包装
来源：http://dh.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://we.huixinmuqiang.cn

[U96] JS：async/await 与异常
来源：http://lp.chemitech.net.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tn.hahajie.cn

[U97] JS：并发请求
来源：http://qo.huixiangedu.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://pc.shxzskj.cn

[U98] JS：fetch 带 JSON
来源：http://fp.jctech888.com.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dk.huixiangedu.cn

[U99] JS：事件监听
来源：http://yg.9csxet.cn

el.addEventListener("click", e => {})
来源：http://mq.panjiajie.cn

[U100] JS：DOM 查询
来源：http://ex.panjiajie.cn

document.querySelector(".item")
来源：http://qj.gzmigu.cn

[U101] JS：classList 操作
来源：http://jo.huixiangedu.cn

el.classList.toggle("active")
来源：http://bv.bookmarksfly.cn

[U102] JS：本地存储
来源：http://aj.gzmigu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://uj.huanxung.cn

[U103] JS：定时器
来源：http://rj.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://te.bookmarksfly.cn

[U104] JS：防抖
来源：http://pl.nszjky.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gg.gzmigu.cn

[U105] JS：节流
来源：http://zw.huanxung.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ev.bookmarksfly.cn

[U106] JS：日期格式化
来源：http://zf.yuntaijiaju.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://dh.bookmarksfly.cn

[U107] JS：数字千分位
来源：http://oy.shxzukj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://et.shxzukj.cn

[U108] JS：随机整数
来源：http://jf.panjiajie.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://id.wgjwhj.cn

[U109] JS：数组分组
来源：http://iy.huixinmuqiang.cn

Object.groupBy(arr, x => x.type)
来源：http://mn.bookmarksfly.cn

[U110] JS：数组分块
来源：http://sq.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mp.jctech888.com.cn

[U111] JS：对象转 Map
来源：http://kh.shxzskj.cn

new Map(Object.entries(obj))
来源：http://xf.haigaiapp.cn

[U112] JS：字符串补位
来源：http://ti.gzmigu.cn

"7".padStart(3, "0")
来源：http://oa.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://zy.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://vu.colortex.cn

[U114] JS：JSON 深比较
来源：http://qr.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://pj.shxzskj.cn

[U115] JS：生成 UUID
来源：http://ym.shxzukj.cn

crypto.randomUUID()
来源：http://lk.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://kh.haigaiapp.cn

/** @param {string} name */ function f(name) {}
来源：http://ju.szxytkj.cn

[U117] JS：单元测试
来源：http://pk.bjjhwx.cn

npm i -D vitest;  npx vitest
来源：http://qa.wgjwhj.cn

[U118] JS：开发服务器
来源：http://er.szsharing.cn

npm i -D vite;  npx vite
来源：http://ru.szsharing.cn

[U119] JS：生产构建
来源：http://ud.muxihuayi.cn

npx vite build
来源：http://hr.yuexingan06.cn

[U120] JS：读取环境变量（Vite）
来源：http://hq.panjiajie.cn

import.meta.env.VITE_API_URL
来源：http://cw.huixinmuqiang.cn

================================================================================
来源：http://sq.yuntaijiaju.cn

统计汇总
来源：http://ai.asd995.cn

================================================================================
来源：http://og.chemitech.net.cn

按语言统计（条）：
来源：http://sr.lnxyls.cn

Python ......... 252
来源：http://hr.huanxung.cn

PHP ............ 252
来源：http://fe.lnxyls.cn

JavaScript ..... 252
来源：http://qf.huixiangedu.cn

TypeScript ..... 212
来源：http://aq.gzmigu.cn

Java ........... 212
来源：http://wz.chemitech.net.cn

Go ............. 212
来源：http://fr.jctech888.com.cn

Ruby ........... 212
来源：http://hb.bjjhwx.cn

C# ............. 212
来源：http://fe.szsharing.cn

C .............. 30
来源：http://ng.huanxung.cn

C++ ............ 30
来源：http://yy.wgjwhj.cn

SQL ............ 90
来源：http://qn.bjjhwx.cn

Bash ........... 80
来源：http://fv.panjiajie.cn

Kotlin ......... 15
来源：http://ib.nszjky.cn

Swift .......... 15
来源：http://xr.asd995.cn

Lua ............ 10
来源：http://yf.chemitech.net.cn

Perl ........... 10
来源：http://mu.nszjky.cn

Scala .......... 10
来源：http://ej.colortex.cn

------------------------------------
来源：http://pk.newstarts.cn

合计 ........... 2106 条
来源：http://hl.gzmigu.cn

按章节统计：
来源：http://wi.yuntaijiaju.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jz.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ul.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://nv.huanxung.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://nn.jctech888.com.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://jk.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tu.jctech888.com.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://xw.shxzskj.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mp.asd995.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pn.chemitech.net.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nf.muxihuayi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oz.haigaiapp.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pw.jianghongdianzi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ue.szsharing.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://pt.panjiajie.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://er.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://af.muxihuayi.cn

Q SQL 专题                              90
来源：http://dj.huixiangedu.cn

R Bash 专题                             80
来源：http://td.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://ri.huixinmuqiang.cn

T 其他语言补充                          60
来源：http://lu.asd995.cn

U 高频实用片段                         120
来源：http://rh.jctech888.com.cn

------------------------------------
来源：http://ps.muxihuayi.cn

合计                                  2106 条
来源：http://in.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://pl.gzmigu.cn

使用提醒
来源：http://so.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://lq.huixinmuqiang.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zw.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wu.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ja.yuntaijiaju.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fh.huixinmuqiang.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vu.huixiangedu.cn

—— 文件结束 ——
来源：http://qq.hahajie.cn

================================================================================
来源：http://px.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ms.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://tx.bookmarksfly.cn

================================================================================
来源：http://ti.9csxet.cn

【收录内容】
来源：http://nw.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://nt.haigaiapp.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ve.bjjhwx.cn

SQL · Bash · C · C++
来源：http://ih.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dd.lnxyls.cn

【使用说明】
来源：http://la.lnxyls.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xa.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://da.bjjhwx.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kx.haigaiapp.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tz.gzmigu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jj.huanxung.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pp.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://hb.haigaiapp.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tq.nszjky.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://vu.521024.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dg.chemitech.net.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wy.yuexingan06.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://cc.bookmarksfly.cn

【文件统计】
来源：http://tv.521024.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ze.hahajie.cn

--------------------------------------------------------------------------------
来源：http://mz.panjiajie.cn

目  录
来源：http://ic.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://xj.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rx.wgjwhj.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://am.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://fq.colortex.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://jo.hahajie.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://gp.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wv.huixinmuqiang.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dk.huanxung.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hz.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://dt.bjjhwx.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://yz.yuntaijiaju.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fz.panjiajie.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wn.haigaiapp.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://kp.hnjuh.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mq.jianghongdianzi.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://uw.lnxyls.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sx.haigaiapp.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xw.szsharing.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ti.yuntaijiaju.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ul.hnjuh.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zo.yuexingan06.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://in.521024.cn


<!-- 参考信息 -->