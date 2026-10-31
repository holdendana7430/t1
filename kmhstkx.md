代发 wailian999

[U05] Py：列表去重且保序
来源：http://qk.9csxet.cn

list(dict.fromkeys(arr))
来源：http://cn.yuexingan06.cn

[U06] Py：合并两个字典
来源：http://wx.shtwfgs.cn

{**a, **b}
来源：http://ru.hahajie.cn

[U07] Py：反转字典键值
来源：http://fa.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://yi.gzmigu.cn

[U08] Py：展平二维列表
来源：http://lx.lnxyls.cn

[y for x in nested for y in x]
来源：http://jv.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://rt.jctech888.com.cn

max(d, key=d.get)
来源：http://fu.newstarts.cn

[U10] Py：按值排序字典
来源：http://aq.shxzskj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ed.yuntaijiaju.cn

[U11] Py：生成器表达式
来源：http://fl.huanxung.cn

(x * 2 for x in arr)
来源：http://xn.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jz.nicolike.cn

Counter(arr).most_common(3)
来源：http://ry.panjiajie.cn

[U13] Py：固定长度队列
来源：http://ng.huanxung.cn

deque(maxlen=10)
来源：http://fh.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://sy.asd995.cn

defaultdict(list)
来源：http://dz.wgjwhj.cn

[U15] Py：高精度计时
来源：http://gi.colortex.cn

t = time.perf_counter()
来源：http://cp.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://ns.hnjuh.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kq.wgjwhj.cn

[U17] Py：初始化日志
来源：http://ew.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://bp.huixinmuqiang.cn

[U18] Py：预编译正则
来源：http://xf.9csxet.cn

pat = re.compile(r"\d+")
来源：http://zz.hnjuh.cn

[U19] Py：正则替换带回调
来源：http://bi.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cq.huanxung.cn

[U20] Py：缓存函数结果
来源：http://eu.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://pu.huanxung.cn

[U21] Py：自定义上下文管理器
来源：http://br.huixiangedu.cn

@contextlib.contextmanager
来源：http://rs.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://lo.haigaiapp.cn

list(zip(*m))
来源：http://se.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://ah.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wg.bookmarksfly.cn

[U24] Py：路径操作
来源：http://fi.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bu.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://kn.9csxet.cn

csv.DictReader(f)
来源：http://fo.szsharing.cn

[U26] Py：并发下载
来源：http://lg.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://cz.shxzskj.cn

[U27] Py：异步 HTTP
来源：http://jc.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://pi.asd995.cn

[U28] Py：类型别名
来源：http://ni.panjiajie.cn

UserId = int
来源：http://er.nicolike.cn

[U29] Py：属性校验
来源：http://aw.shxzskj.cn

@property 与 @x.setter 配合
来源：http://lx.yuexingan06.cn

[U30] Py：数据类
来源：http://qa.huixinmuqiang.cn

@dataclass(slots=True)
来源：http://vh.shxzskj.cn

[U31] Py：单测
来源：http://vt.hnjuh.cn

python -m pytest -q
来源：http://nr.shxzukj.cn

[U32] Py：代码格式化
来源：http://qm.muxihuayi.cn

ruff format . && ruff check --fix .
来源：http://dw.colortex.cn

[U33] Py：打包发布
来源：http://md.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://ac.9csxet.cn

[U34] Py：判断编码
来源：http://qu.huixinmuqiang.cn

chardet.detect(raw)
来源：http://ds.panjiajie.cn

[U35] Py：发送邮件
来源：http://ba.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kp.colortex.cn

[U36] Py：定时任务
来源：http://mm.bjjhwx.cn

schedule.every(10).minutes.do(job)
来源：http://bw.panjiajie.cn

[U37] Py：读写 Excel
来源：http://rp.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ps.yuntaijiaju.cn

[U38] Py：获取脚本所在目录
来源：http://na.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://of.huanxung.cn

[U39] Py：判断是否在交互环境
来源：http://ad.newstarts.cn

sys.stdout.isatty()
来源：http://km.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://ko.szsharing.cn

print("err", file=sys.stderr)
来源：http://mb.panjiajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://sp.bookmarksfly.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qp.asd995.cn

[U42] PHP：PSR-4 自动加载
来源：http://vl.colortex.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://du.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://gj.huanxung.cn

namespace App\Http;
来源：http://cs.huanxung.cn

[U44] PHP：开启严格类型
来源：http://fy.jianghongdianzi.cn

declare(strict_types=1);
来源：http://xf.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://ar.shtwfgs.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rn.newstarts.cn

[U46] PHP：可空类型
来源：http://mu.jctech888.com.cn

?string $name = null
来源：http://mq.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://nc.huixiangedu.cn

int|string $id
来源：http://kr.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://ee.521024.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ej.huanxung.cn

[U49] PHP：只读属性
来源：http://rq.jianghongdianzi.cn

public readonly string $name
来源：http://qe.newstarts.cn

[U50] PHP：构造器属性提升
来源：http://xj.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://kc.hahajie.cn

[U51] PHP：数组解构
来源：http://nv.shxzukj.cn

[$a, $b] = $arr;
来源：http://eq.gzmigu.cn

[U52] PHP：箭头函数
来源：http://qr.bjjhwx.cn

$double = fn($x) => $x * 2;
来源：http://nu.hnjuh.cn

[U53] PHP：空合并运算符
来源：http://ck.asd995.cn

$v = $a ?? $b ?? "default";
来源：http://sx.muxihuayi.cn

[U54] PHP：空安全调用
来源：http://du.muxihuayi.cn

$obj?->method()
来源：http://le.shxzskj.cn

[U55] PHP：match 表达式
来源：http://rs.nszjky.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zj.shxzskj.cn

[U56] PHP：命名参数
来源：http://ys.szxytkj.cn

f(a: 1, b: 2)
来源：http://om.yuexingan06.cn

[U57] PHP：字符串插值
来源：http://ws.9csxet.cn

"值: {$a}"
来源：http://io.huanxung.cn

[U58] PHP：数组三件套
来源：http://qo.asd995.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://pd.huixiangedu.cn

[U59] PHP：自定义排序
来源：http://ub.shxzukj.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gh.haigaiapp.cn

[U60] PHP：JSON 编解码
来源：http://sa.shxzukj.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ng.gzmigu.cn

[U61] PHP：正则
来源：http://lu.colortex.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yl.wgjwhj.cn

[U62] PHP：日期对象
来源：http://mu.huixinmuqiang.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://sn.huixinmuqiang.cn

[U63] PHP：文件读写
来源：http://qo.nicolike.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vz.9csxet.cn

[U64] PHP：目录遍历
来源：http://lw.bookmarksfly.cn

glob("dir/*.php");  scandir("dir");
来源：http://tt.jctech888.com.cn

[U65] PHP：会话
来源：http://ap.jctech888.com.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ed.colortex.cn

[U66] PHP：设置 Cookie
来源：http://pa.hahajie.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oe.wgjwhj.cn

[U67] PHP：处理文件上传
来源：http://on.jianghongdianzi.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kv.hnjuh.cn

[U68] PHP：PDO 连接
来源：http://sf.colortex.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bt.huanxung.cn

[U69] PHP：PDO 预处理
来源：http://ab.gzmigu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://to.chemitech.net.cn

[U70] PHP：PDO 事务
来源：http://zy.bookmarksfly.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gh.huanxung.cn

[U71] PHP：抛出异常
来源：http://tq.asd995.cn

throw new RuntimeException("失败", 500);
来源：http://vv.chemitech.net.cn

[U72] PHP：写错误日志
来源：http://kk.jctech888.com.cn

error_log("失败: " . $e->getMessage());
来源：http://ag.yuntaijiaju.cn

[U73] PHP：读取 ini 配置
来源：http://pb.shxzskj.cn

parse_ini_file("config.ini", true)
来源：http://oy.hahajie.cn

[U74] PHP：读取环境变量
来源：http://pa.asd995.cn

getenv("APP_ENV") ?: "production"
来源：http://fp.yuntaijiaju.cn

[U75] PHP：依赖注入
来源：http://ra.wgjwhj.cn

composer require psr/container
来源：http://fb.bjjhwx.cn

[U76] PHP：简单路由
来源：http://ze.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bm.wgjwhj.cn

[U77] PHP：模板渲染
来源：http://uy.jctech888.com.cn

composer require twig/twig
来源：http://ub.nicolike.cn

[U78] PHP：单元测试
来源：http://rg.szxytkj.cn

composer require --dev phpunit/phpunit
来源：http://uc.panjiajie.cn

[U79] PHP：静态分析
来源：http://zu.shtwfgs.cn

composer require --dev phpstan/phpstan
来源：http://jw.chemitech.net.cn

[U80] PHP：代码规范修复
来源：http://yp.colortex.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mm.newstarts.cn

[U81] JS：初始化项目
来源：http://if.yuntaijiaju.cn

npm init -y;  npm i express
来源：http://zz.nszjky.cn

[U82] JS：package.json 脚本
来源：http://oa.shxzskj.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rh.szsharing.cn

[U83] JS：ES Module 导入导出
来源：http://in.jianghongdianzi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://rj.szsharing.cn

[U84] JS：CommonJS 写法
来源：http://uc.chemitech.net.cn

module.exports = { a };  const { a } = require("./m");
来源：http://yb.asd995.cn

[U85] JS：可选链
来源：http://id.shtwfgs.cn

a?.b?.c
来源：http://ib.521024.cn

[U86] JS：空值合并
来源：http://aq.jianghongdianzi.cn

a ?? b
来源：http://to.chemitech.net.cn

[U87] JS：解构默认值
来源：http://zz.huanxung.cn

const { a = 1, b = 2 } = obj;
来源：http://ny.jianghongdianzi.cn

[U88] JS：对象展开合并
来源：http://hx.jianghongdianzi.cn

{ ...a, ...b }
来源：http://qv.huixiangedu.cn

[U89] JS：数组去重
来源：http://op.colortex.cn

[...new Set(arr)]
来源：http://zc.muxihuayi.cn

[U90] JS：数字数组排序
来源：http://ii.muxihuayi.cn

[...arr].sort((a, b) => a - b)
来源：http://rk.newstarts.cn

[U91] JS：对象键值遍历
来源：http://tl.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://gp.wgjwhj.cn

[U92] JS：深拷贝
来源：http://ou.haigaiapp.cn

structuredClone(obj)
来源：http://lj.shtwfgs.cn

[U93] JS：模板字符串
来源：http://tt.szxytkj.cn

`共 ${n} 条`
来源：http://tq.hnjuh.cn

[U94] JS：箭头函数
来源：http://dm.521024.cn

const double = x => x * 2;
来源：http://no.hahajie.cn

[U95] JS：Promise 包装
来源：http://gn.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://ri.shxzukj.cn

[U96] JS：async/await 与异常
来源：http://rs.nszjky.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://ap.hahajie.cn

[U97] JS：并发请求
来源：http://pj.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://ev.muxihuayi.cn

[U98] JS：fetch 带 JSON
来源：http://bh.muxihuayi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://gp.jctech888.com.cn

[U99] JS：事件监听
来源：http://ox.chemitech.net.cn

el.addEventListener("click", e => {})
来源：http://mo.shtwfgs.cn

[U100] JS：DOM 查询
来源：http://ob.jctech888.com.cn

document.querySelector(".item")
来源：http://tz.yuexingan06.cn

[U101] JS：classList 操作
来源：http://xh.haigaiapp.cn

el.classList.toggle("active")
来源：http://cm.wgjwhj.cn

[U102] JS：本地存储
来源：http://ty.shxzukj.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://by.nszjky.cn

[U103] JS：定时器
来源：http://ft.nicolike.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://gn.haigaiapp.cn

[U104] JS：防抖
来源：http://sr.chemitech.net.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rj.chemitech.net.cn

[U105] JS：节流
来源：http://ra.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ki.panjiajie.cn

[U106] JS：日期格式化
来源：http://lf.haigaiapp.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oe.newstarts.cn

[U107] JS：数字千分位
来源：http://kf.szxytkj.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://uu.huixinmuqiang.cn

[U108] JS：随机整数
来源：http://bg.jianghongdianzi.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zz.newstarts.cn

[U109] JS：数组分组
来源：http://tl.szsharing.cn

Object.groupBy(arr, x => x.type)
来源：http://lt.jctech888.com.cn

[U110] JS：数组分块
来源：http://yx.colortex.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ns.lnxyls.cn

[U111] JS：对象转 Map
来源：http://zl.bookmarksfly.cn

new Map(Object.entries(obj))
来源：http://tp.huanxung.cn

[U112] JS：字符串补位
来源：http://lw.shxzukj.cn

"7".padStart(3, "0")
来源：http://bz.521024.cn

[U113] JS：正则替换全部
来源：http://nq.yuexingan06.cn

s.replaceAll("a", "b")
来源：http://pv.huixiangedu.cn

[U114] JS：JSON 深比较
来源：http://lz.nicolike.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://yf.asd995.cn

[U115] JS：生成 UUID
来源：http://ge.521024.cn

crypto.randomUUID()
来源：http://bo.huanxung.cn

[U116] JS：类型检查（JSDoc）
来源：http://qt.panjiajie.cn

/** @param {string} name */ function f(name) {}
来源：http://jd.nicolike.cn

[U117] JS：单元测试
来源：http://dr.yuexingan06.cn

npm i -D vitest;  npx vitest
来源：http://ih.shtwfgs.cn

[U118] JS：开发服务器
来源：http://jx.hahajie.cn

npm i -D vite;  npx vite
来源：http://vs.yuexingan06.cn

[U119] JS：生产构建
来源：http://yo.huixinmuqiang.cn

npx vite build
来源：http://gd.bjjhwx.cn

[U120] JS：读取环境变量（Vite）
来源：http://wq.newstarts.cn

import.meta.env.VITE_API_URL
来源：http://hp.wgjwhj.cn

================================================================================
来源：http://nt.gzmigu.cn

统计汇总
来源：http://qb.nicolike.cn

================================================================================
来源：http://op.9csxet.cn

按语言统计（条）：
来源：http://ey.bookmarksfly.cn

Python ......... 252
来源：http://au.asd995.cn

PHP ............ 252
来源：http://hp.colortex.cn

JavaScript ..... 252
来源：http://iz.lnxyls.cn

TypeScript ..... 212
来源：http://gb.bjjhwx.cn

Java ........... 212
来源：http://eq.521024.cn

Go ............. 212
来源：http://iq.hnjuh.cn

Ruby ........... 212
来源：http://da.colortex.cn

C# ............. 212
来源：http://yu.panjiajie.cn

C .............. 30
来源：http://ac.haigaiapp.cn

C++ ............ 30
来源：http://pf.hnjuh.cn

SQL ............ 90
来源：http://uq.shtwfgs.cn

Bash ........... 80
来源：http://zh.521024.cn

Kotlin ......... 15
来源：http://gz.gzmigu.cn

Swift .......... 15
来源：http://im.9csxet.cn

Lua ............ 10
来源：http://la.wgjwhj.cn

Perl ........... 10
来源：http://kp.nszjky.cn

Scala .......... 10
来源：http://tm.521024.cn

------------------------------------
来源：http://fl.hahajie.cn

合计 ........... 2106 条
来源：http://un.szsharing.cn

按章节统计：
来源：http://qa.nicolike.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jn.wgjwhj.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://rw.gzmigu.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ta.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://sj.hnjuh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://sw.jianghongdianzi.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pt.lnxyls.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://if.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://se.jianghongdianzi.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://lw.wgjwhj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lv.jctech888.com.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://ym.shtwfgs.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dp.muxihuayi.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://nv.lnxyls.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zb.521024.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ji.huixiangedu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://bt.jianghongdianzi.cn

Q SQL 专题                              90
来源：http://fg.nicolike.cn

R Bash 专题                             80
来源：http://bu.jctech888.com.cn

S C / C++ 专题                          60
来源：http://in.newstarts.cn

T 其他语言补充                          60
来源：http://fs.haigaiapp.cn

U 高频实用片段                         120
来源：http://ip.shxzskj.cn

------------------------------------
来源：http://jr.nicolike.cn

合计                                  2106 条
来源：http://bh.shtwfgs.cn

--------------------------------------------------------------------------------
来源：http://sm.huixiangedu.cn

使用提醒
来源：http://pd.chemitech.net.cn

--------------------------------------------------------------------------------
来源：http://xx.wgjwhj.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://cd.nszjky.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://cz.huixiangedu.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ey.hahajie.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://uq.shxzukj.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://jt.huixinmuqiang.cn

—— 文件结束 ——
来源：http://zl.huixinmuqiang.cn

================================================================================
来源：http://di.chemitech.net.cn

程序语言常见例子速查手册（2024 版）
来源：http://sm.hahajie.cn

Common Programming Examples Cheat Book
来源：http://mp.panjiajie.cn

================================================================================
来源：http://op.521024.cn

【收录内容】
来源：http://zs.wgjwhj.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://en.szxytkj.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vm.bookmarksfly.cn

SQL · Bash · C · C++
来源：http://bg.szxytkj.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://id.9csxet.cn

【使用说明】
来源：http://ha.szsharing.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://sp.shxzskj.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://aq.lnxyls.cn


<!-- 参考信息 -->