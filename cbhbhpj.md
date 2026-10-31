代发 wailian999

[U13] Py：固定长度队列
来源：http://tl.yuexingan06.cn

deque(maxlen=10)
来源：http://ca.newstarts.cn

[U14] Py：分组收集到列表
来源：http://dr.521024.cn

defaultdict(list)
来源：http://vl.521024.cn

[U15] Py：高精度计时
来源：http://ca.shtwfgs.cn

t = time.perf_counter()
来源：http://cs.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://xt.bookmarksfly.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://el.asd995.cn

[U17] Py：初始化日志
来源：http://fh.muxihuayi.cn

logging.basicConfig(level=logging.INFO)
来源：http://wn.asd995.cn

[U18] Py：预编译正则
来源：http://as.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://mb.bjjhwx.cn

[U19] Py：正则替换带回调
来源：http://ov.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xr.asd995.cn

[U20] Py：缓存函数结果
来源：http://ea.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://rg.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://rr.haigaiapp.cn

@contextlib.contextmanager
来源：http://bw.yuexingan06.cn

[U22] Py：矩阵转置
来源：http://sj.bookmarksfly.cn

list(zip(*m))
来源：http://ii.panjiajie.cn

[U23] Py：分块读取大文件
来源：http://jc.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jf.chemitech.net.cn

[U24] Py：路径操作
来源：http://wx.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gm.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://ve.gzmigu.cn

csv.DictReader(f)
来源：http://bz.wgjwhj.cn

[U26] Py：并发下载
来源：http://kk.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gq.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://fs.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://dp.shtwfgs.cn

[U28] Py：类型别名
来源：http://mq.szxytkj.cn

UserId = int
来源：http://ic.hnjuh.cn

[U29] Py：属性校验
来源：http://zu.nszjky.cn

@property 与 @x.setter 配合
来源：http://nk.colortex.cn

[U30] Py：数据类
来源：http://lo.shtwfgs.cn

@dataclass(slots=True)
来源：http://qx.panjiajie.cn

[U31] Py：单测
来源：http://je.yuexingan06.cn

python -m pytest -q
来源：http://ao.jctech888.com.cn

[U32] Py：代码格式化
来源：http://tk.hahajie.cn

ruff format . && ruff check --fix .
来源：http://il.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://zg.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ru.muxihuayi.cn

[U34] Py：判断编码
来源：http://bu.shxzskj.cn

chardet.detect(raw)
来源：http://ww.colortex.cn

[U35] Py：发送邮件
来源：http://ir.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bx.chemitech.net.cn

[U36] Py：定时任务
来源：http://pi.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://eb.shxzskj.cn

[U37] Py：读写 Excel
来源：http://ao.huanxung.cn

pandas.read_excel / DataFrame.to_excel
来源：http://he.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://vw.yuexingan06.cn

Path(__file__).resolve().parent
来源：http://hd.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://mh.huixiangedu.cn

sys.stdout.isatty()
来源：http://dt.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://in.bookmarksfly.cn

print("err", file=sys.stderr)
来源：http://kw.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://hv.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ny.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://vk.shxzskj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xk.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://nz.szxytkj.cn

namespace App\Http;
来源：http://kb.nszjky.cn

[U44] PHP：开启严格类型
来源：http://kt.huixiangedu.cn

declare(strict_types=1);
来源：http://fp.haigaiapp.cn

[U45] PHP：类型声明与返回类型
来源：http://kg.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ce.yuntaijiaju.cn

[U46] PHP：可空类型
来源：http://tz.huixinmuqiang.cn

?string $name = null
来源：http://dm.chemitech.net.cn

[U47] PHP：联合类型
来源：http://ch.bookmarksfly.cn

int|string $id
来源：http://og.huanxung.cn

[U48] PHP：纯枚举
来源：http://zq.haigaiapp.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gr.9csxet.cn

[U49] PHP：只读属性
来源：http://yg.yuexingan06.cn

public readonly string $name
来源：http://ed.colortex.cn

[U50] PHP：构造器属性提升
来源：http://cb.panjiajie.cn

public function __construct(private int $id) {}
来源：http://sl.gzmigu.cn

[U51] PHP：数组解构
来源：http://pu.nicolike.cn

[$a, $b] = $arr;
来源：http://bq.hnjuh.cn

[U52] PHP：箭头函数
来源：http://ua.bookmarksfly.cn

$double = fn($x) => $x * 2;
来源：http://em.yuexingan06.cn

[U53] PHP：空合并运算符
来源：http://bz.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://bd.huixinmuqiang.cn

[U54] PHP：空安全调用
来源：http://ps.bjjhwx.cn

$obj?->method()
来源：http://cr.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://nb.bookmarksfly.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ey.chemitech.net.cn

[U56] PHP：命名参数
来源：http://ca.521024.cn

f(a: 1, b: 2)
来源：http://cl.huixiangedu.cn

[U57] PHP：字符串插值
来源：http://vf.9csxet.cn

"值: {$a}"
来源：http://ux.hahajie.cn

[U58] PHP：数组三件套
来源：http://nv.huixiangedu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://dg.haigaiapp.cn

[U59] PHP：自定义排序
来源：http://nl.haigaiapp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ic.huixinmuqiang.cn

[U60] PHP：JSON 编解码
来源：http://uf.huixinmuqiang.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ly.jianghongdianzi.cn

[U61] PHP：正则
来源：http://mr.yuntaijiaju.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://sp.bookmarksfly.cn

[U62] PHP：日期对象
来源：http://ro.bjjhwx.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://bl.huanxung.cn

[U63] PHP：文件读写
来源：http://ov.jianghongdianzi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xn.huanxung.cn

[U64] PHP：目录遍历
来源：http://xd.muxihuayi.cn

glob("dir/*.php");  scandir("dir");
来源：http://tj.chemitech.net.cn

[U65] PHP：会话
来源：http://dv.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jp.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://ax.szsharing.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ur.asd995.cn

[U67] PHP：处理文件上传
来源：http://oq.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jy.9csxet.cn

[U68] PHP：PDO 连接
来源：http://nz.521024.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://di.szsharing.cn

[U69] PHP：PDO 预处理
来源：http://yu.huanxung.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qr.nszjky.cn

[U70] PHP：PDO 事务
来源：http://cl.huixinmuqiang.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tk.wgjwhj.cn

[U71] PHP：抛出异常
来源：http://gx.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://zr.haigaiapp.cn

[U72] PHP：写错误日志
来源：http://jr.bjjhwx.cn

error_log("失败: " . $e->getMessage());
来源：http://xj.jctech888.com.cn

[U73] PHP：读取 ini 配置
来源：http://wj.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://ro.hnjuh.cn

[U74] PHP：读取环境变量
来源：http://jm.chemitech.net.cn

getenv("APP_ENV") ?: "production"
来源：http://ic.9csxet.cn

[U75] PHP：依赖注入
来源：http://qp.chemitech.net.cn

composer require psr/container
来源：http://vu.huixiangedu.cn

[U76] PHP：简单路由
来源：http://gm.newstarts.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gg.shtwfgs.cn

[U77] PHP：模板渲染
来源：http://ms.szsharing.cn

composer require twig/twig
来源：http://in.bookmarksfly.cn

[U78] PHP：单元测试
来源：http://pe.gzmigu.cn

composer require --dev phpunit/phpunit
来源：http://bf.nicolike.cn

[U79] PHP：静态分析
来源：http://ov.shxzskj.cn

composer require --dev phpstan/phpstan
来源：http://ms.muxihuayi.cn

[U80] PHP：代码规范修复
来源：http://go.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://qt.9csxet.cn

[U81] JS：初始化项目
来源：http://fz.muxihuayi.cn

npm init -y;  npm i express
来源：http://sa.newstarts.cn

[U82] JS：package.json 脚本
来源：http://fh.huixiangedu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://oo.muxihuayi.cn

[U83] JS：ES Module 导入导出
来源：http://mg.wgjwhj.cn

export const a = 1;  import { a } from "./m.js";
来源：http://cm.yuntaijiaju.cn

[U84] JS：CommonJS 写法
来源：http://ce.wgjwhj.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ma.521024.cn

[U85] JS：可选链
来源：http://xo.521024.cn

a?.b?.c
来源：http://iw.shxzskj.cn

[U86] JS：空值合并
来源：http://ut.huixinmuqiang.cn

a ?? b
来源：http://gx.asd995.cn

[U87] JS：解构默认值
来源：http://nm.521024.cn

const { a = 1, b = 2 } = obj;
来源：http://ao.521024.cn

[U88] JS：对象展开合并
来源：http://be.bjjhwx.cn

{ ...a, ...b }
来源：http://xb.shxzukj.cn

[U89] JS：数组去重
来源：http://nz.huixinmuqiang.cn

[...new Set(arr)]
来源：http://an.huixinmuqiang.cn

[U90] JS：数字数组排序
来源：http://gy.hahajie.cn

[...arr].sort((a, b) => a - b)
来源：http://vp.wgjwhj.cn

[U91] JS：对象键值遍历
来源：http://jj.asd995.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wa.jctech888.com.cn

[U92] JS：深拷贝
来源：http://ak.haigaiapp.cn

structuredClone(obj)
来源：http://na.521024.cn

[U93] JS：模板字符串
来源：http://of.haigaiapp.cn

`共 ${n} 条`
来源：http://oi.muxihuayi.cn

[U94] JS：箭头函数
来源：http://mv.wgjwhj.cn

const double = x => x * 2;
来源：http://sh.bookmarksfly.cn

[U95] JS：Promise 包装
来源：http://by.panjiajie.cn

new Promise((resolve, reject) => {})
来源：http://zd.shxzskj.cn

[U96] JS：async/await 与异常
来源：http://bk.asd995.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xj.521024.cn

[U97] JS：并发请求
来源：http://pt.chemitech.net.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hb.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://cz.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://pg.chemitech.net.cn

[U99] JS：事件监听
来源：http://pj.jianghongdianzi.cn

el.addEventListener("click", e => {})
来源：http://io.muxihuayi.cn

[U100] JS：DOM 查询
来源：http://rj.newstarts.cn

document.querySelector(".item")
来源：http://qr.shtwfgs.cn

[U101] JS：classList 操作
来源：http://cy.newstarts.cn

el.classList.toggle("active")
来源：http://vc.shtwfgs.cn

[U102] JS：本地存储
来源：http://hs.521024.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ku.szsharing.cn

[U103] JS：定时器
来源：http://hi.muxihuayi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://fk.hnjuh.cn

[U104] JS：防抖
来源：http://my.haigaiapp.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ud.bjjhwx.cn

[U105] JS：节流
来源：http://kt.hahajie.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ao.yuexingan06.cn

[U106] JS：日期格式化
来源：http://nv.yuexingan06.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rp.9csxet.cn

[U107] JS：数字千分位
来源：http://nl.muxihuayi.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dq.chemitech.net.cn

[U108] JS：随机整数
来源：http://nt.yuexingan06.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://na.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://ul.nicolike.cn

Object.groupBy(arr, x => x.type)
来源：http://xz.shxzukj.cn

[U110] JS：数组分块
来源：http://ll.jianghongdianzi.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iw.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://ss.shtwfgs.cn

new Map(Object.entries(obj))
来源：http://ey.nicolike.cn

[U112] JS：字符串补位
来源：http://lm.szxytkj.cn

"7".padStart(3, "0")
来源：http://kg.huixinmuqiang.cn

[U113] JS：正则替换全部
来源：http://tr.colortex.cn

s.replaceAll("a", "b")
来源：http://ry.haigaiapp.cn

[U114] JS：JSON 深比较
来源：http://yz.lnxyls.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lw.huanxung.cn

[U115] JS：生成 UUID
来源：http://jd.gzmigu.cn

crypto.randomUUID()
来源：http://yn.521024.cn

[U116] JS：类型检查（JSDoc）
来源：http://yz.lnxyls.cn

/** @param {string} name */ function f(name) {}
来源：http://jb.gzmigu.cn

[U117] JS：单元测试
来源：http://bz.gzmigu.cn

npm i -D vitest;  npx vitest
来源：http://gk.chemitech.net.cn

[U118] JS：开发服务器
来源：http://zz.hnjuh.cn

npm i -D vite;  npx vite
来源：http://ym.521024.cn

[U119] JS：生产构建
来源：http://hu.huixinmuqiang.cn

npx vite build
来源：http://tu.huanxung.cn

[U120] JS：读取环境变量（Vite）
来源：http://li.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://es.bjjhwx.cn

================================================================================
来源：http://cb.hahajie.cn

统计汇总
来源：http://xt.nszjky.cn

================================================================================
来源：http://xe.haigaiapp.cn

按语言统计（条）：
来源：http://mu.lnxyls.cn

Python ......... 252
来源：http://km.hahajie.cn

PHP ............ 252
来源：http://yh.bjjhwx.cn

JavaScript ..... 252
来源：http://vn.huixinmuqiang.cn

TypeScript ..... 212
来源：http://oa.haigaiapp.cn

Java ........... 212
来源：http://ra.bjjhwx.cn

Go ............. 212
来源：http://rq.nszjky.cn

Ruby ........... 212
来源：http://uo.jctech888.com.cn

C# ............. 212
来源：http://be.panjiajie.cn

C .............. 30
来源：http://zm.jianghongdianzi.cn

C++ ............ 30
来源：http://mi.bookmarksfly.cn

SQL ............ 90
来源：http://wf.huixinmuqiang.cn

Bash ........... 80
来源：http://dv.huanxung.cn

Kotlin ......... 15
来源：http://ui.bookmarksfly.cn

Swift .......... 15
来源：http://bg.jianghongdianzi.cn

Lua ............ 10
来源：http://ao.hnjuh.cn

Perl ........... 10
来源：http://by.panjiajie.cn

Scala .......... 10
来源：http://hx.gzmigu.cn

------------------------------------
来源：http://mf.nicolike.cn

合计 ........... 2106 条
来源：http://om.panjiajie.cn

按章节统计：
来源：http://fb.hahajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://za.shtwfgs.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ig.jctech888.com.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cq.haigaiapp.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://jd.nszjky.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lg.asd995.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yl.chemitech.net.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://hb.521024.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://qv.newstarts.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tf.9csxet.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://br.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://qe.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lx.bookmarksfly.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://we.chemitech.net.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mh.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zk.chemitech.net.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://yt.9csxet.cn

Q SQL 专题                              90
来源：http://aq.wgjwhj.cn

R Bash 专题                             80
来源：http://qy.jianghongdianzi.cn

S C / C++ 专题                          60
来源：http://lz.9csxet.cn

T 其他语言补充                          60
来源：http://tj.shtwfgs.cn

U 高频实用片段                         120
来源：http://fs.asd995.cn

------------------------------------
来源：http://dx.yuntaijiaju.cn

合计                                  2106 条
来源：http://gm.jctech888.com.cn

--------------------------------------------------------------------------------
来源：http://ln.huanxung.cn

使用提醒
来源：http://vx.hnjuh.cn

--------------------------------------------------------------------------------
来源：http://cj.hahajie.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tj.muxihuayi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://pv.shxzukj.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://yv.shtwfgs.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://lo.nszjky.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wj.wgjwhj.cn

—— 文件结束 ——
来源：http://sp.yuexingan06.cn

================================================================================
来源：http://tr.yuntaijiaju.cn

程序语言常见例子速查手册（2024 版）
来源：http://an.lnxyls.cn

Common Programming Examples Cheat Book
来源：http://sx.panjiajie.cn

================================================================================
来源：http://zp.huixinmuqiang.cn

【收录内容】
来源：http://ol.lnxyls.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://kf.huanxung.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://tk.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://mk.hnjuh.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://kq.szsharing.cn

【使用说明】
来源：http://oz.hahajie.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ty.newstarts.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gb.huixiangedu.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://op.shxzskj.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ee.huixiangedu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://ct.gzmigu.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://iu.colortex.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cb.jianghongdianzi.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rj.muxihuayi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hj.asd995.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yf.lnxyls.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rc.jianghongdianzi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://lc.huixinmuqiang.cn

【文件统计】
来源：http://tv.nicolike.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mm.colortex.cn

--------------------------------------------------------------------------------
来源：http://sj.521024.cn

目  录
来源：http://ix.szsharing.cn

--------------------------------------------------------------------------------
来源：http://tu.haigaiapp.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://gm.bookmarksfly.cn


<!-- 参考信息 -->