代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://ee.hahajie.cn

@contextlib.contextmanager
来源：http://bu.wgjwhj.cn

[U22] Py：矩阵转置
来源：http://tl.bookmarksfly.cn

list(zip(*m))
来源：http://od.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://nt.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xc.gzmigu.cn

[U24] Py：路径操作
来源：http://xx.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fk.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://fv.chemitech.net.cn

csv.DictReader(f)
来源：http://ot.9csxet.cn

[U26] Py：并发下载
来源：http://px.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ih.9csxet.cn

[U27] Py：异步 HTTP
来源：http://qb.gzmigu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ap.muxihuayi.cn

[U28] Py：类型别名
来源：http://bb.bjjhwx.cn

UserId = int
来源：http://rx.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://bu.szsharing.cn

@property 与 @x.setter 配合
来源：http://cl.jctech888.com.cn

[U30] Py：数据类
来源：http://cs.huanxung.cn

@dataclass(slots=True)
来源：http://uh.9csxet.cn

[U31] Py：单测
来源：http://nj.huixinmuqiang.cn

python -m pytest -q
来源：http://qs.yuexingan06.cn

[U32] Py：代码格式化
来源：http://pe.bjjhwx.cn

ruff format . && ruff check --fix .
来源：http://qa.yuexingan06.cn

[U33] Py：打包发布
来源：http://dz.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://fn.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://pi.jctech888.com.cn

chardet.detect(raw)
来源：http://gi.panjiajie.cn

[U35] Py：发送邮件
来源：http://oc.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ig.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://lt.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://jb.nszjky.cn

[U37] Py：读写 Excel
来源：http://zz.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cq.nszjky.cn

[U38] Py：获取脚本所在目录
来源：http://wp.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://ql.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://vj.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://bn.9csxet.cn

[U40] Py：打印到标准错误
来源：http://nz.shxzukj.cn

print("err", file=sys.stderr)
来源：http://te.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://kg.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://pm.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://bp.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://le.nicolike.cn

[U43] PHP：声明命名空间
来源：http://tw.szxytkj.cn

namespace App\Http;
来源：http://oo.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://xt.lnxyls.cn

declare(strict_types=1);
来源：http://rl.panjiajie.cn

[U45] PHP：类型声明与返回类型
来源：http://id.huixinmuqiang.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://on.newstarts.cn

[U46] PHP：可空类型
来源：http://sm.shxzskj.cn

?string $name = null
来源：http://ji.gzmigu.cn

[U47] PHP：联合类型
来源：http://bo.newstarts.cn

int|string $id
来源：http://mi.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://jy.szxytkj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sd.asd995.cn

[U49] PHP：只读属性
来源：http://ns.yuntaijiaju.cn

public readonly string $name
来源：http://kl.szxytkj.cn

[U50] PHP：构造器属性提升
来源：http://tr.shxzukj.cn

public function __construct(private int $id) {}
来源：http://ex.jctech888.com.cn

[U51] PHP：数组解构
来源：http://lc.chemitech.net.cn

[$a, $b] = $arr;
来源：http://rc.szxytkj.cn

[U52] PHP：箭头函数
来源：http://eg.nicolike.cn

$double = fn($x) => $x * 2;
来源：http://qa.yuntaijiaju.cn

[U53] PHP：空合并运算符
来源：http://uq.wgjwhj.cn

$v = $a ?? $b ?? "default";
来源：http://xl.nicolike.cn

[U54] PHP：空安全调用
来源：http://uu.9csxet.cn

$obj?->method()
来源：http://rb.huanxung.cn

[U55] PHP：match 表达式
来源：http://ru.panjiajie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xr.shtwfgs.cn

[U56] PHP：命名参数
来源：http://gl.wgjwhj.cn

f(a: 1, b: 2)
来源：http://kh.gzmigu.cn

[U57] PHP：字符串插值
来源：http://uf.9csxet.cn

"值: {$a}"
来源：http://fu.jctech888.com.cn

[U58] PHP：数组三件套
来源：http://mx.jctech888.com.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dj.jianghongdianzi.cn

[U59] PHP：自定义排序
来源：http://zd.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jf.jianghongdianzi.cn

[U60] PHP：JSON 编解码
来源：http://ri.colortex.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sm.shxzukj.cn

[U61] PHP：正则
来源：http://ty.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://gt.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://zq.jctech888.com.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://hw.szsharing.cn

[U63] PHP：文件读写
来源：http://jc.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://af.shxzukj.cn

[U64] PHP：目录遍历
来源：http://yp.huanxung.cn

glob("dir/*.php");  scandir("dir");
来源：http://tr.colortex.cn

[U65] PHP：会话
来源：http://tw.huixinmuqiang.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://gh.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://lu.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vk.szxytkj.cn

[U67] PHP：处理文件上传
来源：http://je.yuexingan06.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pz.yuexingan06.cn

[U68] PHP：PDO 连接
来源：http://zd.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hm.nszjky.cn

[U69] PHP：PDO 预处理
来源：http://vn.chemitech.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://sz.huanxung.cn

[U70] PHP：PDO 事务
来源：http://tc.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ty.newstarts.cn

[U71] PHP：抛出异常
来源：http://df.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://ew.lnxyls.cn

[U72] PHP：写错误日志
来源：http://nk.colortex.cn

error_log("失败: " . $e->getMessage());
来源：http://zm.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://bk.colortex.cn

parse_ini_file("config.ini", true)
来源：http://ex.panjiajie.cn

[U74] PHP：读取环境变量
来源：http://ju.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ka.colortex.cn

[U75] PHP：依赖注入
来源：http://pl.newstarts.cn

composer require psr/container
来源：http://sw.huanxung.cn

[U76] PHP：简单路由
来源：http://hs.yuexingan06.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qw.lnxyls.cn

[U77] PHP：模板渲染
来源：http://hd.521024.cn

composer require twig/twig
来源：http://bu.shxzukj.cn

[U78] PHP：单元测试
来源：http://ci.nszjky.cn

composer require --dev phpunit/phpunit
来源：http://jh.nicolike.cn

[U79] PHP：静态分析
来源：http://kc.nszjky.cn

composer require --dev phpstan/phpstan
来源：http://yi.bjjhwx.cn

[U80] PHP：代码规范修复
来源：http://dp.jctech888.com.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jy.yuexingan06.cn

[U81] JS：初始化项目
来源：http://uo.szxytkj.cn

npm init -y;  npm i express
来源：http://fq.hahajie.cn

[U82] JS：package.json 脚本
来源：http://oo.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pa.shtwfgs.cn

[U83] JS：ES Module 导入导出
来源：http://uh.nicolike.cn

export const a = 1;  import { a } from "./m.js";
来源：http://az.haigaiapp.cn

[U84] JS：CommonJS 写法
来源：http://xm.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://mk.bjjhwx.cn

[U85] JS：可选链
来源：http://ya.9csxet.cn

a?.b?.c
来源：http://cl.szsharing.cn

[U86] JS：空值合并
来源：http://un.huanxung.cn

a ?? b
来源：http://vi.9csxet.cn

[U87] JS：解构默认值
来源：http://eq.yuntaijiaju.cn

const { a = 1, b = 2 } = obj;
来源：http://vb.521024.cn

[U88] JS：对象展开合并
来源：http://gv.haigaiapp.cn

{ ...a, ...b }
来源：http://cn.nicolike.cn

[U89] JS：数组去重
来源：http://xs.bjjhwx.cn

[...new Set(arr)]
来源：http://rv.521024.cn

[U90] JS：数字数组排序
来源：http://wd.gzmigu.cn

[...arr].sort((a, b) => a - b)
来源：http://wt.chemitech.net.cn

[U91] JS：对象键值遍历
来源：http://ig.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://tq.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://yk.gzmigu.cn

structuredClone(obj)
来源：http://wd.shtwfgs.cn

[U93] JS：模板字符串
来源：http://zp.wgjwhj.cn

`共 ${n} 条`
来源：http://dm.hnjuh.cn

[U94] JS：箭头函数
来源：http://xq.nszjky.cn

const double = x => x * 2;
来源：http://ae.hnjuh.cn

[U95] JS：Promise 包装
来源：http://ee.szxytkj.cn

new Promise((resolve, reject) => {})
来源：http://xo.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://rt.huanxung.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://bu.asd995.cn

[U97] JS：并发请求
来源：http://iv.panjiajie.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ku.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://ej.asd995.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://oh.huanxung.cn

[U99] JS：事件监听
来源：http://mu.huixinmuqiang.cn

el.addEventListener("click", e => {})
来源：http://sk.hahajie.cn

[U100] JS：DOM 查询
来源：http://wf.gzmigu.cn

document.querySelector(".item")
来源：http://pe.asd995.cn

[U101] JS：classList 操作
来源：http://jm.colortex.cn

el.classList.toggle("active")
来源：http://vv.haigaiapp.cn

[U102] JS：本地存储
来源：http://yu.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zm.shxzskj.cn

[U103] JS：定时器
来源：http://fa.521024.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jd.jianghongdianzi.cn

[U104] JS：防抖
来源：http://eh.shxzukj.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qo.jianghongdianzi.cn

[U105] JS：节流
来源：http://jk.wgjwhj.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ex.szsharing.cn

[U106] JS：日期格式化
来源：http://fs.huixinmuqiang.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fy.hnjuh.cn

[U107] JS：数字千分位
来源：http://qx.haigaiapp.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wv.chemitech.net.cn

[U108] JS：随机整数
来源：http://sz.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://as.szxytkj.cn

[U109] JS：数组分组
来源：http://xq.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://cb.szsharing.cn

[U110] JS：数组分块
来源：http://ex.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://lt.bjjhwx.cn

[U111] JS：对象转 Map
来源：http://dq.jctech888.com.cn

new Map(Object.entries(obj))
来源：http://tq.lnxyls.cn

[U112] JS：字符串补位
来源：http://yp.shtwfgs.cn

"7".padStart(3, "0")
来源：http://se.jctech888.com.cn

[U113] JS：正则替换全部
来源：http://hd.shtwfgs.cn

s.replaceAll("a", "b")
来源：http://fk.huixinmuqiang.cn

[U114] JS：JSON 深比较
来源：http://vy.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ql.huixinmuqiang.cn

[U115] JS：生成 UUID
来源：http://ni.jctech888.com.cn

crypto.randomUUID()
来源：http://cm.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://lr.hnjuh.cn

/** @param {string} name */ function f(name) {}
来源：http://tv.hnjuh.cn

[U117] JS：单元测试
来源：http://nv.nszjky.cn

npm i -D vitest;  npx vitest
来源：http://jd.9csxet.cn

[U118] JS：开发服务器
来源：http://ae.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://tk.szsharing.cn

[U119] JS：生产构建
来源：http://so.huanxung.cn

npx vite build
来源：http://yu.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://rj.wgjwhj.cn

import.meta.env.VITE_API_URL
来源：http://nt.haigaiapp.cn

================================================================================
来源：http://fe.haigaiapp.cn

统计汇总
来源：http://xw.huixiangedu.cn

================================================================================
来源：http://lq.521024.cn

按语言统计（条）：
来源：http://sv.muxihuayi.cn

Python ......... 252
来源：http://mu.yuntaijiaju.cn

PHP ............ 252
来源：http://mr.nszjky.cn

JavaScript ..... 252
来源：http://ly.chemitech.net.cn

TypeScript ..... 212
来源：http://hv.521024.cn

Java ........... 212
来源：http://fg.huixinmuqiang.cn

Go ............. 212
来源：http://oc.gzmigu.cn

Ruby ........... 212
来源：http://yt.nszjky.cn

C# ............. 212
来源：http://ir.szxytkj.cn

C .............. 30
来源：http://cy.9csxet.cn

C++ ............ 30
来源：http://lb.muxihuayi.cn

SQL ............ 90
来源：http://ff.muxihuayi.cn

Bash ........... 80
来源：http://pp.wgjwhj.cn

Kotlin ......... 15
来源：http://jj.colortex.cn

Swift .......... 15
来源：http://zh.szsharing.cn

Lua ............ 10
来源：http://zt.newstarts.cn

Perl ........... 10
来源：http://cy.asd995.cn

Scala .......... 10
来源：http://vl.521024.cn

------------------------------------
来源：http://ew.jctech888.com.cn

合计 ........... 2106 条
来源：http://jo.huanxung.cn

按章节统计：
来源：http://bc.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://xo.panjiajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://su.hahajie.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://va.521024.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ra.jianghongdianzi.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mg.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://vy.huixiangedu.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hu.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lb.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://bt.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wp.szxytkj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jp.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://yn.huanxung.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sz.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lj.yuntaijiaju.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://na.szxytkj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://py.huixiangedu.cn

Q SQL 专题                              90
来源：http://wt.9csxet.cn

R Bash 专题                             80
来源：http://vs.muxihuayi.cn

S C / C++ 专题                          60
来源：http://ln.newstarts.cn

T 其他语言补充                          60
来源：http://mk.shxzskj.cn

U 高频实用片段                         120
来源：http://ks.bookmarksfly.cn

------------------------------------
来源：http://iz.lnxyls.cn

合计                                  2106 条
来源：http://qb.yuexingan06.cn

--------------------------------------------------------------------------------
来源：http://ct.colortex.cn

使用提醒
来源：http://ph.szsharing.cn

--------------------------------------------------------------------------------
来源：http://yt.newstarts.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://if.nicolike.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tm.newstarts.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hv.panjiajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fj.szsharing.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cu.shxzskj.cn

—— 文件结束 ——
来源：http://mf.jctech888.com.cn

================================================================================
来源：http://xh.gzmigu.cn

程序语言常见例子速查手册（2024 版）
来源：http://vp.wgjwhj.cn

Common Programming Examples Cheat Book
来源：http://lk.asd995.cn

================================================================================
来源：http://la.hnjuh.cn

【收录内容】
来源：http://rz.huixinmuqiang.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ut.gzmigu.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://rv.gzmigu.cn

SQL · Bash · C · C++
来源：http://jk.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://dx.szsharing.cn

【使用说明】
来源：http://rj.9csxet.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mm.shxzukj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://ba.521024.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://us.szxytkj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://oc.jianghongdianzi.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jr.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://vh.gzmigu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ix.nicolike.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wx.chemitech.net.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ap.hahajie.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vv.bookmarksfly.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://li.shxzukj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://vf.szsharing.cn

【文件统计】
来源：http://kg.bjjhwx.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qh.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://xz.yuntaijiaju.cn

目  录
来源：http://xd.nicolike.cn

--------------------------------------------------------------------------------
来源：http://jz.newstarts.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fn.yuntaijiaju.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://yj.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kz.huanxung.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nt.nszjky.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://po.huixinmuqiang.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ab.nicolike.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://vt.nszjky.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://av.huixiangedu.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zb.yuexingan06.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ps.szsharing.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://zz.yuexingan06.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bi.521024.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gp.yuntaijiaju.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ke.yuexingan06.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://he.panjiajie.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://fh.wgjwhj.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://td.yuntaijiaju.cn


<!-- 参考信息 -->