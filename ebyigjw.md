代发 wailian999

case class User(name: String, age: Int)
来源：http://zo.hnjuh.cn

[T57] Scala：模式匹配
来源：http://rf.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hu.9csxet.cn

[T58] Scala：函数定义
来源：http://vn.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wj.yuntaijiaju.cn

[T59] Scala：循环
来源：http://fd.hahajie.cn

for (i <- 1 to 10) println(i)
来源：http://um.bookmarksfly.cn

[T60] Scala：折叠
来源：http://fx.shxzskj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jf.haigaiapp.cn

================================================================================
来源：http://hd.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://js.hnjuh.cn

================================================================================
来源：http://zf.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://lv.chemitech.net.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wf.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://nh.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uz.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://sy.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hd.shxzukj.cn

[U04] Py：变量调试打印
来源：http://zl.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lq.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://fh.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://nk.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://sl.nicolike.cn

{**a, **b}
来源：http://mr.szxytkj.cn

[U07] Py：反转字典键值
来源：http://lc.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://nj.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://pw.521024.cn

[y for x in nested for y in x]
来源：http://ae.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://ye.wgjwhj.cn

max(d, key=d.get)
来源：http://hs.hnjuh.cn

[U10] Py：按值排序字典
来源：http://ov.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ts.yuexingan06.cn

[U11] Py：生成器表达式
来源：http://bj.hnjuh.cn

(x * 2 for x in arr)
来源：http://pa.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ip.nszjky.cn

Counter(arr).most_common(3)
来源：http://ut.newstarts.cn

[U13] Py：固定长度队列
来源：http://az.haigaiapp.cn

deque(maxlen=10)
来源：http://ib.gzmigu.cn

[U14] Py：分组收集到列表
来源：http://tn.asd995.cn

defaultdict(list)
来源：http://lc.panjiajie.cn

[U15] Py：高精度计时
来源：http://nj.colortex.cn

t = time.perf_counter()
来源：http://sd.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://ch.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kv.hahajie.cn

[U17] Py：初始化日志
来源：http://cp.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://ti.nicolike.cn

[U18] Py：预编译正则
来源：http://ad.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ip.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://ey.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jy.gzmigu.cn

[U20] Py：缓存函数结果
来源：http://el.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://lq.wgjwhj.cn

[U21] Py：自定义上下文管理器
来源：http://ib.newstarts.cn

@contextlib.contextmanager
来源：http://xd.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://yt.asd995.cn

list(zip(*m))
来源：http://sb.yuexingan06.cn

[U23] Py：分块读取大文件
来源：http://gg.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wx.nszjky.cn

[U24] Py：路径操作
来源：http://ng.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ew.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://uj.9csxet.cn

csv.DictReader(f)
来源：http://mj.bookmarksfly.cn

[U26] Py：并发下载
来源：http://vd.asd995.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ag.muxihuayi.cn

[U27] Py：异步 HTTP
来源：http://uy.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://dt.asd995.cn

[U28] Py：类型别名
来源：http://zg.bookmarksfly.cn

UserId = int
来源：http://qu.panjiajie.cn

[U29] Py：属性校验
来源：http://qb.chemitech.net.cn

@property 与 @x.setter 配合
来源：http://px.yuexingan06.cn

[U30] Py：数据类
来源：http://li.haigaiapp.cn

@dataclass(slots=True)
来源：http://js.lnxyls.cn

[U31] Py：单测
来源：http://fu.gzmigu.cn

python -m pytest -q
来源：http://up.yuexingan06.cn

[U32] Py：代码格式化
来源：http://av.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://gg.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://ld.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://kq.muxihuayi.cn

[U34] Py：判断编码
来源：http://dt.bjjhwx.cn

chardet.detect(raw)
来源：http://ce.panjiajie.cn

[U35] Py：发送邮件
来源：http://fm.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pv.muxihuayi.cn

[U36] Py：定时任务
来源：http://wj.chemitech.net.cn

schedule.every(10).minutes.do(job)
来源：http://ni.9csxet.cn

[U37] Py：读写 Excel
来源：http://ec.hnjuh.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tr.shxzukj.cn

[U38] Py：获取脚本所在目录
来源：http://gk.newstarts.cn

Path(__file__).resolve().parent
来源：http://na.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://vn.haigaiapp.cn

sys.stdout.isatty()
来源：http://vp.asd995.cn

[U40] Py：打印到标准错误
来源：http://em.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://lb.nicolike.cn

[U41] PHP：初始化 Composer 项目
来源：http://hi.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://bz.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://bg.bookmarksfly.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qq.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://uj.bookmarksfly.cn

namespace App\Http;
来源：http://is.haigaiapp.cn

[U44] PHP：开启严格类型
来源：http://zn.chemitech.net.cn

declare(strict_types=1);
来源：http://wa.szsharing.cn

[U45] PHP：类型声明与返回类型
来源：http://tr.hnjuh.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://hq.lnxyls.cn

[U46] PHP：可空类型
来源：http://ml.bookmarksfly.cn

?string $name = null
来源：http://og.hahajie.cn

[U47] PHP：联合类型
来源：http://ew.huixinmuqiang.cn

int|string $id
来源：http://dz.szsharing.cn

[U48] PHP：纯枚举
来源：http://br.asd995.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yi.jctech888.com.cn

[U49] PHP：只读属性
来源：http://kw.yuntaijiaju.cn

public readonly string $name
来源：http://hd.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://vq.shxzskj.cn

public function __construct(private int $id) {}
来源：http://tl.bookmarksfly.cn

[U51] PHP：数组解构
来源：http://fy.szsharing.cn

[$a, $b] = $arr;
来源：http://vv.hahajie.cn

[U52] PHP：箭头函数
来源：http://jc.yuntaijiaju.cn

$double = fn($x) => $x * 2;
来源：http://ag.huixinmuqiang.cn

[U53] PHP：空合并运算符
来源：http://jf.yuntaijiaju.cn

$v = $a ?? $b ?? "default";
来源：http://wg.nszjky.cn

[U54] PHP：空安全调用
来源：http://fs.bookmarksfly.cn

$obj?->method()
来源：http://se.bjjhwx.cn

[U55] PHP：match 表达式
来源：http://bh.hnjuh.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ik.shxzskj.cn

[U56] PHP：命名参数
来源：http://yn.szsharing.cn

f(a: 1, b: 2)
来源：http://yx.521024.cn

[U57] PHP：字符串插值
来源：http://yi.szsharing.cn

"值: {$a}"
来源：http://qf.chemitech.net.cn

[U58] PHP：数组三件套
来源：http://hh.chemitech.net.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ew.wgjwhj.cn

[U59] PHP：自定义排序
来源：http://gl.shtwfgs.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://te.chemitech.net.cn

[U60] PHP：JSON 编解码
来源：http://qt.bjjhwx.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qg.szxytkj.cn

[U61] PHP：正则
来源：http://tq.gzmigu.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dj.shxzskj.cn

[U62] PHP：日期对象
来源：http://vt.shxzukj.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wm.chemitech.net.cn

[U63] PHP：文件读写
来源：http://bd.jctech888.com.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bj.wgjwhj.cn

[U64] PHP：目录遍历
来源：http://qw.newstarts.cn

glob("dir/*.php");  scandir("dir");
来源：http://jg.muxihuayi.cn

[U65] PHP：会话
来源：http://dl.newstarts.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://wr.shxzukj.cn

[U66] PHP：设置 Cookie
来源：http://qe.haigaiapp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ib.colortex.cn

[U67] PHP：处理文件上传
来源：http://rp.gzmigu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ya.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://py.newstarts.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eg.huixiangedu.cn

[U69] PHP：PDO 预处理
来源：http://qo.newstarts.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rv.shxzukj.cn

[U70] PHP：PDO 事务
来源：http://tc.shxzskj.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dk.haigaiapp.cn

[U71] PHP：抛出异常
来源：http://xh.9csxet.cn

throw new RuntimeException("失败", 500);
来源：http://ji.521024.cn

[U72] PHP：写错误日志
来源：http://vg.bookmarksfly.cn

error_log("失败: " . $e->getMessage());
来源：http://qt.9csxet.cn

[U73] PHP：读取 ini 配置
来源：http://eh.jctech888.com.cn

parse_ini_file("config.ini", true)
来源：http://uj.asd995.cn

[U74] PHP：读取环境变量
来源：http://qc.shxzukj.cn

getenv("APP_ENV") ?: "production"
来源：http://el.bookmarksfly.cn

[U75] PHP：依赖注入
来源：http://vg.nicolike.cn

composer require psr/container
来源：http://ij.panjiajie.cn

[U76] PHP：简单路由
来源：http://xn.szsharing.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bn.colortex.cn

[U77] PHP：模板渲染
来源：http://xr.colortex.cn

composer require twig/twig
来源：http://ff.huanxung.cn

[U78] PHP：单元测试
来源：http://sm.newstarts.cn

composer require --dev phpunit/phpunit
来源：http://js.jianghongdianzi.cn

[U79] PHP：静态分析
来源：http://gq.szsharing.cn

composer require --dev phpstan/phpstan
来源：http://xp.9csxet.cn

[U80] PHP：代码规范修复
来源：http://ic.9csxet.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://wq.hahajie.cn

[U81] JS：初始化项目
来源：http://cp.huanxung.cn

npm init -y;  npm i express
来源：http://my.shxzukj.cn

[U82] JS：package.json 脚本
来源：http://vm.yuntaijiaju.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ll.hahajie.cn

[U83] JS：ES Module 导入导出
来源：http://qn.yuexingan06.cn

export const a = 1;  import { a } from "./m.js";
来源：http://uf.jianghongdianzi.cn

[U84] JS：CommonJS 写法
来源：http://se.panjiajie.cn

module.exports = { a };  const { a } = require("./m");
来源：http://bl.shxzukj.cn

[U85] JS：可选链
来源：http://gn.lnxyls.cn

a?.b?.c
来源：http://me.bjjhwx.cn

[U86] JS：空值合并
来源：http://hr.newstarts.cn

a ?? b
来源：http://wp.szxytkj.cn

[U87] JS：解构默认值
来源：http://hg.szsharing.cn

const { a = 1, b = 2 } = obj;
来源：http://bt.hnjuh.cn

[U88] JS：对象展开合并
来源：http://xa.nicolike.cn

{ ...a, ...b }
来源：http://vl.yuntaijiaju.cn

[U89] JS：数组去重
来源：http://xm.jianghongdianzi.cn

[...new Set(arr)]
来源：http://ji.huanxung.cn

[U90] JS：数字数组排序
来源：http://wf.bjjhwx.cn

[...arr].sort((a, b) => a - b)
来源：http://hj.521024.cn

[U91] JS：对象键值遍历
来源：http://zm.jctech888.com.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qx.chemitech.net.cn

[U92] JS：深拷贝
来源：http://vn.9csxet.cn

structuredClone(obj)
来源：http://yf.hahajie.cn

[U93] JS：模板字符串
来源：http://yb.haigaiapp.cn

`共 ${n} 条`
来源：http://fc.nszjky.cn

[U94] JS：箭头函数
来源：http://vk.jianghongdianzi.cn

const double = x => x * 2;
来源：http://pr.gzmigu.cn

[U95] JS：Promise 包装
来源：http://tn.hnjuh.cn

new Promise((resolve, reject) => {})
来源：http://iv.muxihuayi.cn

[U96] JS：async/await 与异常
来源：http://mz.szsharing.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hz.bjjhwx.cn

[U97] JS：并发请求
来源：http://qe.shxzskj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hn.521024.cn

[U98] JS：fetch 带 JSON
来源：http://wk.haigaiapp.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://en.haigaiapp.cn

[U99] JS：事件监听
来源：http://ad.asd995.cn

el.addEventListener("click", e => {})
来源：http://ir.wgjwhj.cn

[U100] JS：DOM 查询
来源：http://cp.asd995.cn

document.querySelector(".item")
来源：http://rj.huanxung.cn

[U101] JS：classList 操作
来源：http://mo.muxihuayi.cn

el.classList.toggle("active")
来源：http://xu.szxytkj.cn

[U102] JS：本地存储
来源：http://dp.jianghongdianzi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ea.521024.cn

[U103] JS：定时器
来源：http://bc.yuexingan06.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zc.huixinmuqiang.cn

[U104] JS：防抖
来源：http://yt.colortex.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ed.newstarts.cn

[U105] JS：节流
来源：http://fh.haigaiapp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://br.jianghongdianzi.cn

[U106] JS：日期格式化
来源：http://vv.huixiangedu.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://yj.szsharing.cn

[U107] JS：数字千分位
来源：http://yb.chemitech.net.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wx.asd995.cn

[U108] JS：随机整数
来源：http://ki.yuntaijiaju.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wv.jianghongdianzi.cn

[U109] JS：数组分组
来源：http://cb.yuexingan06.cn

Object.groupBy(arr, x => x.type)
来源：http://er.asd995.cn

[U110] JS：数组分块
来源：http://ms.wgjwhj.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://xu.chemitech.net.cn

[U111] JS：对象转 Map
来源：http://qw.jianghongdianzi.cn

new Map(Object.entries(obj))
来源：http://wn.shxzskj.cn

[U112] JS：字符串补位
来源：http://id.muxihuayi.cn

"7".padStart(3, "0")
来源：http://wm.hnjuh.cn

[U113] JS：正则替换全部
来源：http://qe.jctech888.com.cn

s.replaceAll("a", "b")
来源：http://hz.hnjuh.cn

[U114] JS：JSON 深比较
来源：http://nn.hnjuh.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://cj.muxihuayi.cn

[U115] JS：生成 UUID
来源：http://me.bookmarksfly.cn

crypto.randomUUID()
来源：http://uq.nicolike.cn

[U116] JS：类型检查（JSDoc）
来源：http://js.jctech888.com.cn

/** @param {string} name */ function f(name) {}
来源：http://we.yuntaijiaju.cn

[U117] JS：单元测试
来源：http://sz.haigaiapp.cn

npm i -D vitest;  npx vitest
来源：http://fr.bjjhwx.cn

[U118] JS：开发服务器
来源：http://my.shtwfgs.cn

npm i -D vite;  npx vite
来源：http://ed.szxytkj.cn

[U119] JS：生产构建
来源：http://bw.muxihuayi.cn

npx vite build
来源：http://ih.wgjwhj.cn

[U120] JS：读取环境变量（Vite）
来源：http://vd.nicolike.cn

import.meta.env.VITE_API_URL
来源：http://rr.colortex.cn

================================================================================
来源：http://rm.nszjky.cn

统计汇总
来源：http://pb.jianghongdianzi.cn

================================================================================
来源：http://nt.yuntaijiaju.cn

按语言统计（条）：
来源：http://uo.szsharing.cn

Python ......... 252
来源：http://fo.chemitech.net.cn

PHP ............ 252
来源：http://cz.panjiajie.cn

JavaScript ..... 252
来源：http://ui.shxzukj.cn

TypeScript ..... 212
来源：http://hv.szxytkj.cn

Java ........... 212
来源：http://xo.gzmigu.cn

Go ............. 212
来源：http://vt.wgjwhj.cn

Ruby ........... 212
来源：http://zo.521024.cn

C# ............. 212
来源：http://gg.huixinmuqiang.cn

C .............. 30
来源：http://aa.lnxyls.cn

C++ ............ 30
来源：http://we.jianghongdianzi.cn

SQL ............ 90
来源：http://dm.yuexingan06.cn

Bash ........... 80
来源：http://oh.bookmarksfly.cn

Kotlin ......... 15
来源：http://aj.hahajie.cn

Swift .......... 15
来源：http://ae.yuexingan06.cn

Lua ............ 10
来源：http://oi.jctech888.com.cn

Perl ........... 10
来源：http://pl.shxzskj.cn

Scala .......... 10
来源：http://xb.chemitech.net.cn

------------------------------------
来源：http://nk.shtwfgs.cn

合计 ........... 2106 条
来源：http://uv.jianghongdianzi.cn

按章节统计：
来源：http://nn.shxzskj.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://du.gzmigu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://fq.nszjky.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://fz.szsharing.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://aj.panjiajie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gn.jctech888.com.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ip.9csxet.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ns.jianghongdianzi.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://to.huixiangedu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://uu.nszjky.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dq.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cy.panjiajie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wm.lnxyls.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ul.nicolike.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bl.szsharing.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ea.shtwfgs.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ig.muxihuayi.cn

Q SQL 专题                              90
来源：http://of.yuexingan06.cn

R Bash 专题                             80
来源：http://ey.bookmarksfly.cn

S C / C++ 专题                          60
来源：http://xt.nicolike.cn

T 其他语言补充                          60
来源：http://ik.hahajie.cn

U 高频实用片段                         120
来源：http://mb.colortex.cn

------------------------------------
来源：http://up.nszjky.cn

合计                                  2106 条
来源：http://df.panjiajie.cn

--------------------------------------------------------------------------------
来源：http://df.yuexingan06.cn


<!-- 参考信息 -->