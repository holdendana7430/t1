代发 wailian999

[U15] Py：高精度计时
来源：http://li.lnxyls.cn

t = time.perf_counter()
来源：http://sz.szsharing.cn

[U16] Py：命令行参数解析
来源：http://fj.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yu.colortex.cn

[U17] Py：初始化日志
来源：http://fe.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://ye.chemitech.net.cn

[U18] Py：预编译正则
来源：http://hw.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://cg.asd995.cn

[U19] Py：正则替换带回调
来源：http://xs.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rn.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://ar.muxihuayi.cn

@functools.lru_cache(maxsize=None)
来源：http://up.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://uw.nicolike.cn

@contextlib.contextmanager
来源：http://ub.shxzukj.cn

[U22] Py：矩阵转置
来源：http://js.yuexingan06.cn

list(zip(*m))
来源：http://yk.521024.cn

[U23] Py：分块读取大文件
来源：http://hd.nszjky.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ls.nicolike.cn

[U24] Py：路径操作
来源：http://gw.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qx.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://tt.bookmarksfly.cn

csv.DictReader(f)
来源：http://gz.haigaiapp.cn

[U26] Py：并发下载
来源：http://dp.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ya.lnxyls.cn

[U27] Py：异步 HTTP
来源：http://fy.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://ve.haigaiapp.cn

[U28] Py：类型别名
来源：http://bp.yuntaijiaju.cn

UserId = int
来源：http://pd.colortex.cn

[U29] Py：属性校验
来源：http://ko.hnjuh.cn

@property 与 @x.setter 配合
来源：http://zs.gzmigu.cn

[U30] Py：数据类
来源：http://gc.lnxyls.cn

@dataclass(slots=True)
来源：http://gk.panjiajie.cn

[U31] Py：单测
来源：http://gk.jctech888.com.cn

python -m pytest -q
来源：http://vd.szxytkj.cn

[U32] Py：代码格式化
来源：http://yt.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://fc.colortex.cn

[U33] Py：打包发布
来源：http://bz.huanxung.cn

python -m build  （依赖 pyproject.toml）
来源：http://yn.asd995.cn

[U34] Py：判断编码
来源：http://hd.muxihuayi.cn

chardet.detect(raw)
来源：http://uy.huixiangedu.cn

[U35] Py：发送邮件
来源：http://kk.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mz.haigaiapp.cn

[U36] Py：定时任务
来源：http://tr.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://fg.szsharing.cn

[U37] Py：读写 Excel
来源：http://hq.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ct.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://zv.asd995.cn

Path(__file__).resolve().parent
来源：http://hh.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://zp.shtwfgs.cn

sys.stdout.isatty()
来源：http://is.wgjwhj.cn

[U40] Py：打印到标准错误
来源：http://zn.lnxyls.cn

print("err", file=sys.stderr)
来源：http://iq.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://ka.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cd.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://bl.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://iv.colortex.cn

[U43] PHP：声明命名空间
来源：http://fn.huixinmuqiang.cn

namespace App\Http;
来源：http://vj.wgjwhj.cn

[U44] PHP：开启严格类型
来源：http://do.bjjhwx.cn

declare(strict_types=1);
来源：http://cx.gzmigu.cn

[U45] PHP：类型声明与返回类型
来源：http://zx.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jf.hnjuh.cn

[U46] PHP：可空类型
来源：http://ii.jctech888.com.cn

?string $name = null
来源：http://at.shtwfgs.cn

[U47] PHP：联合类型
来源：http://zu.muxihuayi.cn

int|string $id
来源：http://pr.newstarts.cn

[U48] PHP：纯枚举
来源：http://aj.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yb.panjiajie.cn

[U49] PHP：只读属性
来源：http://lv.shxzskj.cn

public readonly string $name
来源：http://hq.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://po.newstarts.cn

public function __construct(private int $id) {}
来源：http://eu.szxytkj.cn

[U51] PHP：数组解构
来源：http://xx.huixinmuqiang.cn

[$a, $b] = $arr;
来源：http://pf.shxzskj.cn

[U52] PHP：箭头函数
来源：http://gp.colortex.cn

$double = fn($x) => $x * 2;
来源：http://vx.gzmigu.cn

[U53] PHP：空合并运算符
来源：http://vd.huixiangedu.cn

$v = $a ?? $b ?? "default";
来源：http://us.jianghongdianzi.cn

[U54] PHP：空安全调用
来源：http://mf.yuexingan06.cn

$obj?->method()
来源：http://ja.muxihuayi.cn

[U55] PHP：match 表达式
来源：http://fa.huixinmuqiang.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pi.panjiajie.cn

[U56] PHP：命名参数
来源：http://gj.lnxyls.cn

f(a: 1, b: 2)
来源：http://de.521024.cn

[U57] PHP：字符串插值
来源：http://gj.wgjwhj.cn

"值: {$a}"
来源：http://vu.shtwfgs.cn

[U58] PHP：数组三件套
来源：http://ak.szxytkj.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zg.huanxung.cn

[U59] PHP：自定义排序
来源：http://yb.chemitech.net.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wu.nicolike.cn

[U60] PHP：JSON 编解码
来源：http://nq.shtwfgs.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jd.panjiajie.cn

[U61] PHP：正则
来源：http://jw.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uo.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://ny.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wl.bjjhwx.cn

[U63] PHP：文件读写
来源：http://pc.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ji.chemitech.net.cn

[U64] PHP：目录遍历
来源：http://dz.yuntaijiaju.cn

glob("dir/*.php");  scandir("dir");
来源：http://rq.huixinmuqiang.cn

[U65] PHP：会话
来源：http://ub.szxytkj.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vv.huixiangedu.cn

[U66] PHP：设置 Cookie
来源：http://nw.shxzskj.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pz.colortex.cn

[U67] PHP：处理文件上传
来源：http://cp.newstarts.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ay.521024.cn

[U68] PHP：PDO 连接
来源：http://tf.jianghongdianzi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xv.wgjwhj.cn

[U69] PHP：PDO 预处理
来源：http://fn.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://au.lnxyls.cn

[U70] PHP：PDO 事务
来源：http://cz.lnxyls.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ub.nszjky.cn

[U71] PHP：抛出异常
来源：http://gh.chemitech.net.cn

throw new RuntimeException("失败", 500);
来源：http://qt.9csxet.cn

[U72] PHP：写错误日志
来源：http://sg.yuntaijiaju.cn

error_log("失败: " . $e->getMessage());
来源：http://yx.szxytkj.cn

[U73] PHP：读取 ini 配置
来源：http://mh.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://po.nicolike.cn

[U74] PHP：读取环境变量
来源：http://lt.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://en.521024.cn

[U75] PHP：依赖注入
来源：http://xh.shtwfgs.cn

composer require psr/container
来源：http://ae.huixiangedu.cn

[U76] PHP：简单路由
来源：http://ef.jctech888.com.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cn.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://mh.panjiajie.cn

composer require twig/twig
来源：http://sy.yuntaijiaju.cn

[U78] PHP：单元测试
来源：http://jl.panjiajie.cn

composer require --dev phpunit/phpunit
来源：http://wx.bjjhwx.cn

[U79] PHP：静态分析
来源：http://kg.shxzukj.cn

composer require --dev phpstan/phpstan
来源：http://fo.huanxung.cn

[U80] PHP：代码规范修复
来源：http://db.szsharing.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://yg.panjiajie.cn

[U81] JS：初始化项目
来源：http://ii.521024.cn

npm init -y;  npm i express
来源：http://ph.nszjky.cn

[U82] JS：package.json 脚本
来源：http://rl.shxzukj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kk.yuntaijiaju.cn

[U83] JS：ES Module 导入导出
来源：http://ti.bookmarksfly.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cz.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://ye.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ol.521024.cn

[U85] JS：可选链
来源：http://fo.muxihuayi.cn

a?.b?.c
来源：http://yg.chemitech.net.cn

[U86] JS：空值合并
来源：http://ir.huanxung.cn

a ?? b
来源：http://rc.huixiangedu.cn

[U87] JS：解构默认值
来源：http://lj.shxzskj.cn

const { a = 1, b = 2 } = obj;
来源：http://fx.muxihuayi.cn

[U88] JS：对象展开合并
来源：http://hn.newstarts.cn

{ ...a, ...b }
来源：http://ly.shtwfgs.cn

[U89] JS：数组去重
来源：http://wp.szxytkj.cn

[...new Set(arr)]
来源：http://mw.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://sv.chemitech.net.cn

[...arr].sort((a, b) => a - b)
来源：http://ac.huixiangedu.cn

[U91] JS：对象键值遍历
来源：http://ld.newstarts.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://aa.colortex.cn

[U92] JS：深拷贝
来源：http://hv.lnxyls.cn

structuredClone(obj)
来源：http://gs.yuexingan06.cn

[U93] JS：模板字符串
来源：http://pv.muxihuayi.cn

`共 ${n} 条`
来源：http://yd.colortex.cn

[U94] JS：箭头函数
来源：http://ox.jianghongdianzi.cn

const double = x => x * 2;
来源：http://xz.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://cu.hahajie.cn

new Promise((resolve, reject) => {})
来源：http://ag.hahajie.cn

[U96] JS：async/await 与异常
来源：http://ed.bookmarksfly.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mq.shtwfgs.cn

[U97] JS：并发请求
来源：http://lf.jianghongdianzi.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://yo.hahajie.cn

[U98] JS：fetch 带 JSON
来源：http://sf.bjjhwx.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://no.jctech888.com.cn

[U99] JS：事件监听
来源：http://vv.szxytkj.cn

el.addEventListener("click", e => {})
来源：http://xq.nicolike.cn

[U100] JS：DOM 查询
来源：http://tu.colortex.cn

document.querySelector(".item")
来源：http://rt.hahajie.cn

[U101] JS：classList 操作
来源：http://hk.jctech888.com.cn

el.classList.toggle("active")
来源：http://lj.huixinmuqiang.cn

[U102] JS：本地存储
来源：http://qv.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fr.521024.cn

[U103] JS：定时器
来源：http://bo.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wf.colortex.cn

[U104] JS：防抖
来源：http://os.yuexingan06.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lw.newstarts.cn

[U105] JS：节流
来源：http://wh.nicolike.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ke.wgjwhj.cn

[U106] JS：日期格式化
来源：http://dc.wgjwhj.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sl.yuexingan06.cn

[U107] JS：数字千分位
来源：http://ud.bjjhwx.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://je.jctech888.com.cn

[U108] JS：随机整数
来源：http://yq.muxihuayi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kg.nicolike.cn

[U109] JS：数组分组
来源：http://be.bookmarksfly.cn

Object.groupBy(arr, x => x.type)
来源：http://dm.lnxyls.cn

[U110] JS：数组分块
来源：http://ek.newstarts.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wo.lnxyls.cn

[U111] JS：对象转 Map
来源：http://ms.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://hn.521024.cn

[U112] JS：字符串补位
来源：http://lp.yuexingan06.cn

"7".padStart(3, "0")
来源：http://fs.521024.cn

[U113] JS：正则替换全部
来源：http://lh.huanxung.cn

s.replaceAll("a", "b")
来源：http://qz.shtwfgs.cn

[U114] JS：JSON 深比较
来源：http://im.jianghongdianzi.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ix.shtwfgs.cn

[U115] JS：生成 UUID
来源：http://qz.9csxet.cn

crypto.randomUUID()
来源：http://rj.chemitech.net.cn

[U116] JS：类型检查（JSDoc）
来源：http://yo.shxzukj.cn

/** @param {string} name */ function f(name) {}
来源：http://jj.shxzskj.cn

[U117] JS：单元测试
来源：http://sq.huixiangedu.cn

npm i -D vitest;  npx vitest
来源：http://gf.szxytkj.cn

[U118] JS：开发服务器
来源：http://mf.521024.cn

npm i -D vite;  npx vite
来源：http://pg.nicolike.cn

[U119] JS：生产构建
来源：http://ke.newstarts.cn

npx vite build
来源：http://fn.szxytkj.cn

[U120] JS：读取环境变量（Vite）
来源：http://nn.gzmigu.cn

import.meta.env.VITE_API_URL
来源：http://fj.huixiangedu.cn

================================================================================
来源：http://xw.wgjwhj.cn

统计汇总
来源：http://lq.panjiajie.cn

================================================================================
来源：http://ii.hahajie.cn

按语言统计（条）：
来源：http://mg.521024.cn

Python ......... 252
来源：http://td.chemitech.net.cn

PHP ............ 252
来源：http://gw.shxzukj.cn

JavaScript ..... 252
来源：http://mq.chemitech.net.cn

TypeScript ..... 212
来源：http://gx.9csxet.cn

Java ........... 212
来源：http://tt.nicolike.cn

Go ............. 212
来源：http://mg.huixiangedu.cn

Ruby ........... 212
来源：http://ui.newstarts.cn

C# ............. 212
来源：http://ar.hnjuh.cn

C .............. 30
来源：http://ex.asd995.cn

C++ ............ 30
来源：http://ro.nicolike.cn

SQL ............ 90
来源：http://ul.yuexingan06.cn

Bash ........... 80
来源：http://pe.hnjuh.cn

Kotlin ......... 15
来源：http://gt.yuntaijiaju.cn

Swift .......... 15
来源：http://ev.gzmigu.cn

Lua ............ 10
来源：http://vj.hnjuh.cn

Perl ........... 10
来源：http://au.wgjwhj.cn

Scala .......... 10
来源：http://dx.gzmigu.cn

------------------------------------
来源：http://ip.szsharing.cn

合计 ........... 2106 条
来源：http://nl.yuntaijiaju.cn

按章节统计：
来源：http://xd.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wo.shxzukj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://cv.nicolike.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://zb.jianghongdianzi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jn.nicolike.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gv.shtwfgs.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://iw.wgjwhj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uo.bjjhwx.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wk.szxytkj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pi.hahajie.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ct.shxzskj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qm.yuexingan06.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bu.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://va.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://lj.yuexingan06.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ud.muxihuayi.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://nr.panjiajie.cn

Q SQL 专题                              90
来源：http://bc.yuexingan06.cn

R Bash 专题                             80
来源：http://df.hahajie.cn

S C / C++ 专题                          60
来源：http://ys.haigaiapp.cn

T 其他语言补充                          60
来源：http://ow.haigaiapp.cn

U 高频实用片段                         120
来源：http://rp.nicolike.cn

------------------------------------
来源：http://mt.panjiajie.cn

合计                                  2106 条
来源：http://nc.asd995.cn

--------------------------------------------------------------------------------
来源：http://ga.bjjhwx.cn

使用提醒
来源：http://yn.bookmarksfly.cn

--------------------------------------------------------------------------------
来源：http://zi.hnjuh.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fe.haigaiapp.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://tg.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kd.asd995.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://gl.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://nn.huixiangedu.cn

—— 文件结束 ——
来源：http://wh.hahajie.cn

================================================================================
来源：http://pd.hahajie.cn

程序语言常见例子速查手册（2024 版）
来源：http://rf.bookmarksfly.cn

Common Programming Examples Cheat Book
来源：http://ng.szxytkj.cn

================================================================================
来源：http://ws.chemitech.net.cn

【收录内容】
来源：http://if.bookmarksfly.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://mm.521024.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://bn.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://rp.jianghongdianzi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ni.hahajie.cn

【使用说明】
来源：http://vz.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jx.bjjhwx.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://em.newstarts.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://ze.huixiangedu.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ow.nszjky.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://vv.lnxyls.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ja.panjiajie.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://je.huanxung.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://po.bjjhwx.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gc.huixinmuqiang.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://qv.huixiangedu.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://he.szxytkj.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://fs.521024.cn

【文件统计】
来源：http://xr.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kt.asd995.cn

--------------------------------------------------------------------------------
来源：http://bo.gzmigu.cn

目  录
来源：http://va.nicolike.cn

--------------------------------------------------------------------------------
来源：http://bz.shxzskj.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ng.bookmarksfly.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ps.huixinmuqiang.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://vl.jianghongdianzi.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://aa.huixiangedu.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ur.yuntaijiaju.cn


<!-- 参考信息 -->