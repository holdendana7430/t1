代发 wailian999

[U11] Py：生成器表达式
来源：http://wr.szsharing.cn

(x * 2 for x in arr)
来源：http://jd.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://en.nszjky.cn

Counter(arr).most_common(3)
来源：http://rr.yuexingan06.cn

[U13] Py：固定长度队列
来源：http://kl.521024.cn

deque(maxlen=10)
来源：http://gg.huanxung.cn

[U14] Py：分组收集到列表
来源：http://cu.colortex.cn

defaultdict(list)
来源：http://xa.9csxet.cn

[U15] Py：高精度计时
来源：http://yb.nszjky.cn

t = time.perf_counter()
来源：http://di.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://xa.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zy.chemitech.net.cn

[U17] Py：初始化日志
来源：http://vn.asd995.cn

logging.basicConfig(level=logging.INFO)
来源：http://gv.nszjky.cn

[U18] Py：预编译正则
来源：http://eh.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://ba.hahajie.cn

[U19] Py：正则替换带回调
来源：http://dg.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://eu.newstarts.cn

[U20] Py：缓存函数结果
来源：http://xj.bookmarksfly.cn

@functools.lru_cache(maxsize=None)
来源：http://je.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://ic.asd995.cn

@contextlib.contextmanager
来源：http://kj.hnjuh.cn

[U22] Py：矩阵转置
来源：http://uz.jianghongdianzi.cn

list(zip(*m))
来源：http://at.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://ye.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tb.shxzukj.cn

[U24] Py：路径操作
来源：http://yk.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ug.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://gp.yuexingan06.cn

csv.DictReader(f)
来源：http://me.nszjky.cn

[U26] Py：并发下载
来源：http://fa.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nx.521024.cn

[U27] Py：异步 HTTP
来源：http://fk.hahajie.cn

aiohttp.ClientSession() 配合 async with
来源：http://jl.gzmigu.cn

[U28] Py：类型别名
来源：http://so.muxihuayi.cn

UserId = int
来源：http://mc.521024.cn

[U29] Py：属性校验
来源：http://pt.shxzukj.cn

@property 与 @x.setter 配合
来源：http://zs.gzmigu.cn

[U30] Py：数据类
来源：http://wl.newstarts.cn

@dataclass(slots=True)
来源：http://wb.shxzskj.cn

[U31] Py：单测
来源：http://mj.shtwfgs.cn

python -m pytest -q
来源：http://vx.panjiajie.cn

[U32] Py：代码格式化
来源：http://kb.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://bp.nicolike.cn

[U33] Py：打包发布
来源：http://td.jianghongdianzi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ec.jctech888.com.cn

[U34] Py：判断编码
来源：http://gt.yuntaijiaju.cn

chardet.detect(raw)
来源：http://dg.nicolike.cn

[U35] Py：发送邮件
来源：http://mo.huanxung.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jn.panjiajie.cn

[U36] Py：定时任务
来源：http://bh.haigaiapp.cn

schedule.every(10).minutes.do(job)
来源：http://jc.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://kk.nszjky.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vr.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://wg.shxzskj.cn

Path(__file__).resolve().parent
来源：http://dm.huixiangedu.cn

[U39] Py：判断是否在交互环境
来源：http://tz.panjiajie.cn

sys.stdout.isatty()
来源：http://ac.panjiajie.cn

[U40] Py：打印到标准错误
来源：http://iq.muxihuayi.cn

print("err", file=sys.stderr)
来源：http://do.haigaiapp.cn

[U41] PHP：初始化 Composer 项目
来源：http://cx.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rw.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://lc.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zb.lnxyls.cn

[U43] PHP：声明命名空间
来源：http://vl.panjiajie.cn

namespace App\Http;
来源：http://mc.szsharing.cn

[U44] PHP：开启严格类型
来源：http://ka.9csxet.cn

declare(strict_types=1);
来源：http://ns.shxzukj.cn

[U45] PHP：类型声明与返回类型
来源：http://jr.nszjky.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://kn.bjjhwx.cn

[U46] PHP：可空类型
来源：http://sm.9csxet.cn

?string $name = null
来源：http://ch.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://bb.shxzskj.cn

int|string $id
来源：http://rz.9csxet.cn

[U48] PHP：纯枚举
来源：http://lb.szsharing.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lq.shtwfgs.cn

[U49] PHP：只读属性
来源：http://uw.bookmarksfly.cn

public readonly string $name
来源：http://me.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://hp.yuexingan06.cn

public function __construct(private int $id) {}
来源：http://rq.haigaiapp.cn

[U51] PHP：数组解构
来源：http://ls.yuexingan06.cn

[$a, $b] = $arr;
来源：http://qh.bookmarksfly.cn

[U52] PHP：箭头函数
来源：http://wx.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://rp.nszjky.cn

[U53] PHP：空合并运算符
来源：http://au.9csxet.cn

$v = $a ?? $b ?? "default";
来源：http://lc.newstarts.cn

[U54] PHP：空安全调用
来源：http://gs.jianghongdianzi.cn

$obj?->method()
来源：http://fi.521024.cn

[U55] PHP：match 表达式
来源：http://pz.nicolike.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://no.hnjuh.cn

[U56] PHP：命名参数
来源：http://qc.huixiangedu.cn

f(a: 1, b: 2)
来源：http://mh.wgjwhj.cn

[U57] PHP：字符串插值
来源：http://lv.colortex.cn

"值: {$a}"
来源：http://fa.huixinmuqiang.cn

[U58] PHP：数组三件套
来源：http://hw.szsharing.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oz.lnxyls.cn

[U59] PHP：自定义排序
来源：http://ws.bookmarksfly.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tx.newstarts.cn

[U60] PHP：JSON 编解码
来源：http://jk.nszjky.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bq.lnxyls.cn

[U61] PHP：正则
来源：http://za.huanxung.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wv.jianghongdianzi.cn

[U62] PHP：日期对象
来源：http://aa.szsharing.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ly.shtwfgs.cn

[U63] PHP：文件读写
来源：http://wg.chemitech.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hf.jctech888.com.cn

[U64] PHP：目录遍历
来源：http://tp.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://ij.haigaiapp.cn

[U65] PHP：会话
来源：http://jp.hahajie.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://op.hnjuh.cn

[U66] PHP：设置 Cookie
来源：http://cz.hnjuh.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pq.yuexingan06.cn

[U67] PHP：处理文件上传
来源：http://nd.yuntaijiaju.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ek.9csxet.cn

[U68] PHP：PDO 连接
来源：http://xy.9csxet.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://df.shxzukj.cn

[U69] PHP：PDO 预处理
来源：http://ho.huixiangedu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://id.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://wy.muxihuayi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://pq.nszjky.cn

[U71] PHP：抛出异常
来源：http://sn.521024.cn

throw new RuntimeException("失败", 500);
来源：http://lu.huixiangedu.cn

[U72] PHP：写错误日志
来源：http://vb.newstarts.cn

error_log("失败: " . $e->getMessage());
来源：http://bo.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://xj.bookmarksfly.cn

parse_ini_file("config.ini", true)
来源：http://tz.szsharing.cn

[U74] PHP：读取环境变量
来源：http://kt.huixinmuqiang.cn

getenv("APP_ENV") ?: "production"
来源：http://wh.lnxyls.cn

[U75] PHP：依赖注入
来源：http://sn.nicolike.cn

composer require psr/container
来源：http://kn.gzmigu.cn

[U76] PHP：简单路由
来源：http://qq.panjiajie.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bj.huixiangedu.cn

[U77] PHP：模板渲染
来源：http://ny.bookmarksfly.cn

composer require twig/twig
来源：http://dn.wgjwhj.cn

[U78] PHP：单元测试
来源：http://db.bookmarksfly.cn

composer require --dev phpunit/phpunit
来源：http://ba.bookmarksfly.cn

[U79] PHP：静态分析
来源：http://bq.jctech888.com.cn

composer require --dev phpstan/phpstan
来源：http://pz.lnxyls.cn

[U80] PHP：代码规范修复
来源：http://md.huixinmuqiang.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://dk.jctech888.com.cn

[U81] JS：初始化项目
来源：http://ag.huanxung.cn

npm init -y;  npm i express
来源：http://fl.szsharing.cn

[U82] JS：package.json 脚本
来源：http://tw.bookmarksfly.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://zz.521024.cn

[U83] JS：ES Module 导入导出
来源：http://vk.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://he.bookmarksfly.cn

[U84] JS：CommonJS 写法
来源：http://fl.shtwfgs.cn

module.exports = { a };  const { a } = require("./m");
来源：http://oe.colortex.cn

[U85] JS：可选链
来源：http://ty.jianghongdianzi.cn

a?.b?.c
来源：http://po.nicolike.cn

[U86] JS：空值合并
来源：http://jd.nszjky.cn

a ?? b
来源：http://mo.521024.cn

[U87] JS：解构默认值
来源：http://ko.colortex.cn

const { a = 1, b = 2 } = obj;
来源：http://cq.lnxyls.cn

[U88] JS：对象展开合并
来源：http://ps.jianghongdianzi.cn

{ ...a, ...b }
来源：http://rk.hnjuh.cn

[U89] JS：数组去重
来源：http://hz.yuntaijiaju.cn

[...new Set(arr)]
来源：http://jp.szxytkj.cn

[U90] JS：数字数组排序
来源：http://lc.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://xp.nszjky.cn

[U91] JS：对象键值遍历
来源：http://ez.muxihuayi.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mi.shtwfgs.cn

[U92] JS：深拷贝
来源：http://qf.nicolike.cn

structuredClone(obj)
来源：http://zt.szsharing.cn

[U93] JS：模板字符串
来源：http://nc.gzmigu.cn

`共 ${n} 条`
来源：http://bc.gzmigu.cn

[U94] JS：箭头函数
来源：http://au.wgjwhj.cn

const double = x => x * 2;
来源：http://nd.asd995.cn

[U95] JS：Promise 包装
来源：http://zo.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://jc.colortex.cn

[U96] JS：async/await 与异常
来源：http://bx.haigaiapp.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nh.huixiangedu.cn

[U97] JS：并发请求
来源：http://al.jctech888.com.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://cu.bookmarksfly.cn

[U98] JS：fetch 带 JSON
来源：http://sz.yuexingan06.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fe.hnjuh.cn

[U99] JS：事件监听
来源：http://bl.huixiangedu.cn

el.addEventListener("click", e => {})
来源：http://si.9csxet.cn

[U100] JS：DOM 查询
来源：http://zx.jctech888.com.cn

document.querySelector(".item")
来源：http://cj.shxzukj.cn

[U101] JS：classList 操作
来源：http://ww.shxzukj.cn

el.classList.toggle("active")
来源：http://bt.panjiajie.cn

[U102] JS：本地存储
来源：http://om.colortex.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dt.asd995.cn

[U103] JS：定时器
来源：http://ni.wgjwhj.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ln.bookmarksfly.cn

[U104] JS：防抖
来源：http://xv.jctech888.com.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zx.bjjhwx.cn

[U105] JS：节流
来源：http://yi.colortex.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://qe.wgjwhj.cn

[U106] JS：日期格式化
来源：http://em.newstarts.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://es.wgjwhj.cn

[U107] JS：数字千分位
来源：http://ok.szsharing.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wn.asd995.cn

[U108] JS：随机整数
来源：http://xo.shxzskj.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://qr.shtwfgs.cn

[U109] JS：数组分组
来源：http://uq.huanxung.cn

Object.groupBy(arr, x => x.type)
来源：http://ga.bookmarksfly.cn

[U110] JS：数组分块
来源：http://yp.shxzukj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bx.gzmigu.cn

[U111] JS：对象转 Map
来源：http://cy.huixinmuqiang.cn

new Map(Object.entries(obj))
来源：http://gq.jctech888.com.cn

[U112] JS：字符串补位
来源：http://jm.colortex.cn

"7".padStart(3, "0")
来源：http://uz.newstarts.cn

[U113] JS：正则替换全部
来源：http://ow.chemitech.net.cn

s.replaceAll("a", "b")
来源：http://km.yuntaijiaju.cn

[U114] JS：JSON 深比较
来源：http://rx.huanxung.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wj.huanxung.cn

[U115] JS：生成 UUID
来源：http://jn.newstarts.cn

crypto.randomUUID()
来源：http://oa.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://qz.shtwfgs.cn

/** @param {string} name */ function f(name) {}
来源：http://be.asd995.cn

[U117] JS：单元测试
来源：http://vu.bookmarksfly.cn

npm i -D vitest;  npx vitest
来源：http://fw.shxzskj.cn

[U118] JS：开发服务器
来源：http://sm.jctech888.com.cn

npm i -D vite;  npx vite
来源：http://sn.bjjhwx.cn

[U119] JS：生产构建
来源：http://bq.bookmarksfly.cn

npx vite build
来源：http://wo.hahajie.cn

[U120] JS：读取环境变量（Vite）
来源：http://pl.nszjky.cn

import.meta.env.VITE_API_URL
来源：http://mk.hnjuh.cn

================================================================================
来源：http://zv.muxihuayi.cn

统计汇总
来源：http://sl.chemitech.net.cn

================================================================================
来源：http://cu.newstarts.cn

按语言统计（条）：
来源：http://vv.nicolike.cn

Python ......... 252
来源：http://il.9csxet.cn

PHP ............ 252
来源：http://yh.shxzukj.cn

JavaScript ..... 252
来源：http://oz.jianghongdianzi.cn

TypeScript ..... 212
来源：http://vn.yuexingan06.cn

Java ........... 212
来源：http://ot.bjjhwx.cn

Go ............. 212
来源：http://nz.newstarts.cn

Ruby ........... 212
来源：http://fp.wgjwhj.cn

C# ............. 212
来源：http://yx.hahajie.cn

C .............. 30
来源：http://wb.huixiangedu.cn

C++ ............ 30
来源：http://zc.yuexingan06.cn

SQL ............ 90
来源：http://ja.hnjuh.cn

Bash ........... 80
来源：http://yf.nicolike.cn

Kotlin ......... 15
来源：http://hx.shtwfgs.cn

Swift .......... 15
来源：http://jt.shxzukj.cn

Lua ............ 10
来源：http://zf.huixinmuqiang.cn

Perl ........... 10
来源：http://bj.9csxet.cn

Scala .......... 10
来源：http://jj.newstarts.cn

------------------------------------
来源：http://kj.wgjwhj.cn

合计 ........... 2106 条
来源：http://dc.huixinmuqiang.cn

按章节统计：
来源：http://vo.muxihuayi.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://gb.hahajie.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://sq.yuntaijiaju.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ef.szxytkj.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://ye.lnxyls.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://js.chemitech.net.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://yy.nicolike.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uz.gzmigu.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xv.lnxyls.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ut.szxytkj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://pa.bookmarksfly.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pn.nszjky.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://ox.shxzukj.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wd.bjjhwx.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://uh.muxihuayi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uu.panjiajie.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bi.shtwfgs.cn

Q SQL 专题                              90
来源：http://fc.shxzukj.cn

R Bash 专题                             80
来源：http://id.shxzskj.cn

S C / C++ 专题                          60
来源：http://gc.shxzskj.cn

T 其他语言补充                          60
来源：http://im.jianghongdianzi.cn

U 高频实用片段                         120
来源：http://od.wgjwhj.cn

------------------------------------
来源：http://px.yuntaijiaju.cn

合计                                  2106 条
来源：http://tk.shxzskj.cn

--------------------------------------------------------------------------------
来源：http://ab.szsharing.cn

使用提醒
来源：http://af.jianghongdianzi.cn

--------------------------------------------------------------------------------
来源：http://sp.colortex.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://ue.lnxyls.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://du.hnjuh.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://df.szsharing.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uo.chemitech.net.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://xd.panjiajie.cn

—— 文件结束 ——
来源：http://zy.9csxet.cn

================================================================================
来源：http://qw.nicolike.cn

程序语言常见例子速查手册（2024 版）
来源：http://nf.newstarts.cn

Common Programming Examples Cheat Book
来源：http://cr.haigaiapp.cn

================================================================================
来源：http://xj.shtwfgs.cn

【收录内容】
来源：http://za.shxzskj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vt.muxihuayi.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wu.yuntaijiaju.cn

SQL · Bash · C · C++
来源：http://sn.gzmigu.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zd.jctech888.com.cn

【使用说明】
来源：http://is.jianghongdianzi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://dw.hnjuh.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://uq.shxzukj.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uy.yuntaijiaju.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ur.shxzskj.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://xq.shxzskj.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://jz.huanxung.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://zd.huixiangedu.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ko.jianghongdianzi.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fr.shxzukj.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://go.newstarts.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://an.521024.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ul.colortex.cn

【文件统计】
来源：http://pc.yuexingan06.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://bo.lnxyls.cn


<!-- 参考信息 -->