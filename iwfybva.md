代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://uh.colortex.cn

@contextlib.contextmanager
来源：http://wi.gzmigu.cn

[U22] Py：矩阵转置
来源：http://mp.nicolike.cn

list(zip(*m))
来源：http://vk.jianghongdianzi.cn

[U23] Py：分块读取大文件
来源：http://el.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mu.shtwfgs.cn

[U24] Py：路径操作
来源：http://kx.szsharing.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rv.szsharing.cn

[U25] Py：CSV 按字典读
来源：http://la.yuntaijiaju.cn

csv.DictReader(f)
来源：http://jl.yuexingan06.cn

[U26] Py：并发下载
来源：http://to.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ok.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://mw.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://gy.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://rd.chemitech.net.cn

UserId = int
来源：http://sh.gzmigu.cn

[U29] Py：属性校验
来源：http://og.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://xk.szxytkj.cn

[U30] Py：数据类
来源：http://hv.jctech888.com.cn

@dataclass(slots=True)
来源：http://dd.chemitech.net.cn

[U31] Py：单测
来源：http://lt.lnxyls.cn

python -m pytest -q
来源：http://tl.shxzukj.cn

[U32] Py：代码格式化
来源：http://va.colortex.cn

ruff format . && ruff check --fix .
来源：http://sl.hahajie.cn

[U33] Py：打包发布
来源：http://lc.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://kk.haigaiapp.cn

[U34] Py：判断编码
来源：http://ty.huanxung.cn

chardet.detect(raw)
来源：http://ff.bjjhwx.cn

[U35] Py：发送邮件
来源：http://tf.huixiangedu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://in.9csxet.cn

[U36] Py：定时任务
来源：http://nu.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://rw.asd995.cn

[U37] Py：读写 Excel
来源：http://mq.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ao.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://qq.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://sb.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://bn.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://wf.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://ab.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://rz.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://cv.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tp.huixiangedu.cn

[U42] PHP：PSR-4 自动加载
来源：http://gt.szsharing.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rc.nicolike.cn

[U43] PHP：声明命名空间
来源：http://zp.haigaiapp.cn

namespace App\Http;
来源：http://yg.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://zy.lnxyls.cn

declare(strict_types=1);
来源：http://py.521024.cn

[U45] PHP：类型声明与返回类型
来源：http://ar.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://nk.wgjwhj.cn

[U46] PHP：可空类型
来源：http://dx.chemitech.net.cn

?string $name = null
来源：http://tk.asd995.cn

[U47] PHP：联合类型
来源：http://uw.yuexingan06.cn

int|string $id
来源：http://mu.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://ev.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zl.jctech888.com.cn

[U49] PHP：只读属性
来源：http://ci.hahajie.cn

public readonly string $name
来源：http://gs.haigaiapp.cn

[U50] PHP：构造器属性提升
来源：http://uy.szsharing.cn

public function __construct(private int $id) {}
来源：http://qo.asd995.cn

[U51] PHP：数组解构
来源：http://mf.chemitech.net.cn

[$a, $b] = $arr;
来源：http://qy.lnxyls.cn

[U52] PHP：箭头函数
来源：http://jg.521024.cn

$double = fn($x) => $x * 2;
来源：http://hv.huanxung.cn

[U53] PHP：空合并运算符
来源：http://ao.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://sx.shtwfgs.cn

[U54] PHP：空安全调用
来源：http://ba.nszjky.cn

$obj?->method()
来源：http://ip.9csxet.cn

[U55] PHP：match 表达式
来源：http://bm.shxzukj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bv.shxzukj.cn

[U56] PHP：命名参数
来源：http://dq.nicolike.cn

f(a: 1, b: 2)
来源：http://pt.haigaiapp.cn

[U57] PHP：字符串插值
来源：http://uo.521024.cn

"值: {$a}"
来源：http://pl.jianghongdianzi.cn

[U58] PHP：数组三件套
来源：http://rq.9csxet.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://jb.9csxet.cn

[U59] PHP：自定义排序
来源：http://lf.yuexingan06.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ec.szxytkj.cn

[U60] PHP：JSON 编解码
来源：http://tf.9csxet.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://is.muxihuayi.cn

[U61] PHP：正则
来源：http://dd.shxzskj.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hu.newstarts.cn

[U62] PHP：日期对象
来源：http://lv.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://qp.wgjwhj.cn

[U63] PHP：文件读写
来源：http://ve.newstarts.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ca.521024.cn

[U64] PHP：目录遍历
来源：http://ni.szsharing.cn

glob("dir/*.php");  scandir("dir");
来源：http://do.asd995.cn

[U65] PHP：会话
来源：http://sm.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wg.szxytkj.cn

[U66] PHP：设置 Cookie
来源：http://wk.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wk.asd995.cn

[U67] PHP：处理文件上传
来源：http://dv.shtwfgs.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dl.bookmarksfly.cn

[U68] PHP：PDO 连接
来源：http://xt.gzmigu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://uj.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://mi.colortex.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ai.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://uh.yuexingan06.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://el.hahajie.cn

[U71] PHP：抛出异常
来源：http://gx.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://ix.newstarts.cn

[U72] PHP：写错误日志
来源：http://xs.huixinmuqiang.cn

error_log("失败: " . $e->getMessage());
来源：http://nf.yuexingan06.cn

[U73] PHP：读取 ini 配置
来源：http://gp.gzmigu.cn

parse_ini_file("config.ini", true)
来源：http://zc.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://zs.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://yn.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://vn.521024.cn

composer require psr/container
来源：http://ud.hahajie.cn

[U76] PHP：简单路由
来源：http://uw.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vz.521024.cn

[U77] PHP：模板渲染
来源：http://te.hnjuh.cn

composer require twig/twig
来源：http://ml.521024.cn

[U78] PHP：单元测试
来源：http://wl.huanxung.cn

composer require --dev phpunit/phpunit
来源：http://nk.shtwfgs.cn

[U79] PHP：静态分析
来源：http://ap.9csxet.cn

composer require --dev phpstan/phpstan
来源：http://df.newstarts.cn

[U80] PHP：代码规范修复
来源：http://wq.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://xz.jctech888.com.cn

[U81] JS：初始化项目
来源：http://kb.muxihuayi.cn

npm init -y;  npm i express
来源：http://of.colortex.cn

[U82] JS：package.json 脚本
来源：http://ia.asd995.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vd.jianghongdianzi.cn

[U83] JS：ES Module 导入导出
来源：http://gi.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ja.jctech888.com.cn

[U84] JS：CommonJS 写法
来源：http://jj.lnxyls.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yq.nicolike.cn

[U85] JS：可选链
来源：http://pf.szsharing.cn

a?.b?.c
来源：http://ui.colortex.cn

[U86] JS：空值合并
来源：http://rt.lnxyls.cn

a ?? b
来源：http://ql.newstarts.cn

[U87] JS：解构默认值
来源：http://kt.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://va.gzmigu.cn

[U88] JS：对象展开合并
来源：http://um.bookmarksfly.cn

{ ...a, ...b }
来源：http://vp.panjiajie.cn

[U89] JS：数组去重
来源：http://yh.muxihuayi.cn

[...new Set(arr)]
来源：http://ce.wgjwhj.cn

[U90] JS：数字数组排序
来源：http://ty.jianghongdianzi.cn

[...arr].sort((a, b) => a - b)
来源：http://qb.jctech888.com.cn

[U91] JS：对象键值遍历
来源：http://og.huixiangedu.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bu.huanxung.cn

[U92] JS：深拷贝
来源：http://ei.nszjky.cn

structuredClone(obj)
来源：http://kg.hnjuh.cn

[U93] JS：模板字符串
来源：http://vg.huixinmuqiang.cn

`共 ${n} 条`
来源：http://lx.hnjuh.cn

[U94] JS：箭头函数
来源：http://aj.yuntaijiaju.cn

const double = x => x * 2;
来源：http://zk.nszjky.cn

[U95] JS：Promise 包装
来源：http://eh.wgjwhj.cn

new Promise((resolve, reject) => {})
来源：http://xr.haigaiapp.cn

[U96] JS：async/await 与异常
来源：http://mk.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gd.muxihuayi.cn

[U97] JS：并发请求
来源：http://mp.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://az.colortex.cn

[U98] JS：fetch 带 JSON
来源：http://tb.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wc.hahajie.cn

[U99] JS：事件监听
来源：http://ne.yuntaijiaju.cn

el.addEventListener("click", e => {})
来源：http://ju.9csxet.cn

[U100] JS：DOM 查询
来源：http://ea.huixiangedu.cn

document.querySelector(".item")
来源：http://wc.haigaiapp.cn

[U101] JS：classList 操作
来源：http://pq.nicolike.cn

el.classList.toggle("active")
来源：http://eh.haigaiapp.cn

[U102] JS：本地存储
来源：http://ef.hnjuh.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://er.asd995.cn

[U103] JS：定时器
来源：http://of.haigaiapp.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kc.huixiangedu.cn

[U104] JS：防抖
来源：http://ry.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mq.jctech888.com.cn

[U105] JS：节流
来源：http://jl.shtwfgs.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iq.jctech888.com.cn

[U106] JS：日期格式化
来源：http://mr.9csxet.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qu.huanxung.cn

[U107] JS：数字千分位
来源：http://tb.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://km.nicolike.cn

[U108] JS：随机整数
来源：http://up.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://aq.shtwfgs.cn

[U109] JS：数组分组
来源：http://cn.gzmigu.cn

Object.groupBy(arr, x => x.type)
来源：http://uv.9csxet.cn

[U110] JS：数组分块
来源：http://tg.bjjhwx.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sz.9csxet.cn

[U111] JS：对象转 Map
来源：http://dl.chemitech.net.cn

new Map(Object.entries(obj))
来源：http://hl.chemitech.net.cn

[U112] JS：字符串补位
来源：http://ww.shxzskj.cn

"7".padStart(3, "0")
来源：http://dt.jianghongdianzi.cn

[U113] JS：正则替换全部
来源：http://qc.gzmigu.cn

s.replaceAll("a", "b")
来源：http://mb.bookmarksfly.cn

[U114] JS：JSON 深比较
来源：http://zd.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://gu.9csxet.cn

[U115] JS：生成 UUID
来源：http://cy.yuntaijiaju.cn

crypto.randomUUID()
来源：http://sz.bjjhwx.cn

[U116] JS：类型检查（JSDoc）
来源：http://vq.bookmarksfly.cn

/** @param {string} name */ function f(name) {}
来源：http://ov.huixiangedu.cn

[U117] JS：单元测试
来源：http://vb.muxihuayi.cn

npm i -D vitest;  npx vitest
来源：http://xh.lnxyls.cn

[U118] JS：开发服务器
来源：http://gp.shxzukj.cn

npm i -D vite;  npx vite
来源：http://vn.szxytkj.cn

[U119] JS：生产构建
来源：http://vi.jianghongdianzi.cn

npx vite build
来源：http://ce.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://uo.9csxet.cn

import.meta.env.VITE_API_URL
来源：http://vb.chemitech.net.cn

================================================================================
来源：http://tz.chemitech.net.cn

统计汇总
来源：http://rd.szxytkj.cn

================================================================================
来源：http://jw.yuntaijiaju.cn

按语言统计（条）：
来源：http://zb.muxihuayi.cn

Python ......... 252
来源：http://fd.hnjuh.cn

PHP ............ 252
来源：http://xd.shxzskj.cn

JavaScript ..... 252
来源：http://fa.jctech888.com.cn

TypeScript ..... 212
来源：http://vi.nszjky.cn

Java ........... 212
来源：http://ld.panjiajie.cn

Go ............. 212
来源：http://oq.yuexingan06.cn

Ruby ........... 212
来源：http://au.lnxyls.cn

C# ............. 212
来源：http://dw.newstarts.cn

C .............. 30
来源：http://aq.nszjky.cn

C++ ............ 30
来源：http://be.huixiangedu.cn

SQL ............ 90
来源：http://ro.jctech888.com.cn

Bash ........... 80
来源：http://zu.lnxyls.cn

Kotlin ......... 15
来源：http://yh.bjjhwx.cn

Swift .......... 15
来源：http://qd.panjiajie.cn

Lua ............ 10
来源：http://wr.jianghongdianzi.cn

Perl ........... 10
来源：http://sb.shxzskj.cn

Scala .......... 10
来源：http://ik.gzmigu.cn

------------------------------------
来源：http://rt.szsharing.cn

合计 ........... 2106 条
来源：http://mo.newstarts.cn

按章节统计：
来源：http://hp.hnjuh.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://qp.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mt.panjiajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://dr.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://dc.huanxung.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ml.huixiangedu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tw.521024.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://td.huixinmuqiang.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://sh.yuexingan06.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://sz.newstarts.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://li.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jl.newstarts.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://uu.shtwfgs.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fr.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://eh.nszjky.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://xv.lnxyls.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://qx.hahajie.cn

Q SQL 专题                              90
来源：http://yn.haigaiapp.cn

R Bash 专题                             80
来源：http://kx.newstarts.cn

S C / C++ 专题                          60
来源：http://vw.nszjky.cn

T 其他语言补充                          60
来源：http://sd.huanxung.cn

U 高频实用片段                         120
来源：http://ph.panjiajie.cn

------------------------------------
来源：http://nj.shxzskj.cn

合计                                  2106 条
来源：http://ov.szxytkj.cn

--------------------------------------------------------------------------------
来源：http://rl.hahajie.cn

使用提醒
来源：http://mb.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://zv.jianghongdianzi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pb.huanxung.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dn.bookmarksfly.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cs.bookmarksfly.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://xa.yuexingan06.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://tx.shxzskj.cn

—— 文件结束 ——
来源：http://hg.szxytkj.cn

================================================================================
来源：http://hq.asd995.cn

程序语言常见例子速查手册（2024 版）
来源：http://wz.muxihuayi.cn

Common Programming Examples Cheat Book
来源：http://xk.haigaiapp.cn

================================================================================
来源：http://jm.hnjuh.cn

【收录内容】
来源：http://dq.jianghongdianzi.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://yw.huixinmuqiang.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://oj.wgjwhj.cn

SQL · Bash · C · C++
来源：http://cz.yuntaijiaju.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cx.shtwfgs.cn

【使用说明】
来源：http://pl.szxytkj.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lh.jctech888.com.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ui.9csxet.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://eo.huixinmuqiang.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://xo.shxzukj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ub.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://qk.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wi.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://hx.wgjwhj.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://tq.bjjhwx.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://sm.haigaiapp.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://se.9csxet.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fw.huixinmuqiang.cn

【文件统计】
来源：http://cg.9csxet.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rq.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://tx.bjjhwx.cn

目  录
来源：http://ga.yuntaijiaju.cn

--------------------------------------------------------------------------------
来源：http://ky.hahajie.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://az.bjjhwx.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ty.shxzukj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ng.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hq.521024.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://db.lnxyls.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://nv.haigaiapp.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rx.bookmarksfly.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lr.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fb.asd995.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dd.shxzukj.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://pm.nszjky.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://lb.asd995.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://tp.yuexingan06.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://vm.asd995.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://xc.colortex.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ry.huixinmuqiang.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://sn.gzmigu.cn


<!-- 参考信息 -->