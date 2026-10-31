代发 wailian999

[U17] Py：初始化日志
来源：http://bv.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://im.nicolike.cn

[U18] Py：预编译正则
来源：http://uh.szsharing.cn

pat = re.compile(r"\d+")
来源：http://oc.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://rj.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xi.shxzskj.cn

[U20] Py：缓存函数结果
来源：http://jg.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://yc.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://bm.bookmarksfly.cn

@contextlib.contextmanager
来源：http://cv.nicolike.cn

[U22] Py：矩阵转置
来源：http://by.shtwfgs.cn

list(zip(*m))
来源：http://ng.colortex.cn

[U23] Py：分块读取大文件
来源：http://ce.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://en.huixiangedu.cn

[U24] Py：路径操作
来源：http://zn.panjiajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://of.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://hu.hahajie.cn

csv.DictReader(f)
来源：http://nd.jctech888.com.cn

[U26] Py：并发下载
来源：http://kx.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kd.9csxet.cn

[U27] Py：异步 HTTP
来源：http://zv.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qz.szxytkj.cn

[U28] Py：类型别名
来源：http://io.shxzskj.cn

UserId = int
来源：http://oc.shxzukj.cn

[U29] Py：属性校验
来源：http://fa.shxzskj.cn

@property 与 @x.setter 配合
来源：http://qp.muxihuayi.cn

[U30] Py：数据类
来源：http://be.muxihuayi.cn

@dataclass(slots=True)
来源：http://nv.asd995.cn

[U31] Py：单测
来源：http://qq.wgjwhj.cn

python -m pytest -q
来源：http://nb.szxytkj.cn

[U32] Py：代码格式化
来源：http://xx.colortex.cn

ruff format . && ruff check --fix .
来源：http://al.shtwfgs.cn

[U33] Py：打包发布
来源：http://sg.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://gm.huanxung.cn

[U34] Py：判断编码
来源：http://jz.9csxet.cn

chardet.detect(raw)
来源：http://dt.hahajie.cn

[U35] Py：发送邮件
来源：http://yh.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gv.panjiajie.cn

[U36] Py：定时任务
来源：http://qi.shtwfgs.cn

schedule.every(10).minutes.do(job)
来源：http://qs.9csxet.cn

[U37] Py：读写 Excel
来源：http://dd.jianghongdianzi.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tm.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://gq.shxzskj.cn

Path(__file__).resolve().parent
来源：http://td.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://lf.gzmigu.cn

sys.stdout.isatty()
来源：http://eo.shxzskj.cn

[U40] Py：打印到标准错误
来源：http://ok.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://hq.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://sv.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zd.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://oh.chemitech.net.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://he.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://hu.muxihuayi.cn

namespace App\Http;
来源：http://un.jianghongdianzi.cn

[U44] PHP：开启严格类型
来源：http://nl.chemitech.net.cn

declare(strict_types=1);
来源：http://ok.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://rs.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ne.hnjuh.cn

[U46] PHP：可空类型
来源：http://kt.hnjuh.cn

?string $name = null
来源：http://sx.shxzskj.cn

[U47] PHP：联合类型
来源：http://yr.hahajie.cn

int|string $id
来源：http://mc.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://nt.9csxet.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://vr.chemitech.net.cn

[U49] PHP：只读属性
来源：http://hf.muxihuayi.cn

public readonly string $name
来源：http://ul.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://yh.hnjuh.cn

public function __construct(private int $id) {}
来源：http://jp.huanxung.cn

[U51] PHP：数组解构
来源：http://oa.haigaiapp.cn

[$a, $b] = $arr;
来源：http://rb.newstarts.cn

[U52] PHP：箭头函数
来源：http://mc.shxzukj.cn

$double = fn($x) => $x * 2;
来源：http://hq.9csxet.cn

[U53] PHP：空合并运算符
来源：http://pj.jianghongdianzi.cn

$v = $a ?? $b ?? "default";
来源：http://rn.shxzukj.cn

[U54] PHP：空安全调用
来源：http://gh.muxihuayi.cn

$obj?->method()
来源：http://cx.asd995.cn

[U55] PHP：match 表达式
来源：http://cc.jianghongdianzi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pk.haigaiapp.cn

[U56] PHP：命名参数
来源：http://wm.panjiajie.cn

f(a: 1, b: 2)
来源：http://or.nicolike.cn

[U57] PHP：字符串插值
来源：http://yw.shxzskj.cn

"值: {$a}"
来源：http://rr.shxzukj.cn

[U58] PHP：数组三件套
来源：http://bl.jianghongdianzi.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ax.nszjky.cn

[U59] PHP：自定义排序
来源：http://qm.huixiangedu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uf.nszjky.cn

[U60] PHP：JSON 编解码
来源：http://ku.hahajie.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cu.colortex.cn

[U61] PHP：正则
来源：http://ui.huixiangedu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cg.haigaiapp.cn

[U62] PHP：日期对象
来源：http://xb.lnxyls.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pt.hahajie.cn

[U63] PHP：文件读写
来源：http://xo.521024.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bj.jianghongdianzi.cn

[U64] PHP：目录遍历
来源：http://ko.lnxyls.cn

glob("dir/*.php");  scandir("dir");
来源：http://st.panjiajie.cn

[U65] PHP：会话
来源：http://wb.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://mo.hahajie.cn

[U66] PHP：设置 Cookie
来源：http://lw.asd995.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zz.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://hh.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://oq.panjiajie.cn

[U68] PHP：PDO 连接
来源：http://wi.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mr.jctech888.com.cn

[U69] PHP：PDO 预处理
来源：http://dr.muxihuayi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xh.521024.cn

[U70] PHP：PDO 事务
来源：http://ul.hahajie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rs.yuntaijiaju.cn

[U71] PHP：抛出异常
来源：http://kr.shxzskj.cn

throw new RuntimeException("失败", 500);
来源：http://nw.szsharing.cn

[U72] PHP：写错误日志
来源：http://kj.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://kk.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://gu.nicolike.cn

parse_ini_file("config.ini", true)
来源：http://nd.jctech888.com.cn

[U74] PHP：读取环境变量
来源：http://pe.huanxung.cn

getenv("APP_ENV") ?: "production"
来源：http://yl.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://mg.shxzskj.cn

composer require psr/container
来源：http://zy.bookmarksfly.cn

[U76] PHP：简单路由
来源：http://av.bjjhwx.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ep.hnjuh.cn

[U77] PHP：模板渲染
来源：http://oz.hahajie.cn

composer require twig/twig
来源：http://us.nicolike.cn

[U78] PHP：单元测试
来源：http://pl.asd995.cn

composer require --dev phpunit/phpunit
来源：http://zx.szsharing.cn

[U79] PHP：静态分析
来源：http://hx.521024.cn

composer require --dev phpstan/phpstan
来源：http://pp.szxytkj.cn

[U80] PHP：代码规范修复
来源：http://cr.521024.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mg.szxytkj.cn

[U81] JS：初始化项目
来源：http://aa.panjiajie.cn

npm init -y;  npm i express
来源：http://in.muxihuayi.cn

[U82] JS：package.json 脚本
来源：http://cx.haigaiapp.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://yd.lnxyls.cn

[U83] JS：ES Module 导入导出
来源：http://ga.hahajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://jx.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://hf.gzmigu.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pf.lnxyls.cn

[U85] JS：可选链
来源：http://cz.panjiajie.cn

a?.b?.c
来源：http://ke.haigaiapp.cn

[U86] JS：空值合并
来源：http://zu.panjiajie.cn

a ?? b
来源：http://ri.521024.cn

[U87] JS：解构默认值
来源：http://sz.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://za.hnjuh.cn

[U88] JS：对象展开合并
来源：http://jt.chemitech.net.cn

{ ...a, ...b }
来源：http://yu.gzmigu.cn

[U89] JS：数组去重
来源：http://yx.bjjhwx.cn

[...new Set(arr)]
来源：http://gx.haigaiapp.cn

[U90] JS：数字数组排序
来源：http://mc.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://do.shtwfgs.cn

[U91] JS：对象键值遍历
来源：http://nh.521024.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wf.jianghongdianzi.cn

[U92] JS：深拷贝
来源：http://zp.bookmarksfly.cn

structuredClone(obj)
来源：http://kf.shtwfgs.cn

[U93] JS：模板字符串
来源：http://ua.colortex.cn

`共 ${n} 条`
来源：http://ev.wgjwhj.cn

[U94] JS：箭头函数
来源：http://pt.bookmarksfly.cn

const double = x => x * 2;
来源：http://oc.newstarts.cn

[U95] JS：Promise 包装
来源：http://yh.shtwfgs.cn

new Promise((resolve, reject) => {})
来源：http://jz.szsharing.cn

[U96] JS：async/await 与异常
来源：http://gw.lnxyls.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://zv.yuntaijiaju.cn

[U97] JS：并发请求
来源：http://vp.nicolike.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://uh.huanxung.cn

[U98] JS：fetch 带 JSON
来源：http://jy.szxytkj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vi.asd995.cn

[U99] JS：事件监听
来源：http://zl.haigaiapp.cn

el.addEventListener("click", e => {})
来源：http://rr.yuexingan06.cn

[U100] JS：DOM 查询
来源：http://nz.colortex.cn

document.querySelector(".item")
来源：http://yc.yuexingan06.cn

[U101] JS：classList 操作
来源：http://to.nszjky.cn

el.classList.toggle("active")
来源：http://sk.huixiangedu.cn

[U102] JS：本地存储
来源：http://ih.huixiangedu.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dy.hnjuh.cn

[U103] JS：定时器
来源：http://st.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://of.lnxyls.cn

[U104] JS：防抖
来源：http://zh.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nb.shxzukj.cn

[U105] JS：节流
来源：http://tw.521024.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vr.panjiajie.cn

[U106] JS：日期格式化
来源：http://ae.shxzskj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ju.yuntaijiaju.cn

[U107] JS：数字千分位
来源：http://fx.asd995.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yg.muxihuayi.cn

[U108] JS：随机整数
来源：http://im.shtwfgs.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kw.hahajie.cn

[U109] JS：数组分组
来源：http://yg.521024.cn

Object.groupBy(arr, x => x.type)
来源：http://pz.muxihuayi.cn

[U110] JS：数组分块
来源：http://kg.9csxet.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wk.bookmarksfly.cn

[U111] JS：对象转 Map
来源：http://wa.szsharing.cn

new Map(Object.entries(obj))
来源：http://sa.nicolike.cn

[U112] JS：字符串补位
来源：http://fv.szsharing.cn

"7".padStart(3, "0")
来源：http://ni.haigaiapp.cn

[U113] JS：正则替换全部
来源：http://ak.nicolike.cn

s.replaceAll("a", "b")
来源：http://vx.huanxung.cn

[U114] JS：JSON 深比较
来源：http://lh.szsharing.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://om.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://jj.asd995.cn

crypto.randomUUID()
来源：http://to.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://sv.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://rd.shxzskj.cn

[U117] JS：单元测试
来源：http://fz.asd995.cn

npm i -D vitest;  npx vitest
来源：http://oy.shxzskj.cn

[U118] JS：开发服务器
来源：http://tj.shxzskj.cn

npm i -D vite;  npx vite
来源：http://ix.asd995.cn

[U119] JS：生产构建
来源：http://bx.shtwfgs.cn

npx vite build
来源：http://uj.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://ok.yuexingan06.cn

import.meta.env.VITE_API_URL
来源：http://wz.9csxet.cn

================================================================================
来源：http://wx.haigaiapp.cn

统计汇总
来源：http://uu.lnxyls.cn

================================================================================
来源：http://dn.chemitech.net.cn

按语言统计（条）：
来源：http://lr.jianghongdianzi.cn

Python ......... 252
来源：http://gt.newstarts.cn

PHP ............ 252
来源：http://wj.wgjwhj.cn

JavaScript ..... 252
来源：http://hc.haigaiapp.cn

TypeScript ..... 212
来源：http://xf.9csxet.cn

Java ........... 212
来源：http://hl.chemitech.net.cn

Go ............. 212
来源：http://cg.hahajie.cn

Ruby ........... 212
来源：http://oy.lnxyls.cn

C# ............. 212
来源：http://xh.yuexingan06.cn

C .............. 30
来源：http://rq.gzmigu.cn

C++ ............ 30
来源：http://jo.panjiajie.cn

SQL ............ 90
来源：http://dr.colortex.cn

Bash ........... 80
来源：http://fd.9csxet.cn

Kotlin ......... 15
来源：http://eg.haigaiapp.cn

Swift .......... 15
来源：http://dr.bookmarksfly.cn

Lua ............ 10
来源：http://as.gzmigu.cn

Perl ........... 10
来源：http://dy.wgjwhj.cn

Scala .......... 10
来源：http://yn.jianghongdianzi.cn

------------------------------------
来源：http://cq.jctech888.com.cn

合计 ........... 2106 条
来源：http://rr.yuntaijiaju.cn

按章节统计：
来源：http://uf.yuexingan06.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ry.jctech888.com.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vr.haigaiapp.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://pl.newstarts.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ky.bookmarksfly.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mi.huanxung.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ty.asd995.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qt.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xo.panjiajie.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://qu.huixiangedu.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dl.nicolike.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ft.szxytkj.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hs.yuexingan06.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zx.huanxung.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uv.lnxyls.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fo.9csxet.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xs.colortex.cn

Q SQL 专题                              90
来源：http://cl.nicolike.cn

R Bash 专题                             80
来源：http://tc.shxzskj.cn

S C / C++ 专题                          60
来源：http://ev.hahajie.cn

T 其他语言补充                          60
来源：http://cq.hahajie.cn

U 高频实用片段                         120
来源：http://tq.jctech888.com.cn

------------------------------------
来源：http://jo.yuntaijiaju.cn

合计                                  2106 条
来源：http://tg.muxihuayi.cn

--------------------------------------------------------------------------------
来源：http://pu.shxzukj.cn

使用提醒
来源：http://nw.haigaiapp.cn

--------------------------------------------------------------------------------
来源：http://ia.shxzukj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tf.huixiangedu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://dc.asd995.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ah.wgjwhj.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bj.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://os.yuexingan06.cn

—— 文件结束 ——
来源：http://rd.yuntaijiaju.cn

================================================================================
来源：http://lw.bookmarksfly.cn

程序语言常见例子速查手册（2024 版）
来源：http://nq.szxytkj.cn

Common Programming Examples Cheat Book
来源：http://sh.panjiajie.cn

================================================================================
来源：http://iw.bjjhwx.cn

【收录内容】
来源：http://ym.nszjky.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://td.shtwfgs.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ij.bjjhwx.cn

SQL · Bash · C · C++
来源：http://ec.shtwfgs.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mn.colortex.cn

【使用说明】
来源：http://xr.nicolike.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://rr.bookmarksfly.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://xq.colortex.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iz.shtwfgs.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://vl.huanxung.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ho.wgjwhj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xd.521024.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://dg.shxzukj.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nc.gzmigu.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hq.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://aj.bjjhwx.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gx.huixinmuqiang.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ft.hnjuh.cn

【文件统计】
来源：http://jf.gzmigu.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://zn.hahajie.cn

--------------------------------------------------------------------------------
来源：http://ot.huanxung.cn

目  录
来源：http://zm.wgjwhj.cn

--------------------------------------------------------------------------------
来源：http://if.hnjuh.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gy.newstarts.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://fm.shxzskj.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rj.bjjhwx.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://vd.hnjuh.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ed.yuntaijiaju.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aj.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ew.hahajie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ks.asd995.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zp.newstarts.cn


<!-- 参考信息 -->