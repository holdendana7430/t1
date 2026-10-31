代发 wailian999

[U17] Py：初始化日志
来源：http://sg.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://xg.jctech888.com.cn

[U18] Py：预编译正则
来源：http://bm.bjjhwx.cn

pat = re.compile(r"\d+")
来源：http://xj.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://xj.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fb.huanxung.cn

[U20] Py：缓存函数结果
来源：http://eg.yuexingan06.cn

@functools.lru_cache(maxsize=None)
来源：http://ln.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://wu.haigaiapp.cn

@contextlib.contextmanager
来源：http://ir.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://tr.521024.cn

list(zip(*m))
来源：http://ki.newstarts.cn

[U23] Py：分块读取大文件
来源：http://os.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wk.panjiajie.cn

[U24] Py：路径操作
来源：http://bg.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pz.asd995.cn

[U25] Py：CSV 按字典读
来源：http://rw.shxzukj.cn

csv.DictReader(f)
来源：http://ag.huixiangedu.cn

[U26] Py：并发下载
来源：http://sh.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xt.hahajie.cn

[U27] Py：异步 HTTP
来源：http://ok.shtwfgs.cn

aiohttp.ClientSession() 配合 async with
来源：http://is.muxihuayi.cn

[U28] Py：类型别名
来源：http://ft.shtwfgs.cn

UserId = int
来源：http://ny.haigaiapp.cn

[U29] Py：属性校验
来源：http://er.9csxet.cn

@property 与 @x.setter 配合
来源：http://lb.521024.cn

[U30] Py：数据类
来源：http://il.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://qo.lnxyls.cn

[U31] Py：单测
来源：http://kv.asd995.cn

python -m pytest -q
来源：http://gs.nicolike.cn

[U32] Py：代码格式化
来源：http://qh.colortex.cn

ruff format . && ruff check --fix .
来源：http://ht.szsharing.cn

[U33] Py：打包发布
来源：http://ie.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://wn.szxytkj.cn

[U34] Py：判断编码
来源：http://kd.bjjhwx.cn

chardet.detect(raw)
来源：http://gq.huixinmuqiang.cn

[U35] Py：发送邮件
来源：http://rm.9csxet.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cy.jianghongdianzi.cn

[U36] Py：定时任务
来源：http://gr.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://yy.nicolike.cn

[U37] Py：读写 Excel
来源：http://rj.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://cv.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://br.szxytkj.cn

Path(__file__).resolve().parent
来源：http://xz.nszjky.cn

[U39] Py：判断是否在交互环境
来源：http://mo.nszjky.cn

sys.stdout.isatty()
来源：http://fs.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://nu.huanxung.cn

print("err", file=sys.stderr)
来源：http://zo.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://sh.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zn.shtwfgs.cn

[U42] PHP：PSR-4 自动加载
来源：http://sp.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://bb.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://wc.521024.cn

namespace App\Http;
来源：http://gi.shxzukj.cn

[U44] PHP：开启严格类型
来源：http://eg.colortex.cn

declare(strict_types=1);
来源：http://ji.huixiangedu.cn

[U45] PHP：类型声明与返回类型
来源：http://zm.wgjwhj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ak.haigaiapp.cn

[U46] PHP：可空类型
来源：http://xp.bjjhwx.cn

?string $name = null
来源：http://cf.hnjuh.cn

[U47] PHP：联合类型
来源：http://rn.wgjwhj.cn

int|string $id
来源：http://cd.szsharing.cn

[U48] PHP：纯枚举
来源：http://ql.yuntaijiaju.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zc.wgjwhj.cn

[U49] PHP：只读属性
来源：http://md.colortex.cn

public readonly string $name
来源：http://sv.shxzukj.cn

[U50] PHP：构造器属性提升
来源：http://vb.huanxung.cn

public function __construct(private int $id) {}
来源：http://mv.muxihuayi.cn

[U51] PHP：数组解构
来源：http://ek.szxytkj.cn

[$a, $b] = $arr;
来源：http://gg.gzmigu.cn

[U52] PHP：箭头函数
来源：http://uc.jianghongdianzi.cn

$double = fn($x) => $x * 2;
来源：http://bl.szxytkj.cn

[U53] PHP：空合并运算符
来源：http://zo.shxzskj.cn

$v = $a ?? $b ?? "default";
来源：http://ne.asd995.cn

[U54] PHP：空安全调用
来源：http://sg.haigaiapp.cn

$obj?->method()
来源：http://ar.bookmarksfly.cn

[U55] PHP：match 表达式
来源：http://fi.9csxet.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ad.huixiangedu.cn

[U56] PHP：命名参数
来源：http://za.haigaiapp.cn

f(a: 1, b: 2)
来源：http://fb.chemitech.net.cn

[U57] PHP：字符串插值
来源：http://wv.521024.cn

"值: {$a}"
来源：http://io.hnjuh.cn

[U58] PHP：数组三件套
来源：http://ay.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hs.huixinmuqiang.cn

[U59] PHP：自定义排序
来源：http://xj.huixinmuqiang.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mv.muxihuayi.cn

[U60] PHP：JSON 编解码
来源：http://ps.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uv.9csxet.cn

[U61] PHP：正则
来源：http://ku.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kw.yuntaijiaju.cn

[U62] PHP：日期对象
来源：http://ue.huanxung.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kg.hnjuh.cn

[U63] PHP：文件读写
来源：http://fu.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zu.huanxung.cn

[U64] PHP：目录遍历
来源：http://dz.wgjwhj.cn

glob("dir/*.php");  scandir("dir");
来源：http://aa.shtwfgs.cn

[U65] PHP：会话
来源：http://dc.nszjky.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kb.521024.cn

[U66] PHP：设置 Cookie
来源：http://vs.szxytkj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qr.9csxet.cn

[U67] PHP：处理文件上传
来源：http://qg.lnxyls.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pa.nszjky.cn

[U68] PHP：PDO 连接
来源：http://ic.lnxyls.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yo.huixinmuqiang.cn

[U69] PHP：PDO 预处理
来源：http://bs.hahajie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wi.bjjhwx.cn

[U70] PHP：PDO 事务
来源：http://py.nszjky.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://bx.szsharing.cn

[U71] PHP：抛出异常
来源：http://zx.hahajie.cn

throw new RuntimeException("失败", 500);
来源：http://mz.colortex.cn

[U72] PHP：写错误日志
来源：http://jp.shxzskj.cn

error_log("失败: " . $e->getMessage());
来源：http://ys.chemitech.net.cn

[U73] PHP：读取 ini 配置
来源：http://nj.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://yv.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://eg.szxytkj.cn

getenv("APP_ENV") ?: "production"
来源：http://lr.9csxet.cn

[U75] PHP：依赖注入
来源：http://xn.nszjky.cn

composer require psr/container
来源：http://rn.hahajie.cn

[U76] PHP：简单路由
来源：http://aj.521024.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://nf.lnxyls.cn

[U77] PHP：模板渲染
来源：http://ga.newstarts.cn

composer require twig/twig
来源：http://uj.hnjuh.cn

[U78] PHP：单元测试
来源：http://ay.yuexingan06.cn

composer require --dev phpunit/phpunit
来源：http://jy.jctech888.com.cn

[U79] PHP：静态分析
来源：http://rw.bookmarksfly.cn

composer require --dev phpstan/phpstan
来源：http://qh.colortex.cn

[U80] PHP：代码规范修复
来源：http://vb.panjiajie.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://od.gzmigu.cn

[U81] JS：初始化项目
来源：http://st.wgjwhj.cn

npm init -y;  npm i express
来源：http://mv.asd995.cn

[U82] JS：package.json 脚本
来源：http://aa.lnxyls.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ez.haigaiapp.cn

[U83] JS：ES Module 导入导出
来源：http://od.panjiajie.cn

export const a = 1;  import { a } from "./m.js";
来源：http://kf.huixiangedu.cn

[U84] JS：CommonJS 写法
来源：http://ji.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xt.newstarts.cn

[U85] JS：可选链
来源：http://ir.521024.cn

a?.b?.c
来源：http://br.szsharing.cn

[U86] JS：空值合并
来源：http://dx.huixiangedu.cn

a ?? b
来源：http://xb.huixinmuqiang.cn

[U87] JS：解构默认值
来源：http://ij.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://we.521024.cn

[U88] JS：对象展开合并
来源：http://bt.yuexingan06.cn

{ ...a, ...b }
来源：http://gu.panjiajie.cn

[U89] JS：数组去重
来源：http://ob.asd995.cn

[...new Set(arr)]
来源：http://la.hnjuh.cn

[U90] JS：数字数组排序
来源：http://kl.shtwfgs.cn

[...arr].sort((a, b) => a - b)
来源：http://es.yuntaijiaju.cn

[U91] JS：对象键值遍历
来源：http://kq.yuexingan06.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gf.asd995.cn

[U92] JS：深拷贝
来源：http://qm.nszjky.cn

structuredClone(obj)
来源：http://wk.lnxyls.cn

[U93] JS：模板字符串
来源：http://uk.szxytkj.cn

`共 ${n} 条`
来源：http://st.bjjhwx.cn

[U94] JS：箭头函数
来源：http://ep.colortex.cn

const double = x => x * 2;
来源：http://yl.shxzukj.cn

[U95] JS：Promise 包装
来源：http://cj.szsharing.cn

new Promise((resolve, reject) => {})
来源：http://qs.gzmigu.cn

[U96] JS：async/await 与异常
来源：http://ri.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qa.newstarts.cn

[U97] JS：并发请求
来源：http://og.hnjuh.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://to.lnxyls.cn

[U98] JS：fetch 带 JSON
来源：http://sm.shxzskj.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ho.jctech888.com.cn

[U99] JS：事件监听
来源：http://cc.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://ep.jianghongdianzi.cn

[U100] JS：DOM 查询
来源：http://mk.panjiajie.cn

document.querySelector(".item")
来源：http://gi.9csxet.cn

[U101] JS：classList 操作
来源：http://fg.huixiangedu.cn

el.classList.toggle("active")
来源：http://xw.yuntaijiaju.cn

[U102] JS：本地存储
来源：http://om.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fy.panjiajie.cn

[U103] JS：定时器
来源：http://ym.asd995.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vw.yuntaijiaju.cn

[U104] JS：防抖
来源：http://ps.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fc.muxihuayi.cn

[U105] JS：节流
来源：http://dx.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fz.nszjky.cn

[U106] JS：日期格式化
来源：http://mt.asd995.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bz.asd995.cn

[U107] JS：数字千分位
来源：http://ln.shtwfgs.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://ur.nicolike.cn

[U108] JS：随机整数
来源：http://ia.huanxung.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://he.bookmarksfly.cn

[U109] JS：数组分组
来源：http://lg.shtwfgs.cn

Object.groupBy(arr, x => x.type)
来源：http://er.haigaiapp.cn

[U110] JS：数组分块
来源：http://rq.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ji.huixiangedu.cn

[U111] JS：对象转 Map
来源：http://yh.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://ut.bjjhwx.cn

[U112] JS：字符串补位
来源：http://rb.haigaiapp.cn

"7".padStart(3, "0")
来源：http://tk.yuntaijiaju.cn

[U113] JS：正则替换全部
来源：http://fs.wgjwhj.cn

s.replaceAll("a", "b")
来源：http://xc.9csxet.cn

[U114] JS：JSON 深比较
来源：http://sh.shxzskj.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://oj.yuexingan06.cn

[U115] JS：生成 UUID
来源：http://qz.szsharing.cn

crypto.randomUUID()
来源：http://ye.hnjuh.cn

[U116] JS：类型检查（JSDoc）
来源：http://st.9csxet.cn

/** @param {string} name */ function f(name) {}
来源：http://db.9csxet.cn

[U117] JS：单元测试
来源：http://wj.jctech888.com.cn

npm i -D vitest;  npx vitest
来源：http://xw.panjiajie.cn

[U118] JS：开发服务器
来源：http://hx.yuntaijiaju.cn

npm i -D vite;  npx vite
来源：http://yw.asd995.cn

[U119] JS：生产构建
来源：http://og.hahajie.cn

npx vite build
来源：http://in.hnjuh.cn

[U120] JS：读取环境变量（Vite）
来源：http://up.szsharing.cn

import.meta.env.VITE_API_URL
来源：http://ep.muxihuayi.cn

================================================================================
来源：http://id.9csxet.cn

统计汇总
来源：http://mw.yuntaijiaju.cn

================================================================================
来源：http://vl.yuntaijiaju.cn

按语言统计（条）：
来源：http://jc.wgjwhj.cn

Python ......... 252
来源：http://bm.shtwfgs.cn

PHP ............ 252
来源：http://ar.jctech888.com.cn

JavaScript ..... 252
来源：http://oz.shxzukj.cn

TypeScript ..... 212
来源：http://td.gzmigu.cn

Java ........... 212
来源：http://uy.lnxyls.cn

Go ............. 212
来源：http://qt.szsharing.cn

Ruby ........... 212
来源：http://ds.yuexingan06.cn

C# ............. 212
来源：http://qp.9csxet.cn

C .............. 30
来源：http://el.huixiangedu.cn

C++ ............ 30
来源：http://yq.huixiangedu.cn

SQL ............ 90
来源：http://bu.nszjky.cn

Bash ........... 80
来源：http://na.jianghongdianzi.cn

Kotlin ......... 15
来源：http://hx.bookmarksfly.cn

Swift .......... 15
来源：http://oh.bjjhwx.cn

Lua ............ 10
来源：http://tk.yuexingan06.cn

Perl ........... 10
来源：http://id.bookmarksfly.cn

Scala .......... 10
来源：http://uz.lnxyls.cn

------------------------------------
来源：http://le.jctech888.com.cn

合计 ........... 2106 条
来源：http://cc.huanxung.cn

按章节统计：
来源：http://lw.nszjky.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://yi.newstarts.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xn.jianghongdianzi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xf.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://fl.hahajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://fs.shxzukj.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ij.hnjuh.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ns.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tl.nicolike.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://fg.muxihuayi.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yz.huixinmuqiang.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jj.9csxet.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dm.shxzskj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://fi.newstarts.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://xk.jianghongdianzi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ls.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://pt.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://dj.hahajie.cn

R Bash 专题                             80
来源：http://bx.huanxung.cn

S C / C++ 专题                          60
来源：http://gt.gzmigu.cn

T 其他语言补充                          60
来源：http://xp.521024.cn

U 高频实用片段                         120
来源：http://fm.huanxung.cn

------------------------------------
来源：http://ip.jianghongdianzi.cn

合计                                  2106 条
来源：http://ah.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://qd.9csxet.cn

使用提醒
来源：http://zt.colortex.cn

--------------------------------------------------------------------------------
来源：http://ps.muxihuayi.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://rd.shtwfgs.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xu.yuexingan06.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://us.521024.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fi.jianghongdianzi.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ta.colortex.cn

—— 文件结束 ——
来源：http://vc.chemitech.net.cn

================================================================================
来源：http://ec.szxytkj.cn

程序语言常见例子速查手册（2024 版）
来源：http://bh.nicolike.cn

Common Programming Examples Cheat Book
来源：http://qk.nicolike.cn

================================================================================
来源：http://io.hahajie.cn

【收录内容】
来源：http://un.asd995.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://zh.bjjhwx.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://iy.jctech888.com.cn

SQL · Bash · C · C++
来源：http://hc.chemitech.net.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ue.521024.cn

【使用说明】
来源：http://xa.colortex.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://fd.yuexingan06.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://oz.bookmarksfly.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://yr.nicolike.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fq.9csxet.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vm.colortex.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cq.szsharing.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wm.szsharing.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fx.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://pp.wgjwhj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://cl.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mx.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://kf.wgjwhj.cn

【文件统计】
来源：http://pb.shtwfgs.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ui.szsharing.cn

--------------------------------------------------------------------------------
来源：http://hg.panjiajie.cn

目  录
来源：http://wn.colortex.cn

--------------------------------------------------------------------------------
来源：http://rw.huixinmuqiang.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rr.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ay.bjjhwx.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rk.gzmigu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qd.nicolike.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://il.yuexingan06.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://my.bjjhwx.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rp.chemitech.net.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rg.huanxung.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zq.wgjwhj.cn


<!-- 参考信息 -->