代发 wailian999

val a = 1;  var b = 2
来源：http://by.colortex.cn

[T53] Scala：字符串插值
来源：http://og.huixinmuqiang.cn

s"值: $b"
来源：http://gs.jctech888.com.cn

[T54] Scala：集合映射
来源：http://al.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://qb.9csxet.cn

[T55] Scala：集合过滤
来源：http://dp.yuntaijiaju.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oi.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://hy.huanxung.cn

case class User(name: String, age: Int)
来源：http://vj.nszjky.cn

[T57] Scala：模式匹配
来源：http://ey.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vs.nicolike.cn

[T58] Scala：函数定义
来源：http://en.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vd.jianghongdianzi.cn

[T59] Scala：循环
来源：http://eg.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://zs.bookmarksfly.cn

[T60] Scala：折叠
来源：http://kw.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oz.huanxung.cn

================================================================================
来源：http://ei.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rw.szxytkj.cn

================================================================================
来源：http://tl.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://ys.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tw.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://yu.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lh.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://jn.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dy.szsharing.cn

[U04] Py：变量调试打印
来源：http://fa.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jf.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://hs.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://cn.shxzukj.cn

[U06] Py：合并两个字典
来源：http://fs.521024.cn

{**a, **b}
来源：http://ik.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ty.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://tp.huanxung.cn

[U08] Py：展平二维列表
来源：http://jt.hahajie.cn

[y for x in nested for y in x]
来源：http://sr.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://lb.szsharing.cn

max(d, key=d.get)
来源：http://di.lnxyls.cn

[U10] Py：按值排序字典
来源：http://ye.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fi.nicolike.cn

[U11] Py：生成器表达式
来源：http://oz.shtwfgs.cn

(x * 2 for x in arr)
来源：http://fj.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cb.szsharing.cn

Counter(arr).most_common(3)
来源：http://wy.huixiangedu.cn

[U13] Py：固定长度队列
来源：http://hl.521024.cn

deque(maxlen=10)
来源：http://de.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://ao.nszjky.cn

defaultdict(list)
来源：http://yn.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://bs.nicolike.cn

t = time.perf_counter()
来源：http://qe.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://bx.jctech888.com.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dt.haigaiapp.cn

[U17] Py：初始化日志
来源：http://zv.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://ka.bookmarksfly.cn

[U18] Py：预编译正则
来源：http://kj.newstarts.cn

pat = re.compile(r"\d+")
来源：http://gj.521024.cn

[U19] Py：正则替换带回调
来源：http://lb.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lc.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://gk.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://aq.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://mm.bjjhwx.cn

@contextlib.contextmanager
来源：http://ia.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://hl.9csxet.cn

list(zip(*m))
来源：http://mk.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://tw.hahajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oe.hahajie.cn

[U24] Py：路径操作
来源：http://wq.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jr.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://fh.gzmigu.cn

csv.DictReader(f)
来源：http://kx.shxzukj.cn

[U26] Py：并发下载
来源：http://yf.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vi.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://en.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://bm.asd995.cn

[U28] Py：类型别名
来源：http://wb.yuexingan06.cn

UserId = int
来源：http://wv.szxytkj.cn

[U29] Py：属性校验
来源：http://oy.shxzskj.cn

@property 与 @x.setter 配合
来源：http://kh.lnxyls.cn

[U30] Py：数据类
来源：http://rq.shxzskj.cn

@dataclass(slots=True)
来源：http://ey.shxzukj.cn

[U31] Py：单测
来源：http://ec.jctech888.com.cn

python -m pytest -q
来源：http://vf.newstarts.cn

[U32] Py：代码格式化
来源：http://ny.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://uk.muxihuayi.cn

[U33] Py：打包发布
来源：http://sv.shxzskj.cn

python -m build  （依赖 pyproject.toml）
来源：http://jg.colortex.cn

[U34] Py：判断编码
来源：http://og.szsharing.cn

chardet.detect(raw)
来源：http://ja.asd995.cn

[U35] Py：发送邮件
来源：http://wu.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nk.yuexingan06.cn

[U36] Py：定时任务
来源：http://ij.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://nu.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://io.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qe.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://nw.hahajie.cn

Path(__file__).resolve().parent
来源：http://at.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://rw.panjiajie.cn

sys.stdout.isatty()
来源：http://zz.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://zc.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://bw.nszjky.cn

[U41] PHP：初始化 Composer 项目
来源：http://vt.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ta.bookmarksfly.cn

[U42] PHP：PSR-4 自动加载
来源：http://bh.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xf.asd995.cn

[U43] PHP：声明命名空间
来源：http://zx.szxytkj.cn

namespace App\Http;
来源：http://ef.szsharing.cn

[U44] PHP：开启严格类型
来源：http://xs.shxzskj.cn

declare(strict_types=1);
来源：http://uy.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://qb.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://yg.gzmigu.cn

[U46] PHP：可空类型
来源：http://sl.shxzukj.cn

?string $name = null
来源：http://er.wgjwhj.cn

[U47] PHP：联合类型
来源：http://ah.hahajie.cn

int|string $id
来源：http://sm.haigaiapp.cn

[U48] PHP：纯枚举
来源：http://sy.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lg.huixiangedu.cn

[U49] PHP：只读属性
来源：http://az.jianghongdianzi.cn

public readonly string $name
来源：http://ii.panjiajie.cn

[U50] PHP：构造器属性提升
来源：http://hm.hnjuh.cn

public function __construct(private int $id) {}
来源：http://ca.jctech888.com.cn

[U51] PHP：数组解构
来源：http://vh.colortex.cn

[$a, $b] = $arr;
来源：http://tu.gzmigu.cn

[U52] PHP：箭头函数
来源：http://tz.shtwfgs.cn

$double = fn($x) => $x * 2;
来源：http://rf.newstarts.cn

[U53] PHP：空合并运算符
来源：http://zt.huanxung.cn

$v = $a ?? $b ?? "default";
来源：http://cp.nszjky.cn

[U54] PHP：空安全调用
来源：http://yx.bjjhwx.cn

$obj?->method()
来源：http://nb.yuexingan06.cn

[U55] PHP：match 表达式
来源：http://fi.shxzskj.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tr.jianghongdianzi.cn

[U56] PHP：命名参数
来源：http://jp.521024.cn

f(a: 1, b: 2)
来源：http://ew.jctech888.com.cn

[U57] PHP：字符串插值
来源：http://we.muxihuayi.cn

"值: {$a}"
来源：http://oh.gzmigu.cn

[U58] PHP：数组三件套
来源：http://ns.newstarts.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wx.bjjhwx.cn

[U59] PHP：自定义排序
来源：http://kh.newstarts.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tj.szsharing.cn

[U60] PHP：JSON 编解码
来源：http://lb.huanxung.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ri.szsharing.cn

[U61] PHP：正则
来源：http://mw.bookmarksfly.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yp.hnjuh.cn

[U62] PHP：日期对象
来源：http://tt.jianghongdianzi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gh.gzmigu.cn

[U63] PHP：文件读写
来源：http://bt.bookmarksfly.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://yq.asd995.cn

[U64] PHP：目录遍历
来源：http://ca.jianghongdianzi.cn

glob("dir/*.php");  scandir("dir");
来源：http://sy.shxzskj.cn

[U65] PHP：会话
来源：http://fa.shtwfgs.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bl.shtwfgs.cn

[U66] PHP：设置 Cookie
来源：http://hs.yuexingan06.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://tb.panjiajie.cn

[U67] PHP：处理文件上传
来源：http://qq.wgjwhj.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rb.szxytkj.cn

[U68] PHP：PDO 连接
来源：http://gb.bookmarksfly.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ck.521024.cn

[U69] PHP：PDO 预处理
来源：http://av.9csxet.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ve.hnjuh.cn

[U70] PHP：PDO 事务
来源：http://ew.521024.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://db.bookmarksfly.cn

[U71] PHP：抛出异常
来源：http://ox.jianghongdianzi.cn

throw new RuntimeException("失败", 500);
来源：http://yw.wgjwhj.cn

[U72] PHP：写错误日志
来源：http://vh.asd995.cn

error_log("失败: " . $e->getMessage());
来源：http://fl.newstarts.cn

[U73] PHP：读取 ini 配置
来源：http://ka.hnjuh.cn

parse_ini_file("config.ini", true)
来源：http://al.gzmigu.cn

[U74] PHP：读取环境变量
来源：http://nr.lnxyls.cn

getenv("APP_ENV") ?: "production"
来源：http://ct.haigaiapp.cn

[U75] PHP：依赖注入
来源：http://oz.jianghongdianzi.cn

composer require psr/container
来源：http://vn.lnxyls.cn

[U76] PHP：简单路由
来源：http://co.hnjuh.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jz.newstarts.cn

[U77] PHP：模板渲染
来源：http://bd.bjjhwx.cn

composer require twig/twig
来源：http://ee.bjjhwx.cn

[U78] PHP：单元测试
来源：http://zf.szsharing.cn

composer require --dev phpunit/phpunit
来源：http://wd.bjjhwx.cn

[U79] PHP：静态分析
来源：http://ax.huixiangedu.cn

composer require --dev phpstan/phpstan
来源：http://tz.yuntaijiaju.cn

[U80] PHP：代码规范修复
来源：http://vb.szxytkj.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sw.chemitech.net.cn

[U81] JS：初始化项目
来源：http://cz.nicolike.cn

npm init -y;  npm i express
来源：http://nk.yuexingan06.cn

[U82] JS：package.json 脚本
来源：http://zq.newstarts.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qt.gzmigu.cn

[U83] JS：ES Module 导入导出
来源：http://kd.hnjuh.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ry.muxihuayi.cn

[U84] JS：CommonJS 写法
来源：http://qa.nicolike.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kv.colortex.cn

[U85] JS：可选链
来源：http://pk.muxihuayi.cn

a?.b?.c
来源：http://tc.hahajie.cn

[U86] JS：空值合并
来源：http://ug.9csxet.cn

a ?? b
来源：http://gn.shtwfgs.cn

[U87] JS：解构默认值
来源：http://ne.newstarts.cn

const { a = 1, b = 2 } = obj;
来源：http://wy.huanxung.cn

[U88] JS：对象展开合并
来源：http://ct.jianghongdianzi.cn

{ ...a, ...b }
来源：http://ox.colortex.cn

[U89] JS：数组去重
来源：http://hi.szxytkj.cn

[...new Set(arr)]
来源：http://fx.jctech888.com.cn

[U90] JS：数字数组排序
来源：http://nw.bookmarksfly.cn

[...arr].sort((a, b) => a - b)
来源：http://se.jianghongdianzi.cn

[U91] JS：对象键值遍历
来源：http://ed.shxzskj.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ai.bookmarksfly.cn

[U92] JS：深拷贝
来源：http://pp.huanxung.cn

structuredClone(obj)
来源：http://dh.szsharing.cn

[U93] JS：模板字符串
来源：http://lg.jianghongdianzi.cn

`共 ${n} 条`
来源：http://iy.wgjwhj.cn

[U94] JS：箭头函数
来源：http://wr.panjiajie.cn

const double = x => x * 2;
来源：http://ye.jianghongdianzi.cn

[U95] JS：Promise 包装
来源：http://cc.yuntaijiaju.cn

new Promise((resolve, reject) => {})
来源：http://ch.jctech888.com.cn

[U96] JS：async/await 与异常
来源：http://qx.jctech888.com.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://pa.yuexingan06.cn

[U97] JS：并发请求
来源：http://ge.szxytkj.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nm.szxytkj.cn

[U98] JS：fetch 带 JSON
来源：http://sn.nicolike.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ip.muxihuayi.cn

[U99] JS：事件监听
来源：http://zp.asd995.cn

el.addEventListener("click", e => {})
来源：http://pp.hahajie.cn

[U100] JS：DOM 查询
来源：http://xj.huixinmuqiang.cn

document.querySelector(".item")
来源：http://qk.huixiangedu.cn

[U101] JS：classList 操作
来源：http://lw.bookmarksfly.cn

el.classList.toggle("active")
来源：http://yx.huixiangedu.cn

[U102] JS：本地存储
来源：http://ss.hahajie.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://nx.shxzukj.cn

[U103] JS：定时器
来源：http://yh.huanxung.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mp.bookmarksfly.cn

[U104] JS：防抖
来源：http://nw.yuntaijiaju.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wg.szxytkj.cn

[U105] JS：节流
来源：http://ha.yuntaijiaju.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fd.lnxyls.cn

[U106] JS：日期格式化
来源：http://dn.521024.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rf.gzmigu.cn

[U107] JS：数字千分位
来源：http://pj.nszjky.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://rq.yuexingan06.cn

[U108] JS：随机整数
来源：http://il.521024.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mz.szxytkj.cn

[U109] JS：数组分组
来源：http://fb.jctech888.com.cn

Object.groupBy(arr, x => x.type)
来源：http://vb.hahajie.cn

[U110] JS：数组分块
来源：http://io.huixiangedu.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ec.jianghongdianzi.cn

[U111] JS：对象转 Map
来源：http://hd.wgjwhj.cn

new Map(Object.entries(obj))
来源：http://li.shxzukj.cn

[U112] JS：字符串补位
来源：http://dw.yuntaijiaju.cn

"7".padStart(3, "0")
来源：http://iy.bjjhwx.cn

[U113] JS：正则替换全部
来源：http://lf.szsharing.cn

s.replaceAll("a", "b")
来源：http://bv.szxytkj.cn

[U114] JS：JSON 深比较
来源：http://nt.521024.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://zo.bjjhwx.cn

[U115] JS：生成 UUID
来源：http://jb.bookmarksfly.cn

crypto.randomUUID()
来源：http://rg.szsharing.cn

[U116] JS：类型检查（JSDoc）
来源：http://qr.asd995.cn

/** @param {string} name */ function f(name) {}
来源：http://pf.nicolike.cn

[U117] JS：单元测试
来源：http://av.hnjuh.cn

npm i -D vitest;  npx vitest
来源：http://gz.lnxyls.cn

[U118] JS：开发服务器
来源：http://eq.huixiangedu.cn

npm i -D vite;  npx vite
来源：http://fo.9csxet.cn

[U119] JS：生产构建
来源：http://lu.asd995.cn

npx vite build
来源：http://rq.chemitech.net.cn

[U120] JS：读取环境变量（Vite）
来源：http://ed.jianghongdianzi.cn

import.meta.env.VITE_API_URL
来源：http://yq.newstarts.cn

================================================================================
来源：http://zv.chemitech.net.cn

统计汇总
来源：http://ub.muxihuayi.cn

================================================================================
来源：http://xa.bookmarksfly.cn

按语言统计（条）：
来源：http://ox.hnjuh.cn

Python ......... 252
来源：http://zh.gzmigu.cn

PHP ............ 252
来源：http://kd.panjiajie.cn

JavaScript ..... 252
来源：http://ee.newstarts.cn

TypeScript ..... 212
来源：http://ek.hnjuh.cn

Java ........... 212
来源：http://rv.yuntaijiaju.cn

Go ............. 212
来源：http://rg.muxihuayi.cn

Ruby ........... 212
来源：http://pq.yuntaijiaju.cn

C# ............. 212
来源：http://cv.muxihuayi.cn

C .............. 30
来源：http://rm.nszjky.cn

C++ ............ 30
来源：http://kq.521024.cn

SQL ............ 90
来源：http://ww.szsharing.cn

Bash ........... 80
来源：http://md.shxzskj.cn

Kotlin ......... 15
来源：http://ms.jianghongdianzi.cn

Swift .......... 15
来源：http://dj.newstarts.cn

Lua ............ 10
来源：http://cx.chemitech.net.cn

Perl ........... 10
来源：http://it.shxzukj.cn

Scala .......... 10
来源：http://kl.jianghongdianzi.cn

------------------------------------
来源：http://yd.jctech888.com.cn

合计 ........... 2106 条
来源：http://py.nszjky.cn

按章节统计：
来源：http://oz.panjiajie.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://af.lnxyls.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://ja.szxytkj.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://kw.yuexingan06.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://oh.yuexingan06.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gl.huixinmuqiang.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://bw.shxzukj.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://qr.haigaiapp.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://em.shxzskj.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ef.shxzskj.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ll.shxzukj.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://sa.huixiangedu.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://pi.haigaiapp.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ha.yuntaijiaju.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://nt.bjjhwx.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://pv.shxzskj.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wo.newstarts.cn


<!-- 参考信息 -->